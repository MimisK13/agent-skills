# Drum Hardware

Use this reference when extracting drum hardware requirements from a technical rider.

The primary goal is to identify which drum hardware must be supplied and separate it from shells, cymbals, microphones, and general stage equipment.

## Extract

Capture hardware requirements for:

- cymbal stands
- snare stands
- hi-hat stand
- kick pedal
- double pedal
- drum throne
- tom holders
- rack system
- clamps
- mounting arms
- drum rug
- stick tray / accessory tray
- music stand or tablet stand, only if explicitly listed for the drummer

For each item, preserve when available:

- quantity
- manufacturer
- model / series
- type
- compatibility notes
- supply responsibility
- required / preferred / acceptable / optional status

## Supply Responsibility

Normalize supply responsibility to:

- `Artist Supplied`
- `Local Production`
- `Venue Supplied`
- `Unspecified`

Examples:

`Drummer brings pedal and sticks`

→ pedal is `Artist Supplied`

`Please provide 4 cymbal boom stands and drum throne`

→ listed hardware is `Local Production`

`House hardware available`

→ `Venue Supplied`

Do not assume local production provides hardware just because a local drum kit is requested.

## Breakables

Treat breakables separately from standard hardware when the rider uses that language.

Common breakables may include:

- snare drum
- cymbals
- kick pedal
- sticks
- brushes / mallets
- drum throne, only if the rider classifies it as breakable

Do not assume the artist supplies breakables unless explicitly stated.

Flag ambiguity when the rider says `artist brings breakables` but later asks local production for cymbals, snare, or pedals.

## Pedals

Distinguish between:

- single kick pedal
- double kick pedal
- hi-hat stand / pedal
- remote hi-hat pedal

Examples:

- `01 x DW 5000 Single Pedal`
- `01 x Tama Iron Cobra Double Pedal`
- `01 x Remote Hi-Hat Stand`

Do not convert `kick pedal` into `double pedal` unless stated.

Do not assume the pedal is included with the kick drum.

## Cymbal Stands

Preserve stand type when specified:

- boom stand
- straight stand
- heavy-duty stand
- short boom
- cymbal arm
- clamp / mounting arm

If the rider says:

`4 cymbal stands`

preserve exactly that. Do not infer which stands are boom or straight.

## Snare Stands

Capture snare stands separately from snare drums.

Examples:

- `01 x Snare Stand`
- `02 x Snare Stands, one for side snare`

If the rider lists a side snare, check whether a second snare stand is explicitly requested or implied by a hardware list. Flag missing hardware if unclear.

## Hi-Hat Stand

Capture hi-hat stand requirements separately from hi-hat cymbals.

Examples:

- `01 x Hi-Hat Stand`
- `01 x DW 5000 Hi-Hat Stand`

Do not assume hi-hat cymbals include the stand.

## Drum Throne

Capture drum throne requirements separately.

Examples:

- `01 x Drum Throne`
- `01 x Roc-N-Soc throne preferred`

Do not omit the throne just because it is commonly included with a kit.

## Tom Mounting

Capture mounting requirements when specified:

- tom holder
- floor tom legs
- cymbal stand tom mount
- rack system
- multi-clamp
- L-arm

Preserve compatibility notes, such as brand-specific tom mounts.

Do not infer tom mounting hardware from shell sizes alone.

## Drum Rug

Capture drum rugs when explicitly requested.

Examples:

- `01 x Drum Rug`
- `Carpet under drum kit required`

Do not assume a rug is required unless stated.

## Required / Preferred / Acceptable

Preserve the rider's semantics:

- `must`, `required`, `no substitutions` → required
- `preferred`, `ideally`, `first choice` → preferred
- `acceptable`, `or equivalent`, `alternatives` → acceptable
- `if available`, `optional` → optional

Never convert a preference into a requirement.

## Output Format

Use one line per hardware item:

`QTY x HARDWARE TYPE MANUFACTURER MODEL NOTES — STATUS — SUPPLY`

Examples:

- `04 x Cymbal Boom Stand — Required — Local Production`
- `01 x Hi-Hat Stand DW 5000 — Preferred — Local Production`
- `01 x Double Pedal Tama Iron Cobra — Required — Artist Supplied`
- `01 x Drum Throne — Required — Local Production`
- `01 x Drum Rug — Optional — Venue Supplied`

## Cross-Checks

Compare hardware against:

- shells
- cymbals
- input list
- stage plot
- breakables notes

Flag missing or inconsistent requirements.

Examples:

- Cymbal list has hi-hat, ride, and two crashes, but hardware lists only one cymbal stand and no hi-hat stand.
- Rider asks for side snare but only one snare stand.
- Stage plot shows auxiliary percussion at drum position, but hardware list has no table or clamps.

Do not invent missing hardware; list it as an advance question.
