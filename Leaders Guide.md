# Scouts Electronics Activity Badge: Leaders’ Guide

**Working draft**

This guide is for adult Leaders preparing and supervising electronics activities for Scouts and Explorers aged 10 to 16. It complements the [learner booklet](Scouts%20Electronics%20Activity%20Badge%20Booklet.md); it does not replace current Scouts policy, activity-specific risk assessment, manufacturer instructions, or component data sheets.

This is a UK-centric project. Check current UK Scouts and Health and Safety Executive guidance before each activity. A source from another country may use different rules, equipment, terminology, or assumptions.

## Use alongside the learner booklet

The learner booklet contains explanations and practical work for young people. Use this guide to plan sessions, check equipment and circuits, and decide which work needs direct adult involvement. Keep instructions to Scouts short and practical, then let them do as much of the work as their experience and the activity risk assessment allow.

Check the current [Scouts Electronics Activity Badge requirements](https://www.scouts.org.uk/scouts/activity-badges/electronics/) when planning the programme. The requirements listed in the learner booklet were checked against the Scouts page on 2026-11-06.

## Plan a badge programme

The badge asks Scouts to identify components, read resistor and capacitor markings, use circuit symbols, recognise diode polarity and an IC pin, use a multimeter, compare analogue and digital circuits, build three circuits, explain how they work, and discuss how electronics is used. One circuit should be mainly digital. If possible, at least one should be soldered on stripboard or a PCB.

Plan a sequence that gives Scouts time to build, test, explain, and improve their circuits. A possible progression is:

1. Identify components and symbols; practise reading resistor markings.
2. Build and measure a simple, low-voltage circuit before adding more parts.
3. Introduce analogue control and digital logic with a circuit or simulation.
4. Build the three badge circuits and record their purpose, operation, supply voltage, and measured values.
5. If suitable, solder a through-hole project such as the Woggle PCB with close adult supervision.
6. Give each Scout time to explain what they built and what they would change.

Adapt this sequence to the group's experience, access needs, time, equipment, and current Scouts guidance. The Woggle PCB is through-hole. Surface-mount soldering and PCB repair are optional advanced topics, not requirements for the Woggle activity.

## Activity ideas

The reviewed [IET activity-pack review](Source%20Documents/iet-scout-electronics-badge-activity-pack-review.md) records ideas from an older pack: an electronics diary, resistor-colour game, multimeter exercises, brush bug, steady-hand game, light-sensitive night light, light-up map, electronic dice, memory and reaction game, flashing guide, and open-ended design challenges.

Treat those as project prompts only. The original PDF's diagrams and build instructions were not visually checked, and some extracted text was unclear. Before using an idea, choose or design a circuit for the actual components and supply, verify the parts and ratings, and check that the activity suits the group. Do not reproduce a circuit from a title or partial text alone.

## Safety preparation

Follow Scouts' current [Safety Policy](https://www.scouts.org.uk/por/2a-key-policies/2a8-safety-policy/) and [risk-assessment guidance](https://www.scouts.org.uk/volunteers/staying-safe-and-safeguarding/risk-assessments/). Assess the actual venue, participants, tools, materials, and task before the session, and keep reviewing conditions while the activity is in progress. This section is a planning aid, not a substitute for the required activity assessment or local procedures.

Before starting, check that:

- the work area is stable, tidy, well lit, and suitable for the task;
- tools and power supplies are undamaged and suitable for the project;
- the Leader in charge has explained the safe working area, tool handling, stop signal, and what to do if something goes wrong;
- young people have suitable supervision, eye protection where needed, and a clear place to put hot tools;
- each circuit has been checked before power is connected;
- the group's first-aid and emergency arrangements are in place.

### Soldering and fume control

Soldering irons and recently soldered parts can burn. Secure the iron in its stand when it is not in use, route its cable to reduce snagging, and keep hot tools away from people and combustible materials. Wear safety glasses when soldering and trimming leads. Let joints and clipped leads cool before handling them.

Flux fume needs effective control. The HSE identifies rosin-based solder-flux fume as a cause of occupational asthma and advises using fume extraction, keeping the head out of the plume, and not overheating the iron. See the [HSE solderer guidance](https://www.hse.gov.uk/asthma/solderers.htm). Position extraction so it captures the fume at the source; ordinary room ventilation is not a substitute for effective extraction where it is needed.

Some solder contains lead. Keep food and drink away from the work area, prevent solder and clipped leads from reaching mouths, and have everyone wash their hands after handling solder. See the [HSE lead hygiene guidance](https://www.hse.gov.uk/lead/mostatrisk.htm). Select solder and flux for the task and follow their labels and safety information.

### Batteries, power, and flammable cleaners

Use only a supply appropriate to the verified circuit. Check polarity, component ratings, and the risk of short circuits before connecting a battery or USB supply. A low voltage does not make a short circuit harmless: batteries can deliver enough current to heat wires or damage components. Keep mains-powered equipment closed and out of beginner repair activities.

Isopropyl alcohol and some other board cleaners are flammable. Follow the product label and safety information, keep containers closed and away from ignition sources, and do not clean a board near a soldering iron, hot-air station, or hot plate. Let the board dry fully before applying power. Do not put solvent into an ultrasonic cleaner unless the equipment and cleaner manufacturers explicitly approve that use and the relevant risk controls are in place.

## Check a circuit before power is applied

Use a consistent check with Scouts before connecting the supply:

1. Compare the built circuit with the schematic and the project instructions.
2. Check battery or supply polarity and voltage.
3. Check component orientation, especially LEDs, diodes, electrolytic capacitors, transistors, and IC pin 1.
4. Confirm that each LED has suitable current limiting for its supply and the actual LED.
5. Look for solder bridges, loose wires, exposed conductors, and possible shorts.
6. Confirm the multimeter is in the correct mode and its leads are in the correct sockets before measuring.
7. Connect power only after the Leader has completed the check.

If a circuit behaves unexpectedly, disconnect power before inspecting or changing it. Do not troubleshoot a powered circuit by moving bare wires or probing where a short could occur.

## Helping Scouts use a multimeter

Demonstrate the meter before the activity. Resistance is measured on an unpowered circuit. Voltage is measured across two points in parallel. Current is measured with the meter in series, which means the circuit must be opened and the meter inserted into the current path. Putting a meter set to current directly across a battery can short the supply and damage the meter or wiring.

Before each measurement, have Scouts check the dial, sockets, range, and lead polarity. Use a known simple circuit and follow the meter manufacturer's instructions. Ask Scouts to predict what they expect to measure, take the reading, and explain whether it agrees with their prediction.

## Soldering the Woggle PCB

The Woggle is a through-hole project with LEDs and a small DIP eight-pin microcontroller. Before the session, identify the parts, confirm the board and component instructions, and prepare the soldering stations and fume extraction. Demonstrate one joint, then let Scouts practise on a sacrificial board or spare pads if available.

Use the learner booklet's through-hole sequence: fit and secure a component, heat the pad and lead together, feed a small amount of solder into the joint, let it cool without movement, inspect it, then trim the lead while retaining the solder fillet. For the IC, verify the notch or pin-one mark against the PCB before soldering the socket or component. On a multi-pin part, tack a pin, check alignment, solder several other pins, then reflow the first pin. This can relieve stresses as the part settles and gives an opportunity to add a little solder if needed.

Do not treat one iron temperature or soldering time as universal. Follow the iron, solder, and component guidance and adjust the process to the joint. The learner booklet records Philip's reported bench setting separately from general advice.

## Advanced topics for Leaders

The learner booklet keeps surface-mount soldering in further reading because the Woggle is through-hole. If you demonstrate surface-mount work, treat it as a separate advanced activity. Check the board, parts, paste, flux, heating equipment, extraction, and cleaning process first; secure the board; protect nearby components; and inspect the finished joints before power is applied.

Hot-air rework, hot plates, solder-paste stencils, IC removal, track cutting, and jumper-wire repairs can damage components or boards and introduce additional heat, fume, chemical, and tool hazards. They are not beginner badge tasks. The Leader should have relevant practical experience, follow the equipment and material instructions, and decide whether the activity is appropriate for the participants and venue.

### Prototype PCB track repair

This is advanced prototype rework, not a badge activity. Philip reports cutting an incorrect PCB track with a small scalpel or a drill bit chosen for the track size, then checking with a multimeter that the unwanted connection is open. For the corrected connection, he uses enamelled copper wire as a jumper and secures it flat to the board with superglue so it is less likely to catch on something. More detail is in the adult-focused [PCB rework draft](blog-drafts/pcb-rework.md).

Treat this as one person's reported method, not a universal repair instruction. Before attempting it, confirm the intended circuit connection from the design files, disconnect the board from power, assess sharp-tool and debris risks, secure the board, and protect the eyes. Check the cut for electrical isolation and the repair for continuity before reconnecting power. Check the jumper's insulation and mechanical support, and make sure the adhesive is suitable for the board and repair. Do not use this method on mains-connected or otherwise hazardous equipment.

### Philip's reported bench setup

Philip reports using two temperature-controlled soldering irons at home: a small USB-C iron and a bench iron with a hot-air rework station. He also has a small hot plate. His soldering iron and hot-air station are set to 400 °C for his own work; this is his reported setup, not a recommended setting for another tool or project.

Philip also reports that his helping hands and vice use magnetic bases, and that he replaced the aluminium base under his USB microscope with a steel one so the magnetic holders can attach. This may be useful as a bench-layout idea, but check stability and keep magnets and metal fixtures clear of exposed electrical connections.

## Sources and status

- [Scouts Electronics Activity Badge requirements](https://www.scouts.org.uk/scouts/activity-badges/electronics/)
- [Scouts Safety Policy](https://www.scouts.org.uk/por/2a-key-policies/2a8-safety-policy/)
- [Scouts risk-assessment guidance](https://www.scouts.org.uk/volunteers/staying-safe-and-safeguarding/risk-assessments/)
- [HSE solderer guidance](https://www.hse.gov.uk/asthma/solderers.htm)
- [HSE lead hygiene guidance](https://www.hse.gov.uk/lead/mostatrisk.htm)
- [Review of the older IET Scout activity pack](Source%20Documents/iet-scout-electronics-badge-activity-pack-review.md)

This guide is a working draft. Check linked guidance and equipment instructions again before running an activity; they can change. Add project-specific risk controls and circuit notes as each session is developed.
