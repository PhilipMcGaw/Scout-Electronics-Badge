# KiCad feature request: automatic placement of PCB footprint fields

- **Captured:** 2026-11-13
- **Status:** Proposed; not submitted to the KiCad issue tracker
- **Type:** Feature request, not a bug report
- **Related project work:** [PCB silkscreen blog draft](../pages/sites/scouts-electronics-badge/blog/pcb-silkscreens.txt)

## Idea

Request a PCB Editor equivalent to the Schematic Editor's **Autoplace Fields** command (`O`). The proposed function would automatically position each footprint's reference designator beside its owning footprint, rather than merely aligning selected text objects with one another.

This would be especially useful after globally resizing reference designators for silkscreen readability, or after moving and rotating components during layout.

## Draft issue

### Title

**PCB Editor: add automatic placement of footprint fields**

### Summary

Please add an automatic field-placement function to the KiCad PCB Editor, comparable to **Autoplace Fields** (`O`) in the Schematic Editor.

The function should automatically position footprint reference designators (and optionally other footprint fields) in a clear, consistent position relative to their associated footprints.

### Problem

When laying out a PCB, reference designators often need to be moved manually to avoid pads, component outlines, other text, and board-edge constraints.

This becomes particularly time-consuming when:

- Components are moved or rotated during layout.
- Reference designators are resized globally to meet silkscreen manufacturing requirements.
- A design is reorganised late in the layout process.
- A consistent visual arrangement of reference designators is required.

The Schematic Editor already provides an Autoplace Fields command, accessed using `O`. There does not appear to be an equivalent operation in the PCB Editor.

### Proposed behaviour

Provide an **Autoplace Footprint Fields** command in the PCB Editor.

The command should:

1. Identify each footprint's reference designator and its owning footprint.
2. Automatically position the reference designator close to its associated footprint.
3. Consider the footprint outline, pads, courtyard, other text, and board edges when selecting a position.
4. Avoid overlapping other reference designators and visible silkscreen graphics wherever possible.
5. Maintain readable text orientation, including for rotated footprints.
6. Optionally snap the resulting field positions to the active or a user-configurable grid.
7. Support applying the operation to selected footprints or the entire board.

### Additional options

It would be useful to provide options for:

- Preferred placement: above, below, left, or right of the footprint.
- Text orientation: keep horizontal or rotate with the footprint.
- Minimum clearance from pads and other graphical objects.
- Grid spacing for the resulting positions.
- Whether to reposition only reference designators or all eligible footprint fields.

### Expected benefit

This would reduce repetitive manual editing, improve silkscreen consistency, and make it easier to apply manufacturing-friendly text sizing across an entire PCB.

It would be particularly useful after using the global text and graphics properties editor to resize reference designators.

The aim is not to guarantee a perfect placement in every case, but to provide a sensible automatic starting position that the designer can subsequently adjust manually.

## Technical distinctions to retain

- The schematic editor's `O` command is documented as **Autoplace Fields**.
- In the PCB Editor, moving a field can use the active grid, and Align/Distribute tools align selected objects relative to one another. Those operations do not provide the requested per-footprint automatic placement.
- The request should focus on positioning a field relative to its owning footprint. Grid snapping is a useful option, but is not the central feature.
- A Python-based placement utility could be explored separately, but it is not an existing or verified native capability and should not be presented as one.

## Before submitting

- Search the KiCad issue tracker for an existing request covering automatic PCB footprint-field placement; avoid creating a duplicate.
- Confirm the current KiCad version and exact terminology/menu names.
- Add a small PCB example or annotated screenshot if it helps demonstrate the manual repositioning problem.
- Submit as a feature proposal and invite discussion of placement rules and collision handling.

## References

- [KiCad Schematic Editor documentation](https://docs.kicad.org/10.0/en/eeschema/eeschema.html) — Autoplace Fields.
- [KiCad PCB Editor documentation](https://docs.kicad.org/10.0/en/pcbnew/pcbnew.html) — footprint fields, text/graphics editing, grid snapping, and Align/Distribute.
- [KiCad issue tracker](https://gitlab.com/kicad/code/kicad/-/issues).
