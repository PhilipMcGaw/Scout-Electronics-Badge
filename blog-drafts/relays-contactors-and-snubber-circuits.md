# Relays, contactors and contact protection

**Status:** Outline started; no circuit values or construction instructions.

**Audience:** Adult electronics makers. Keep any Scout-facing explanation to basic relay operation and Leader-supervised, extra-low-voltage examples.

## Purpose

Explain what a relay and contactor do, why contacts can arc when switching a load, and how suppression can reduce electrical stress in a suitable design. Separate suppression across the switched load/contacts from suppression across the relay or contactor coil.

## Planned outline

1. Compare a relay and a contactor, and explain coil, armature, normally-open and normally-closed contacts.
2. Explain that load type matters: resistive, inductive, motor and capacitive loads place different demands on contacts. Rated current alone does not establish suitability.
3. Explain why inductive current continues when a contact opens and may sustain an arc. Briefly describe how arcing can wear or damage contacts and create electrical noise.
4. Introduce suppression choices at a conceptual level:
   - a diode or diode-plus-Zener clamp across a DC inductive load;
   - an RC snubber or a correctly rated varistor/TVS for applications where a simple diode is unsuitable;
   - manufacturer-designed suppression accessories for a relay or contactor coil.
5. Clearly separate **load/contact suppression** from **coil suppression**. A device across the coil protects the control circuit from the coil’s turn-off transient; it does not automatically protect the main contacts switching another load.
6. Explain trade-offs: suppression can change release/drop-out time; a diode clamp often delays release more than higher-voltage clamps; RC networks can cause off-state leakage; capacitors can cause closing inrush and contact welding if selected or connected incorrectly.
7. Explain that effectiveness and component ratings depend on load waveform, voltage, current, switching frequency, wiring, relay/contact ratings and the specific suppression device. Select from relay/contactor and suppressor manufacturer data and validate the actual application.
8. Add a safety boundary: mains, high-current DC, motors and contactors are not appropriate for an unsupervised hobby snubber experiment. Do not present a generic RC value as a universal fix or a replacement for an under-rated relay/contactor.
9. Finish with a short, original knowledge check. Cover normally-open versus normally-closed contacts, the difference between coil and contact ratings, why load type changes contact suitability, what a coil suppressor protects, and why a flyback diode can slow release. Give feedback with each answer; do not copy questions or wording from the linked quiz.

### Possible knowledge-check questions

1. In a conventional non-latching relay, what does “normally open” describe? **Answer:** The contacts are open when the coil is not energised.
2. Does a relay’s coil voltage tell you the voltage and current its contacts can switch? **Answer:** No. Coil ratings and contact ratings describe different parts of the relay.
3. Why is a contact rating for a resistive load not enough to choose a relay for a motor? **Answer:** A motor’s starting and inductive behaviour can stress contacts differently; check the relay data for the actual load type and switching conditions.
4. What does a suppressor placed across a DC relay coil mainly protect? **Answer:** The coil-switching circuit from the voltage transient when the coil is switched off; it does not automatically suppress arcing at contacts switching a separate load.
5. What is one trade-off of a diode across a DC coil? **Answer:** It limits the turn-off voltage, but can make the relay release more slowly.

## Source assessment and checks

- element14 Community, [“Relay Technologies”](https://community.element14.com/learn/learning-center/essentials/w/documents/27489/relay-technologies), created 2022-02-23 and last updated 2022-12-16; sponsored by TE Connectivity. Useful topic map for relay operation, NO/NC/changeover contacts, relay types, and selection factors. Treat its broad comparisons, ratings, timing and application claims as historical or product-specific pointers: check the exact current relay datasheet and manufacturer application guidance. In particular, do not assume all relays provide galvanic isolation or transfer its generic current/voltage ranges and SSR comparisons to a chosen device. Write original explanations and visuals.
- Wikipedia’s [snubber overview](https://en.wikipedia.org/wiki/Snubber?useskin=vector) is a broad topic overview only.
- Making Easy Circuits’ [relay-contact snubber article](https://makingcircuits.com/blog/snubber-circuits-for-protecting-relay-contacts-from-arcing/) introduces diode, RC and varistor approaches, but its generalised selection numbers are not design rules.
- Homemade Circuit Projects’ [relay arcing article](https://www.homemade-circuits.com/prevent-relay-arcing-using-rc-snubber-circuits/) discusses RC concepts, but its generic numerical suggestions and comment advice for mains circuits are not suitable to reuse.
- Panasonic’s [relay contact-protection guidance](https://industry.panasonic.com/ap/en/products/control/relay/cautions_use) documents application-dependent failure modes, load placement and suppression trade-offs.
- Omron’s [automotive relay precautions](https://omronfs.omron.com/en_US/ecb/products/pdf/auto_precautions.pdf) discusses contact protection and warns that it can extend relay release time; the automotive examples are not universal.
- TE Connectivity’s [DC relay coil suppression note](https://www.te.com/en/products/relays-and-contactors/electromechanical-relays/intersection/relay-coil-suppression-dc-relays.html) distinguishes coil transients from contact-load behaviour.
- Siemens’ [SIRIUS contactor manual](https://cache.industry.siemens.com/dl/files/557/60306557/att_894291/v1/manual_SIRIUS_contactors_3RT_en-US.pdf) and Schneider Electric’s [contactor suppressor guidance](https://www.se.com/ca/en/faqs/FA102916/) show coil suppressors and manufacturer-specific drop-out-time effects. Check the current manual for the exact contactor.
- element14 Community / Omron, [Power Relays Quiz](https://community.element14.com/products/manufacturers/omron-electronic-components/w/quiz/4497/power-relays-quiz). The 25-question quiz covers electromechanical relays, electrical contacts and PCB power relays. Use it as inspiration for topic coverage only; write original questions and check answers against the post and current manufacturer information.

## Visuals

- If a diagram is needed, create an original low-voltage DC example that labels the coil and switched load separately. Do not copy the source diagrams.
- No mains wiring diagram or generic RC component values are planned.
