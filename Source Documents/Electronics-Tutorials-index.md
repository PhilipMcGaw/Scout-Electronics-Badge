# Electronics Tutorials: curated source index

**Reviewed:** 2026-11-08

**Site:** [Electronics Tutorials](https://www.electronics-tutorials.ws/)

**Site map:** [Tutorial sitemap](https://www.electronics-tutorials.ws/sitemap)

This is a curated reading map for topics already in the booklet and blog drafts, not a review of every lesson on the site. The sitemap itself says it is not comprehensive. The tutorials can help locate a topic or offer an alternate explanation, but they are secondary sources. Check circuit values, ratings and safety claims against current manufacturer documentation and applicable UK primary guidance. Do not reuse site wording or figures without checking the copyright and reuse terms.

## Core circuit ideas

| Topic | Tutorial | Project use and limits |
|---|---|---|
| Voltage, current and resistance | [DC Circuit Theory](https://www.electronics-tutorials.ws/dccircuits/dcp_1.html) | Broad topic map for [electronics fundamentals](../blog-drafts/electronics-fundamentals.md). Do not adopt its electron-flow-first explanation as the definition of current, its “current source likes a short circuit” analogy, or its absolute claims about current and voltage. Keep conventional current as the circuit-analysis convention and explain sources using their real operating limits. |
| Potential dividers | [Voltage Divider Circuits](https://www.electronics-tutorials.ws/dccircuits/voltage-divider.html) | Useful worked-circuit starting point for the [resistor](../blog-drafts/resistors.md) and [sensor-logging](../blog-drafts/arduino-sensor-datalogging.md) drafts. Account for load/input impedance, sensor curve, supply/reference and ADC behaviour; a divider output is a voltage, not a direct resistance measurement. |
| Resistor combinations | [Resistors in Series](https://www.electronics-tutorials.ws/resistor/res_3.html), [Resistors in Parallel](https://www.electronics-tutorials.ws/resistor/res_4.html), and [Resistors in Series and Parallel](https://www.electronics-tutorials.ws/resistor/res_5.html) | Clear equivalent-resistance examples for the resistor draft. Recalculate each example and check individual resistor power, voltage limits, tolerances and thermal conditions before using a combination in a real circuit. |
| Resistor power | [Resistor Power Rating](https://www.electronics-tutorials.ws/resistor/res_7.html) | Useful topic pointer for the resistor draft’s heat and power discussion. Do not treat listed standard wattages as universal; use the exact resistor datasheet and appropriate derating. |
| Resistor markings | [Colour Codes and Tolerances](https://www.electronics-tutorials.ws/resistor/res_2.html) | Optional alternate reference for colour bands in the resistor draft. Choose a chart matching band count; verify tolerance and unusual codes rather than assuming all parts use one system. |

## Components and timing

| Topic | Tutorial | Project use and limits |
|---|---|---|
| Capacitor technologies | [Types of Capacitor](https://www.electronics-tutorials.ws/capacitor/cap_2.html) and [Capacitor Characteristics](https://www.electronics-tutorials.ws/capacitor/cap_3.html) | Topic discovery for the [capacitor draft](../blog-drafts/capacitors.md). Some statements about ceramic capacitance ranges, voltage ratings and technology characteristics are broad or outdated. Use manufacturer datasheets and current manufacturer guides for dielectric, polarity, DC-bias, temperature and ageing behaviour. |
| RC timing | [RC Charging Circuit](https://www.electronics-tutorials.ws/rc/rc_1.html) and [RC Discharging Circuit](https://www.electronics-tutorials.ws/rc/rc_2.html) | Useful diagrams and sequence for explaining charging, discharging and time constants in the capacitor draft and booklet. “Five time constants” is an approximation for reaching close to the final value, not a universal switching time; circuit thresholds and tolerances matter. |
| LEDs | [Light Emitting Diodes](https://www.electronics-tutorials.ws/diode/diode_8.html) | Alternate introduction for the LED current-limit example in the [resistor draft](../blog-drafts/resistors.md). Select current and series resistance from the exact LED datasheet, supply range and required brightness; do not reuse generic forward-voltage or current values as specifications. |
| BJT switching | [Transistor as a Switch](https://www.electronics-tutorials.ws/transistor/tran_4.html) | Useful conceptual example for transistor switching and relay-driver topics. Its example calculations and simplified saturation assumptions are not a substitute for checking base drive, collector current, dissipation, switching conditions and inductive-load suppression against the exact transistor and load documentation. |

## Sensors, interfaces and protection

| Topic | Tutorial | Project use and limits |
|---|---|---|
| Thermistors | [Thermistors and NTC Thermistors](https://www.electronics-tutorials.ws/io/thermistors.html) | Topic source for the NTC divider example in the resistor draft. Use the selected thermistor’s resistance-temperature curve, tolerance, dissipation and manufacturer circuit guidance; there is no universal NTC curve. |
| Logic inputs | [Pull-up and Pull-down Resistors](https://www.electronics-tutorials.ws/logic/pull-up-resistor.html) | Alternate explanation for the [Arduino buttons draft](../blog-drafts/arduino-buttons-and-pullups.md). Verify internal pull-up values, logic thresholds, input voltage and wiring against the chosen board. |
| Input and output circuits | [Input Interfacing Circuits](https://www.electronics-tutorials.ws/io/input-interfacing-circuits.html) and [Output Interfacing Circuits](https://www.electronics-tutorials.ws/io/output-interfacing-circuits.html) | A useful topic map for the [Arduino interface-protection draft](../blog-drafts/arduino-interface-circuit-protection.md). Treat generic examples as concepts only; check the receiving board, driver, sensor, load and protection-device datasheets. |
| Relays | [Electrical Relay and Solid State Relays](https://www.electronics-tutorials.ws/io/io_5.html) and [Relay Switching Circuits](https://www.electronics-tutorials.ws/blog/relay-switch-circuit.html) | Optional background for the [relay/contact-protection draft](../blog-drafts/relays-contactors-and-snubber-circuits.md). Relay contact configuration, isolation, ratings and coil suppression are device-specific; use the exact relay documentation. |
| Transient suppression | [Transient Suppression Devices](https://www.electronics-tutorials.ws/power/transient-suppression.html) | Topic index for the Arduino interface-protection and relay drafts. Do not copy generic clamp values or treat one suppression device as interchangeable with another. Verify pulse shape, source impedance, energy, clamping voltage, wiring and protected-device limits. |

## Source-quality notes

- The site is broad and convenient for discovering topics, but some introductory explanations collapse distinct ideas or overstate simplified models. For example, the DC theory page mixes conventional current, electron movement and holes in a way that should not be copied into the booklet.
- The capacitor-types page makes wide generalisations about ceramic values and voltage ratings. These depend on dielectric, package, manufacturer and application; use current datasheets and manufacturer application material.
- The transistor-switch and transient-suppression pages include illustrative circuits and calculations. Their examples are not validated recommendations for a selected board, relay or load.
- The site is not a source for UK Scout requirements, electrical safety law, product conformity, current standards editions or component operating limits.
- Existing project sources already cover several of these topics in more authoritative or product-specific detail. Use this index to find candidate explanations, then prefer primary sources for claims that affect a design or safety.
