# Batteries: capacity, current, and voltage under load

**Status:** Outline started; draft not written.

**Purpose:** Explain why a battery's stated voltage does not tell the whole story about how it will perform in a circuit.

## Planned outline

1. Distinguish voltage, current, power, and stored energy in plain language.
2. Explain battery capacity and what a capacity rating can and cannot tell you about operating time.
3. Introduce internal resistance and show why terminal voltage can fall when a load draws current.
4. Compare a battery's open-circuit voltage with a suitable under-load measurement.
5. Use a simple, low-voltage circuit or Falstad simulation to show how changing the load affects voltage and current.
6. Explain how battery type, condition, temperature, and load affect the result; check the manufacturer's data for the actual cell.

## Notes to carry forward

- The *Basic Electronics* source includes battery capacity, internal resistance, and voltage-drop examples. Its car-starting example is not suitable for this beginner-oriented article; use a small, current-limited low-voltage example instead.
- Do not short a battery, use an unknown load, or deliberately heat a resistor. Select any demonstration load from its calculated current and power, check its rating, and keep it within safe operating limits.
- Distinguish energy capacity from the maximum current a cell can safely supply. Do not imply that a larger capacity rating alone guarantees a longer runtime in every circuit.
- Link to the [electronics fundamentals post](electronics-fundamentals.md) for the basic voltage, current, resistance, and power relationships.
- Keep the explanation applicable to low-voltage battery-powered projects. Do not include mains-derived supplies or mains construction.

## Sources and visuals

- Check current manufacturer datasheets for the chosen battery chemistry, capacity test conditions, internal resistance information, discharge limits, and temperature range.
- Use an original circuit diagram or a clearly attributed Falstad simulation if permission and reuse terms allow it.
