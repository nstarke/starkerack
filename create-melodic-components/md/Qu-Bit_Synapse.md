# Qu-Bit — Synapse

- [Manual PDF](../../manuals/Synapse.pdf)

---

[Manual PDF](attachment)

# Qu-Bit Synapse: using it to create melodic components

Synapse is not a pitch quantizer or traditional sequencer, but it **can absolutely be used to build melodic material** because it combines:

- 4 crossfaders
- routable/sequential switching
- 8 memory states
- internal +5V offsets
- internal LFOs
- CV/audio compatibility throughout

That means it can act as a:

- stepped CV composer
- phrase selector
- melodic router
- stored-voltage pattern source
- animated modulation source for pitch-related destinations

## What Synapse does that matters for melody

From the manual, the most melody-relevant features are:

- **DC-coupled inputs**: works with CV as well as audio
- **Per-channel A/B crossfading**: blend between two voltages per channel
- **+5V DC offset normalled to each B input**: lets each channel generate CV without external sources
- **8 memory locations**: store crossfade positions and recall them with one knob
- **Sequential/routable outputs via Terminal and Advance**
- **Inertia**: slews transitions between stored states
- **Internal LFOs**: can animate pitch/modulation patterns
- **Sum outputs**: combine channels into more complex control voltages

## Important melodic concept

Synapse excels when you think of it as a **voltage-scene morphing router**.

Each of the 4 channels can hold a voltage or blend between two voltages.  
Then the module can:

- save those blends into memory slots
- advance/swizzle routing
- sum channels
- slew transitions

So instead of a classic “one note per step” sequencer, it’s more like:

- **one harmonic/melodic state per memory**
- **one destination/output arrangement per switch state**
- **one evolving phrase through interpolation, switching, and summed CV**

## Melodic patch strategies

## 1. Use Synapse as a 4-stage stored voltage sequencer

This is the most direct melodic use.

### How
- Enable the **+5V DC offset** on B inputs.
- Leave A inputs unpatched, or feed them with 0V / another reference voltage.
- Use each channel’s crossfade knob to choose a voltage between A and B.
- Send a channel output to an oscillator’s **1V/oct** input, ideally through a quantizer if you want strict tuning.
- Use **Advance** to step routing through outputs.

### Why it works
With DC offset enabled, each crossfade becomes a voltage chooser.  
The manual explicitly notes this can make Synapse function like:

- a **four step sequencer**
- an **eight stage stored voltage source**

### Musical result
You can create:

- bassline steps
- lead note contours
- transposition voltages
- motif fragments

### Best companion modules
- quantizer
- sample & hold / clock source
- envelope + VCA
- oscillator with stable tracking

### Tip
Because the B input is +5V when enabled, the crossfade knob becomes a performance control for stored CV amount. Save multiple memories and you get phrase recall.

---

## 2. Build 8 melodic “phrases” with Memory

Memory is where Synapse becomes especially useful for composition.

### How
- Create four voltage settings across the four crossfade channels.
- Save them to one memory slot.
- Change the four fader positions to a new shape.
- Save again.
- Repeat for up to **8 memories**.

Then sweep or CV the **Memory** control to recall different stored voltage arrangements.

### Why it’s musical
Each memory slot can represent:

- a chord tone set
- a bass phrase
- a transposition profile
- a melodic contour
- a verse/chorus variation

### Important manual behavior
- When a memory location is selected, **crossfade CV inputs are disabled**
- Changes aren’t stored until **Save** is pressed
- Fully CCW on Memory = **memory bypass**

### Melodic uses
- 8 different note clusters
- 8 phrase presets
- 8 harmonic regions for transposition
- song section changes without repatching

### Strong patch idea
Use:
- **Out 1** -> quantizer -> VCO pitch
- **Out 2** -> second quantizer/VCO pitch
- **Out 3** -> filter cutoff
- **Out 4** -> FM amount or wavefold amount

Now each memory slot becomes a full melodic “scene.”

---

## 3. Use it as a melody generator before a quantizer

Synapse is especially powerful **upstream of a quantizer**.

### How
Patch Synapse output into:
- quantizer input
- then quantizer output to oscillator 1V/oct

### Why
Synapse can generate rich, unstable, blended, slewed, shuffled voltages. A quantizer then converts those into usable musical notes.

### What this gives you
- playable melodic randomness
- phrase morphing
- evolving sequences
- repeated motifs with variation

### Great sources for A/B inputs
Feed the A and B inputs with:
- slow LFOs
- envelopes
- offsets
- random stepped voltages
- another sequencer’s rows
- pressure/controller CV

Then use Synapse to blend and reroute before quantization.

### Result
Instead of programming exact notes, you shape a **melodic probability field** that the quantizer turns into scales/arpeggios.

---

## 4. Crossfade between two pitch sequences

A very strong use case.

### How
For each channel:
- patch one sequencer row or CV source into **A**
- patch another sequence into **B**
- send the resulting output to a quantizer or oscillator pitch input

### What happens
The crossfade knob and CV let you interpolate between two melodic lines.

### Musical outcomes
- phrase mutation
- call/response between two melodies
- morphing bassline
- gradual harmonic transition

### With Memory
Store multiple crossfade positions:
- Memory 1 = mostly A
- Memory 2 = balanced
- Memory 3 = mostly B
- etc.

Now you have recallable interpolation states between two sequences.

### With Inertia
Add glide between memory changes for:
- portamento
- phrase smearing
- expressive transitions

---

## 5. Use 4 channels as harmonic interval generators

Synapse can generate related CVs on multiple outputs.

### How
Set each channel to a different fixed CV amount using the +5V offset or external voltage references.

For example:
- Ch1 = root
- Ch2 = third-ish voltage
- Ch3 = fifth-ish voltage
- Ch4 = octave or seventh

Then send those outputs to:
- multiple quantizers/oscillators
- precision adders
- switch matrix destinations

### Result
You can create:
- chord voicings
- parallel melodic intervals
- stacked canon lines
- drone harmony structures

### Better with quantizers
Because raw CV won’t necessarily correspond to exact intervals, quantizers make this much more musical and repeatable.

---

## 6. Sequentially route one melodic line to different voices

The **Terminal** switching section makes Synapse useful as a melodic distributor.

### How
Patch a pitch CV source or melodic blend through Synapse, then use the outputs to address:
- multiple oscillators
- different quantizers/scales
- separate voice chains

Use:
- **Terminal encoder** for manual routing shifts
- **Advance** input for clocked movement
- **Scatter** for shuffled routing

### Melodic use
One sequence can be sent to different destinations over time, creating:
- rotating counterpoint
- pseudo-rounds/canons
- changing voice assignments
- phrase movement across timbres

### Example
- Out 1 -> quantizer in C minor -> VCO 1
- Out 2 -> quantizer in pentatonic -> VCO 2
- Out 3 -> filter ping pitch CV
- Out 4 -> FM oscillator pitch

Advance the switch with a clock and one source becomes a changing melodic orchestrator.

---

## 7. Use Scatter for melodic permutation

The **Scatter** function shuffles output positions.

### Why this is good for melody
It creates permutations of where voltages go.

If each output drives a different pitch destination or quantizer, a shuffle creates:
- rearranged melodic order
- changed voicings
- altered call/response behavior
- spatialized note movement

### Best patch
Set up 4 distinct voltage channels, each feeding different harmonic functions, then trigger Scatter rhythmically but not every beat.

This gives phrase reshuffling without changing the underlying note material.

---

## 8. Use Sum outputs for composite melodic CV

Synapse includes:
- **1+2**
- **3+4**
- **Sum**

From the manual:
- **1+2 / 3+4** are post-switch sums
- **Sum** is pre-switch sum of each crossfade channel

### Melodic use
Summing CV sources is extremely useful for:
- transposition
- interval stacking
- phrase complexity
- combining motion layers

### Patch examples
- Channel 1 = base pitch contour
- Channel 2 = small interval modulation
- Channel 3 = octave jumps
- Channel 4 = slow transposition

Then:
- **Sum** -> quantizer -> oscillator

Now your pitch line is the combined result of multiple independent melodic influences.

### Another option
Use:
- **1+2** as bass pitch CV
- **3+4** as lead pitch CV

This can create related but distinct melodic lines from the same patch.

---

## 9. Use Inertia for melodic glide and phrase smoothing

The **Inertia** control adds slew to changes in:
- memory location
- crossfade knob moves
- crossfade CV input changes

Range is up to **5 seconds**.

### Why it matters
This turns abrupt CV changes into:
- portamento
- slide between notes
- phrase rubato feel
- smoothed transitions between melodic states

### Great use cases
- acid-style slides
- gliding between stored memory phrases
- smoothing random voltages before quantization
- generating legato motion from stepped sources

### Tip
Use moderate inertia before a quantizer for evolving melodic movement, or after quantized pitch if you want actual continuous pitch glide.

---

## 10. Internal LFOs for animated melodic modulation

The internal triangle LFOs can modulate each crossfade channel.

### Why useful for melody
If the channels are producing pitch CV or transposition voltages, the internal LFOs can create:
- vibrato-like pitch motion
- note cycling between A and B voltages
- repeating melodic oscillation
- canon-like phased movement between channels

### Key LFO features
- per-channel amplitude
- shared frequency
- multiple relationship modes:
  - Phase Offset
  - Alternating
  - Cascading
  - Synchronous

### Best melodic application
Use internal LFOs **before quantization**.  
That way the LFOs don’t just create vibrato—they create **motion through discrete notes** once quantized.

### Especially useful modes
- **Phase Offset**: creates rotating melodic movement between channels
- **Alternating**: useful for call/response two-voice phrases
- **Cascading**: excellent for sequential melodic activation
- **Synchronous**: stacked harmonic pulsing

---

## Practical melodic patch examples

## Patch 1: 8-state bass sequencer

### Goal
A recallable bassline source.

### Patch
- Enable **+5V DC offset**
- Set four channels to four different CV levels
- Patch **Sum** -> quantizer -> VCO 1V/oct
- Clock envelopes/VCA separately
- Save 8 different memory states

### Result
Each memory becomes a different bass pattern contour.  
Use the Memory knob manually or with CV to move between bass phrases.

---

## Patch 2: Morphing lead between two melodies

### Goal
Blend two sequencers into one evolving lead.

### Patch
- Sequencer A CV -> channel A inputs
- Sequencer B CV -> channel B inputs
- Crossfade outputs -> quantizer -> VCO
- Use crossfade CV inputs or internal LFOs
- Add **Inertia** for glide

### Result
A lead line that continuously mutates between two source melodies.

---

## Patch 3: Four-note chord engine

### Goal
Create harmonic material from fixed voltages.

### Patch
- Enable +5V offset
- Set channels to four different voltage levels
- Out 1-4 -> four quantizer channels / four oscillators
- Save multiple memory states as different voicings
- Use Advance or Terminal to rotate assignments

### Result
Stored chord voicings and melodic inversions with dynamic voice reassignment.

---

## Patch 4: Quantized melody from animated voltages

### Goal
Generate self-moving melodic content.

### Patch
- Enable +5V offset or patch offsets/random CV into A/B inputs
- Set LFO amplitudes per channel
- Choose **Cascading** or **Phase Offset** LFO relationship
- Patch **Sum** -> quantizer -> oscillator

### Result
An automatically evolving melodic line with recurring structure.

---

## Patch 5: Counterpoint by switched destination routing

### Goal
One CV source creates multiple interrelated melodic voices.

### Patch
- Build 4 distinct CV blends on Synapse
- Route outputs to:
  - Out 1 -> quantizer 1 -> VCO 1
  - Out 2 -> quantizer 2 -> VCO 2
  - Out 3 -> precision adder transpose input
  - Out 4 -> FM voice pitch
- Use **Advance** with clock divisions
- Occasionally trigger **Scatter**

### Result
Rotating contrapuntal lines and shifting harmonic functions.

---

## Patch 6: Memory as song-section transposer

### Goal
Use Synapse to transpose a melodic sequence differently per section.

### Patch
- Main sequencer -> precision adder input A
- Synapse output -> precision adder transpose input
- Build memory states containing different DC voltages
- Save 8 transposition values or 8 four-channel transposition sets

### Result
Verse, chorus, bridge transpositions are instantly recallable.

---

## Things to watch out for

## 1. Raw pitch CV may need quantization
Synapse outputs continuous CV. For tonal melodic work, a **quantizer** is highly recommended.

## 2. Memory disables channel CV inputs
When a memory slot is selected, the crossfade CV inputs are disabled.  
So if your melody depends on external modulation per channel, memory mode changes that behavior.

## 3. LFO frequency goes very high
It ranges up to **1kHz**, which is more audio-rate territory.  
For melody, you’ll usually want much slower settings unless intentionally creating complex CV behavior.

## 4. Switching and pitch
Click-less switching is great for audio, but for pitch CV changes you may still want to manage:
- clock timing
- quantizer response
- slew via Inertia

## 5. Saved state behavior
A lot of the module’s state is stored to permanent memory. That’s helpful for performance patches, but remember your last-used settings may reappear on reboot.

## Best companion modules for melodic systems

Synapse pairs especially well with:

- **Quantizers**: essential for tonal pitch generation
- **Precision adders**: for transposition workflows
- **Sequential clocks/gates**: to drive Advance and event timing
- **Envelope/VCA chains**: to articulate notes
- **Oscillators with good 1V/oct tracking**
- **Clock dividers/probability modules**: for phrase variation
- **Buffered mults/mixers**: to distribute melodic CV
- **Sample and hold/random sources**: for semi-composed melodies

## Best musical roles for Synapse

If you’re building melodic music, Synapse is strongest as:

1. **a stored voltage phrase generator**
2. **a sequencer morphing tool**
3. **a transposition and interval source**
4. **a multi-voice pitch router**
5. **an evolving CV composer before a quantizer**

It is less ideal as:
- a precise note-entry sequencer
- a standalone quantized melody source
- a traditional keyboard replacement

## Bottom line

Synapse is best understood as a **melodic infrastructure module** rather than a dedicated sequencer.

It helps create melody by letting you:

- generate CV from offsets
- blend between two melodic voltages
- store phrase states
- slew between them
- sum them into more complex pitch contours
- route them across multiple voices
- animate them with internal LFOs
- permute destination assignments

In a Eurorack melodic system, the most powerful setup is usually:

**Synapse -> quantizer / precision adder -> oscillator(s)**

That turns its fluid, morphing voltage behavior into playable, structured musical notes.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)