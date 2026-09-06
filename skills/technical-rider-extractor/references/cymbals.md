# Cymbals

Use this reference when extracting cymbal requirements from a technical rider.

The primary goal is to identify cymbal requirements and keep them separate from cymbal stands, drum shells, and general breakables notes.

## Extract

For each cymbal requirement, capture when available:

- quantity
- size
- cymbal type
- manufacturer
- model / series
- finish, only if explicitly specified
- special notes
- supply responsibility
- required / preferred / acceptable / optional status

## Supply Responsibility

Normalize supply responsibility to:

- `Artist Supplied`
- `Local Production`
- `Venue Supplied`
- `Unspecified`

Examples:

`Drummer brings own cymbals`

→ cymbals are `Artist Supplied`

`Please provide Zildjian K cymbals`

→ listed cymbals are `Local Production`

`House cymbals available if needed`

→ `Venue Supplied` or `Optional`, depending on wording

Do not assume cymbal responsibility from common touring practice.

## Cymbal Types

Normalize obvious labels to:

- Hi-Hat Pair
- Crash
- Ride
- Splash
- China
- Stack
- Effects Cymbal

Do not infer cymbal type from size alone.

Example:

`18" Zildjian`

→ ambiguous cymbal type

not:

`18" Crash`

unless the rider says crash.

## Hi-Hats

Treat hi-hats as one pair unless the rider specifies otherwise.

Examples:

- `01 x 14" Hi-Hat Pair`
- `01 x 15" Hi-Hat Pair`

Do not list hi-hat top and bottom as separate requirements unless the rider explicitly writes them separately.

Capture hi-hat stand requirements in `hardware.md`, not here.

## Crash Cymbals

Preserve quantity and size.

Examples:

- `02 x 18" Crash`
- `01 x 17" Crash`
- `01 x 19" Crash`

Do not assume two crashes unless the rider specifies two crashes or lists separate crash inputs/positions that need confirmation.

## Ride Cymbals

Preserve ride type and size when specified.

Examples:

- `01 x 20" Ride`
- `01 x 22" Ride Zildjian K`
- `01 x 21" Sweet Ride`

Do not infer ride brand or series from another cymbal in the list.

## China, Splash, Stack, and Effects

Preserve special cymbals separately.

Examples:

- `01 x 18" China`
- `01 x 10" Splash`
- `01 x Stack`
- `01 x FX Cymbal`

Do not merge these into a generic `cymbal set` unless the rider itself uses that wording.

## Manufacturer and Series

Preserve manufacturer and series when specified.

Examples:

- `Zildjian K`
- `Zildjian A Custom`
- `Sabian HHX`
- `Meinl Byzance`
- `Paiste 2002`

If the rider gives alternatives, preserve the preference language.

Example:

`Zildjian K preferred, Sabian HHX acceptable`

must preserve:

- Preferred: `Zildjian K`
- Acceptable: `Sabian HHX`

Do not treat acceptable alternatives as equal preferences.

## Breakables

Cymbals are often considered drummer breakables, but do not assume responsibility.

Extract only what the rider says:

- `Drummer brings own cymbals` → `Artist Supplied`
- `Please provide cymbals` → `Local Production`
- no statement → `Unspecified`

Flag ambiguity when breakables notes and cymbal lists disagree.

## Required / Preferred / Acceptable

Preserve the rider's semantics:

- `must`, `required`, `no substitutions` → required
- `preferred`, `ideally`, `first choice` → preferred
- `acceptable`, `or equivalent`, `alternatives` → acceptable
- `if available`, `optional` → optional

Never convert a preference into a requirement.

## Output Format

Use one line per cymbal item:

`QTY x SIZE TYPE MANUFACTURER MODEL NOTES — STATUS — SUPPLY`

Omit fields that are not specified.

Examples:

- `01 x 14" Hi-Hat Pair Zildjian K — Required — Artist Supplied`
- `02 x 18" Crash Zildjian A Custom — Required — Local Production`
- `01 x 22" Ride Zildjian K — Preferred — Local Production`
- `01 x 18" China — Optional — Unspecified`

## Stage Plot

Use stage plots as supporting information for:

- cymbal count
- drummer position
- stand count cross-checks
- additional percussion or auxiliary cymbal stations

Do not treat every drawn cymbal as a confirmed local requirement unless the rider text supports it.

## Cross-Checks

Compare cymbals against:

- drum hardware
- backline notes
- input list
- stage plot
- breakables notes

Flag conflicts when:

- cymbals are shown on the stage plot but not listed in backline
- cymbal count exceeds cymbal stand count
- rider says artist brings breakables but also lists cymbals under local backline
- input list has many cymbal microphones but cymbal requirements are missing or unclear

Do not resolve conflicting quantities, models, sizes, or supply responsibility by assumption.
