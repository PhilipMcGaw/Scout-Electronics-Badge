# Using an LDR in a voltage divider

**Status:** Outline started; draft not written.

**Purpose:** Show how a light-dependent resistor (LDR) and a fixed resistor can turn a change in light into a change in voltage that a transistor, comparator, or microcontroller can use.

## Planned outline

1. Explain how an LDR's resistance changes with light, using the selected part's datasheet rather than assuming a universal value.
2. Introduce a two-resistor voltage divider and show how the output voltage depends on which resistor is connected to the supply and which is connected to 0 V.
3. Show how changing the fixed resistor changes the sensor circuit's response.
4. Explain that a transistor, comparator, or digital input can use the changing voltage to switch an output, while noting that each has different input and threshold requirements.
5. Use Falstad to explore the circuit, then compare it with low-voltage measurements in bright and dim conditions.
6. Connect the example to the booklet's light-sensitive alarm project and identify the limits of a simple LDR circuit.

## Notes to carry forward

- The *Basic Electronics* source covers LDRs and voltage dividers, but its component values and circuit examples need checking against the actual sensor, supply, and output device.
- Avoid presenting one divider orientation or fixed-resistor value as universally correct. Label the output node and explain how the voltage changes when the LDR is placed on either side of the divider.
- Keep this to low-voltage sensor circuits. Do not include mains sensing, mains-powered lighting control, or mains-derived supply designs.
- A simulation is useful for showing the direction of change; real LDR behaviour varies with the part, illumination, geometry, and environment.

## Sources and visuals

- Check the LDR and output-device datasheets for resistance range, voltage limits, input thresholds, and current limits.
- Use an original labelled schematic and a Falstad simulation if permission and reuse terms allow it.
