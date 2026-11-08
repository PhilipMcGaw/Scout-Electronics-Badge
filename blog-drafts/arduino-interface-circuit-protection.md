# Protecting an Arduino and its interface circuits

An Arduino board is a useful controller, but its pins are not universal, fault-proof inputs and outputs. A sensor, switch, cable or motor can expose a pin to voltage, current or electrical noise that the board was never designed to handle. A little thought at the interface can make a project more dependable and easier to repair.

This is a practical introduction to protection for low-voltage hobby circuits. It is not an automotive design guide and does not claim that a protected Arduino meets LV 124.

## What does “hardened” mean?

People use *hardened* to mean that a circuit is less likely to fail when something goes wrong or when it meets electrical noise, temperature changes, vibration or moisture. The word does not name one universal performance level. Start by writing down the actual conditions the project must survive: supply range, cable length, likely wiring mistakes, load current, environment and what counts as acceptable behaviour after a fault.

LV 124 is a vehicle-component test specification for electrical and environmental conditions in the 12 V onboard systems of passenger vehicles up to 3.5 tonnes. Its test families include overvoltage, undervoltage, jump-start, reverse-polarity, short-circuit, interruptions, temperature, mechanical and climatic conditions. The required tests and limits depend on the applicable edition, vehicle maker requirements, component role and project test plan. Adding a fuse, diode or transient suppressor to an Arduino does not establish LV 124 compliance. That requires design against the applicable requirements and evidence from the prescribed validation process.

For a hobby project, LV 124 can be useful context for the kinds of stress automotive electronics consider. It should not be treated as a menu of component values or a do-it-yourself certification checklist.

### Emissions, immunity and electrical robustness are different checks

Electromagnetic compatibility (EMC) work includes different questions. **Emissions** testing measures disturbance a product puts onto its supply leads or radiates into its surroundings. **Immunity** testing checks how it behaves when disturbances are applied to it. Neither alone checks every electrical fault or environmental condition.

The linked comparison article covers conducted emissions under CISPR 25 (automotive components), CISPR 11 (industrial, scientific and medical equipment), and MIL-STD-461G (defence equipment). It shows why test results depend on the specified measurement network, frequency range, detector, cable arrangement and other setup details. A LISN or artificial network creates a defined measurement impedance and helps isolate the device under test from supply-line noise; different standards use different networks and procedures. A bench spectrum-analyser check can help find noise sources, but it does not become a standards-compliant measurement simply by adding a LISN.

CISPR 25 is aimed at controlling disturbances that could affect receivers on board vehicles. It is an emissions standard, not a substitute for LV 124, which also includes electrical stress and environmental tests. The cited comparison dates from 2021 and discusses specific earlier editions; check the current applicable standard and customer requirements before relying on its numerical test details.

## Start with the board’s limits

“Arduino” covers many boards and microcontrollers. Before connecting anything, use the exact board’s official documentation and microcontroller datasheet to check logic voltage, input range, output-current limits, total-current limits, power-input range and any protection already fitted. Absolute maximum ratings describe stress limits, not normal operating targets. Do not assume a pin can safely absorb a fault because a different Arduino model can.

The board itself is only one part of the system. Check the sensor, module, cable, power supply and load too. A 3.3 V sensor may be damaged by a 5 V signal even if the controller can tolerate it.

## Common failure paths and design responses

The article “10 Ways to Destroy an Arduino” usefully groups several mistakes: shorting outputs, applying an out-of-range signal, reversing or misapplying power, shorting a supply rail, feeding power backwards, and exceeding combined pin-current limits. Its examples are tied to particular Arduino hardware and should not be assumed to describe every board. Treat its proposed Rugged Circuits protections as the manufacturer’s claims about its own products, not as a general design recipe.

A more useful design habit is to identify the fault current path and decide what should limit it, where the energy goes, and what remains connected if the protection operates.

### Signals from switches and sensors

- Keep external signals within the receiving pin’s permitted range in normal operation and during credible faults.
- Use a suitable divider or buffer where signal voltage must be reduced. Calculate for input impedance, source tolerance and fault conditions; a divider alone may not protect against every transient.
- Use a series resistor when it can limit current into a pin’s input protection without causing measurement or timing problems. Do not rely on the microcontroller’s internal clamp diodes to carry continuous fault current.
- For long or off-board cables, consider filtering, a suitable transient protection device, and a more robust interface such as a differential receiver. Select parts for the signal, expected transient and layout; a TVS diode is not automatically suitable just because its label says “5 V”.
- A Zener or TVS diode does not hold a pin at one exact voltage. Its clamp voltage rises with current, and the source must limit that current. Check the protector’s clamp voltage at the expected pulse current against the receiving device’s limits, and check pulse energy, return path and signal effects. A nominal Zener voltage alone does not show that a pin is safe.
- Treat signal-pin protection and supply overvoltage protection as different jobs. A series disconnect, crowbar and shunt clamp work in different ways; a crowbar intentionally draws high current and needs a suitable current-limited source or coordinated fuse.
- Give inputs a defined state with a pull-up or pull-down, and consider filtering and software debounce for switches.

### Outputs and loads

- Do not power motors, relays, lamps or other substantial loads directly from an I/O pin. Use a driver rated for the load and its start-up or stall current.
- Inductive loads need a safe path for their stored energy when switched off. The clamp or recirculation arrangement depends on whether the load is switched on the low side or high side and how quickly it must release.
- Check each pin’s operating current and the combined limits for the microcontroller, board regulator, connector and supply. Staying below one headline per-pin maximum is not enough.
- A MOSFET load switch can let a small control signal switch power to a larger load. A high-side P-channel MOSFET is one option, but it must be fully enhanced at the available gate-to-source voltage. Threshold voltage only marks the beginning of conduction at a small test current; it does not show that the device will have low enough on-resistance in the intended circuit.
- Check MOSFET conduction loss and temperature, gate-voltage limits, body-diode direction, start-up/inrush current and any load transients. An optocoupler may provide signal isolation, but it does not by itself protect the power input or load output from reverse polarity, overcurrent or transients.
- A resistor can limit current for a simple LED, but calculate it from the supply voltage, LED forward voltage and a suitable operating current.

### Power inputs and wiring mistakes

- Choose one supported power method and follow the board maker’s instructions. Avoid feeding external power into a rail that is also driven by USB unless the board explicitly supports that arrangement.
- Use reverse-polarity protection where reversed connections are credible. A series diode is simple but drops voltage and dissipates power; a MOSFET arrangement can reduce the drop but must be designed for the real voltage and fault conditions.
- Select a fuse for the circuit’s normal current, voltage, fault current and required opening behaviour; check its time-current data, interrupting rating, temperature derating and the wiring it is meant to protect. A fuse does not clamp voltage, and it may not protect a delicate semiconductor before it opens.
- A resettable PTC fuse behaves differently from a one-shot fuse: it rises to a high resistance during a fault, may still pass current, and needs to cool before it returns towards its normal state. Check the selected part’s hold/trip behaviour and do not treat it as an interchangeable replacement for a fuse.
- Add local decoupling and bulk capacitance as needed, with suitable voltage and ripple ratings. Capacitors do not replace transient or overcurrent protection.
- Keep high-current load returns from sharing a narrow or noisy path with sensitive signal references. Plan grounding and connector pinout deliberately.

## Protection is a system, not a parts list

Protection parts have limits. A resistor may reduce current but cannot absorb unlimited energy. A TVS device must be paired with a source impedance or other current-limiting measure and placed so the transient current has a short return path. A fuse must interrupt the available fault current safely. A reverse-polarity circuit must tolerate the source and load. Layout, connectors, wiring, enclosure and software behaviour all affect the result.

For a project that controls equipment, operates unattended, connects to a vehicle, or could cause injury or damage, use a qualified design process and the applicable product requirements. Do not connect a prototype Arduino directly to a vehicle electrical system on the strength of this introductory article.

## A practical review checklist

1. Identify the exact board and read its current pinout, power guidance and datasheet limits.
2. List each connection that leaves the board and the normal, fault and transient voltages it may encounter.
3. Trace where fault current and stored energy will flow.
4. Select protection for the actual signal or load, then check its ratings, tolerances, temperature behaviour and failure mode.
5. Check connector orientation, cable length, grounding, enclosure and power-source interactions.
6. Verify the design with controlled, appropriate tests and record the conditions and results. Do not deliberately damage a board or apply automotive transients without suitable equipment and a safe test plan.

## Quick knowledge check

1. Does a fuse protect a circuit from every overvoltage event? **No.** A fuse responds to current over time; it is not a voltage clamp.
2. Is a fuse’s current rating enough to establish that it is suitable? **No.** Check its voltage rating, time-current behaviour, interrupting rating, temperature conditions and the circuit’s available fault current.
3. Does a fuse open instantly whenever current exceeds its rating? **No.** Opening time depends on the current and the fuse’s time-current characteristics.
4. How does a resettable PTC differ from a one-shot fuse? **A one-shot fuse opens the circuit and must be replaced; a PTC rises to a high resistance during a fault and can recover after cooling, while still allowing some current to pass.**
5. Why check a fuse’s interrupting rating? **It must be able to safely interrupt the maximum fault current available in the circuit.**

## Sources and further reading

- Rugged Circuits, [“10 Ways to Destroy an Arduino”](https://www.rugged-circuits.com/10-ways-to-destroy-an-arduino/). A useful list of failure modes, but its examples concern specific hardware and its product protection descriptions are promotional claims. Its values are not universal recommendations.
- Dyethin, [“How to design an overvoltage protection circuit?”](https://www.dyethin.com/blog/projects/how-to-design-an-overvoltage-protection-circuit), 2023-09-21. Topic prompt only: its Zener examples (including 5.1 V and 6.8 V) are not general-purpose microcontroller input protection values. A clamp voltage depends on current and device characteristics; check the selected pin and protector datasheets.
- Texas Instruments, [“TVS Surge Protection in High-Temperature Environments”](https://www.ti.com/lit/an/slva930/slva930.pdf). Explains the difference between TVS stand-off, breakdown and clamp voltages, including the rise in clamp voltage from dynamic resistance.
- Texas Instruments, [“Data Line ESD Protect: TVS Diodes or Chip Varistors?”](https://www.ti.com/document-viewer/lit/html/SLVAFR3). Discusses clamp performance and line capacitance when selecting protection for data signals.
- Codrey Electronics, [“Power MOSFET Load Switch”](https://www.codrey.com/electronic-circuits/power-mosfet-load-switch/), updated 2021-08-18. Useful as an example of a high-side P-channel switch and isolated control idea. Do not reuse the circuit or its approximate power/current claims without checking the exact schematic, MOSFET safe operating conditions, gate drive, thermal design, optocoupler drive and load behaviour.
- Infineon, [IRF9540N datasheet](https://www.infineon.com/dgdl/Infineon-IRF9540N-DataSheet-v01_01-EN.pdf?fileId=5546d462533600a401535611cfa21dc8). Its on-resistance is specified at −10 V gate-to-source; the threshold test is at only −250 µA, illustrating why threshold voltage is not a full-on design value. This is an example part cited by Codrey, not a recommendation.
- AnalogicTips, [“A comparison of EMI test setups and specifications for automotive, industrial and defense applications, part 1: conducted emissions”](https://www.analogictips.com/a-comparison-of-emi-test-setups-and-specifications-for-automotive-industrial-and-defense-applications-part-1-conducted-emissions/), by Texas Instruments applications engineer Timothy Hegarty, 2021-04-02. Useful comparison of CISPR 25, CISPR 11 and MIL-STD-461G test setups; numerical details refer to editions current at publication and must be checked against current requirements.
- IEC, [CISPR Guide 2024](https://assets.iec.ch/further_informations/1298/CISPR%20Guide%202024.pdf), product-to-standard applicability overview.
- IEC, [CISPR 25:2021](https://cdn.standards.iteh.ai/samples/103028/81d3c4d3a2484c4091f04f7305870091/CISPR-25-2021.pdf) sample. Describes the standard’s purpose as controlling vehicle/module emissions to protect on-board receivers; use the full applicable standard for test work.
- Weiss Technik, [LV 124 technical information sheet](https://backend.weiss-technik.com/webapp/weisstechnik/detailpages/environmental-simulation/LV124/Weiss-Technik-Technical-information-sheet-LV-124.pdf). Overview of electrical and environmental test categories; use the applicable controlled specification for engineering work.
- Deutsche Akkreditierungsstelle, [testing laboratory accreditation annex](https://www.dakks.de/files/data/as/pdf/D-PL-21612-02-00e.pdf). Illustrates that LV 124 is applied as defined test methods with scoped laboratory accreditation.
- Arduino, [UNO R3 documentation](https://docs.arduino.cc/hardware/uno-rev3), as an example of board-specific information. Use the documentation for the actual board, not this example, when checking ratings.
- Iain Sharp, [Electronics for Artists, Part 2](https://lushprojects.com/electronicsforartists/electronicsforartistsp2.pdf) (revision 2.2, 2019), uses a transistor to drive a speaker and describes relay-coil suppression. Treat its circuits as historical examples only; verify the exact driver, coil, contacts, load, board limits and suppression. A relay does not guarantee safe isolation for every connected circuit. The notes are CC BY-NC-SA 3.0 Unported; do not reproduce figures or wording without meeting the licence terms.
- element14 Community, [“Circuit Protection: PCB-Mounted Fuses”](https://community.element14.com/learn/learning-center/essentials/w/documents/3133/circuit-protection-pcb-mounted-fuses), created 2017 and last updated 2023. Useful for introductory fuse terminology and types, but its component examples and standards summaries need current verification; no ratings or part choices are adopted from it.
- The same element14 module includes a 15-question knowledge check. Use it as topic inspiration only; the five questions above are original and should be checked against current fuse manufacturer information.
- Littelfuse, [Fuseology design guide](https://www.littelfuse.com/assetdocs/fuseology-selection-guide?assetguid=d812dff2-1c47-4dc3-bce7-07a4001ddc32). Manufacturer guidance on time-current curves, I²t, fault current and fuse selection; check the exact fuse datasheet for a real design.
- Littelfuse, [PolySwitch PPTC resettable devices](https://www.littelfuse.com/products/fuses-overcurrent-protection/polyswitch-resettable-pptc-devices). Compares resettable PTC behaviour with conventional fuses; actual trip current, hold current and recovery are part-specific.

*Editorial note: this draft uses the linked article as a topic prompt, not as a source for universal circuit designs. No personal build or test experience is claimed.*
