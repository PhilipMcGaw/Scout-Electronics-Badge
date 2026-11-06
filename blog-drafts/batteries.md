# Batteries: capacity, current, and voltage under load

**Status:** Outline started; draft not written.

**Purpose:** Explain why a battery's stated voltage does not tell the whole story about how it will perform in a circuit.

**Source note:** The user supplied transcripts headed “Battery capacity”, “Batteries in series and parallel”, and “Challenge: Power a light bulb”. The last is a motor challenge; “light bulb” was a mistaken pasted heading. The matching exercise handout is titled “Challenge: Combine batteries in series and/or parallel to power a motor”. Use them as background, correct their simplifications and arithmetic, and write original explanations.

## Planned outline

1. Distinguish voltage, current, power, and stored energy in plain language.
2. Explain battery capacity and what a capacity rating can and cannot tell you about operating time.
3. Introduce internal resistance and show why terminal voltage can fall when a load draws current.
4. Compare a battery's open-circuit voltage with a suitable under-load measurement.
5. Explain series and parallel cell arrangements, their nominal voltage and capacity effects, and why matched, manufacturer-approved packs are essential.
6. Use a simple, low-voltage circuit or Falstad simulation to show how changing the load affects voltage and current.
7. Explain how battery type, condition, temperature, and load affect the result; check the manufacturer's data for the actual cell.

## Notes to carry forward

- The *Basic Electronics* source includes battery capacity, internal resistance, and voltage-drop examples. Explain internal resistance as the battery’s opposition to current inside the cell: under load it contributes to the difference between open-circuit voltage and terminal voltage. Treat it as an equivalent model whose value depends on chemistry, state of charge, temperature, age, and measurement conditions, not a single universal constant. Its car-starting example is not suitable for this beginner-oriented article; use a small, current-limited low-voltage example instead.
- Do not short a battery, use an unknown load, or deliberately heat a resistor. Select any demonstration load from its calculated current and power, check its rating, and keep it within safe operating limits. If illustrating internal resistance from voltage readings, use only a manufacturer-approved test method with a known, suitable load; never infer it by short-circuit testing.
- Distinguish energy capacity from the maximum current a cell can safely supply. Do not imply that a larger capacity rating alone guarantees a longer runtime in every circuit.
- Define amp-hours (`Ah`) and milliamp-hours (`mAh`) as charge capacity, distinct from current (`A` or `mA`). One amp-hour equals 3,600 coulombs. A rough runtime estimate is rated capacity divided by average load current, but only as a starting estimate: the rating depends on test current, temperature, and cutoff voltage, and delivered capacity changes with discharge rate and use pattern. Use `1,000 mAh ÷ 10 mA = 100 h` only as an idealised calculation, not a runtime promise. Never infer safe maximum current from capacity.
- Explain nominal voltage as a designated approximate value, not the voltage at the halfway point of discharge. Battery voltage under load and during discharge depends on chemistry, condition, load, temperature, and state of charge. Do not imply every battery’s voltage declines in the same way.
- Compare nominal cell voltage by chemistry, not just by physical size. Common rechargeable NiCd and NiMH cells are typically 1.2 V per cell; alkaline primary cells of the same size are typically 1.5 V. Explain that this can affect compatibility, but do not imply all rechargeable chemistries have a 1.2 V nominal voltage. Check the device and exact cell datasheets.
- Apply the series example to the Woggle: its holder takes two AAA cells in series. Two alkaline cells are nominally 3.0 V; two NiCd or NiMH cells are nominally 2.4 V. Check the Woggle's allowed supply range before recommending a chemistry substitution.
- Explain that matched cells in series add nominal voltage while the pack's amp-hour capacity remains approximately that of one cell. The same current passes through each series cell; for a fixed resistive load, adding series cells raises the voltage and changes the current drawn. Do not say series connection leaves each cell's discharge rate unchanged without specifying the load.
- Explain that a designed parallel pack keeps approximately one cell's voltage and can increase capacity, but do not claim the current divides equally or that maximum current ratings simply add unless exact cell and pack data support it. Do not recommend that readers connect loose cells in parallel; use only manufacturer-approved packs and protection.
- Use matched cells of the same chemistry, type, age, and state of charge as specified by the manufacturer. Do not mix old and new cells: they can discharge unevenly, potentially over-discharging the weaker cell and causing leakage or damage. Keep parallel-pack construction out of the Scouts activity.
- Do not repeat the transcript's generic AA examples (50 mA typical drain, 100 mA for a two-cell parallel pack, or 4,800/7,200 mAh totals) without a specific cell datasheet and test conditions. The 20 Ω / 1.5 V arithmetic gives 75 mA in an ideal circuit, but does not prove a particular cell can safely provide that current.
- Do not copy the transcript’s capacity figures or current capabilities for AAA and D cells without the exact cell datasheets and their test conditions. Do not suggest that an amp-hour rating allows arbitrary current-time trades (for example, tens of amps for minutes).
- The exercise handout's alkaline-cell chart gives examples for 9 V, AAA, AA, C, and D cells: nominal voltages of 9 V or 1.5 V, typical drain currents of 15, 10, 50, 100, and 200 mA respectively, and capacities of 500, 1,000, 2,400, 6,000, and 13,000 mAh respectively. These are values printed in that course handout, not universal specifications; do not use them as current product data or a design guarantee.
- The motor-sizing challenge specifies 6 V, 150 mA, and 48 h, an idealised charge requirement of `150 mA × 48 h = 7,200 mAh` at that load. Four D cells in series are a candidate under the handout's simplified chart (6 V, 13,000 mAh, 200 mA typical drain), but the chart does not provide enough test conditions to establish runtime, and the motor's start/stall current must also be checked. Treat this only as an exercise answer, not a real pack recommendation. Do not recommend loose cells wired in parallel.
- The transcript's 9 V, 10 kΩ example should calculate to `0.9 mA`, not `9 mA`. Its 9 V across 2 Ω calculation gives an ideal demand of `4.5 A`, but this is not a safe battery test and must not be used to claim a generic 9 V battery can provide that current.
- Link to the [electronics fundamentals post](electronics-fundamentals.md) for the basic voltage, current, resistance, and power relationships.
- Keep the explanation applicable to low-voltage battery-powered projects. Do not include mains-derived supplies or mains construction.

## Sources and visuals

- Check current manufacturer datasheets for the chosen battery chemistry, capacity test conditions, internal resistance information, discharge limits, and temperature range.
- For terminology and alkaline-cell examples, use the manufacturer’s [battery glossary](https://data.energizer.com/battery-glossary-faq/) and [alkaline application manual](https://data.energizer.com/pdfs/alkaline_appman.pdf), then check the current datasheet for the exact cell used.
- For nominal-voltage examples, use [Panasonic’s battery chemistry guide](https://www.panasonic.com/global/energy/study/academy/battery-structure.html) alongside a datasheet for the specific alkaline cell.
- Follow the manufacturer's [battery-use guidance](https://www.panasonic.com/global/energy/products/battery/dry_batteries_faq.html) on using matched cells and avoiding mixed or incorrectly installed batteries.
- Use an original circuit diagram or a clearly attributed Falstad simulation if permission and reuse terms allow it.
