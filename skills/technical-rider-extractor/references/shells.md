# Drum Shells

Use this reference when extracting drum shell requirements from a technical rider.

The primary goal is to identify which drum shells are required, preferred, acceptable, artist-supplied, locally supplied, venue-supplied, or unspecified.

## Extract

For each shell, capture when available:

- quantity
- diameter
- depth
- drum type
- manufacturer
- model / series
- finish, only if explicitly required
- heads, only if specified
- tuning / special notes
- supply responsibility
- required / preferred / acceptable / optional status

## Supply Responsibility

Normalize supply responsibility to:

- `Artist Supplied`
- `Local Production`
- `Venue Supplied`
- `Unspecified`

Examples:

`Artist travels with snare and cymbals`

→ snare is `Artist Supplied`

`Please provide 22" kick, 12" rack, 16" floor tom`

→ listed shells are `Local Production`

`House drum kit may be used`

→ `Venue Supplied`

Do not assume shell responsibility from common touring practice.

## Common Shell Types

Normalize obvious labels to:

- Kick Drum / Bass Drum
- Snare Drum
- Side Snare
- Rack Tom
- Floor Tom

Do not merge multiple toms into `Tom Set` unless the rider itself uses that wording.

## Sizes

Preserve shell sizes exactly as written.

Examples:

- `22" x 18" Kick Drum`
- `20" x 16" Kick Drum`
- `14" x 6.5" Snare Drum`
- `12" x 8" Rack Tom`
- `16" x 16" Floor Tom`

If only diameter is given, do not invent depth.

Example:

`14" Snare`

→ `01 x 14" Snare Drum`

not:

`01 x 14" x 6.5" Snare Drum`

## Kick Drum

Capture:

- size
- ported / unported resonant head requirement
- internal mic hole, only if stated
- dampening, only if stated
- pedal requirement only when the rider includes it in the shell notes

Keep pedal requirements in `hardware.md` when they are listed as hardware or breakables.

## Snare Drums

Distinguish between:

- main snare
- side snare
- piccolo snare
- artist-supplied snare
- locally supplied snare

Do not assume the snare is part of a shell pack if the rider lists it separately.

If the rider says `breakables supplied by artist`, treat snare responsibility according to the rider wording and flag ambiguity if the snare is also listed in local backline.

## Toms

Preserve each tom separately when listed separately.

Examples:

- `01 x 10" Rack Tom`
- `01 x 12" Rack Tom`
- `01 x 16" Floor Tom`

If the rider says `3 toms` without sizes, preserve that as an incomplete requirement and flag the missing sizes.

## Drum Heads

Capture drum-head requirements only when stated.

Examples:

- `Remo Coated Ambassador on snare`
- `Clear Emperor tom heads`
- `Powerstroke 3 kick batter`
- `New heads required`

Do not infer head type from genre, artist, shell brand, or common practice.

## Manufacturer and Model

Preserve manufacturer and series when specified.

Examples:

- `Yamaha Absolute`
- `DW Collector's Series`
- `Gretsch USA Custom`
- `Ludwig Black Beauty`

Do not substitute equivalent brands unless explicitly asked to evaluate alternatives.

## Required / Preferred / Acceptable

Preserve the rider's semantics:

- `must`, `required`, `no substitutions` → required
- `preferred`, `ideally`, `first choice` → preferred
- `acceptable`, `or equivalent`, `alternatives` → acceptable
- `if available`, `optional` → optional

Never convert a preference into a requirement.

## Output Format

Use one line per shell:

`QTY x SIZE DRUM TYPE MANUFACTURER MODEL NOTES — STATUS — SUPPLY`

Omit fields that are not specified.

Examples:

- `01 x 22" x 18" Kick Drum Yamaha Absolute — Required — Local Production`
- `01 x 14" x 6.5" Snare Drum Ludwig Black Beauty — Required — Artist Supplied`
- `01 x 12" Rack Tom — Required — Local Production`
- `01 x 16" Floor Tom — Preferred — Venue Supplied`

## Stage Plot

Use stage plots as supporting evidence for:

- number of drum stations
- position of the drum kit
- possible tom or cymbal count
- riser placement

Do not treat every drawn drum object as a confirmed local rental requirement unless the rider text also supports it.

## Conflicts

Flag conflicts between:

- drum setup section
- backline list
- input list
- stage plot
- general notes / breakables notes

Examples:

- Rider says `4-piece drum kit`, but input list includes `Rack Tom 1`, `Rack Tom 2`, and `Floor Tom`.
- Rider says artist brings snare, but backline asks local production for a snare.
- Stage plot shows two drum kits, but backline lists only one.

Do not resolve conflicting quantities, models, sizes, or supply responsibility by assumption.
