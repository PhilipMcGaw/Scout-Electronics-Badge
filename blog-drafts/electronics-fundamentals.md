# Electronics fundamentals: voltage, current, resistance, and power

**Status:** Outline started; draft not written.

**Purpose:** Connect the basic electrical quantities to a simple circuit, then check the explanation with safe low-voltage measurements.

**Source note:** This outline uses ideas from the user-pasted transcripts headed “The fundamentals of electronics”, “What you should know”, “Electrical charge”, and “Safety message”. The presenter is identified as Barron Stone; the exact course URL and publication details were not supplied. Treat the transcripts as background and write original explanations rather than reproducing their wording.

The local course-exercise folder contains a parts list, a multimeter list, an SI-prefix reference, and two circuit-challenge PDFs. A user-supplied screenshot of the parts list shows two 9 V batteries and two connectors, a 6.15 V, 0.5 A miniature bulb and holder, a red LED, a 470 Ω resistor, and SparkFun TOL-12966 and Extech MN36 multimeters. The listed shop links are US-oriented. Treat these as course examples, not UK purchasing recommendations. The screenshot does not show the circuit connections, so do not assume how the bulb, LED, or resistor are used together. The remaining exercise PDFs have not yet been reviewed.

## Planned outline

1. Introduce electrical charge using a static-electricity example, then define charge in coulombs and current as the rate of charge flow.
2. Start with a simple closed circuit and relate voltage, current, resistance, and power to its parts.
3. Use water flow through pipes as a first analogy, then explain where the analogy stops being exact.
4. Show the relationships `V = I × R` and `P = V × I` with one checked, low-voltage example.
5. Compare an ideal voltage source with a real battery: explain that a real source has limits and its terminal voltage can change with load.
6. Measure voltage across a component and current through the circuit with a multimeter, following the booklet's meter-safety steps.
7. Use Falstad to explore the circuit and compare the model with measurements from the real low-voltage build.
8. Link to the resistor article for power ratings and the battery article for capacity and voltage under load.

## Notes to carry forward

- The Scouts booklet already gives short definitions and the formulae. The blog post should add a worked example, a practical measurement, and a clear explanation of the limits of the water analogy rather than repeat the definitions at length.
- Explain static charge as a transfer of electrons between materials, not charge created by friction. Describe the atom picture as a simplified model and distinguish electron movement in metal wires from conventional current shown on circuit diagrams.
- Assume the reader is new to electronics. Build understanding before introducing equations, keep the mathematics to basic arithmetic, and use only the calculations needed to show how the quantities relate.
- Keep examples to checked, low-voltage circuits. Do not include mains measurements, mains-powered equipment, or construction of power supplies.
- The pasted safety segment is US-context and gives an approximate 50 V threshold. Do not use that number as a general UK safety boundary. Follow current UK Scouts guidance and risk-assess the actual task; do not describe a circuit as safe simply because it uses a low voltage.
- Check the available current and risks of short circuits, heating, stored energy, and the work environment. Keep all mains work outside the scope of this post and the Scout activity.
- Make clear that an ideal source is a useful circuit model, while actual sources have operating limits. Check any quantitative example against the selected battery and load data.
- Explain multimeter connections precisely: voltage is measured in parallel; current is measured in series. Follow the meter's instructions and the existing booklet safety guidance.
- If the simulation does not model the real source's limits, describe the simplification and do not present the simulation as a measurement of the physical battery.

## Sources and visuals

- Check the actual battery, meter, and component datasheets used in the example.
- [Scouts Safety Policy](https://www.scouts.org.uk/por/2a-key-policies/2a8-safety-policy/) and [HSE electrical safety FAQs](https://www.hse.gov.uk/electricity/faq.htm).
- Use an original schematic and a clearly labelled Falstad simulation where it helps explain the relationships.
