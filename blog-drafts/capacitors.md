# Capacitors: markings, polarity, and charge

**Status:** Outline started; draft not written.

**Existing articles:** [Capacitor Basics](https://philipmcgaw.com/capacitors/) and [Capacitor value prefixes](https://philipmcgaw.com/capacitor-value-prefixes/).

**Purpose:** Build on the concise existing post with practical ways to identify capacitors and understand what happens in a simple circuit.

## Planned outline

1. What capacitance means and how a capacitor differs from a battery and an inductor.
2. Recognise common units and read typical ceramic-capacitor markings.
3. Identify polarised and non-polarised parts; explain polarity and voltage rating, and what can happen if a polarised electrolytic capacitor is connected backwards.
4. Show a resistor-capacitor charge and discharge circuit, including the time constant.
5. Use a Falstad simulation to explore how changing resistance or capacitance changes the timing.
6. Note practical limits: real components have tolerances and other non-ideal properties.

Use the course’s teaching progression as a conceptual guide: first show that a capacitor charges and discharges over time through a resistor, then explain that a transistor can use the changing capacitor voltage to switch another part of the circuit. Derive any example circuit, values and operating limits independently; do not copy the course’s 9 V kit diagrams or body-contact/pencil-probe activities.

## Notes to carry forward

- The existing post covers capacitor uses, charge, energy, and the RC time constant.
- Review the value-prefix article before reusing its table. It lists 1 mF as 0.0001 F; the correct conversion is 0.001 F, and “millifarard” is a spelling error. It also presents electrolytic capacitors as more common above about 100 nF, which must not be treated as a technology boundary: ceramic and film types are also available at higher capacitances, as shown in [KEMET’s capacitor range](https://www.kemet.com/en/us/capacitors.html). Recheck every prefix, marking, and technology comparison against current references before publication.
- Reader comments ask for clearer definitions of symbols and a comparison with battery and inductor energy storage.
- Do not imply that all capacitors above or below a particular value use one construction or have the same polarity rules.
- Iain Sharp’s 2010 [Electronics for Absolute Beginners](https://lushprojects.com/absolutebeginners/) notes offer a simple RC charge/discharge activity followed by transistor-based timing circuits. The companion parts list includes 10 µF and 100 µF axial capacitors rated at 15 V or more, alongside ceramic capacitors from 470 pF to 100 nF; treat these as historical kit choices, not a recommended bill of materials. This sequence can help explain how a gradual capacitor-voltage change becomes a switching action. The notes’ broad shortcut that capacitors below 1 µF are usually non-polar and larger ones usually polarised is not a reliable selection rule. Identify polarity from the exact part and datasheet, and verify voltage, resistor current and capacitor discharge conditions before adapting any experiment. The notes are CC BY-NC-SA 3.0 Unported; do not reproduce their wording or figures without meeting the licence terms.
- A useful overview is All About Circuits’ [“X7R, X5R, C0G…: A Concise Guide to Ceramic Capacitor Types”](https://www.allaboutcircuits.com/technical-articles/x7r-x5r-c0g...-a-concise-guide-to-ceramic-capacitor-types/), but treat it as an introduction. X7R/X5R describe Class 2 temperature characteristics; C0G/NP0 is a Class 1 dielectric with much better temperature stability. Do not let the temperature code imply that the nominal capacitance stays constant under operating voltage: Class 2 MLCCs can lose substantial capacitance under DC bias, and can also age. Check the exact part’s datasheet at the actual bias and temperature.
- Class 2 ceramics can also produce or respond to mechanical vibration (often called piezoelectric or electrostrictive behaviour), which can make audible noise in some circuits. This is an application-dependent effect, not a reason to describe all X7R/X5R parts as unsuitable for audio.
- Keep the EIA temperature code explanation tied to its specified temperature range and capacitance-change class. Do not present it as a complete description of tolerance, DC-bias behaviour, ageing, voltage rating, or suitability for a circuit.
- Murata’s [temperature-characteristics guide](https://article.murata.com/en-us/article/temperature-characteristics-electrostatic-capacitance) is a useful manufacturer explanation of Class 1 temperature coefficients versus Class 2 capacitance-change ranges. It also distinguishes the temperature code from voltage-bias and ageing behaviour. Cite it alongside the actual part datasheet; its standard tables and examples may not cover every current regional standard or product.
- Explain that a reversed aluminium electrolytic can heat up and fail; use a manufacturer source such as [KEMET’s aluminium electrolytic capacitor data sheet](https://content.kemet.com/datasheets/KEM_A4093_ALA8A.pdf), and keep the practical advice simple: check the capacitor markings and circuit before connecting power.

## Sources and visuals

- Check component markings and ratings against manufacturer datasheets.
- KEMET, [Ceramic Capacitor FAQ and Application Guide](https://www.kemet.com/en/us/capacitors/ceramic/ceramics-faq.html), for Class 2/Class 3 DC-bias effects and the need to check capacitance under operating conditions.
- TDK, [CeraLink technical article on DC-bias effects](https://www.tdk-electronics.tdk.com/en/373562/tech-library/articles/applications-cases/applications-cases/ceralink/3472416), with comparative Class I/Class II capacitance behaviour.
- Murata, [“What is the temperature characteristics of ceramic capacitors?”](https://article.murata.com/en-us/article/temperature-characteristics-electrostatic-capacitance), final revision 2023-12-01, for Class 1 temperature coefficients and Class 2 capacitance-change categories.
- Murata, [Class 1 versus Class 2 ceramic capacitor FAQ](https://www.murata.com/en-us/support/faqs/capacitor/ceramiccapacitor/char/0017), comparing temperature, DC-bias and ageing characteristics.
- Use an original circuit diagram or a clearly attributed simulation screenshot if permission and reuse terms allow it.
