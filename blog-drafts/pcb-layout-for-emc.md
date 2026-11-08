# PCB layout for better EMC

**Status:** Outline started; no compliance claim or fixed design rules.

**Audience:** Adult makers and experienced Scouts/Explorers with Leader support. Keep examples at extra-low voltage.

## Purpose

Show how PCB geometry, return paths, switching edges, cables and enclosures can affect electromagnetic emissions and susceptibility. Present layout practices as ways to reduce risk, not guarantees of passing a test.

## Planned outline

1. Begin with a simple source, path and victim model: a fast switching edge or noisy converter, a coupling path, and a sensitive input or nearby receiver.
2. Explain that current flows in a loop. For fast-changing signals, the return path tends to follow close to the signal path when a continuous reference plane is available; interruptions can enlarge loops and increase coupling.
3. Discuss practical layout habits with limits:
   - place decoupling components close to the IC supply pins and provide a short return path;
   - keep high-current switching loops compact;
   - keep sensitive analogue inputs away from noisy switching nodes and motor/relay currents;
   - avoid routing fast signals across gaps in their reference plane;
   - plan connectors, cable return conductors, enclosure bonding and board edges as part of the system;
   - choose edge rates and switching frequencies appropriate to function, while following device requirements.
4. Avoid simplistic rules such as “all traces are transmission lines” without considering edge rate, geometry and length. Avoid splitting ground planes by default; explain that return paths and partitioning need a circuit-specific plan.
5. Introduce low-cost troubleshooting and pre-compliance tools at a high level: near-field probes, current probes, LISNs and spectrum analysers each answer different questions and require suitable setup, calibration/corrections and safety controls.
6. Explain that measurements made with different cables, grounding, distances, operating modes or detector settings may not be comparable with a standard test. A spectrum plot or software limit line alone is not a compliance result.
7. State that emissions and immunity are separate test areas, and that final product performance depends on the complete board, enclosure, cables, power supply and intended installation.

## Sources and assessment

- Kenneth Wyatt, EDN, [“Design PCBs for EMI, part 1: How signals move”](https://www.edn.com/design-pcbs-for-emi-part-1-how-signals-move/), 2019-03-05. Helpful engineering discussion of fields, reference planes and return paths. Treat its broad rules as an introduction, not universal requirements; check examples against the design’s rise time, stack-up and current path.
- Tekbox, [EMCview PC software](https://www.tekbox.com/product/emcview-pc-software-emc-compliance-testing/). Vendor description of software for emissions pre-compliance and some immunity workflows with supported instruments. Use as a product capability reference, not independent validation that any setup is standards-compliant.
- Elektor, [Dual DC LISN (150 kHz–200 MHz)](https://www.elektor.com/products/elektor-dual-dc-lisn-150-khz-200-mhz) and [user manual](https://s3.eu-central-1.amazonaws.com/elektormagazine/shopify/l6LMLHfRQh1GdMZuqj2UEK8wvDGW6bVj.pdf). Product-specific example of a dual 5 µH / 50 Ω DC LISN for conducted-emissions pre-compliance work, with a specified 150 kHz–200 MHz RF bandwidth, <60 V DC and <10 A DC limits. The manual describes a CISPR 25 / ISO 7637 automotive context and restricts use to authorised technical staff. Do not present it as a universal LISN, a formal compliance setup by itself, or a Scout activity; follow the manual and applicable test method.
- IEC, [IEC TR 61000-1-1:2023](https://webstore.iec.ch/en/publication/70473). Terminology and distinction between standardised EMC tests and in-situ checks.
- UK Government, [Electromagnetic Compatibility Regulations 2016: Great Britain](https://www.gov.uk/government/publications/electromagnetic-compatibility-regulations-2016/electromagnetic-compatibility-regulations-2016-great-britain), for product-level context.

## Visuals

- Create an original diagram showing a signal trace over a reference plane, close return path, a plane gap causing a detour, and a separate high-current switching loop. Label it as a simplified model.
- Do not reproduce the EDN diagrams or Tekbox product screenshots without permission and attribution checks.
