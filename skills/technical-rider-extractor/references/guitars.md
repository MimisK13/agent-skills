# Guitars

Use this reference when extracting guitar backline requirements from a technical rider.

The primary goal is to determine which guitar equipment is:

- artist supplied
- locally supplied / rented
- venue supplied
- optional
- unspecified

## Extract

Identify requirements for:

- Electric Guitar
- Acoustic Guitar
- Guitar Amplifier Head
- Guitar Cabinet
- Guitar Combo Amplifier

For each item, preserve when available:

- quantity
- manufacturer
- model
- type / configuration
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

`Artist travels with guitars`

→ `Artist Supplied`

`Please provide Gibson Les Paul`

→ `Local Production`

`Guitar amps provided by venue`

→ `Venue Supplied`

Do not assume that an item must be rented simply because it appears in the backline section.

Do not assume that the artist carries an item unless explicitly stated.

## Guitars

Extract instruments only when explicitly mentioned.

Examples:

- `01 x Gibson Les Paul`
- `01 x Gibson SG`
- `01 x Fender Stratocaster`
- `01 x Acoustic Guitar`

Preserve relevant requirements such as:

- manufacturer
- model
- guitar type
- tuning
- left-handed / right-handed
- number of strings

Do not infer unspecified characteristics.

## Guitar Amplification

Distinguish between:

- Amplifier Head
- Guitar Cabinet
- Combo Amplifier

Examples:

- `01 x Marshall JCM800`
- `01 x Peavey 6505`
- `01 x 4x12" Guitar Cabinet Marshall`
- `01 x Roland JC-120 Combo`

Preserve requested manufacturer, model, cabinet configuration, and quantity.

Do not replace a requested head + cabinet setup with a combo, or vice versa, unless explicitly listed as an acceptable alternative.

## Full Stack / Half Stack

Preserve stack terminology when explicitly stated.

Interpret only when the rider makes the configuration clear.

Typical configurations:

- Half Stack → amplifier head + one cabinet
- Full Stack → amplifier head + two cabinets

Do not infer cabinet size or model unless specified.

## Alternatives

Preserve preferred and acceptable alternatives.

Example:

`Marshall JCM800 preferred, Peavey 6505 acceptable`

must remain:

- Preferred: Marshall JCM800
- Acceptable: Peavey 6505

Do not treat them as equivalent.

## Artist-Supplied vs Local Production

Preserve who is responsible for providing each item.

Distinguish between:

- artist supplied
- local production supplied
- venue supplied
- unspecified

Do not assume responsibility based on common touring practice.

## Stage Plot

Use the stage plot as supporting information for:

- amplifier position
- cabinet quantity
- performer position

Do not automatically treat equipment shown only on the stage plot as a confirmed rental requirement.

## Conflicts

Flag conflicts between:

- backline section
- equipment list
- stage plot

Do not resolve conflicting quantities, models, or supply responsibility by assumption.