# Batteries: capacity, current, and voltage under load

**Status:** Outline started; draft not written.

**Purpose:** Explain why a battery's stated voltage does not tell the whole story about how it will perform in a circuit.

**Source note:** The user supplied a transcript headed “Battery capacity”. Use it as background, correct its simplifications and arithmetic, and write original explanations.

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
- Define amp-hours (`Ah`) and milliamp-hours (`mAh`) as charge capacity, distinct from current (`A` or `mA`). One amp-hour equals 3,600 coulombs. A rough runtime estimate is rated capacity divided by average load current, but only as a starting estimate: the rating depends on test current, temperature, and cutoff voltage, and delivered capacity changes with discharge rate and use pattern. Use `1,000 mAh ÷ 10 mA = 100 h` only as an idealised calculation, not a runtime promise. Never infer safe maximum current from capacity.
- Explain nominal voltage as a designated approximate value, not the voltage at the halfway point of discharge. Battery voltage under load and during discharge depends on chemistry, condition, load, temperature, and state of charge. Do not imply every battery’s voltage declines in the same way.
- Compare nominal cell voltage by chemistry, not just by physical size. Common rechargeable NiCd and NiMH cells are typically 1.2 V per cell; alkaline primary cells of the same size are typically 1.5 V. Explain that this can affect compatibility, but do not imply all rechargeable chemistries have a 1.2 V nominal voltage. Check the device and exact cell datasheets.
- Do not copy the transcript’s capacity figures or current capabilities for AAA and D cells without the exact cell datasheets and their test conditions. Do not suggest that an amp-hour rating allows arbitrary current-time trades (for example, tens of amps for minutes).
- The transcript's 9 V, 10 kΩ example should calculate to `0.9 mA`, not `9 mA`. Its 9 V across 2 Ω calculation gives an ideal demand of `4.5 A`, but this is not a safe battery test and must not be used to claim a generic 9 V battery can provide that current.
- Link to the [electronics fundamentals post](electronics-fundamentals.md) for the basic voltage, current, resistance, and power relationships.
- Keep the explanation applicable to low-voltage battery-powered projects. Do not include mains-derived supplies or mains construction.

## Sources and visuals

- Check current manufacturer datasheets for the chosen battery chemistry, capacity test conditions, internal resistance information, discharge limits, and temperature range.
- For terminology and alkaline-cell examples, use the manufacturer’s [battery glossary](https://data.energizer.com/battery-glossary-faq/) and [alkaline application manual](https://data.energizer.com/pdfs/alkaline_appman.pdf), then check the current datasheet for the exact cell used.
- For nominal-voltage examples, use [Panasonic’s battery chemistry guide](https://www.panasonic.com/global/energy/study/academy/battery-structure.html) alongside a datasheet for the specific alkaline cell.
- Use an original circuit diagram or a clearly attributed Falstad simulation if permission and reuse terms allow it.
