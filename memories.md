# Project memories

This is the durable working context for the Scouts Electronics Activity Badge project. It records useful decisions and preferences across conversations; it is not a transcript or a task list. Current actions are tracked in [TODO.md](TODO.md).

## 2026-11-07 — H-bridge motor-driver article assessed

- **Source assessment:** Circuit Digest’s 2019 article provides an introduction to diagonal switching, but its high-current circuit claims and some switching explanations need independent review. Its schematic and images were not reused.
- **Technical cross-check:** TI documentation confirms that an H-bridge must manage inductive motor current during switching and avoid shoot-through; integrated drivers may insert dead time and define current paths. No specific motor or driver has been selected for this project.
- **Project outcome:** Added an adult-facing conceptual draft. It is not construction guidance and remains outside the Scouts booklet; a specific motor/driver datasheet review is required before adding build instructions. See [TODO.md](TODO.md).

## 2026-11-07 — PMOS reverse-polarity protection article assessed

- **Source assessment:** Components101’s 2020 guide is a useful topic introduction, but its suggested values and MOSFET selection shortcuts should not be treated as a ready-made design. Its diagrams and simulation were not reused.
- **Technical cross-check:** onsemi application note AND90146/D explains the P-channel MOSFET body diode and gate clamp, and stresses checking the actual device ratings and thermal conditions. Automotive transient requirements in that note are outside the scope of the general low-voltage draft.
- **Project outcome:** Added an adult-audience first draft on reverse-polarity protection. A specific circuit and exact component datasheets still need review before publication; see [TODO.md](TODO.md).

## 2026-11-07 — DFRobot Arduino beginner tutorial assessed

- **Repository fact checked:** The 133-page DFRobot tutorial covers Arduino setup, LED flashing, buttons and pull-ups, traffic lights, PWM fading/RGB LEDs, buzzers, sensors, servos, and IR projects. Its PDF metadata dates from 2015; it includes legacy Windows driver and IDE setup steps.
- **Source assessment:** Button-input and PWM explanations are useful starting topics, but board pinouts, logic levels, PWM support, library APIs, and electrical limits must be checked against current Arduino documentation and the selected board. Do not copy the tutorial’s diagrams or code; reuse rights were not established.
- **Project outcome:** First drafts now cover button inputs/pull-ups and PWM LED fading. Before publication, verify each with the chosen board and parts; see [TODO.md](TODO.md).

## 2026-11-07 — Trimmer-potentiometer image assessed

- **Repository fact checked:** `Source Documents/IMG_4103.JPG` shows a trimmer potentiometer, its wiper and terminals, and example three-digit resistance codes. The `103` = 10 kΩ example is consistent with Bourns Trimpot documentation; markings and pin layout must still be checked against the exact manufacturer and part.
- **Source/licensing assessment:** The image bears a visible “Rizwan Khan” signature, but its origin and reuse licence are not recorded. Do not reproduce it without verifying rights; use a licensed manufacturer drawing or original diagram if a visual is needed.
- **Project outcome:** The resistor article outline now includes trimmer operation and qualified resistance-code examples; the Scouts booklet is unchanged.

## 2026-11-07 — Lithium-ion label image assessed

- **Repository fact checked:** `Source Documents/IMG_3816.JPG` compares ICR, INR, IMR, NCR, and IFR cylindrical-cell labels. It assigns broad capacity and discharge-rate rankings by family and gives one nominal/charge voltage pair per chemistry. Those generalisations are not specifications for individual cells.
- **Source/licensing assessment:** The image creator and licence are not recorded; do not reproduce it in a blog post.
- **Project outcome:** Two adult-audience drafts now cover chemistry-code shorthand and how to read cell datasheets. This topic is outside the Scouts booklet. Exact manufacturer data is still needed before publication; see [TODO.md](TODO.md).

## 2026-11-07 — Battery glossary adapted for booklet and blog drafts

- **Source assessment:** The supplied *Battery A to Z* glossary is most useful for explaining capacity under specified conditions, internal resistance, state of charge, state of health, battery management, cell balancing, and thermal management in larger packs. Its vehicle-scale details and figures should not be presented as household-cell specifications.
- **Project outcome:** Two first drafts now cover battery capacity and voltage under load, and battery-pack monitoring and thermal management. The booklet adds a short BMS and state-of-charge/state-of-health explanation. Drafts still need exact manufacturer data if named cells or packs are added; see [TODO.md](TODO.md).

## 2026-11-06 — Converted *Electronics For Dummies* reviewed

- **Repository fact checked:** The converted 433-page copy is readable; the earlier statement that *Electronics for Dummies.pdf* was encrypted refers to the original copy and does not apply to the converted PDF.
- **Source assessment:** The 2005 US-oriented book mostly overlaps with the existing booklet. Its breadboard chapter usefully explains internal contact groups and prototyping before soldering. The Scout booklet and Leaders’ Guide now include concise, UK-appropriate breadboard notes, and the blog index includes a possible breadboard-prototyping post. The separate review records scope and cautions: [Electronics For Dummies review](Source%20Documents/Electronics-for-Dummies-review.md).
- **Open action:** Verify layouts and ratings against a specific breadboard and circuit before developing the standalone article; see [TODO.md](TODO.md).
- **User-reported decision:** The converted source PDF is not needed in the repository; it was removed on 2026-11-07. The review note and project drafts retain the useful breadboard findings and source assessment.

## 2026-11-07 — 2021 course handouts assessed

- **Source assessment:** The five course handouts’ useful points are carried in the fundamentals, resistor, and battery drafts. The parts list matches the saved summary but has US-oriented sales links and no circuit diagram; do not reuse its imagery without checking rights. The DMM sheet names models without specifications, so check current manuals and UK suitability before making recommendations. See the [review note](Source%20Documents/Electronics-Foundations-Fundamentals-2021-review.md) and [TODO.md](TODO.md).
- **User-reported decision:** The user reviewed the DMM list PDF and said it does not need to be retained. The file was removed; its model names and lack of specifications remain in the source review note. The separate current-manual check remains open.
- **Follow-up decision:** The user said the whole course folder could be removed if its files were no longer needed. After confirming the useful content and open checks are recorded in project notes, all remaining course PDFs were removed; the review note retains their summaries.

## 2026-11-06 — Consolidated project context

### Project, audience, and structure

- **Project fact:** This repository develops the Scouts Electronics Activity Badge booklet and supporting learning resources. The main booklet is [Scouts Electronics Activity Badge Booklet.md](Scouts%20Electronics%20Activity%20Badge%20Booklet.md); print instructions from the original booklet were to be ignored during conversion.
- **Audience decision:** Write the main booklet for Scouts and Explorers aged 10–16, with an adult Leader supporting activities. Keep the explanations practical and age-appropriate. A separate Leaders’ Guide can hold leader-facing safety controls and advanced material.
- **Scope decision:** Keep the main practical work low-voltage and through-hole, using the Woggle PCB with LEDs and a small DIP-8 microcontroller. Surface-mount soldering and PCB rework are optional advanced reading for a blog post or annex, not core Woggle activities. Exclude mains wiring instruction.
- **Regional context:** This is a UK-centric project. US or other territory material can use different standards, symbols, safety rules, suppliers, and terminology; verify it against current UK sources before adopting it. Use ISO/IEC schematic symbols as the default, with only a brief note that ANSI-style symbols also exist.

### Editorial and technical decisions

- **House style:** Use British English, clear conversational explanations, and SI units with a space between value and unit (for example, `400 °C`). Retain the source wording only when it is a quotation; distinguish it from editorial explanation and Philip’s own experience.
- **Current direction:** Use conventional current in the main explanations: current flows from positive to negative. Electron flow may be mentioned in an advanced note or as a clearly labelled trick question.
- **LEDs:** A bare LED needs a current-limiting resistor. Explain that increasing current generally increases brightness and heating, but excessive current can damage the LED. About 20 mA is a sensible upper working limit for many 3 mm and 5 mm LEDs, subject to the component datasheet.
- **Other component cautions:** Include warnings against deliberately overheating resistors and against reversing electrolytic capacitors. Thermistors are more relevant to Philip’s projects than LDRs. Put voltage dividers in the resistor material and link the existing [potential-divider calculator](https://philipmcgaw.com/potential-divider-calculator/).
- **Batteries:** The Woggle uses two AAA cells in series. Explain that series adds voltage, that rechargeable NiCd/NiMH cells have lower nominal voltage than alkaline cells of the same size, and that users should not mix old and new cells. Consider internal resistance and real load limits when discussing battery performance. Do not imply a battery’s stated capacity guarantees a particular runtime.
- **Adapters and grounding:** UK/EU low-voltage AC-to-DC adapters are commonly isolated and floating, rather than Earth-referenced; check the specific adapter. Do not suggest combining adapters or grounded sources in series. Keep mains work outside the Scout activity.
- **Multimeters:** Explain that a current measurement is made in series and that accidentally measuring voltage while configured for current can blow the meter’s fuse. Describe at a high level that a fuse opens the circuit to protect the meter; do not say the meter necessarily “breaks”. Check current UK suitability and the actual manual before recommending a model.
- **Static electricity:** A balloon static-electricity activity belongs in the booklet, not as a separate blog article.
- **Image policy:** Do not create AI images for the booklet. Use supplied or appropriately licensed material with attribution. For Charlieplexing, Philip intends to draw an original diagram or make a Falstad simulation; do not reuse `CharliePlex.GIF` unless its licence is cleared.

### Philip’s reported workshop preferences

These are Philip’s statements about his own equipment and methods, not universal instructions or independently verified product guidance:

- He has two temperature-controlled soldering irons: a small USB-C iron and a benchtop iron with a hot-air rework station. He normally sets the iron to 400 °C and the hot-air station to about 400 °C. He also has a small hot plate.
- He does not use a soldering-iron timer and does not keep isopropyl alcohol in a COSHH cabinet. Do not write booklet text that claims otherwise about his practice.
- His helping hands/vice use a magnetic base. He replaced the aluminium base on his USB microscope with a steel one. Blu Tack is also useful to him for holding parts still.
- He prefers stranded-core wire because it is more flexible, and tins the wire before attaching it to a switch. On a multipin component, after soldering some pins he reflows the first pin to relieve stress from the component settling and to add solder if needed.
- For hand-soldered SMDs, he dislikes drag soldering and prefers feeding solder to one pin at a time. Flux pens are essential in his SMD work. He commonly works with 0805 and sometimes 0604 parts; smaller parts are possible but difficult. His preferred upper limit for hand-soldered IC pitch is 1.27 mm SOIC.

### Tools, suppliers, and publishing

- **ECAD and boards:** Philip uses KiCad. Eagle is deprecated and Autodesk has moved it into Fusion 360; KiCad is preferred for usability, and KiCad can open Eagle files. PCBWay is the PCB manufacturer Philip uses. The Woggle tutorial should cover KiCad setup, changing the group name, producing a BOM, selecting components, and sending the board files to PCBWay.
- **Parts suppliers:** Prefer Pimoroni and The Pi Hut where suitable; Kitronik is a suggested UK supplier for educational kits and electronics parts. SparkFun may be recommended with a clear label that it is US-based and overseas delivery charges may apply.
- **Simulation and articles:** Philip commonly embeds Falstad Circuit Simulator in blog posts using an iframe. Self-hosting its JavaScript or making a WordPress plugin is a possible future project, not an implemented feature.
- **Blog workflow:** Keep one Markdown file per planned post in `blog-drafts/`. Blog posts can provide more detail than the booklet. WordPress access is expected to be available later from another computer; see [TODO.md](TODO.md) for the queued updates and broken-page diagnosis.

### Source material and provenance

- Treat course transcripts, PDFs, product pages, and supplied images as source material, not as automatically correct local guidance. Preserve attribution and verify safety, electrical values, and regional applicability before publication.
- The reviewed course-exercise PDFs contained useful SI-prefix, DMM, LED-current-limit, and battery-sizing material. The battery challenge’s figures are teaching examples without manufacturer, model, or test-condition basis; do not present their capacities or runtime calculations as guarantees. The exercise describes a motor, despite transcript headings that called it a light bulb. All course PDFs were removed after review; the [course materials review](Source%20Documents/Electronics-Foundations-Fundamentals-2021-review.md) and related drafts retain needed details.
- Some source-course material was US-oriented. Its DMM models, suppliers, power-source examples, and safety claims need current UK checks before use. The course parts-list PDF was visually checked against the item summary in the fundamentals draft; its shop links were US-oriented and it showed no circuit connections. The DMM models still need current manual checks before any recommendation. See TODO.md.
- `Electronics for Dummies.pdf` was encrypted and could not be reviewed; Philip said he may revisit it later.
- Useful existing web articles include [learn about resistors](https://philipmcgaw.com/learn-about-resistors/), [capacitors](https://philipmcgaw.com/capacitors/), [LED resistor values](https://philipmcgaw.com/led-resistors-values/), [Ohm’s and Watt’s laws](https://philipmcgaw.com/ohms-law-and-watts-law/), [capacitor value prefixes](https://philipmcgaw.com/capacitor-value-prefixes/), and [special symbols in engineering reports](https://philipmcgaw.com/special-symbols-used-in-engineering-reports/). Related revisions and other article ideas are tracked in `TODO.md` and `blog-drafts/`.

### Current project state

- **Repository fact checked 2026-11-06:** `TODO.md` is the action index. It includes the Leaders’ Guide, illustration, blog planning and drafting, WordPress updates, KiCad/PCBWay walkthrough, Charlieplexing visual, silkscreen post, and advanced PCB rework post. Check it for current status instead of relying on this memory entry.
- **Source notes:** PDF review notes are stored under `Source Documents/`. Their conclusions and open checks belong to those notes; consult the relevant source note before reusing detailed findings.
- **Git:** Project changes are expected to be committed and pushed to the repository’s `main` branch. Follow the Git workflow in `AGENTS.md`, stage only task-related files, and preserve unrelated changes.
