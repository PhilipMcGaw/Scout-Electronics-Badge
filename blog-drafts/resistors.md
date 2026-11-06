# Resistors: values, ratings, dividers, and practical use

**Status:** Outline started; draft not written.

**Existing articles:** [Learn about Resistors](https://philipmcgaw.com/learn-about-resistors/), [LED Resistor Values](https://philipmcgaw.com/led-resistors-values/), and the [Potential Divider Calculator](https://philipmcgaw.com/potential-divider-calculator/).

**Purpose:** Refresh the existing article with clearer explanations and a practical example that shows how resistor choice affects a real circuit.

## Planned outline

1. What a resistor does: set current, create voltage drops, and dissipate energy as heat.
2. Read through-hole colour bands and common surface-mount markings.
3. Choose a value and power rating for an LED indicator; explain the calculation and assumptions.
4. Explain the potential divider and use the existing calculator to explore how resistor values set the output voltage.
5. Use a thermistor as one resistor in a potential divider to show how temperature changes can produce a changing voltage.
6. Explain tolerance, temperature effects, and failure modes at a useful level.
7. Explain that electrical power dissipated by a resistor becomes heat, and include a warning against deliberately overloading or touching a hot resistor.
8. Show the examples in Falstad, then compare the simulation with measurements from a real low-voltage circuit.

## Notes to carry forward

- The existing post already covers Ohm’s law, resistor markings, power dissipation, temperature effects, reliability, and component-selection factors.
- Review of the current [Learn about Resistors](https://philipmcgaw.com/learn-about-resistors/) page (checked 2026-11-06): revise the “conventional current” section so it presents conventional current from positive to negative as the standard direction used in this series, with electron flow as a brief optional note rather than calling the convention a lie. The page’s temperature-coefficient equation assumes a positive coefficient; explain that resistance may increase or decrease with temperature and check any example against the selected resistor’s datasheet. Replace the broad claim that surface-mount markings follow the first three colour bands with a short explanation that marking systems vary by package and manufacturer. Remove or qualify the broad claim that through-hole resistors are rarely encountered outside prototyping and hobby electronics. Explain Kirchhoff’s current and voltage laws in plain language or omit them here if they distract from practical resistor selection. The reliability model and failure-rate figures are specialist material; omit them unless the intended reader needs them and a suitable primary source is added.
- Link to the [electronics fundamentals post](electronics-fundamentals.md) for the voltage, current, resistance, and power overview; keep this article focused on resistor choice and use.
- Use the Potential Divider Calculator as an interactive companion to the explanation. Check that its inputs, equations, units, and displayed results are clear, then show how changing either resistor affects the divider output.
- Philip is more likely to use thermistors than LDRs, so use a thermistor for the main sensor example. Check whether the selected part is NTC or PTC, and use its datasheet rather than assuming a universal resistance curve or divider value.
- Keep the sensor example inside the resistor article as an application of the potential divider. If Falstad does not model the selected thermistor, use a variable resistor only as a clearly labelled approximation of its changing resistance.
- The LED-resistor post has a table for several LED colours, three supply voltages, and three target currents. Carry the table forward only after rechecking each calculation against the assumed LED forward voltage and supply. Its blue and white LED examples at 3.3 V have very little voltage across the resistor, so explain why the current can vary significantly.
- Recheck resistor power as well as LED current. For example, the published red LED, 12 V, 560 Ω case dissipates about 0.19 W in the resistor if the assumed LED drop is 1.7 V, so a 1/8 W resistor would be undersized; check the exact design and rating before recommending a part.
- Include a safety warning that a resistor can become hot when it dissipates power. The *Basic Electronics* source demonstrates this by overloading a low-value resistor from a battery and telling the reader to feel it; do not repeat that experiment. Explain heat using the power calculation and resistor rating, and do not ask readers to touch a component to judge its temperature.
- Explain how the actual LED datasheet, supply tolerance, target current, resistor tolerance, and resistor power rating affect the result. A simulation and a measured low-voltage example can show the difference between an estimate and a built circuit.
- Review the wording and equations carefully; comments on the existing post flag places where notation and terminology need clearer explanation.
- Keep specialised reliability models and failure-rate figures only if they serve the intended reader and can be checked against a suitable source.

## Sources and visuals

- Check current resistor manufacturer datasheets for value, tolerance, power, voltage, and temperature-coefficient examples.
- Use an original circuit diagram or a clearly attributed simulation screenshot if permission and reuse terms allow it.
