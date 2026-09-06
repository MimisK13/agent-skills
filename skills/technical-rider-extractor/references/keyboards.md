# Keyboards

Use this reference when extracting keyboard backline requirements from a technical rider.

The primary goal is to determine which keyboard-related equipment is:

- Artist Supplied
- Local Production
- Venue Supplied
- Unspecified

## Extract

Identify requirements for:

- Keyboard
- Stage Piano
- Synthesizer
- Organ
- Keyboard Stand
- Keyboard Bench / Stool
- Sustain Pedal
- Expression Pedal
- DI Box
- Keyboard Amplifier, when explicitly required

For each item, preserve when available:

- quantity
- manufacturer
- model
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

`Artist travels with Nord Stage`

→ `Artist Supplied`

`Please provide Yamaha CP88`

→ `Local Production`

Do not assume a keyboard must be rented simply because it appears in the backline section.

## Keyboards

Extract instruments only when explicitly mentioned.

Examples:

- `01 x Nord Stage 4`
- `01 x Yamaha CP88`
- `01 x Korg Kronos`
- `01 x Hammond XK-5`

Preserve manufacturer, model and type exactly when specified.

Do not infer:

- key count
- weighted action
- sound engine
- MIDI capability
- internal speakers

unless explicitly stated.

## Keyboard Stands

Capture stand requirements separately.

Examples:

- `01 x Single Keyboard Stand`
- `01 x Double Keyboard Stand`
- `01 x X-Style Keyboard Stand`

Preserve tier count when specified.

Do not infer stand type from the number of keyboards.

## Pedals

Capture separately when required:

- Sustain Pedal
- Expression Pedal
- Volume Pedal
- Foot Controller

Preserve manufacturer and model when specified.

## DI

Capture DI boxes when explicitly included in the keyboard backline requirement.

Preserve:

- quantity
- mono / stereo requirement
- manufacturer
- model
- whether supplied locally

Do not assume that every keyboard requires a DI unless stated or clearly required by the rider.

## Preferences and Alternatives

Preserve preferred and acceptable alternatives.

Example:

`Nord Stage 4 preferred, Nord Stage 3 acceptable`

must preserve:

- Preferred: Nord Stage 4
- Acceptable: Nord Stage 3

Do not treat them as equivalent.

## Output

Use:

`QTY x ITEM NOTES — SUPPLY`

Examples:

- `01 x Nord Stage 4 — Local Production`
- `01 x Double Keyboard Stand — Local Production`
- `01 x Sustain Pedal — Local Production`
- `01 x Yamaha CP88 — Artist Supplied`

## Conflicts

Flag conflicts between:

- backline section
- equipment list
- input list
- stage plot

Do not resolve conflicting models, quantities or supply responsibility by assumption.