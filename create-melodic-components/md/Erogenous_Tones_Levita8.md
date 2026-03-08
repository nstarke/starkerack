# Erogenous Tones — Levita8

- [Manual PDF](../../manuals/l8-instructions.pdf)

---

[Manual PDF](http://erogenous-tones.com)

# Erogenous Tones LEVIT8 — melodic use cases

The LEVIT8 is an **8-channel attenuator / gain / inverter / mixer utility**. It is not a sound source or quantizer by itself, but in a melodic Eurorack patch it is extremely useful as a **CV sculpting and pitch-combining tool**.

## What it does musically

From the manual:

- 8 channels of **linear attenuation/gain**
- max gain about **2x**
- some channels have **invert switches**
- works with **audio, CV, gates**
- if nothing is patched to an input, that input is normalized to **+5V**
- outputs can act as:
  - **8 independent processors**
  - **one or two 4-to-1 mixers**
  - **one 8-to-1 mixer**
- channels saturate around **±10V**

That means LEVIT8 is great for building melodic control voltages from simpler sources.

---

## Best melodic roles for LEVIT8

## 1. Pitch CV attenuator for sequence control

A common melodic use is scaling pitch-related CV before it reaches an oscillator.

### Patch idea
- Sequencer pitch CV -> LEVIT8 input
- LEVIT8 output -> quantizer or oscillator 1V/oct input

### Why
- Reduce melodic range for tighter basslines
- Boost weak CV sources
- Invert contours for contrary motion melodies

Because gain goes up to about 2x, you can make a small modulation source cover a larger pitch range.

---

## 2. Manual transpose source using normalized +5V

Since unpatched inputs are normalized to **5V**, each unused channel can become a **manual DC voltage generator**.

### Patch idea
- Leave a channel input empty
- Turn its knob to create a chosen voltage
- Send output to:
  - oscillator pitch input
  - quantizer transpose input
  - sequencer transpose input

### Why
This gives you a quick manual transpose control.  
On invert-capable channels, you can generate **negative offsets** too.

This is one of the most useful melodic tricks in the module:
- create base pitch offsets
- shift a sequence up/down by intervals
- bias random CV before quantization

---

## 3. Mix several CV sources into one melody

LEVIT8 can sum multiple channels at output 4 or output 8 depending on the MIX switch settings.

### Patch idea
Use the 4-channel mix:
- Ch 1: sequencer pitch
- Ch 2: slow LFO
- Ch 3: DC offset from empty normalized jack
- Ch 4: random stepped voltage
- MIX on channel 4 up
- Output 4 -> quantizer -> oscillator

### Result
You get a composite melodic CV made from:
- structured notes
- vibrato or contour
- transposition
- random variation

This is one of the strongest melodic uses for LEVIT8: **CV summing before quantization**.

---

## 4. Create quantizer-friendly melodies from modulation sources

LEVIT8 is very good before a quantizer.

### Patch idea
- Patch several modulation sources into channels:
  - triangle LFO
  - envelope
  - random stepped CV
  - DC offset
- Mix them at output 4 or 8
- Send mixer output to a quantizer
- Quantizer output -> oscillator pitch

### Why
A quantizer turns mixed analog voltages into notes, and LEVIT8 lets you shape:
- melodic density
- interval size
- direction
- register

This is an excellent way to make evolving melodies from non-sequencer CV.

---

## 5. Invert melodic motion

The invert switches let some channels flip voltage polarity.

### Patch idea
- Sequencer CV multed to two LEVIT8 channels
- One normal, one inverted
- Send the two outputs to different oscillators, or mix selectively

### Musical use
- oscillator 1 rises while oscillator 2 falls
- create contrary-motion counterpoint
- invert modulation before quantizing for a mirrored melody

If your downstream module expects pitch CV, inversion can create musically related but opposite contours.

---

## 6. Make interval layers and harmonized pitch CV

Because channels can independently scale copies of the same source, LEVIT8 can build related pitch lines.

### Patch idea
- Mult one pitch sequence into several LEVIT8 channels
- Set each channel to a different amount/offset
- Send:
  - one output to oscillator A
  - another to oscillator B
  - another through a quantizer for a third line

### Why
This allows:
- reduced or expanded intervals
- offset versions of the same melody
- parallel melodic voices

For strict harmony, send the processed CVs through quantizers or use quantizer transpose inputs.

---

## 7. Use it as a precision-ish performance macro for melody

While it is not marketed as a precision adder, LEVIT8 can still be used performatively to shape melodic behavior.

### Patch idea
- Ch 1: main sequence
- Ch 2: manual DC offset
- Ch 3: envelope amount to pitch
- Ch 4: random stepped CV
- Output 4 -> quantizer

Now the knobs become performance controls for:
- transposition
- sequence range
- ornament amount
- instability/randomness

This can turn a static melody into an expressive one.

---

## 8. Build an 8-source melodic CV bus

If channel 8 mix is engaged while channel 4 mix is off, output 8 becomes a mix of **all 8 channels**.

### Patch idea
Send up to 8 sources:
- sequencer row A
- sequencer row B
- offset voltage
- LFO
- random source
- envelope
- gate-derived accent CV
- keyboard CV

Then:
- Output 8 -> quantizer -> oscillator

### Why
This creates a powerful “meta-melody” bus.  
You can blend many influences into one final note stream.

This is especially effective in generative patches.

---

## 9. Shift melodies with DC offset for register control

Because unused inputs default to +5V, LEVIT8 is very handy for moving a melody into a different octave/register.

### Patch idea
- Ch 1: melody CV
- Ch 2: empty input, knob set as offset
- Mix to output 4
- Output 4 -> quantizer or oscillator

### Result
You can move the melody:
- slightly upward/downward
- into a higher register
- into saturation for more extreme effects

This is useful for live performance transitions.

---

## 10. Process gates or accents into melodic influence

The manual says it works with **gates** too.

### Patch idea
- Gate or trigger pattern -> LEVIT8 channel
- Attenuate heavily
- Mix with pitch CV
- Send to quantizer

### Result
Gates become stepped voltage contributions that alter pitch only when active, creating:
- accents that also transpose
- conditional note jumps
- rhythmic melody shifts

This is a smart way to tie rhythm and melody together.

---

# Practical melodic patch examples

## Patch 1: Simple transposable sequence
- Sequencer pitch out -> Ch 1
- Empty Ch 2 as DC offset
- Channel 4 MIX up
- Out 4 -> quantizer -> VCO 1V/oct

Use:
- Ch 1 knob for sequence range
- Ch 2 knob for transpose

---

## Patch 2: Generative melody builder
- Stepped random CV -> Ch 1
- Slow LFO -> Ch 2
- Envelope -> Ch 3
- Empty Ch 4 for offset
- Channel 4 MIX up
- Out 4 -> quantizer -> oscillator

Use the knobs to balance:
- randomness
- contour
- note density
- register

---

## Patch 3: Two related melodic voices
- Main sequence multed to Ch 1 and Ch 5
- Random stepped CV -> Ch 2
- Empty Ch 3 for transpose
- Slow LFO -> Ch 6
- MIX Ch 4 up for voice A
- MIX Ch 8 up with Ch 4 also engaged for voice B
- Out 4 -> quantizer A -> oscillator A
- Out 8 -> quantizer B -> oscillator B

This gives two separate melodic streams derived from related material.

---

## Patch 4: Contrary-motion duet
- Sequencer pitch multed to one normal channel and one invert-capable channel
- Add separate offsets to each path using empty normalized channels
- Send each output to separate quantizers/oscillators

Result:
- one melody ascends
- the other mirrors or counters it

---

# Strengths for melodic patching

LEVIT8 is especially good at:

- **combining multiple CV sources**
- **manual transposition**
- **offsetting and biasing CV**
- **inverting melodic contours**
- **building pre-quantizer composite voltages**
- **making one sequence produce several related voices**

---

# Important caveats

## 1. Not a quantizer
For tonal melody, LEVIT8 works best with a **quantizer** after it.

Without quantization, summed voltages may not land on exact musical intervals.

## 2. Not guaranteed as a precision adder
The manual presents it as a gain/invert/mix utility, not a precision pitch utility.  
So for exact octave transposition at 1V/oct, use care and test by ear/tuner.

## 3. Beware normalized DC in mixes
If a channel is unpatched, it adds DC from the normalized +5V source.  
That is useful for transpose, but if you forget to turn the knob down, it will affect the melody unexpectedly.

---

# Bottom line

The LEVIT8 is a **melodic CV utility powerhouse**. It shines when used to:

- scale sequencer voltages
- mix random and deterministic CV
- add manual transpose
- invert pitch movement
- create layered or generative note streams before a quantizer

By itself it does not create notes, but together with a **sequencer, random source, quantizer, and oscillator**, it becomes a central tool for designing expressive melodic control voltages.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)