# Bass

Use this reference when extracting bass backline requirements from a technical rider.

The primary goal is to determine which bass equipment is:

- artist supplied
- locally supplied / rented
- optional
- unspecified

## Extract

Identify requirements for:

- Bass Guitar
- Bass Amplifier Head
- Bass Cabinet
- Bass Combo Amplifier

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

`Artist travels with bass guitar`

→ `Artist Supplied`

`Please provide Fender Precision Bass`

→ `Local Production`

`Bass amp provided by venue`

→ `Venue Supplied`

Do not assume that an item must be rented simply because it appears in the backline section.

Do not assume that the artist carries an item unless explicitly stated.

## Bass Guitar

Extract bass instruments only when explicitly mentioned.

Examples:

- `01 x Fender Precision Bass`
- `01 x Fender Jazz Bass`
- `01 x 5-String Bass`

Preserve relevant requirements such as:

- manufacturer
- model
- number of strings
- tuning
- left-handed / right-handed

Do not infer unspecified characteristics.

## Bass Amplification

Distinguish between:

- Amplifier Head
- Bass Cabinet
- Combo Amplifier

Examples:

- `01 x Ampeg SVT-CL`
- `01 x 8x10" Bass Cabinet Ampeg`
- `01 x Fender Rumble 500 Combo`

Preserve requested manufacturer, model, cabinet configuration, and quantity.

## Alternatives

Preserve preferred and acceptable alternatives.

Example:

`Ampeg SVT-CL preferred, SVT-VR acceptable`

must remain:

- Preferred: Ampeg SVT-CL
- Acceptable: Ampeg SVT-VR

Do not treat them as equivalent.

## Output

List only bass backline items relevant to supply or rental decisions.

Use:

`QTY x ITEM NOTES — SUPPLY`

Examples:

- `01 x Fender Precision Bass — Local Production`
- `01 x Ampeg SVT-CL — Local Production`
- `01 x 8x10" Bass Cabinet Ampeg — Local Production`
- `01 x Music Man StingRay — Artist Supplied`

## Conflicts

If different sections of the rider disagree about who supplies an item, flag the conflict.

Do not decide the responsibility by assumption.