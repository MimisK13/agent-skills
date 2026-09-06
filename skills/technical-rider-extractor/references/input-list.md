# Input List

Use this reference when extracting input-list requirements from a technical rider.

The primary goal is to identify each required audio input and preserve the requested source, microphone, DI, stand, and channel-specific notes.

## Extract

For each input, capture when available:

- channel number
- source
- microphone
- DI
- stand / mounting
- phantom power
- insert / processing requirement
- notes

## Channel Order

Preserve the channel order from the rider.

Do not reorder channels by instrument type.

If channel numbers are not provided, preserve the listed order without inventing channel numbers.

## Source

Preserve the source name as closely as possible.

Common examples:

- Kick In
- Kick Out
- Snare Top
- Snare Bottom
- Hi-Hat
- Rack Tom
- Floor Tom
- Overhead L
- Overhead R
- Bass DI
- Bass Mic
- Guitar L
- Guitar R
- Keyboard L
- Keyboard R
- Vocal
- Talkback

Normalize obvious wording differences only when the meaning is unambiguous.

Do not merge separate inputs.

Example:

- `Bass DI`
- `Bass Mic`

must remain two separate inputs.

## Microphones

Capture the requested microphone manufacturer and model when specified.

Examples:

- Shure Beta 91A
- Shure SM57
- Sennheiser e604
- Sennheiser MD421
- Neumann KM184

Preserve preferred and acceptable alternatives when stated.

Do not substitute microphones based on common industry practice.

## DI Boxes

Capture DI requirements separately from microphone requirements.

Preserve when available:

- active / passive
- mono / stereo
- manufacturer
- model
- notes

Examples:

- Radial J48
- Radial JDI
- Stereo DI

Do not assume a DI is required unless explicitly stated.

## Phantom Power

Capture phantom-power requirements when explicitly stated.

Examples:

- `+48V`
- `Phantom`
- `48V Required`

Do not infer phantom power solely from the microphone or DI model.

## Stands and Mounting

Capture stand or mounting requirements when specified.

Examples:

- Short Boom
- Tall Boom
- Straight Stand
- Clamp
- Drum Mount
- No Stand

Do not infer stand type from microphone placement.

## Stereo Inputs

Preserve stereo sources as separate inputs when the rider lists separate left and right channels.

Example:

- `Keyboard L`
- `Keyboard R`

Do not collapse them into a single input.

## Output Format

Use one line per input:

`CH - SOURCE - MIC / DI - NOTES`

Examples:

- `01 - Kick In - Shure Beta 91A`
- `02 - Kick Out - Shure Beta 52A`
- `03 - Snare Top - Shure SM57`
- `04 - Snare Bottom - Shure SM57 - Phase Reverse`
- `15 - Bass DI - Radial J48`
- `16 - Bass Mic - Sennheiser MD421`
- `21 - Keyboard L - DI`
- `22 - Keyboard R - DI`

If information is missing, omit it rather than inventing it.

## Preferences and Alternatives

Preserve distinctions between:

- required
- preferred
- acceptable
- alternative
- optional

Do not treat alternative microphone or DI models as equivalent unless the rider does.

## Input Count

When possible, determine the total number of required inputs.

Do not assume the highest channel number equals the total input count if:

- numbering contains gaps
- spare channels are included
- channels are intentionally skipped

## Stage Plot

Use the stage plot as supporting information for:

- source identification
- performer position
- stereo relationships
- microphone placement

Do not create additional inputs solely because an instrument appears on the stage plot.

## Conflicts

Flag conflicts between:

- input list
- patch sheet
- stage plot
- backline specification
- monitor section

Examples:

- different microphone models
- different channel numbering
- stereo source shown as mono elsewhere
- input present in one section but missing in another

Do not resolve conflicts by assumption.