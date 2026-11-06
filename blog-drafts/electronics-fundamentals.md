# Electronics fundamentals: voltage, current, resistance, and power

**Status:** Outline started; draft not written.

**Purpose:** Connect the basic electrical quantities to a simple circuit, then check the explanation with safe low-voltage measurements.

**Related article to review:** [Is P = I x V Part of Ohm’s Law?](https://philipmcgaw.com/ohms-law-and-watts-law/).

**Source note:** This outline uses ideas from the user-pasted transcripts headed “The fundamentals of electronics”, “What you should know”, “Electrical charge”, “Conductors and insulators”, “Voltage”, “Current”, “Circuit basics”, “Safety message”, “Resistance and Ohm’s Law”, and “SI prefixes”. The presenter is identified as Barron Stone; the exact course URL and publication details were not supplied. Treat the transcripts as background and write original explanations rather than reproducing their wording.

The local course-exercise folder contains a parts list, a multimeter list, an SI-prefix reference, and two circuit-challenge PDFs. A user-supplied screenshot of the parts list shows two 9 V batteries and two connectors, a 6.15 V, 0.5 A miniature bulb and holder, a red LED, a 470 Ω resistor, and SparkFun TOL-12966 and Extech MN36 multimeters. The listed shop links are US-oriented. Treat these as course examples, not UK purchasing recommendations. The screenshot does not show the circuit connections, so do not assume how the bulb, LED, or resistor are used together. The remaining exercise PDFs have not yet been reviewed.

## Planned outline

1. Introduce electrical charge using a static-electricity example, then define current as charge passing a point per second and show that voltage drives current only around a complete circuit.
2. Explain conductors and insulators with a wire's copper core and plastic covering, and show how conductivity varies by material and conditions.
3. Define voltage as a potential difference between two points and explain why a stated voltage needs a reference point.
4. Introduce a source, load, and conducting path; explain closed and open circuits, a switch, voltage across an open switch, and short-circuit risks.
5. Define resistance as opposition to current, measured in ohms (`Ω`), and use water flow through pipes as a first analogy. Explain where the analogy stops being exact.
6. Introduce Ohm’s law, `V = I × R`, rearrange it to find current, and show the relationships `V = I × R` and `P = V × I` with a checked, low-voltage example.
7. Introduce common SI prefixes used with electrical units, with examples of converting between milliamperes and amperes, and kilo-ohms and ohms.
8. Compare an ideal voltage source with a real battery: explain that a real source has limits and its terminal voltage can change with load.
9. Measure voltage across a component and current through the circuit with a multimeter, following the booklet's meter-safety steps.
10. Use Falstad to explore the circuit and compare the model with measurements from the real low-voltage build.
11. Link to the resistor article for power ratings and the battery article for capacity and voltage under load.

## Notes to carry forward

- The Scouts booklet already gives short definitions and the formulae. The blog post should add a worked example, a practical measurement, and a clear explanation of the limits of the water analogy rather than repeat the definitions at length.
- Explain static charge as a transfer of electrons between materials, not charge created by friction. Use conventional current direction (+ to −) throughout; put the opposite electron drift in metal wires in a clearly labelled advanced note.
- Explain that conductors and insulators are useful categories on a range of conductivity, and that temperature can affect conductivity differently in different materials. Use the copper-core and plastic-insulation example; do not use optical transparency as a stand-in for electrical conductivity.
- Treat voltage as a difference between two points, not a property of one point on its own. Explain that `0 V`, common, and ground name a chosen reference in a circuit; this does not necessarily mean a connection to the Earth. Avoid the transcript's North American mains example. Use a checked, low-voltage battery example.
- Explain that current is not used up by a lamp: in a simple series loop, the same conventional current flows through each part while electrical energy is transferred. Do not claim all current is a flow of holes; hole current is a model used for semiconductors.
- Do not describe electrons as choosing an “easier” route. A short circuit is an unintended low-resistance path that can draw excessive current; explain that current division depends on the complete circuit, not on electrons making choices.
- Assume the reader is new to electronics. Build understanding before introducing equations, keep the mathematics to basic arithmetic, and use only the calculations needed to show how the quantities relate.
- Teach SI prefixes as powers of ten and emphasise that prefix symbols are case-sensitive: `M` means mega (one million), while `m` means milli (one thousandth). Cover kilo, mega, giga, milli, micro, nano, and pico, then use practical conversions such as `42 mA = 0.042 A` and `24 kΩ = 24,000 Ω`. Choose the prefix that makes a value easy to read, and retain a space between the number and unit (`24 kΩ`).
- For the resistance example, `9 V ÷ 20 Ω = 0.45 A` is arithmetically correct for an ideal, fixed 20 Ω resistance. Label it as a calculation example, not a recommended bulb circuit: a real lamp’s resistance changes as its filament heats, and the exercise parts list includes a 6.15 V, 0.5 A bulb, so do not imply it should be connected directly to 9 V. Explain that Ohm’s law relates voltage, current, and resistance; a fixed resistance gives a proportional relationship only while its resistance remains effectively constant.
- Coordinate with the existing [Ohm’s law and Watt’s law article](https://philipmcgaw.com/ohms-law-and-watts-law/): distinguish `V = I × R` from the electrical power relationship `P = V × I`, while explaining why they are often used together. Do not say resistance is always constant; the simple proportional form applies to ohmic behaviour under specified conditions, and components such as filament lamps change resistance as they heat. Avoid making the historical naming distinction more prominent than the practical calculation.
- Keep the hose analogy as a rough model: pressure difference can stand in for voltage, flow rate for current, and restrictions for resistance. Do not say a bend in a hose maps directly to a particular electrical resistance or imply that all components have fixed resistance. Return to the complete circuit when explaining how changing voltage or resistance affects current.
- Keep examples to checked, low-voltage circuits. Do not include mains measurements, mains-powered equipment, or construction of power supplies.
- The pasted safety segment is US-context and gives an approximate 50 V threshold. Do not use that number as a general UK safety boundary. Follow current UK Scouts guidance and risk-assess the actual task; do not describe a circuit as safe simply because it uses a low voltage.
- Check the available current and risks of short circuits, heating, stored energy, and the work environment. Keep all mains work outside the scope of this post and the Scout activity.
- Make clear that an ideal source is a useful circuit model, while actual sources have operating limits. Check any quantitative example against the selected battery and load data.
- Explain multimeter connections precisely: voltage is measured in parallel; current is measured in series. Follow the meter's instructions and the existing booklet safety guidance.
- If the simulation does not model the real source's limits, describe the simplification and do not present the simulation as a measurement of the physical battery.

## Sources and visuals

- Check the actual battery, meter, and component datasheets used in the example.
- Offer Philip’s [Special Symbols used in Engineering Reports](https://philipmcgaw.com/special-symbols-used-in-engineering-reports/) as optional further reading for unit symbols and technical-document spacing. Keep the project’s SI style: put a non-breaking space between a value and its unit.
- [Scouts Safety Policy](https://www.scouts.org.uk/por/2a-key-policies/2a8-safety-policy/) and [HSE electrical safety FAQs](https://www.hse.gov.uk/electricity/faq.htm).
- Use an original schematic and a clearly labelled Falstad simulation where it helps explain the relationships.
