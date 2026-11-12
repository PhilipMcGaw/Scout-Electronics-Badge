# Project memories

## 2026-11-11 — Voltage-divider level-shifting guidance

- **Source assessment:** The user supplied the “Shift voltage levels” transcript. Cover resistor dividers only as limited one-way signal interfaces after checking exact pin limits, thresholds, loading, speed and direction. Do not generalise the course’s 5 V/3.3 V Arduino/accelerometer example, use a divider for a supply, or adapt its wall-adapter example for Scouts; Scout circuits remain limited to 12 V DC.

## 2026-11-11 — Voltage-divider lesson assessed

- **Source assessment:** The user supplied the “Voltage dividers” transcript and a diagram frame showing the divider formula. The diagram uses the correct R2 numerator; the transcript says R1 once, then gives the correct R2 ratio. The resistor article plan covers the unloaded formula and load effect. Do not reuse the course frame without image rights.

## 2026-11-11 — Series-resistor lesson assessed

- **Source assessment:** The user supplied the “Resistors in series” transcript. The resistor article plan now covers resistance sums, worst-case tolerance bounds, same-current power calculations for each part, and separate voltage/power/thermal checks. The transcript’s 20 mA across 3 kΩ example requires 60 V and is outside the 12 V DC maximum for Scout circuit activities; do not use it as a Scout example.

## 2026-11-11 — Resistor-types knowledge check

- **Project outcome:** Completed the six-question resistor-types knowledge check in the booklet. Use “fixed-value resistor” in place of the source quiz’s “static resistor”; describe through-hole as a leaded package style that fits standard breadboards; distinguish working voltage from power and time-limited overload ratings; explain tolerance as a percentage range around nominal resistance; present wider band spacing as a clue, not a guarantee; isolate a resistor for an individual resistance reading when parallel paths could affect it.

## 2026-11-11 — Resistance measurement guidance

- **Source assessment:** The user supplied the “Measure resistance” course transcript. The resistor article outline now calls for safe DMM measurement, model-specific manual instructions, power-off and capacitor-discharge precautions, isolating a resistor to avoid parallel paths, and consideration of meter accuracy. Do not repeat the body-resistance demonstration.

## 2026-11-11 — Cover preferred resistor values

- **User direction:** Include a brief explanation of standard resistor values in the resistor article. Distinguish IEC 60063 E-series preferred values (for example, E12/E24/E96) from the EIA-96 SMD marking code.

## 2026-11-11 — Resistor code calculator

- **Project outcome:** Built a standalone browser calculator for 4-, 5- and 6-band resistor colour codes and common SMD 3-digit, 4-digit, R-notation and EIA-96 markings. The tool labels scheme limits and links to Vishay references. The refreshed article still needs the calculator hosted and linked.

## 2026-11-11 — Resistor colour-code transcript assessed

- **Source assessment:** The user supplied the “Read resistor color codes” lesson transcript. The blog outline now calls for worked four- and five-band examples, tolerance ranges, reading direction, and a note on six-band TCR and SMD code variation. Do not infer precision from band count alone or reuse the course chart without cleared rights.
## 2026-11-11 — Resistor voltage ratings in blog

- **User direction:** Include a small note on resistor maximum working voltage and overvoltage/overload ratings because it is relevant to one of the user’s projects. Keep the project unnamed; distinguish continuous operation from short-duration ratings and check exact datasheet conditions.
## 2026-11-11 — Lead-free and RoHS context for resistor blog

- **User direction:** Include lead-free resistor finishes and RoHS regulations in the resistor blog. Explain the distinction between component lead-free claims, solder alloy, and finished-equipment compliance; verify UK scope, limits, exemptions, and GB/NI differences against current official guidance.
## 2026-11-11 — Resistor technology comparison for blog

- **User direction:** Expand the resistor article to compare construction types by price, initial tolerance/accuracy, and thermal stability. Treat any ordering as a sourced trend, not a universal rule; distinguish initial tolerance from temperature coefficient and long-term drift, and verify exact technical data and current UK prices.

## 2026-11-10 — Resistor characteristics transcript assessed

- **Source assessment:** Reviewed the user-pasted “Resistor characteristics” transcript. The booklet now covers tolerance, maximum working voltage, power derating, and finding the exact part datasheet. The source review corrects its carbon-film/carbon-composition conflation and flags its approximate resistance cutoff as unsuitable general guidance.

## 2026-11-10 — Thermistor preference

- **User-reported preference:** Philip uses thermistors more often than LDRs (photoresistors). In resistor teaching, distinguish temperature-responsive and light-responsive resistors from hand-adjusted potentiometers and rheostats; use thermistors as the preferred sensor example where appropriate.

## 2026-11-10 — SMD resistor package preference

- **User-reported workshop preference:** Philip normally uses 0805 SMD resistors. Treat 0805 as his usual package choice, not a project-wide requirement; check the PCB footprint, power rating, and availability for each design.

## 2026-11-10 — Through-hole resistor power preference

- **User-reported workshop preference:** Philip commonly uses ¼ W through-hole resistors because they are readily available. Treat this as a practical preference, not a default rating for every circuit; calculate dissipation and check the component rating and suitable margin.

## 2026-11-10 — Fixed-value resistor terminology

- **User preference:** Use “fixed-value resistor” rather than “static resistor” or the shorter “fixed resistor” in project teaching text.

## 2026-11-10 — Resistor types transcript assessed

- **Source assessment:** The user supplied the “Types of resistors” transcript from LinkedIn Learning’s *Electronics Foundations: Basic Circuits*. Useful coverage includes standard series for fixed-value resistors, through-hole versus surface-mount packages, power ratings, potentiometer/rheostat use, and LDR behaviour. The booklet now explains these with qualifications; see the course [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|source review]].

## 2026-11-10 — Schematic knowledge-check item

- **Project outcome:** Completed the four-question booklet breadboard check. The questions cover jumper terminology, schematics as graphical representations, solid-core wire for bare breadboard jumpers, and the difference between schematic and physical layout. Leader answers are included.


## 2026-11-10 — Breadboard jumper knowledge check

- **Project outcome:** Added a short booklet knowledge-check question distinguishing a jumper wire from a breadboard power bus, resistor, and power supply; the Leader answer identifies ‘jumper’ or ‘jumper wire’.


## 2026-11-10 — Breadboard supply module assessment

- **Source assessment:** Checked the user-suggested Pimoroni listing against the manufacturer’s WPM467 page and manual. The module accepts 5 V via USB-C or 7–12 V DC via barrel jack, supplies 3.3/5 V rails up to 500 mA, and fits MB-102-compatible 830-point breadboards. Pimoroni no longer stocks this model; the booklet identifies it as a technical example, not a purchase recommendation.

## 2026-11-10 — Breadboard photo and supplier example

- **Project outcome:** Added a Wikimedia Commons public-domain photo by Evan-Amos beside the booklet's solderless-breadboard guidance, with source/licence credit, and linked The Pi Hut's 400-point half-size breadboard as a supplier example. The image is embedded from Wikimedia Commons because network restrictions prevented a local download; confirm external-image loading in the target DokuWiki instance.


## 2026-11-10 — Repository inbox folder

- **User decision:** Add a repository-level `inbox/` for newly supplied project material awaiting review. Treat it as temporary intake, not a canonical DokuWiki or source-review location; move useful findings into the appropriate project page or source note and remove material when no longer needed.

## 2026-11-10 — IEC schematic-symbol preference

- **User preference:** Use IEC schematic symbols in project diagrams by default. ANSI/IEEE symbols may be explained as an alternate style when useful for recognising outside schematics. The user prefers resistor-value labels without the Ω symbol when context is clear, positive supply nodes pointing up, ground/0 V nodes pointing down, left-to-right signal flow, clear net names, and small jump-over bridges to mark non-joining crossings. When a board has physical layout requirements, note them on the schematic or an accompanying layout drawing instead of relying on schematic positions or line lengths. The booklet's schematic guidance reflects these preferences.

## 2026-11-10 — 12 V maximum for Scout circuit supplies

- **User decision:** Scout circuit activities must use battery or DC power-supply outputs no higher than 12 V. Check the maximum charged battery-pack output; the 12 V cap is a project limit, not a complete safety assessment. The user clarifies that the 50 V figure discussed in the course safety transcript refers to SELV context in BS 7671; SELV also has separation requirements, and the figure is not the Scout activity ceiling. See the booklet's [[pages/sites/scouts-electronics-badge/booklet.txt|Using this booklet]] safety scope and the course [[pages/sites/scouts-electronics-badge/sources/electronics-foundations-basic-circuits-review.txt|source review]].

## 2026-11-10 — Basic Circuits exercise bundle reviewed

- **Source assessment:** Reviewed the 2021 LinkedIn Learning exercise files and retained a topic map and editorial cautions in the [[pages/sites/scouts-electronics-badge/sources/electronics-foundations-basic-circuits-exercises-review.txt|source review]]. The bundle includes several resistor, sensor, RC, filter, and RL examples. The two analogue sketches assume a 5 V reference and 0–1023 ADC readings; one bridge challenge's light/dark conditions do not distinguish the states. A simple LDR potential-divider explanation was added to the booklet's light-sensitive alarm project; the supplied files were removed after review, and no course graphics or code were adopted.

## 2026-11-10 — Basic Circuits course transcript assessed

- **Source assessment:** Reviewed the user-pasted “Principles of basic electronic circuits”, “What you should know”, “Using the exercise files”, “Safety warnings”, “Read electrical schematics”, and “Build circuits on breadboards” transcripts and course description for Barron Stone’s LinkedIn Learning *Electronics Foundations: Basic Circuits*. They offer topic and teaching-sequence context for the fundamentals and breadboard drafts, but no verified circuit details in the supplied excerpts. The course expects basic algebra and logarithms; that is not a Scouts badge prerequisite. Its component and sinusoid claims need qualification; the 50 V statement has an SELV context and is not the Scout project's 12 V limit. “Filter surrogates” appears to be a transcription error. The course treats Arduino code as a circuit-interface demonstration, its parts list is not a current UK recommendation, and its breadboard layout and mains-adapter example are not universal Scout instructions. The schematic lesson prompted concise booklet clarifications on symbolic versus physical layout and reference designators. See the [[pages/sites/scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|source review]].

## 2026-11-10 — Blog index ordered as a suggested reading path

- **Project outcome:** Added an order column to the blog index, placing beginner fundamentals and the Woggle project first, followed by optional specialist topics. The numbers indicate suggested reading order, not publication priority.

## 2026-11-10 — Internal and external button pull-ups compared

- **Project outcome:** Expanded the Arduino button post with the wiring and firmware simplicity of internal pull-ups, the value and reset-state control available from external resistors, and the current/noise trade-off. Exact board behaviour remains subject to the selected microcontroller documentation and the existing TODO review.

## 2026-11-10 — Two buttons can share an input with switched bias

- **Project outcome:** Added a conceptual two-switch method that samples one pin with internal pull-up and pull-down modes. A centre-off, up/off/down SPDT rocker can make the two positions mechanically exclusive; verify its contact action. If using two independent pushbuttons, series current-limiting resistors in both branches are needed to limit current if both are pressed. Exact values and state readings need review against the selected board before publication; see [TODO.md](TODO.md).

## 2026-11-09 — Descriptive media filenames

- **User preference:** Give project images descriptive lowercase kebab-case filenames and keep DokuWiki media references aligned with file renames.

## 2026-11-09 — Canonical pages moved to DokuWiki layout

- **User decision:** Move the canonical booklet, Leaders’ Guide, blog drafts, source reviews, project landing page, and booklet images into the DokuWiki page and media paths under `pages/sites/scouts-electronics-badge/` and `media/sites/scouts-electronics-badge/`. Convert page content to core DokuWiki syntax and use fully qualified namespace IDs.
- **Workflow:** Source-controlled `.txt` pages are now canonical. The live DokuWiki instance still needs page, namespace, media, and link verification before its pages become an editing surface. No page-metadata convention is established; do not invent plugin metadata.
- **Follow-up:** Target-instance verification is tracked in [TODO.md](TODO.md).

## 2026-11-08 — Three-capacitor decoupling rule assessed

- **Source assessment:** Eric Bogatin, Larry Smith and Steve Sandler’s 2020 Signal Integrity Journal article, [“The Myth of Three Capacitor Values”](https://www.signalintegrityjournal.com/articles/1589-the-myth-of-three-capacitor-values), argues that the traditional decade-spaced capacitor recipe grew from older leaded-part assumptions and is not automatically appropriate for modern MLCC designs. It also discusses parallel resonances and the need to consider the full power distribution network.
- **Technical context:** The article is specialist and model-dependent. Do not generalise its preferred combinations or imply that decoupling capacitors can be removed. Specific IC datasheets and layout guides take precedence; placement, loop inductance, regulator stability and effective MLCC capacitance under DC bias all matter.
- **Project outcome:** Added a first draft in [decoupling capacitors draft](pages/sites/scouts-electronics-badge/blog/decoupling-capacitors.txt). Technical review against exact device documentation remains in [TODO.md](TODO.md).

## 2026-11-11 — Course decoupling lesson reviewed

- **Source assessment:** The pasted “Decoupling capacitors” transcript is a useful introduction to local supply decoupling and the difference between schematic grouping and physical placement. Its 100 nF plus 1 µF/10 µF suggestions are examples, not universal requirements, and the “drain AC noise to ground” analogy needs limits for real impedance, layout and return paths. Thermal noise should not be described as automatically removed by a shunt capacitor.
- **Project outcome:** Added the assessment to the [course review](pages/sites/scouts-electronics-badge/sources/electronics-foundations-basic-circuits-review.txt) and a concise treatment to the [fundamentals outline](pages/sites/scouts-electronics-badge/blog/electronics-fundamentals.txt). The dedicated [decoupling article](pages/sites/scouts-electronics-badge/blog/decoupling-capacitors.txt) remains subject to exact-device datasheet and layout review tracked in TODO.md.

## 2026-11-11 — PIC decoupling example added to draft

- **User-reported project example:** Philip’s 2022 CE-mark article shows before/after graphs labelled fail and pass, and attributes the difference to a 100 nF capacitor between Vcc and GND on a PIC microcontroller. The underlying test details are not established here; do not infer the exact measurement or generalise the result to every PIC design.
- **Project outcome:** Added this as a short case study with links to the original graphs in the [decoupling-capacitor draft](pages/sites/scouts-electronics-badge/blog/decoupling-capacitors.txt). Regulatory statements elsewhere on that older article require separate current-source checking.

This is the durable working context for the Scouts Electronics Activity Badge project. It records useful decisions and preferences across conversations; it is not a transcript or a task list. Current actions are tracked in [TODO.md](TODO.md).

## 2026-11-08 — Poeth SMD manufacturing article assessed

- **Source assessment:** Dean F. Poeth II’s overview for small manufacturers and hobbyists was originally published in *CQ* in 2003 and revised in 2004. It discusses manual SMD assembly, rework, tools, and component handling.
- **Technical context:** Treat its tool settings, adhesives, cleaning solvents, abrasive methods, and soldering materials as historical and specific to its context, not current universal advice. Its general workspace ideas (lighting, magnification, part containment, and practice on scrap boards) may be useful prompts.
- **Project outcome:** Added a qualified source note to the SMD soldering draft. Verify current equipment/material instructions, UK safety guidance and SDS before writing procedures; check permission before reusing text or images.

## 2026-11-08 — Elektor dual DC LISN assessed

- **Source assessment:** Elektor’s product page describes a dual 5 µH / 50 Ω DC LISN with a 150 kHz–200 MHz RF bandwidth, <60 V DC and <10 A DC operating limits, designed with Würth Elektronik. Its manual frames the instrument around CISPR 25 / ISO 7637 automotive measurements and says it is for authorised technical staff.
- **Project outcome:** Added it as a product-specific adult-tool example in the PCB EMC draft. Do not imply that it is a universal LISN, that it establishes conformity on its own, or that it is suitable for Scout use. Follow the manual and exact applicable test method.

## 2026-11-08 — Schematic-reading tutorial assessed

- **Source assessment:** SparkFun’s beginner tutorial explains symbols, connections, junctions, named nets, voltage nodes, reference designators and reading a schematic by functional blocks. It is a US-oriented learning resource and uses ANSI/IEEE-style zigzag resistor symbols alongside examples that may differ from the project’s IEC convention.
- **Project outcome:** Added it as supplementary reading in the Leaders’ Guide. Use it for connection-reading concepts while retaining IEC symbols in the booklet and verifying specific symbols against the applicable standard.

## 2026-11-08 — Electronics Tutorials site assessed as a reference index

- **Source assessment:** Electronics Tutorials is a broad catalogue covering DC and AC circuits, components, analogue and digital electronics, power topics and online tools. The homepage is a topic index rather than a specific technical lesson.
- **Project outcome:** The user asked to map useful tutorials to project topics. Added a curated source index in [Source Documents](pages/sites/scouts-electronics-badge/sources/electronics-tutorials-index.txt) and linked it from the fundamentals draft. The tutorials are secondary sources; the index records relevant draft mappings and cautions against copying simplified claims or using the site for current ratings, UK safety requirements or standards.

## 2026-11-08 — Relay technologies module assessed

- **Source assessment:** element14’s *Relay Technologies* module was created in 2022 and last updated 2022-12-16; it is sponsored by TE Connectivity. Its coverage of relay operation, contact configurations and selection factors is a useful topic map.
- **Technical context:** Treat its broad relay-type comparisons, timing and electrical ranges as dated or product-specific. Galvanic isolation, switching capacity and SSR/EMR behaviour depend on the exact device and application; check the current relay datasheet and manufacturer guidance.
- **Project outcome:** Added it as qualified background to the adult relay/contact-protection draft. No numeric ratings, product recommendations or source figures adopted.

## 2026-11-08 — Instructables LED beginner guide assessed

- **Source assessment:** Noahw’s 2006 *LEDs for Beginners* is a personal step-by-step tutorial that explains LED polarity, series resistance and simple calculations. Its example parts and US RadioShack context are dated.
- **Technical context:** Do not repeat its “20 mA is standard” claim or resistor-free LED experiments as instructions. LEDs need suitable current limiting based on the actual part and supply; parallel LEDs generally need individual current-limiting resistors to account for forward-voltage variation.
- **Project outcome:** Added a qualified style/source note to the resistor draft. Do not reuse its wording or photos without checking the licence and attribution requirements.

## 2026-11-08 — Operational-amplifier Q&A assessed

- **Source assessment:** Nuts & Volts’ Q&A compares a differential-amplifier circuit with a two-stage inverting-plus-summing arrangement for subtracting two DC voltages. Its key trade-off is flexibility and gain adjustment versus an additional amplifier stage and its noise contribution.
- **Project outcome:** Added it as optional advanced reading in the electronics-fundamentals outline, not as a Scout build recipe. Any implementation would require checking resistor ratios/matching and the chosen op-amp’s common-mode, output-swing and supply limits against its datasheet.

## 2026-11-08 — Appliance insulation-class article assessed

- **Source assessment:** Fidus Power explains Classes I, II and III from a power-supply manufacturer’s perspective, but refers to superseded EN 60950-1 and makes broad statements about voltage limits and touch safety that should not be reused as universal rules.
- **UK/technical context:** HSE HSG107 describes Class I and II portable equipment but does not cover Class III. IEC material shows that classification and protection depend on the complete appliance and applicable product standard; battery-powered devices may be treated under separate requirements. Do not infer an appliance class for a Scout low-voltage circuit or teach that Class III means “safe to touch” in every circumstance.
- **Project outcome:** Added this caveat and current-source pointers to the Leaders’ Guide. No numeric limits or mains instructions were adopted.

## 2026-11-08 — Human-centred hardware design article assessed

- **Source assessment:** Hackaday’s 2023 *Design For People* column discusses making hardware understandable and dependable for the people who install, operate and maintain it. Examples include clear labelling, mounting provisions, reliability measures and concise operating information; it is an opinion piece, not an engineering standard.
- **Project outcome:** Added a usability point to the Woggle KiCad outline: check that polarity/pin markings and connector labels are legible after assembly, and include clear assembly and checking information. Apply advice to the actual design rather than adding features such as watchdogs without a project need.

## 2026-11-08 — Hot-air soldering video assessed

- **Source assessment:** element14 member shabaz’s 2023 video documents a personal attempt to solder capacitors onto a thick, four-layer PCB. The author calls it non-best-practice, notes using several-year-expired solder paste, and says the component results were not yet known.
- **Technical context:** The post’s temperature settings and comments are anecdotal and alloy/equipment/workpiece-specific. Do not present them as a process recipe or claim that the demonstrated components worked. Check the exact equipment, solder paste, PCB and component guidance before describing hot-air rework.
- **Project outcome:** Added a source note and cautions to the existing SMD soldering draft. Keep the procedure adult-facing and verify tool safety and ventilation before publication.

## 2026-11-08 — HackHitchin Arduino kit resource queued for review

- **Access status:** The supplied page could not be fetched by the web reader, the in-app browser host was unavailable, and exact-title searches returned no results. Its kit contents and activities have not been assessed.
- **Project outcome:** Added a TODO to revisit the resource and map only suitable, verified beginner activities to existing Arduino drafts. Check board and component assumptions, safety, and reuse rights before adapting content.

## 2026-11-08 — Creepage calculator idea recorded

- **Source assessment:** Creepage.com presents an interactive clearance and creepage calculator based on IEC 62368-1:2023, Fourth Edition. It describes two clearance procedures, creepage inputs such as working voltage and material group, and altitude correction; it also says to verify critical dimensions against the full standard and certification body. Its own disclaimer provides no warranty.
- **Project context:** Creepage.com was originally assessed as workflow inspiration for a possible calculator, not as a source to copy. After the user identified an existing creepage-and-clearance article on Philip’s site, review that article first and decide whether a calculator would add value; any tool would need an established use case, independently validated calculations, resolved standards-data rights, and clear limits against implying a safety or compliance determination. See [TODO.md](TODO.md).
- **UK context:** BSI lists BS EN IEC 62368-1:2024+A11:2024 as the current UK release. A future calculator must not silently present the IEC 2023 edition as the UK edition.

## 2026-11-08 — Existing creepage and clearance article identified

- **User-provided context:** Philip already has a [Creepage and Clearance article](https://philipmcgaw.com/creepage-and-clearance/), published 2023-02-21. The page presents IPC-2221 spacing guidance and summaries relating to appliance insulation and safety classifications; it is an article, not a calculator.
- **Project outcome:** Replaced the TODO to assess a new calculator with a review of the existing article and a decision on whether an additional tool would add value. Check the article’s scope, safety classifications and tabulated standard values against authorised current sources before revising it; see [TODO.md](TODO.md).

## 2026-11-08 — Arduino analogue-input example assessed

- **Source assessment:** Arduino’s beginner example uses a potentiometer or photoresistor divider and maps the analogue reading to an LED blink interval. The input measures voltage from the divider, not resistance directly.
- **Technical context:** Its 5 V supply, 10-bit `analogRead()` range, pin 13 LED and 220 Ω external LED resistor are not universal across Arduino boards. Verify the selected board’s input limits, ADC behaviour, pin assignments and LED circuit before adapting it.
- **Project outcome:** Added a qualified source note to the sensor data-logging draft; it remains an example of an input-to-output activity rather than a verified sensor measurement project.

## 2026-11-08 — Arduino button draft expanded

- **Project outcome:** Added a pull-up/pull-down state comparison, a matched-resistor current example, and a non-blocking `millis()` debounce sketch to the button draft. The `50` ms interval is illustrative, not a universal switch specification. Exact board support, electrical limits and behaviour with the selected switch still need review before publication; see [TODO.md](TODO.md).

## 2026-11-08 — PCB-design curriculum article assessed

- **Source assessment:** Altium’s article argues that PCB design education connects circuit design, layout, manufacturing and prototyping. It is vendor-authored and aimed at university engineering curricula; its Altium product promotion and North American workforce claims do not establish UK Scout or employment needs.
- **Project outcome:** Added a qualified teaching point to the Woggle KiCad outline: use the practical PCB workflow to show how circuit, physical layout and manufacturing information fit together, without expanding the activity into professional tools or advanced simulation.

## 2026-11-08 — Resistor article sources assessed

- **Source assessment:** K7MEM’s calculator explores non-standard resistance values using parallel combinations and includes power estimates when voltage is supplied. The All About Circuits forum thread concerns a complex 160 V high-side programmable current source; it is not an appropriate Scout build or a general resistor example.
- **Technical context:** Series/parallel combinations require checking individual dissipation, voltage rating, tolerance and thermal conditions. A digital potentiometer has terminal-voltage, current and package-power limits and is not a drop-in high-voltage or high-power resistor.
- **Project outcome:** Added a custom-combination and digital-potentiometer section to the resistor article outline, with no copied schematic or construction advice. High-voltage work remains outside Scout activities; see [TODO.md](TODO.md).

## 2026-11-08 — Relay quiz resource assessed

- **Source assessment:** The correct element14 Community page is the [Power Relays Quiz](https://community.element14.com/products/manufacturers/omron-electronic-components/w/quiz/4497/power-relays-quiz), an Omron-sponsored 25-question quiz covering electromechanical relays, electrical contacts and PCB power relays. The earlier `4496/power-relays-quiz-resource` URL was not the quiz page.
- **Project outcome:** Added an original five-question knowledge check to the relay article outline, covering contact states, coil/contact ratings, load type, coil suppression and release time. Do not copy quiz wording; verify explanations against current relay manufacturer documentation.

## 2026-11-08 — Maker power module assessed

- **Source assessment:** element14’s *Power Essentials for Makers* is a broad topic map covering AC/DC power fundamentals, sources and converters, maker-board power architectures, and design considerations. The module was created in 2017 and last updated in 2023.
- **Technical context:** Its board-specific figures and product examples are historical and can be stale; its safety and standards summaries need current UK verification. Do not transfer its specifications to current boards.
- **Project outcome:** Added it as a background source to the electronics-fundamentals outline. Check product-specific and UK guidance before reusing any detail; see [TODO.md](TODO.md).

## 2026-11-08 — PCB fuse module assessed

- **Source assessment:** element14’s *Circuit Protection: PCB-Mounted Fuses* introduces fuse operation, ratings, I²t, PCB fuse types and resettable PTCs, and includes a 15-question quiz. It was created in 2017 and last updated in 2023; product examples and standards summaries need current checking.
- **Technical context:** Fuse selection depends on normal current, voltage, available fault current, time-current behaviour, interrupting rating and temperature. A resettable PTC can remain at high resistance and pass some current during a fault, unlike a fuse that opens; selection remains part-specific.
- **Project outcome:** Added fuse and PTC selection cautions, Littelfuse manufacturer references and an original five-question knowledge check to the Arduino interface-protection draft. No example fuse ratings or construction instructions adopted; see [TODO.md](TODO.md).

## 2026-11-08 — Voltage-reference module assessed

- **Source assessment:** element14’s *Voltage References* module covers reference architectures, performance terms and uses in ADCs, sensors and comparators. It was created in 2019 and last updated in 2022, includes Maxim product examples, and has a 15-question quiz.
- **Technical context:** Reference performance depends on more than nominal voltage; initial accuracy, temperature coefficient, input and load regulation, noise and long-term behaviour may matter. Product examples and numerical claims should be checked against current datasheets; calculations and simplified explanations need independent review.
- **Project outcome:** Added an optional advanced voltage-reference note to the electronics-fundamentals outline and cited TI selection guidance. No part-specific values or quiz content adopted.

## 2026-11-08 — Precision-measurement module assessed

- **Source assessment:** element14’s *Analog Electronics: Precision Measurement* covers ADCs, op amps, current-sense amplifiers, voltage references and measurement-system quality. It was created in 2020 and last updated in 2022; its examples focus on Maxim precision ICs and include a 15-question quiz.
- **Technical context:** Keep accuracy, precision, repeatability and resolution distinct. Repeatable readings can still have a systematic offset, and ADC bit count or display digits alone do not establish accuracy. Use BIPM/NIST terminology for measurement claims.
- **Project outcome:** Added a beginner-level measurement-quality note to the fundamentals post and an accuracy caveat to the sensor-logging draft. No Maxim product claims, values or quiz content adopted.

## 2026-11-08 — Electronics for Absolute Beginners course assessed

- **Source assessment:** Iain Sharp’s 2010 one-day course progresses through basic circuits, breadboards, resistors, LEDs, transistors, capacitors, oscillators and a decade-counter project. Its companion parts sheet specifies a historical kit including ¼ W resistors, four-band colour markings, 10 µF/100 µF electrolytics, small ceramic capacitors, a 2N3704 transistor and a 4017 decade counter. These are course examples, not current UK buying recommendations. Its notes are licensed CC BY-NC-SA 3.0 Unported.
- **Technical context:** The course’s values and experiments are tied to a particular kit and need current component and safety checks. Its shortcut that capacitor size predicts polarity is not reliable; identify polarity from the exact part. Its breadboard diagram is only one layout. Do not reuse source figures without licence and product-layout checks.
- **Project outcome:** Added qualified references to the fundamentals, resistor, capacitor and breadboard drafts. The companion parts sheet has now been reviewed; the resistor and capacitor drafts record its kit-specific ratings and values without treating them as universal design rules. Updated the booklet’s resistor-band section to distinguish four-band and five-band codes, clarified that SMD resistor codes vary, and noted that transistors can operate as switches as well as amplifiers. Added a brief RC timing explanation: a resistor-capacitor circuit changes voltage over time, and a transistor can use that change to switch another circuit. Use the course for teaching sequence only; verify examples and check non-commercial/share-alike licence compatibility before adapting source text or figures.

## 2026-11-08 — Electronics for Artists course assessed

- **Source assessment:** Iain Sharp’s two-day *Electronics for Artists* course, first presented in 2010 and updated in 2019, repeats the component/breadboard material and adds Arduino-based inputs, analogue dividers, PWM, drivers and an interactive organ. Its notes are licensed CC BY-NC-SA 3.0 Unported.
- **Technical context:** Arduino Part 2 uses classic Uno-era 5 V pin examples and older software instructions. Do not transfer pin ranges, PWM values, supply advice or relay-isolation claims to another board without checking its current documentation and the connected component datasheets. Its body-contact sensor activities are not a Scout circuit specification.
- **Project outcome:** Added bounded source notes to the fundamentals and Arduino button, PWM, sensor-logging and interface-protection drafts. Verify all board-specific details and licence compatibility; see [TODO.md](TODO.md).

## 2026-11-08 — Overvoltage protection article assessed

- **Source assessment:** Dyethin’s article is a topic prompt, not a source for universal Arduino or microcontroller protection values. Its suggested 5.1 V and 6.8 V Zener examples cannot be assumed safe for logic inputs.
- **Technical context:** Zener and TVS clamp voltage varies with current and device characteristics; the source impedance, pulse energy and return path matter. Signal-pin clamps, series disconnects and crowbars have different behaviours. Check the exact receiving-device limits and protection-device datasheet.
- **Project outcome:** Added these distinctions to the Arduino interface-circuit protection draft and cited TI application material on TVS clamping and data-line selection. No circuit values or build instructions adopted; exact board and component review remains tracked in [TODO.md](TODO.md).

## 2026-11-08 — EMC post series scoped

- **Source assessment:** Nemko’s page is a commercial overview of emissions and immunity testing; Tekbox describes its EMCview pre-compliance software and supported equipment. EDN’s PCB article is a useful engineering introduction to signal fields and return paths. PCB HERO’s EMI/EMS/EMC terminology is inconsistent and should not be used as a technical authority.
- **Technical context:** UK EMC requirements address both disturbance generated and immunity to expected disturbance. Emissions, immunity, bench debugging, pre-compliance and formal product conformity are related but distinct. PCB layout guidance should avoid universal rules detached from edge rate, stack-up, current paths and final product configuration.
- **Project outcome:** Added separate outlines for an EMC terminology/UK-context post and a PCB-layout/pre-compliance post. Check applicable GB/NI/EU requirements at publication; see [TODO.md](TODO.md).

## 2026-11-08 — Relay and contactor snubber topic scoped

- **Source assessment:** Wikipedia provides a general snubber overview. The two linked hobby articles discuss relay contact suppression but include generic values and unsafe-looking advice in comment sections; their numbers and mains suggestions were not adopted.
- **Technical cross-check:** Panasonic, Omron, TE Connectivity, Siemens and Schneider materials distinguish suppression across switched loads/contacts from suppression across relay or contactor coils. Suppressors can alter release time; RC networks also require consideration of off-state current and contact-closing inrush.
- **Project outcome:** Added an adult-facing outline with no component values or mains wiring. Exact device/load review is still needed before technical design instructions; see [TODO.md](TODO.md).

## 2026-11-08 — Existing relay and contactor articles identified

- **User-provided context:** Philip has published [Learn about Relays](https://philipmcgaw.com/relays-what-you-should-know/), [Automotive Relays](https://philipmcgaw.com/automotive-relays/) and [Contactors, More than just a Relay](https://philipmcgaw.com/contactors-more-than-a-relay/). Together they cover relay basics, automotive terminal numbering and contactors, so the planned snubber article should continue that series rather than repeat the introductions.
- **Technical review note:** The automotive relay article currently labels terminal 87 as common, 87a as normally closed and 87b as normally open. Lucas Electrical’s terminal guide and HELLA relay catalogue show the usual arrangement as 30 common/switch input, 87 normally open, 87a normally closed, and 85/86 for the coil. Treat this as a correction to verify against the exact relay schematic and datasheet, not as a universal pinout.
- **Project outcome:** Added the three posts and manufacturer references to the relay draft, and updated [TODO.md](TODO.md) to track review and cross-linking of the existing series before completing the snubber follow-up.

## 2026-11-08 — Lithium-ion series-pack article assessed

- **Source assessment:** Hackaday’s 2024 article explains series/parallel notation and discusses how cell capacity and resistance differences can limit a series string. It also suggests opening packs and improvised loose-cell testing; those procedures are not suitable for the Scout-facing project guidance and were not reused.
- **Technical context:** Pack voltage does not reveal the voltage or condition of each series cell. UK OPSS PLEV safety research describes cell-level over-voltage risks and the role/limits of pack balancing. Correct charge limits, monitoring and protection are properties of the complete, chemistry-specific pack design.
- **Project outcome:** Added a high-level caution and source note to the battery-pack management draft. No battery assembly, pack-opening or loose-cell test instructions were added.

## 2026-11-08 — KiCad mechanical-footprint persistence assessed

- **Source assessment:** Smayze’s 2024 article recommends schematic symbols paired with footprints to preserve and manage mechanical items through board updates, plus 3D review for physical fit and label visibility. A comment notes the simpler **Not in schematic** attribute for board-only footprints.
- **Technical cross-check:** KiCad 9 documentation confirms that footprints marked **Not in schematic** are preserved when updating a board from the schematic, while the separate **Exclude from position files** and **Exclude from BOM** attributes control those outputs. Locking is for movement protection. Text visibility/occlusion is a separate silkscreen-layer and fabrication-output check.
- **Project outcome:** Added these distinctions and source references to the Woggle KiCad walkthrough outline. Check exact menus against the KiCad version used in the eventual guide.

## 2026-11-08 — Ceramic-capacitor Wikipedia article assessed

- **Source assessment:** The article is a broad overview of ceramic capacitor construction, classes, temperature behaviour, frequency effects and applications. It is useful for finding topics and terminology, but it is collaboratively edited and should not be the project’s authority for technical specifications or current component-selection claims.
- **Project outcome:** No Wikipedia text, tables or images were copied into the project. The capacitor draft already covers the relevant Class 1/Class 2 distinction and uses Murata, KEMET and TDK sources for claims that need manufacturer support.

## 2026-11-08 — Murata ceramic-capacitor temperature guide assessed

- **Source assessment:** Murata’s guide, originally published 2012 and revised 2023-12-01, explains Class 1 temperature coefficients and the bounded temperature-change categories for Class 2 ceramic dielectrics. It usefully separates these from voltage-bias and ageing effects.
- **Technical context:** Treat codes such as X7R/X5R as specified temperature behaviour under standard test conditions, not as a complete prediction of effective capacitance. Exact part, operating temperature and DC bias still matter; consult the manufacturer’s datasheet and characteristic curves.
- **Project outcome:** Added Murata’s guide and FAQ as manufacturer references in the capacitor draft. No part-specific values were added.

## 2026-11-08 — Ceramic capacitor dielectric guide assessed

- **Source assessment:** All About Circuits’ 2023 overview clearly introduces C0G/NP0, X7R, X5R and Y5V temperature codes, but is not a complete component-selection guide.
- **Technical cross-check:** Manufacturer guidance confirms Class 2 MLCC capacitance can fall substantially under DC bias; actual capacitance also depends on temperature, ageing, package and part-specific construction. X7R/X5R temperature classification alone does not state effective in-circuit capacitance. C0G/NP0 is more stable across temperature and bias. Some Class 2 ceramics can also create audible mechanical vibration in certain circuits.
- **Project outcome:** Added qualified notes and manufacturer references to the capacitor article outline. Keep exact effective-capacitance claims part-specific; capacitor article refresh remains tracked in [TODO.md](TODO.md).

## 2026-11-08 — Conducted-emissions comparison assessed

- **Source assessment:** The 2021 AnalogicTips article by a Texas Instruments applications engineer compares conducted-emissions setups for CISPR 25, CISPR 11 and MIL-STD-461G. Its numeric setup details are edition-specific and should not be reused as current universal requirements.
- **Technical context:** Conducted emissions, immunity, LV 124 electrical stress and environmental testing address different requirements. LISNs/artificial networks and cable configurations are standard-specific; a bench pre-compliance scan is not a formal standards test.
- **Project outcome:** Added this distinction to the Arduino interface-protection draft. For this project, explain EMC concepts only at a high level; no compliance test procedure is proposed.

## 2026-11-08 — MOSFET load-switch article assessed

- **Source assessment:** Codrey’s 2021 article shows a high-side P-channel MOSFET switch with optional optocoupler control. Its stated approximate power capability and component choices are not transferable without checking the circuit and operating conditions.
- **Technical cross-check:** The cited IRF9540N datasheet specifies on-resistance at −10 V gate-to-source; its threshold voltage is measured at a very small drain current and does not establish low-loss switching at a given gate drive. Load inrush, dissipation, diode orientation and transient behaviour also need review.
- **Project outcome:** Added general load-switch selection cautions to the Arduino interface-protection draft. No circuit values or build steps were adopted; see [TODO.md](TODO.md) for the pending board and component review.

## 2026-11-08 — Arduino protection and LV 124 article scoped

- **Source assessment:** Rugged Circuits’ “10 Ways to Destroy an Arduino” groups useful failure modes, but its examples are hardware-specific and its proposed protections are product claims. Do not reuse its values as universal circuit recommendations.
- **Technical context:** LV 124 covers electrical and environmental testing for 12 V vehicle components; adding protection parts does not establish compliance. Applicable OEM requirements and the prescribed validation process matter.
- **Project outcome:** Added an adult-facing introductory draft on interface protection, with no build values or claim of automotive qualification. Board and circuit-specific review remains open; see [TODO.md](TODO.md).

## 2026-11-07 — Arduino sensor data-logging article assessed

- **Source assessment:** Duino4Projects’ indexed 2019 article text describes an Uno, Ethernet shield, microSD card, LM335Z and photoresistor. The page could not be fetched directly, so its wiring, code and claims were not verified or reused.
- **Technical context:** A sensor’s ADC reading depends on the exact board and circuit. The LM335 output and operating circuit need datasheet-based conversion; a photoresistor divider gives a relative response unless calibrated. SD-card pin assignments and electrical requirements are board/module-specific.
- **Project outcome:** Added an adult-facing draft about timestamps, units, calibration and checking saved data. Exact build steps remain open pending selection and review of hardware; see [TODO.md](TODO.md).

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
- **Source assessment:** The 2005 US-oriented book mostly overlaps with the existing booklet. Its breadboard chapter usefully explains internal contact groups and prototyping before soldering. The Scout booklet and Leaders’ Guide now include concise, UK-appropriate breadboard notes, and the blog index includes a possible breadboard-prototyping post. The separate review records scope and cautions: [Electronics For Dummies review](pages/sites/scouts-electronics-badge/sources/electronics-for-dummies-review.txt).
- **Open action:** Verify layouts and ratings against a specific breadboard and circuit before developing the standalone article; see [TODO.md](TODO.md).
- **User-reported decision:** The converted source PDF is not needed in the repository; it was removed on 2026-11-07. The review note and project drafts retain the useful breadboard findings and source assessment.

## 2026-11-07 — 2021 course handouts assessed

- **Source assessment:** The five course handouts’ useful points are carried in the fundamentals, resistor, and battery drafts. The parts list matches the saved summary but has US-oriented sales links and no circuit diagram; do not reuse its imagery without checking rights. The DMM sheet names models without specifications, so check current manuals and UK suitability before making recommendations. See the [review note](pages/sites/scouts-electronics-badge/sources/electronics-foundations-fundamentals-2021-review.txt) and [TODO.md](TODO.md).
- **User-reported decision:** The user reviewed the DMM list PDF and said it does not need to be retained. The file was removed; its model names and lack of specifications remain in the source review note. The separate current-manual check remains open.
- **Follow-up decision:** The user said the whole course folder could be removed if its files were no longer needed. After confirming the useful content and open checks are recorded in project notes, all remaining course PDFs were removed; the review note retains their summaries.

## 2026-11-06 — Consolidated project context

### Project, audience, and structure

- **Project fact:** This repository develops the Scouts Electronics Activity Badge booklet and supporting learning resources. The main booklet is [Scouts Electronics Activity Badge Booklet](pages/sites/scouts-electronics-badge/booklet.txt); print instructions from the original booklet were to be ignored during conversion.
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
- **Blog workflow:** Keep one Markdown file per planned post in `pages/sites/scouts-electronics-badge/blog/`. Blog posts can provide more detail than the booklet. WordPress access is expected to be available later from another computer; see [TODO.md](TODO.md) for the queued updates and broken-page diagnosis.

### Source material and provenance

- Treat course transcripts, PDFs, product pages, and supplied images as source material, not as automatically correct local guidance. Preserve attribution and verify safety, electrical values, and regional applicability before publication.
- The reviewed course-exercise PDFs contained useful SI-prefix, DMM, LED-current-limit, and battery-sizing material. The battery challenge’s figures are teaching examples without manufacturer, model, or test-condition basis; do not present their capacities or runtime calculations as guarantees. The exercise describes a motor, despite transcript headings that called it a light bulb. All course PDFs were removed after review; the [course materials review](pages/sites/scouts-electronics-badge/sources/electronics-foundations-fundamentals-2021-review.txt) and related drafts retain needed details.
- Some source-course material was US-oriented. Its DMM models, suppliers, power-source examples, and safety claims need current UK checks before use. The course parts-list PDF was visually checked against the item summary in the fundamentals draft; its shop links were US-oriented and it showed no circuit connections. The DMM models still need current manual checks before any recommendation. See TODO.md.
- `Electronics for Dummies.pdf` was encrypted and could not be reviewed; Philip said he may revisit it later.
- Useful existing web articles include [learn about resistors](https://philipmcgaw.com/learn-about-resistors/), [capacitors](https://philipmcgaw.com/capacitors/), [LED resistor values](https://philipmcgaw.com/led-resistors-values/), [Ohm’s and Watt’s laws](https://philipmcgaw.com/ohms-law-and-watts-law/), [capacitor value prefixes](https://philipmcgaw.com/capacitor-value-prefixes/), and [special symbols in engineering reports](https://philipmcgaw.com/special-symbols-used-in-engineering-reports/). Related revisions and other article ideas are tracked in `TODO.md` and `pages/sites/scouts-electronics-badge/blog/`.

### Current project state

- **Repository fact checked 2026-11-06:** `TODO.md` is the action index. It includes the Leaders’ Guide, illustration, blog planning and drafting, WordPress updates, KiCad/PCBWay walkthrough, Charlieplexing visual, silkscreen post, and advanced PCB rework post. Check it for current status instead of relying on this memory entry.
- **Source notes:** PDF review notes are stored under `pages/sites/scouts-electronics-badge/sources/`. Their conclusions and open checks belong to those notes; consult the relevant source note before reusing detailed findings.
- **Git:** Project changes are expected to be committed and pushed to the repository’s `main` branch. Follow the Git workflow in `AGENTS.md`, stage only task-related files, and preserve unrelated changes.

## 2026-11-10 — Blog index tracks published articles

- **Workflow decision:** Keep a **Published article** column beside each blog draft; link an existing article when it is the clear match, and use `—` until a draft has a matching live article.

## 2026-11-10 — Fruit and vinegar cell activity considered

- **Discussion outcome, not an approved booklet change:** A lemon or vinegar cell could work as a short optional investigation alongside the booklet’s battery and multimeter material. It can introduce chemical energy, electrodes, electrolyte, polarity, voltage measurement, and comparison of cells. It does not count as one of the three constructed circuits because it is a source rather than a complete circuit.
- Keep expectations realistic: simple fruit or vinegar cells provide little current, so use a multimeter rather than promising to light an LED. Use known copper and zinc electrodes rather than coins, whose materials and coatings vary. A vinegar cell is a simpler alternative; comparing vinegar, lemon juice, or salty water with the same electrodes can make a controlled investigation. A potato cell is a similar option.
- **Open point:** No decision has been made to add the activity to the canonical booklet.

## 2026-11-11 — Resistive-sensor measurement transcript assessed

- **Source assessment:** The “Measure resistive sensors” excerpt explains using a divider and ADC voltage reading to infer sensor resistance. For the resistor article, use a thermistor as the main example per Philip's preference; do not reuse the excerpt's LDR values or Arduino readings as general specifications. State divider orientation, ADC/reference assumptions and handle near-rail readings carefully. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:resistors|resistor draft]].

## 2026-11-11 — Potentiometer lesson assessed

- **Source assessment:** The “Potentiometers” transcript distinguishes a three-terminal adjustable divider from a two-terminal rheostat use. In the resistor article, verify the exact pinout and keep any wiper-to-ADC voltage within the selected board's limits; do not generalise the course's 10 kΩ/20 kΩ parts or 5 V Arduino example. A rheostat must be rated for its actual load and dissipation. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:resistors|resistor draft]].

## 2026-11-11 — Parallel-resistor lesson assessed

- **Source assessment:** The “Resistors in parallel” transcript gives the reciprocal-resistance method and current/power examples. In the resistor draft, identify reciprocal resistance as conductance in siemens, check each branch's current and dissipation, and measure resistance only when de-energised. The 10 kΩ/20 kΩ values are illustrative course examples. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:resistors|resistor draft]].

## 2026-11-11 — Parallel-resistor diagram assessed

- **Source assessment:** Philip supplied the course frame showing the parallel-resistance equation and branches across common rails. It agrees with the topology recorded in the source review. Do not reuse the course image; draw any project figure in the preferred IEC schematic style.

## 2026-11-11 — Kirchhoff's laws transcript assessed

- **Source assessment:** The “Kirchhoff's circuit laws” transcript introduces current balance at a node and signed voltage balance around a loop. Add both to the fundamentals article outline with clear reference directions, IEC symbols, and explicit junction versus crossing conventions; the transcript's 9 V values are illustrative, not Scout activity instructions. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:electronics-fundamentals|fundamentals draft]].

## 2026-11-11 — Wheatstone-bridge transcript assessed

- **Source assessment:** The “Wheatstone Bridge” transcript connects two dividers and introduces differential measurement. With the stated output convention ''Vout = VR − VL'', preserve sign when calculating an unbalanced bridge; the 5 V, 10 kΩ, 10 kΩ, 10 kΩ and sub-1 kΩ example at −2.3 V implies about 417 Ω. Qualify claims of accuracy and use the bridge only as a checked, low-voltage sensor example. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:resistors|resistor draft]].

## 2026-11-11 — Light-activated bridge challenge assessed

- **Source assessment:** The new “Challenge: Light activated switch” transcript specifies relay logic ''A > B'' on and ''A ≤ B'' off, clarifying the 03_09 worksheet's overlapping dark condition. Treat its LDR values as examples, and do not adapt its unspecified relay/stereo interface into a Scout build. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-exercises-review|exercise-file review]], the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course review]], and the [[sites:scouts-electronics-badge:blog:resistors|resistor draft]].

## 2026-11-11 — Light-activated bridge solution assessed

- **Source assessment:** The course solution defines bridge output as ''VA − VB'', opposite to the earlier bridge transcript's ''VR − VL''; the polarity choice is arbitrary, so label the midpoint wiring and equation consistently. The ideal 5 V example puts A at 2.5 V and uses a 5 kΩ top resistor to balance a 5 kΩ LDR threshold. Calculated outputs with the transcript's 1 kΩ/10 kΩ LDR values are about +1.67 V in bright light and −0.83 V in darkness. Treat course sensor values and reported checks as examples, not guaranteed behaviour. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:resistors|resistor draft]].

## 2026-11-11 — Resistor and sensor quiz items assessed

- **Source assessment:** All eight supplied quiz questions are reviewed. They cover series resistance and dividers, photoresistors, passive-divider limits, parallel resistance, rheostats, Wheatstone bridges, and Kirchhoff's Current Law. Preserve the divider circuit conditions and note that its output stays between the source rails. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]].

## 2026-11-11 — Oscilloscope lesson assessed

- **Source assessment:** The “What is an oscilloscope?” transcript gives the voltage-versus-time overview. Add this as optional fundamentals material, not as a requirement or purchase recommendation. Treat its bandwidth/sample-rate ranges, used-scope advice, and Rigol model as historical examples; check exact probe ratings and grounding before any practical low-voltage demonstration. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:electronics-fundamentals|fundamentals draft]].

## 2026-11-11 — Oscilloscope signal-measurement lesson assessed

- **Source assessment:** “Measure a signal” supports an optional exercise in probe setup, compensation, coupling, reading volts/div and time/div, and calculating peak-to-peak voltage and period. Probe loading, attenuation, compensation and grounding depend on the exact equipment; many bench-scope probe grounds are Earth-connected. Never treat the probe ground clip like a freely movable reference. The course’s 3 V peak-to-peak, 1 ms period example is arithmetic from its stated settings, not a verified Scout setup. Keep Scout supplies at or below 12 V. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:electronics-fundamentals|fundamentals draft]].

## 2026-11-11 — Oscilloscope display-settings lesson assessed

- **Source assessment:** “Oscilloscope display settings” supports explaining volts/div, seconds/div, vertical position and viewing multiple channels. Scope controls are model-specific. A noisy-looking trace on an unconnected input can be environmental pickup or instrument noise and does not show that the circuit itself is noisy. Use a known signal and a correctly connected, rated probe; keep the Scout supply at or below 12 V. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:electronics-fundamentals|fundamentals draft]].

## 2026-11-11 — Oscilloscope trigger-settings lesson assessed

- **Source assessment:** “Oscilloscope trigger settings” supports an optional explanation of edge slope, trigger level, trigger source, and normal, auto and single acquisition modes. Trigger mode Auto differs from an Auto/Autoset display button. A non-triggered or wandering trace does not establish signal behaviour; distinguish signal changes, noise and setup. Use a specified scope with a checked low-voltage source and input limits. Keep Scout supplies at or below 12 V. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:electronics-fundamentals|fundamentals draft]].

## 2026-11-11 — Instructor oscilloscope identified

- **User clarification:** The instructor’s scope is a Rigol DS1054. The pasted course transcript calls it a DS1054Z; Rigol’s DS1000Z user guide includes the DS1054Z and lists it as four-channel, 50 MHz. Preserve the model-name discrepancy and check the unit label/manual before using model-specific settings or ratings. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[https://www.rigol.com/dam/global/downloads/brochures/en/user-manual/oscilloscopes/DS1000Z_UserGuide_EN.pdf|Rigol DS1000Z-series User Guide]].

## 2026-11-11 — Oscilloscope display quiz items assessed

- **Source assessment:** All six supplied oscilloscope quiz questions are reviewed. They cover voltage versus time axes, divisions and their scales, shared horizontal versus channel-specific vertical controls, and Auto trigger mode. Explain that an oscilloscope plots voltage against time; V/div and s/div give the quantity represented by each division. Auto updates may not be synchronised. The channel controls are confirmed for the instructor’s Rigol DS1054/DS1054Z; verify other models. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:electronics-fundamentals|fundamentals draft]].

## 2026-11-11 — Capacitor introduction assessed

- **Source assessment:** “What is a capacitor?” is useful for introducing capacitance, dielectric-separated electrodes, stored energy, units and the battery comparison. Avoid the literal balloon/electron model and clarify that charge does not conduct through the dielectric. Distinguish external charging current from steady-state DC, include leakage and retained charge, and avoid treating pF-to-µF as a practical range limit or making a universal energy-density comparison. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:capacitors|capacitor draft]].

## 2026-11-11 — Capacitor types and safety lesson assessed

- **Source assessment:** “Types of capacitors” introduces common ceramic and electrolytic parts, package recognition, polarity and stored-charge hazards. Capacitance ranges overlap; ceramic parts are generally non-polarised, while many but not all electrolytic parts are polarised. Check the exact component marking and datasheet. Do not repeat the advice to short a charged capacitor with a screwdriver; use an appropriately rated, approved discharge method and verify voltage before handling. Describe reverse-polarity failure without asserting that every electrolytic explodes or fails short. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:capacitors|capacitor draft]].

## 2026-11-11 — Add ESR to capacitor-selection guidance

- **User preference:** Include ESR when discussing capacitor selection and values. Explain ESR as a frequency- and temperature-dependent loss parameter, connect it to ripple-current heating, and check datasheet conditions. Avoid implying that lower ESR is always preferable because substitutions can change circuit stability. See the [[sites:scouts-electronics-badge:blog:capacitors|capacitor draft]].

## 2026-11-11 — Capacitor-failure joke terminology

- **User wording:** “Factory smoke” is another name for “magic smoke”. If this joke is used in learner-facing copy, keep it clear that smoke or venting indicates a component failure and needs safe attention.

## 2026-11-11 — Preferred capacitor discharge method

- **User preference:** Philip prefers discharging capacitors through a resistor, typically around 1 kΩ. Treat that as a starting point only; check capacitor voltage, capacitance, initial resistor power, pulse-energy rating and discharge time, then measure the remaining voltage. Keep Scout activities within the 12 V maximum supply rule.

## 2026-11-11 — Capacitor value-marking lesson assessed

- **Source assessment:** “Read capacitor values” gives correct examples for the assumed three-digit pF code: 103 = 10 nF and 334K = 330 nF ±10 %. Marking and tolerance codes vary; many MLCCs are unmarked. Do not assume a missing tolerance letter means Z or use printed voltage as a universal operating limit. Check the exact part datasheet, and isolate/discharge capacitors before DMM capacitance measurement. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:capacitors|capacitor draft]].

## 2026-11-11 — Capacitor characteristics lesson assessed

- **Source assessment:** “Capacitor characteristics” covers voltage rating, capacitance tolerance, leakage and ESR. Keep the course’s 2× voltage selection as a rule of thumb only. Do not generalise its few-nA leakage or technology-wide ESR ranges; these depend on component construction and datasheet test conditions. Check effective capacitance, voltage, temperature, ripple, leakage and ESR as the application requires. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:capacitors|capacitor draft]].

## 2026-11-11 — Capacitors in parallel lesson assessed

- **Source assessment:** The “Capacitors in parallel” example correctly sums 10 µF + 1 µF + 1 µF to 12 µF. The lowest-rated part limits the bank’s working voltage, subject to any further derating. Equal relative tolerances produce the same relative tolerance in the sum; mixed tolerances require adding individual minimum and maximum values. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:capacitors|capacitor draft]].

## 2026-11-11 — Capacitors in series lesson assessed

- **Source assessment:** The “Capacitors in series” reciprocal formula is sound, but the 10 µF + 1 µF + 1 µF example evaluates to approximately 0.476 µF; its intermediate reciprocal values are in inverse farads. Series capacitors do not automatically provide a safe higher voltage rating because real parts can share voltage unevenly, and manufacturer guidance varies by capacitor type. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:capacitors|capacitor draft]]. Keep learner circuits at or below 12 V.

## 2026-11-11 — Class X/Y capacitors in blog context

- **User direction:** Cover Class X/Y safety capacitors and LVD context in the capacitor blog only, not in the Scouts booklet.
- **Technical context:** X and Y are safety classifications for EMI suppression capacitors and indicate distinct permitted circuit positions; they do not mean a pair of capacitors wired in series. Some individual capacitors are approved for both classifications. Keep any discussion descriptive, distinguish component approval from finished-product compliance, and give no mains construction instructions. See the [capacitor draft](pages/sites/scouts-electronics-badge/blog/capacitors.txt).

## 2026-11-11 — RC circuits lesson assessed

- **Source assessment:** The user supplied the “RC circuits” transcript. The examples 1 kΩ × 1,000 µF = 1 s and 1 kΩ × 10 µF = 0.01 s are correct. The capacitor reaches 63.2 % of the total voltage change after one time constant and approaches, but does not exactly reach, its final voltage; after five time constants it is about 99.3 % there. On discharge 36.8 % remains after one time constant. See the course [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|source review]] and [[sites:scouts-electronics-badge:blog:capacitors|capacitor draft]].

## 2026-11-11 — Camera-flash capacitor challenge assessed

- **Source assessment:** The ideal 9 V/15 mA charging limit gives 600 Ω as the theoretical minimum resistor. For a constant 2 Ω load, the ideal capacitor minimum to remain above 3 V for 2 ms from 9 V is approximately 910 µF. Real resistor tolerances/supply maximum, lamp filament resistance, capacitor tolerance and ESR, and circuit resistance need consideration; the ideal starting discharge current is 4.5 A. Keep the camera-flash topic as an adult blog calculation, never dismantle a flash unit, and do not turn this pulse circuit into a Scout build simply because its supply is 9 V. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:capacitors|capacitor draft]].

- **Solution check:** The instructor’s 680 Ω / 1,000 µF choice gives about 13.2 mA maximum initial charging current, 0.12 W initial resistor dissipation, and a 2 ms time constant for a constant 2 Ω load. In the ideal model, the capacitor is about 3.3 V at 2 ms and remains above 3 V for about 2.2 ms. These calculations do not establish a safe or reliable build with the actual bulb and capacitor.

## 2026-11-11 — Capacitor quiz: electric field

- **Source assessment:** All eight supplied questions from the course’s capacitor quiz are correct in context: a capacitor stores energy in the electric field between differently charged plates; the common three-digit value code indicates picofarads; electrolytic capacitors are usually polarised; ideal capacitances add in parallel; “twice” is the intended voltage-rating margin; the simple RC time-constant answer is 63 %; capacitors in series use the reciprocal-sum relationship like resistors in parallel; and the resistor limits current in the simple series RC charge circuit. Clarify that pF is for the common code, non-polarised electrolytics exist, 2× is only a rule of thumb subject to exact-part derating, 63.2 % is the total voltage change after one time constant for an initially uncharged step response, and actual charging current depends on the whole circuit.

## 2026-11-11 — AC and DC lesson assessed

- **Source assessment:** “Alternating current vs. direct current” is a useful comparison, but DC is not necessarily constant and AC is not necessarily sinusoidal. Use conventional current direction in schematics and describe electron drift in metal as opposite. The transcript’s 60 Hz outlet example is North American; UK mains context is nominal 230 V, 50 Hz. Keep that descriptive only: Scout practical supplies stay at or below 12 V DC, with no mains construction or measurement. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:electronics-fundamentals|fundamentals draft]].

## 2026-11-11 — EPCI capacitor technology chart reviewed

- **Source assessment:** The supplied capacitance-versus-voltage graphic matches Figure 2 in EPCI’s “Capacitor, What is it?” overview and reflects a broad, older mass-market range, not hard technology limits or part-selection data. Use only to explain overlapping envelopes; distinguish low-voltage individual supercapacitor cells from higher-voltage series modules. EPCI’s site states its content is CC BY-SA 4.0 unless otherwise noted, but warns that some images may have separate copyright with no licence provided. Do not reproduce this image until its image-specific rights are confirmed; an original chart still needs sourced, checked ranges. Recorded in the [[sites:scouts-electronics-badge:blog:capacitors|capacitor draft]].

## 2026-11-11 — EPCI capacitor applications table reviewed

- **Source assessment:** The supplied “Typical applications overview table” matches Figure 3 in EPCI’s “Capacitor, What is it?” overview. Its coupling, decoupling, filter, smoothing, pulse-energy and snubbing categories are useful prompts, but its component requirements are broad and application-dependent. It also depicts 230 VAC EMI suppression and legacy TV circuits; keep these descriptive only and out of Scout builds. EPCI’s image-specific reuse caveat applies here too. The capacitor draft records the source and visual-rights check.

## 2026-11-11 — Ceramic capacitor voltage-coefficient plot reviewed

- **Source assessment:** The supplied “Voltage Coefficients” figure matches Figure K-2 in the Knowles/NOVACAP technical brochure. Its x-axis is volts per mil of dielectric thickness; the curves are construction/formulation examples, not universal X7R, Y5V or BX behaviour. Applied DC bias can reduce Class 2 ceramic capacitance, but modern selection requires the exact part’s DC-bias curve or datasheet. Do not reuse this image without confirming rights. See the [[sites:scouts-electronics-badge:blog:capacitors|capacitor draft]].

## 2026-11-11 — Charge, capacitance and voltage mnemonic

- **Source assessment:** The supplied equation triangle represents ''Q = C × V'', with rearrangements ''C = Q/V'' and ''V = Q/C''. Treat it as a formula memory aid, not an electrical or schematic symbol; label Q in coulombs, C in farads and V in volts. No image source or reuse licence was supplied, so make an original visual if the mnemonic is used. See the [[sites:scouts-electronics-badge:blog:capacitors|capacitor draft]].

## 2026-11-11 — MLCC DC-bias example plot reviewed

- **Source assessment:** The supplied 4.7 µF capacitance-versus-voltage graph matches Figure 19 in Power Integrations AN-90, which identifies it as a simulated TDK characteristic for selected X5R/X7R package sizes and voltage ratings. It usefully shows that nominally equal capacitors can retain different effective capacitance under bias; it is not a universal size/rating rule. Use the exact manufacturer part’s current curve or datasheet, and do not reproduce the figure without confirmed rights. See the [[sites:scouts-electronics-badge:blog:capacitors|capacitor draft]].

## 2026-11-11 — Sine-wave characteristics lesson assessed

- **Source assessment:** The “Sine wave characteristics” transcript introduces amplitude, frequency, period and relative phase. Question 1 of its six-question quiz confirms “phase” as a waveform’s position in time. Use peak amplitude and peak-to-peak voltage precisely; “semi-amplitude” is not the preferred term. For a zero-centred sine, ''Vpp = 2Vp''; with DC offset, measure amplitude from the midline. State ''T = 1/f'' with seconds (the transcript’s 3 Hz example has period 1/3 s). Define phase relative to a reference and compare same-frequency waves; a quarter-cycle offset is 90°. Avoid claiming that all ocean, sound or light waves are sinusoidal. See the course source review and [[sites:scouts-electronics-badge:blog:electronics-fundamentals|fundamentals draft]].

## 2026-11-11 — RF wavelength in fundamentals article

- **User preference:** Include wavelength with the waveform characteristics because Philip works extensively with RF; treat it as an optional advanced blog note, not Scouts core content.
- **Technical note:** Wavelength is ''λ = v_p/f''. Use free-space speed ''c'' only for free-space wavelength; for a cable or PCB trace, use the guided phase velocity (often described by velocity factor). See the [[sites:scouts-electronics-badge:blog:electronics-fundamentals|fundamentals draft]].

## 2026-11-11 — AC voltage and RMS lesson assessed

- **Source assessment:** The full six-question sine-wave quiz identifies phase as waveform time position, RMS voltage as equivalent DC voltage for equal resistor power, the course’s “semi amplitude” as the midline-to-peak difference, “false” for AC electrons moving only in one direction, peak-to-peak amplitude as the peak-to-trough voltage span, and frequency as cycles per second. Use “peak amplitude” in project writing. Explain AC as periodically reversing current, with electron drift opposite conventional current in metal; do not imply all AC has zero mean when a DC component is present. The course’s US example (120 V RMS, 60 Hz; about 170 V peak for a sine wave) is correct. Adapt UK/EU context to nominal 230 V RMS, 50 Hz (about 325 V peak for a sine wave). Explain RMS generally as the square root of the mean squared waveform; ''Vp/sqrt(2)'' is a sine-only shortcut. AC DMM results on distorted signals depend on meter method and specifications such as bandwidth, crest factor and coupling. The outlet procedure must not become a Scout activity; keep practical examples generated and at or below 12 V DC. See the [[sites:scouts-electronics-badge:blog:electronics-fundamentals|fundamentals draft]] and course [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|source review]].

## 2026-11-11 — EMC Engineering Basics course notes assessed

- **Source assessment:** The supplied note summarizes six EMC Engineering Basics slide-note PDFs (lessons 1–5 and 7); it reports that lesson 6 was a hardware demonstration with no PDF. Topics include source–path–victim, conducted/radiated coupling, fields and loops, PCB returns, enclosures, switching harmonics and design mitigations. Treat these as attributed course-summary topics, not independently verified claims or evidence that Philip watched/completed the course. See the [[sites:scouts-electronics-badge:sources:emc-engineering-basics-course-note|course-material note]] and EMC article outlines.

## 2026-11-11 — UK live-conductor terminology

- **User preference:** In UK-context mains references, say “live” or “live conductor”, not the North American term “hot”. Use UK/EU nominal values in explanatory examples and put US equivalents in brackets when useful. The course’s “Measure AC voltage” transcript uses “hot” and US 120 V/60 Hz values; retain these only when describing the source, label them as US terminology, and pair them with UK/EU 230 V/50 Hz context. See the course [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|source review]].

## 2026-11-11 — BS 7671 voltage-drop footnote

- **Editorial decision:** Add a brief UK-only footnote to the fundamentals blog distinguishing the 230 V declared supply under ESQCR from voltage drop along installation wiring under BS 7671. IET explanatory guidance gives recommended public-supply values of 3% for lighting and 5% for other uses. Before publication, verify both ESQCR Regulation 27 (including voltage variation) and the current BS 7671:2018+A4:2026 wording and figures. This is contextual information, not a Scout activity. See the [[sites:scouts-electronics-badge:blog:electronics-fundamentals|fundamentals outline]].

## 2026-11-11 — Frequency-domain lesson assessed

- **Source assessment:** The course’s frequency-domain explanation is useful, but “every signal is a collection of sinusoids” needs qualification: periodic signals use discrete Fourier-series components, while aperiodic signals may have continuous spectra. A DC offset appears at 0 Hz. An FFT efficiently computes a DFT of sampled finite data; frequency resolution and spectral leakage depend on acquisition and windowing, while magnitude-only plots omit phase. See the course [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|source review]] and [[sites:scouts-electronics-badge:blog:electronics-fundamentals|fundamentals outline]].

## 2026-11-11 — Spectrum analyser context

- **User-reported experience:** Philip uses spectrum analysers extensively for EMC and RF work. Include spectrum analysis as an optional advanced topic in the fundamentals blog, alongside scope FFTs. Explain their complementary frequency-domain role and model-dependent settings such as span, RBW and detector; do not suggest that either an FFT or analyser trace alone establishes EMC compliance. See the [[sites:scouts-electronics-badge:blog:electronics-fundamentals|fundamentals outline]].

## 2026-11-11 — EMC course-inspired blog ideas

- **Editorial decision:** Add two optional, adult-facing topics from Karen Burnham’s course-note summaries: switching noise/harmonics/edge rates, and enclosure seams/apertures/cable entries. Keep these separate from the EMC primer and PCB-layout post, use the course only as a topic map, and verify technical claims against primary sources. See the [[sites:scouts-electronics-badge:blog:emc-switching-noise-harmonics|switching-noise idea]], [[sites:scouts-electronics-badge:blog:emc-enclosure-seams-apertures|enclosure idea]] and [[sites:scouts-electronics-badge:sources:emc-engineering-basics-course-note|course note]].

## 2026-11-11 — Bandwidth and square-wave course section

- **Source assessment:** The user supplied the “Bandwidth and square waves” transcript from Barron Stone’s basic-circuits course. Add an optional advanced explanation to the fundamentals post: signal bandwidth versus circuit passband, square-wave harmonics, finite edge rates and finite circuit bandwidth. Qualify that waveform distortion depends on the source, interconnect and load, and avoid one-size-fits-all bandwidth rules. The transcript’s animation is illustrative, not a verified design guide; Scout builds remain at or below 12 V DC.

## 2026-11-11 — Signal-source course section

- **Source assessment:** The user supplied the “Signal sources” transcript. Treat transducers and controlled test sources as useful fundamentals topics. Do not call function generators inherently clean; check exact output specifications. Audio outputs are audio-band sources, and square-wave distortion can result from the entire source-to-measurement chain, not necessarily the playback device alone. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:electronics-fundamentals|fundamentals outline]].

## 2026-11-11 — Frequency-domain quiz wording

- **Source assessment:** The user supplied all six questions from the course’s “Frequency domain” quiz. The intended answers are “sine waves”, “transducer”, “bandwidth”, “a DC offset” for the zero-frequency component, “true” for time- and frequency-domain views representing the same signal, and “time domain” for the standard oscilloscope display. Keep the Fourier-series/transform qualification so quiz shorthand is not read as every signal being a finite sum of sinusoids; explain transducers as energy converters, distinguish sensing from actuation where useful, and define the frequency range meant by bandwidth. Note that some digital oscilloscopes also provide spectrum or FFT displays. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]].

## 2026-11-11 — Impedance course section

- **Source assessment:** The user supplied the “Impedance” transcript and a course slide frame. Correct “reactants” to **reactance**, describe impedance as complex (''Z = R + jX'' for a series combination) rather than adding scalar magnitudes, and state that capacitor current leads voltage by 90° in the ideal sinusoidal case. The frame’s ''1/(2πfC)'' values are reactance magnitudes, not complex impedance; at 10 Hz, 10 µF gives about 1.592 kΩ, and zero frequency is a limit rather than direct substitution. Distinguish ideal DC blocking from real capacitor leakage and include ESR/ESL limits at high frequency. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:electronics-fundamentals|fundamentals outline]].

## 2026-11-11 — Filter frequency-response course section

- **Source assessment:** The user supplied the “Filter frequency response” transcript. Explain frequency response with voltage-amplitude gain and phase versus frequency, typically as Bode plots. Keep voltage and power gain distinct, qualify passive-filter claims by topology and measurement conditions, and do not present the course’s reported low-pass values as reproducible without its schematic and setup. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:electronics-fundamentals|fundamentals outline]].

## 2026-11-11 — Logarithmic-scale course section

- **Source assessment:** The user supplied the “Logarithmic scale” transcript. Explain that equal distances on a logarithmic axis represent equal ratios; define decade (×10) and octave (×2), and distinguish semi-log from log-log plots. In Bode plots, keep logarithmic frequency spacing distinct from expressing magnitude in decibels; zero is not shown on a log frequency axis. Do not reuse the course’s US building-height examples or first-person claims. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:electronics-fundamentals|fundamentals outline]].

## 2026-11-11 — Decibels course section

- **Source assessment:** The user supplied the “Decibels” transcript and its conversion table. Distinguish power-ratio dB from voltage-ratio dB and state impedance conditions; distinguish relative dB gains from referenced levels dBm, dBW and dBV. Use the case-sensitive notation, explain dB summation only for consistently defined cascaded gains, and describe zero ratio as the −∞ dB limit rather than a finite reading. The table is consistent to its rounded precision, with voltage ratios interpreted as power-equivalent only at equal impedances. Do not apply the course’s power-ratio range example to voltage ratios. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:electronics-fundamentals|fundamentals outline]].

## 2026-11-11 — RC low-pass filter course section

- **Source assessment:** The user supplied the “RC low pass filter” transcript. Its nominal 10 kΩ/10 nF cutoff calculation is correct for the unloaded first-order topology. Explain that source resistance, load and part tolerance affect the response; at cutoff, the ideal first-order filter has 0.707 voltage ratio and −45° phase. Half-power language assumes equal impedances, and phase lag is not a fixed time delay. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:electronics-fundamentals|fundamentals outline]].

## 2026-11-11 — RC high-pass filter course section

- **Source assessment:** The user supplied the “RC high pass filter” transcript. For the ideal unloaded series-C/shunt-R topology, use ''H(jω) = jωRC/(1 + jωRC)'' and ''f_c = 1/(2πRC)''; 10 kΩ and 10 nF give about 1.59 kHz. At cutoff, output amplitude is 0.707 of passband and phase lead is +45°; half-power wording requires equal impedances. A settled DC component is blocked, but transitions in offset create transients and circuit bias determines the output reference. Check source/load effects and do not treat course scope traces as reproducible without setup details. See the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course source review]] and [[sites:scouts-electronics-badge:blog:electronics-fundamentals|fundamentals outline]].

## 2026-11-11 — Impedance bridging and matching course section

- **Source assessment:** The user supplied the “Impedance matching and bridging” transcript. Distinguish high-input/low-output impedance voltage bridging from matching for maximum power or transmission-line reflection control. The 10:1 load/source ratio is a rule of thumb, not a universal boundary; a resistive voltage-divider model gives 90.9% of open-circuit voltage at 10:1 and 99.9% at 1000:1. For reactive AC maximum-power transfer, use complex-conjugate matching. Do not describe every lumped impedance mismatch as reflected travelling energy.
- **Project outcome:** Added this distinction to the course review and fundamentals outline, with an RF tutorial and university voltage-divider lab as references.

## 2026-11-12 — Audio low-pass filter challenge

- **Source assessment:** The user supplied the “Challenge: Filter audio” transcript. Treat its 150 Hz ±10 Hz target as a first-order signal-level low-pass design exercise. The source impedance and amplifier input impedance affect the actual cutoff; a representative 11 kΩ/100 nF pair gives about 146.2 Hz with 3 Ω source and 1 MΩ load, but those are assumptions to label. Explain the 20 dB/decade roll-off and distinguish this single RC stage from a complete speaker crossover.
- **Project outcome:** Added the loaded calculation and example to the course review and fundamentals outline. The outline points to the University of Colorado Boulder filter and voltage-divider labs.

## 2026-11-12 — Audio filter solution checked

- **Source assessment:** The supplied solution selects 10 kΩ and 100 nF. This gives 159.2 Hz unloaded, or about 159.6 Hz with assumed 3 Ω source and 3 MΩ load, within the 140–160 Hz tolerance. A 1 MΩ load would shift it to about 160.7 Hz. The reported 0.71 amplitude ratio at 150 Hz is approximate; the ideal unloaded ratio is about 0.728. Keep measured scope values distinct from calculated ideal values, and explain that the single-pole response is not a complete subwoofer crossover.
- **Project outcome:** Added the course solution and its checked assumptions to the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|source review]] and [[sites:scouts-electronics-badge:blog:electronics-fundamentals|fundamentals outline]].
- **Diagram handling:** The user supplied the solution’s schematic frame, confirming a 10 kΩ series resistor and 100 nF shunt capacitor with output across the capacitor. Do not reuse the course image; use an original IEC-style redraw with left-to-right signal flow and circuit common below.

## 2026-11-12 — Impedance quiz questions 1–12

- **Source assessment:** Question 1 correctly selects a load impedance significantly greater than the source impedance for maximising voltage transfer. Question 2 selects equal impedances for maximum power transfer in a simple resistive model; for complex AC impedances, the load must be the source’s complex conjugate. Question 3’s “AC signals” answer is best described as unwanted AC ripple/noise that the capacitor may shunt, subject to impedance and layout. Question 4’s 71% is the rounded −3 dB voltage-amplitude ratio relative to the passband; it equals a fraction of input amplitude only with unity passband gain. Question 5 correctly says first-order RC high-pass and low-pass filters can use the same resistor and capacitor in different arrangements. Question 6’s intended answer is “low”, but this only describes the series capacitor in a high-pass filter; a low-pass filter’s shunt capacitor diverts high-frequency components. Question 7 correctly identifies high frequencies as what a low-pass filter attenuates; phrase this as attenuation, not total removal. Question 8’s 50% is the power ratio at −3 dB relative to the passband; output/input power comparison assumes matching reference impedances. Question 9 correctly identifies impedance’s unit as the ohm, not the farad. Question 10 correctly selects resistance and reactance as the components of impedance; explain this as the complex combination ''Z = R + jX'', not a scalar addition of magnitudes. Question 11 correctly identifies gain and phase shift as the quantities shown in a Bode plot versus frequency; magnitude may be shown as a linear ratio or in decibels, with phase and frequency axes clearly labelled. Question 12 correctly selects high-frequency signals: a capacitor’s ideal reactance magnitude decreases with frequency, within its capacitive operating range; parasitic inductance limits the trend at high frequencies. Only questions 1–12 of the 15-question quiz have been supplied.
- **Project outcome:** Recorded the questions and their distinctions in the [[sites:scouts-electronics-badge:sources:electronics-foundations-basic-circuits-review|course review]].
