# Resistors: values, ratings, and practical use

**Status:** Outline started; draft not written.

**Existing articles:** [Learn about Resistors](https://philipmcgaw.com/learn-about-resistors/) and [LED Resistor Values](https://philipmcgaw.com/led-resistors-values/).

**Purpose:** Refresh the existing article with clearer explanations and a practical example that shows how resistor choice affects a real circuit.

## Planned outline

1. What a resistor does: set current, create voltage drops, and dissipate energy as heat.
2. Read through-hole colour bands and common surface-mount markings.
3. Choose a value and power rating for an LED indicator; explain the calculation and assumptions.
4. Explain tolerance, temperature effects, and failure modes at a useful level.
5. Explain that electrical power dissipated by a resistor becomes heat, and include a warning against deliberately overloading or touching a hot resistor.
6. Show the example in Falstad, then compare the simulation with measurements from a real low-voltage circuit.

## Notes to carry forward

- The existing post already covers Ohm’s law, resistor markings, power dissipation, temperature effects, reliability, and component-selection factors.
- The LED-resistor post has a table for several LED colours, three supply voltages, and three target currents. Carry the table forward only after rechecking each calculation against the assumed LED forward voltage and supply. Its blue and white LED examples at 3.3 V have very little voltage across the resistor, so explain why the current can vary significantly.
- Recheck resistor power as well as LED current. For example, the published red LED, 12 V, 560 Ω case dissipates about 0.19 W in the resistor if the assumed LED drop is 1.7 V, so a 1/8 W resistor would be undersized; check the exact design and rating before recommending a part.
- Include a safety warning that a resistor can become hot when it dissipates power. The *Basic Electronics* source demonstrates this by overloading a low-value resistor from a battery and telling the reader to feel it; do not repeat that experiment. Explain heat using the power calculation and resistor rating, and do not ask readers to touch a component to judge its temperature.
- Explain how the actual LED datasheet, supply tolerance, target current, resistor tolerance, and resistor power rating affect the result. A simulation and a measured low-voltage example can show the difference between an estimate and a built circuit.
- Review the wording and equations carefully; comments on the existing post flag places where notation and terminology need clearer explanation.
- Keep specialised reliability models and failure-rate figures only if they serve the intended reader and can be checked against a suitable source.

## Sources and visuals

- Check current resistor manufacturer datasheets for value, tolerance, power, voltage, and temperature-coefficient examples.
- Use an original circuit diagram or a clearly attributed simulation screenshot if permission and reuse terms allow it.
