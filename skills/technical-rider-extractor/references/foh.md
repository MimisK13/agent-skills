# FOH

Use this reference when extracting FOH audio requirements from a technical rider.

The primary goal is to determine what FOH equipment must be supplied locally, what the artist carries, and which mixing-console or signal-distribution requirements must be satisfied.

## Extract

Identify requirements for:

- FOH Mixing Console
- FOH Engineer
- Stagebox
- Digital Snake
- Signal Split
- Outboard Processing
- Plugins / Waves systems
- Playback or control computers
- Network requirements
- FOH position requirements
- Power requirements

For each item, preserve when available:

- quantity
- manufacturer
- model
- minimum technical requirement
- notes
- supply responsibility

## Supply Responsibility

Determine who must provide each FOH item.

Normalize to:

- `Artist Supplied`
- `Local Production`
- `Venue Supplied`
- `Unspecified`

Examples:

`Artist carries FOH console`

→ `Artist Supplied`

`Please provide Midas M32`

→ `Local Production`

`House console may be used`

→ `Venue Supplied`

Do not assume a console must be rented simply because it is named in the rider.

## Mixing Console

Capture:

- manufacturer
- model
- preferred console
- acceptable alternatives
- minimum input count
- minimum output / bus count
- required local I/O
- sample-rate requirements
- redundant power requirements when stated

Examples:

- `01 x Midas M32`
- `01 x Allen & Heath dLive`
- `DiGiCo SD12 preferred`

Do not infer console suitability unless explicitly asked to evaluate it.

## Stagebox and Digital Snake

Capture requirements for:

- stagebox
- remote I/O
- digital snake
- connection protocol
- cable requirements
- redundant connections
- ownership of preamp gain

Examples may include:

- DL32
- Rio
- GX4816
- DiGiCo SD-Rack

Preserve the exact requested relationship between console and stagebox.

## Signal Split

Capture when specified:

- analog split
- digital split
- transformer-isolated split
- passive split
- active split
- FOH / Monitor split
- broadcast / recording split
- gain ownership

Do not assume FOH and Monitor consoles can share preamp gain.

## FOH Engineer

Capture whether the rider requires:

- artist FOH engineer
- local FOH engineer
- house engineer
- system technician

Preserve who supplies the engineer.

Do not infer staffing requirements from the console specification.

## Outboard and Processing

Capture explicitly requested:

- compressors
- gates
- EQ
- effects processors
- system processors
- plugin hosts
- Waves systems
- recording interfaces

Do not infer standard outboard requirements.

## FOH Position

Capture explicit FOH-position requirements such as:

- audience-centre position
- distance from stage
- unobstructed line of sight
- no booth / enclosure
- riser requirements
- table size
- rain cover
- lighting
- power

Do not infer placement from normal venue practice.

## Network and Control

Capture when explicitly required:

- Ethernet
- managed network
- Wi-Fi
- control computer
- remote control device
- redundant network
- dedicated router

Do not infer networking needs from the console model alone.

## Preferences and Alternatives

Preserve distinctions between:

- required
- preferred
- acceptable
- alternative
- optional

Example:

`DiGiCo SD12 preferred, SD10 or Quantum 338 acceptable`

must preserve:

- Preferred: DiGiCo SD12
- Acceptable: DiGiCo SD10, Quantum 338

Do not treat them as equivalent.

## Conflicts

Flag conflicts between:

- FOH section
- equipment list
- input list
- monitor section
- stage plot
- production notes

Do not resolve conflicting console, I/O, split, or supply requirements by assumption.