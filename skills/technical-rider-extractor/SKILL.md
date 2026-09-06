---
name: technical-rider-extractor
description: Extracts structured production data from artist technical riders. Use for rider PDFs, stage plots, backline, drums, amplifiers, microphones, input lists, monitors, IEM, stage requirements, and other live audio production specifications.
license: Apache-2.0
metadata:
  author: mimisk
  version: "0.1"
---

# Technical Rider Extractor

Extract technical rider information into structured data.

## Rules

- Never invent missing information.
- Preserve required / preferred / acceptable / optional semantics.
- Preserve quantities, dimensions, manufacturer and model.
- Record source page when possible.
- Flag contradictions and ambiguities.
- Inspect visual PDF pages when tables, stage plots or diagrams matter.

## References

Load only the references relevant to the rider content.

### Backline

- Drums: [references/drums.md](references/drums.md)
- Guitars: [references/guitars.md](references/guitars.md)
- Bass: [references/bass.md](references/bass.md)
- Keyboards: [references/keyboards.md](references/keyboards.md)
- Percussion: [references/percussion.md](references/percussion.md)

### Monitoring

- Monitors / IEM / Personal Monitoring: [references/monitor.md](references/monitor.md)

### FOH and PA

- FOH: [references/foh.md](references/foh.md)
- PA: [references/pa.md](references/pa.md)

### Inputs

- Input List: [references/input-list.md](references/input-list.md)

## Drum References

When drum requirements are present, use the relevant drum references:

- Shells: [references/shells.md](references/shells.md)
- Hardware: [references/hardware.md](references/hardware.md)
- Cymbals: [references/cymbals.md](references/cymbals.md)
