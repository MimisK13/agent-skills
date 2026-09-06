# Percussion

Use this reference when extracting percussion backline requirements from a technical rider.

The primary goal is to determine which percussion equipment is:

- Artist Supplied
- Local Production
- Venue Supplied
- Unspecified

## Extract

Identify percussion instruments and related hardware explicitly requested in the rider.

Common examples include:

- Congas
- Bongos
- Timbales
- Cajón
- Djembe
- Cowbell
- Tambourine
- Shaker
- Chimes
- Wood Block
- Claves
- Triangle
- Percussion Table
- Percussion Stand

For each item, preserve when available:

- quantity
- size
- manufacturer
- model / series
- type
- notes
- supply responsibility

## Supply Responsibility

Determine who must provide each item.

Normalize to:

- `Artist Supplied`
- `Local Production`
- `Venue Supplied`
- `Unspecified`

Examples:

`Artist carries own percussion`

→ `Artist Supplied`

`Please provide LP congas`

→ `Local Production`

Do not assume percussion is locally supplied simply because it appears in the rider.

## Instruments

Preserve each percussion instrument separately.

Examples:

- `02 x Conga LP`
- `01 x Cajón`
- `01 x Tambourine`
- `02 x Shaker`

Do not combine multiple different percussion items into a generic `Percussion Set` unless the rider itself uses that description.

## Sizes

Preserve sizes when explicitly stated.

Examples:

- `01 x 11" Conga`
- `01 x 12" Conga`
- `01 x 14" Timbale`

Do not infer conventional sizes.

## Hardware

Capture percussion-specific hardware separately when required.

Examples:

- Conga Stand
- Bongo Stand
- Timbale Stand
- Percussion Table
- Accessory Clamp
- Mounting Arm

Preserve quantities and any compatibility requirements.

## Preferences and Alternatives

Preserve preferred and acceptable alternatives.

Example:

`LP preferred, Meinl acceptable`

must preserve:

- Preferred: LP
- Acceptable: Meinl

Do not treat them as equivalent.

## Output

Use:

`QTY x SIZE ITEM NOTES — SUPPLY`

Omit `SIZE` when it is not specified.

Examples:

- `01 x 11" Conga LP — Local Production`
- `01 x Cajón — Local Production`
- `02 x Shaker — Artist Supplied`
- `01 x Percussion Table — Local Production`

## Stage Plot

Use the stage plot as supporting information for:

- percussion position
- number of percussion stations
- instrument placement
- hardware placement

Do not automatically treat every illustrated percussion item as a confirmed rental requirement.

## Conflicts

Flag conflicts between:

- backline section
- equipment list
- input list
- stage plot

Do not resolve conflicting quantities, models, sizes or supply responsibility by assumption.