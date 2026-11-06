# Preparing the Woggle PCB with KiCad

**Status:** Outline started.

**Purpose:** Give Scouts and their Leaders a step-by-step path from the supplied Woggle design files to a checked PCB order and component list.

## Planned outline

1. Confirm the Woggle project files and board revision.
2. Open the project in KiCad and inspect the schematic and PCB layout. Follow a connection from its schematic symbol through the board tracks to the relevant pads.
3. Explain how the Woggle uses Charlieplexing to drive its LEDs with fewer microcontroller pins. Check the LED connections and firmware before describing the scan pattern.
4. Change the group name and check project metadata.
5. Generate a CSV bill of materials and match each item to the assembly instructions.
6. Prepare the manufacturing files requested by PCBWay and inspect the online previews.
7. Check quantities, parts, order details, and total cost with a Leader before ordering.
8. When the boards arrive, compare them with the design and assemble one at a time.

## Notes to verify before drafting

- Record the exact KiCad version and menu names used for the walkthrough.
- Confirm the current group-name change workflow and the Woggle source-file licence.
- Check PCBWay’s current file and order requirements; do not reuse prices or lead times without checking them.
- Verify the BOM fields, component references, footprints, quantities, and part sources against the selected Woggle revision.
- The project contains `CharliePlex.GIF` as a general reference diagram. A [PICBasic forum thread](https://www.picbasic.co.uk/forum/showthread.php/19618-Charlie-plexing) appears to show the same image under a forum member's name, but does not establish a reuse licence. Confirm the creator and redistribution permission before publication; otherwise make or source a compatible diagram. Do not infer the Woggle's LED count or scan sequence from that general diagram.

## Visuals

- Plan original screenshots of the KiCad project, BOM export, manufacturing-file checks, and PCBWay preview. Hide personal or account information.
