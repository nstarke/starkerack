# Hexinverter — Orbitals

- [Manual PDF](../../manuals/hexinverter-orbitals.pdf)

---

[Manual PDF](#)

# Hexinverter Orbitals — using it for melodic components

Orbitals is a **dual bipolar voltage-controlled step sequencer** that can work as:

- **2 independent 8-step sequencers**
- **1 combined 16-step sequencer**

For melody-making, that makes it especially useful as:

- a pitch sequencer
- a rhythm/gate pattern source
- a transposable melodic line generator
- a voltage-addressed note selector
- a two-lane melody/countermelody tool

## What Orbitals contributes musically

From the manual, the key melody-oriented features are:

- **Per-step CV knobs** for programming note values
- **Per-step gate switches** for deciding which notes articulate
- **Bipolar or unipolar CV output**
- **Transpose input on Sequencer A**
- **Sequence length control**
- **Multiple playback modes**:
  - Forward
  - Reverse
  - Pendulum
  - Random
  - CV addressed
  - Clocked CV addressed
- **Internal or external clocking**
- **Reset, run, reverse, and slave/sync options**
- **Selectable output ranges via rear jumpers**

This is enough to build classic melodic sequencing, but also more experimental note selection and phrase variation.

---

## Core melodic use cases

## 1. Classic pitch sequencer

The most obvious use is to send:

- **CV OUT** → oscillator **1V/oct**
- **GATE OUT** → envelope gate input

Then tune each step knob by ear to a scale or motif.

### Why it works well
- The gate switches let you create rests.
- Length control can turn an 8-step line into 3, 5, 7, etc. steps for evolving loops.
- Bipolar mode lets you center pitches around 0V if your downstream patch likes positive and negative modulation.

### Musical results
- basslines
- lead sequences
- repeating ostinati
- Berlin-school/Tangerine Dream-style patterns

The manual explicitly mentions the transpose input for keyboard-based transposition in this style.

---

## 2. 16-step melodic phrase builder

If **Sequencer A length is set over 8**, Orbitals automatically enters **16-step mode**.

In this mode, the module becomes a longer melodic sequencer for:

- full-bar phrases
- call-and-response within one row
- verse-like repeated pitch structures
- longer melodic arcs than typical 8-step loops

### Practical approach
- Program steps 1–8 as motif A
- Program steps 9–16 as motif B or a variation
- Use gate switches to create rhythmic contour
- Clock externally from your master clock for tight timing

This is great when 8 steps feel too short and repetitive.

---

## 3. Dual melody + countermelody patch

In **dual 8-step mode**, A and B can run independently.

This allows:

- **A** = bassline
- **B** = lead line

or

- **A** = melodic pitch CV
- **B** = second voice / harmony / counterline

Because each sequencer has:
- its own rate
- its own mode
- its own clock/reset/run inputs
- its own gate length
- its own sequence length

you can create **polymetric melodic relationships** very easily.

### Example
- A length = 5
- B length = 7
- same clock source
- both quantized downstream

Result: a constantly shifting melodic relationship that takes a long time to repeat.

---

## 4. Transposable melodic sequencing

One of Orbitals’ best musical features is:

- **TRANS A input**

This input adds an external voltage to Sequencer A’s CV output.

### Melodic uses
- Play a keyboard into TRANS A to transpose a sequence live
- Use another sequencer, offset generator, or precision adder source to shift the melody by intervals
- Send a slow CV to transpose the whole line over time

### Musical applications
- verse/chorus key changes
- root-note movement under a repeating melodic pattern
- live performance transposition
- classic modular “play the sequencer from a keyboard” patches

This is one of the most direct ways Orbitals creates richer melodic content instead of a static loop.

---

## 5. Voltage-addressed note selection

Orbitals has two special modes for step selection:

- **CV mode**
- **CLK mode**

In these modes, the **RST/CV input** becomes a **0–5V step address input**.

That means instead of advancing step-by-step, an incoming voltage chooses the current step.

### CV mode
- Incoming CV directly selects the step
- A new gate is generated whenever the step changes

### CLK mode
- CV selects the step
- A new gate only happens on clock events

### Why this matters melodically
This turns Orbitals into something more like:
- a note lookup table
- a manually programmable quantized melody bank
- a non-linear pitch source

### Patch ideas
- Use an LFO, random voltage, joystick, or another sequencer to address steps
- Program each step as a note from a scale
- Let incoming CV “scan” the melody map

This creates:
- non-linear melodies
- repeatable but less predictable pitch order
- generative melodic structures

CLK mode is especially useful when you want rhythmic stability but non-linear note choice.

---

## 6. Random melodic generator

In **RND mode**, every clock selects a random step.

If the step knobs are tuned to notes of a scale, this becomes a playable random melody source.

### Best practice
For more musical randomness:
- tune all active steps to a limited note set
- disable some gates for rests
- use shorter sequence lengths to constrain choices
- transpose the result with TRANS A

### Result
You get melodies that feel:
- unpredictable
- bounded
- stylistically coherent

This is very effective for ambient, generative, and IDM-style patches.

---

## 7. Pendulum and reverse for phrase variation

Orbitals includes:
- **FW**
- **REV**
- **PND**

These are simple, but extremely musical.

### Reverse
Great for:
- inversion-like phrase behavior
- turning a lead into a response phrase
- variation without repatching

### Pendulum
Great for:
- symmetrical melodies
- arpeggio-like up/down movement
- longer-feeling loops from fewer steps

A short 4-step programmed phrase in pendulum mode can sound much more animated than plain forward playback.

---

## 8. Sequence length as a melodic tool

The **LENGTH** knobs do more than shorten loops — they reshape melody.

### Useful musical tricks
- Set a sequence to 3, 5, or 7 steps for looping against 4/4 rhythm
- Use A at 8 and B at 5 for evolving harmony
- Make a short motif repeat unevenly before resolving

This is one of the easiest ways to get melodies that feel alive without needing additional modules.

---

## 9. Gate pattern as melodic phrasing

Because each step has a **gate switch**, Orbitals separates:

- pitch progression
- note articulation

This is very important musically.

Even if pitch steps continue internally, only selected steps create notes.

### Melodic phrasing possibilities
- create rests
- create syncopation
- emphasize certain notes
- thin out dense pitch patterns

Combined with gate length control, this can move a sequence from:
- plucky staccato
to
- sustained legato-like lines

The manual notes that at fast speeds, longer gate settings can tie gates together, which can be musically useful for smoother phrasing.

---

## 10. Using Sequencer B as melodic support for A

Even if you only need one main melody, Sequencer B is still very useful.

### Good companion roles for B
- second melodic voice
- transposition source for other modules
- modulation for filter or wavefolder tied to the melody
- rhythmic gate pattern for another voice
- alternate phrase layer

With the **SLAVE B>A** switch, B can share A’s transport control inputs, making it easy to keep them synchronized without extra patching.

This is ideal when building:
- harmonized lines
- bass + lead relationships
- melody + ornament pairs

---

## Practical patch recipes

## Patch 1: Simple melodic line
- Orbitals A **CV OUT** → VCO 1V/oct
- Orbitals A **GATE OUT** → envelope gate
- Envelope → VCA CV
- VCO → VCA → mixer
- Set A to **FW**
- Tune the 8 knobs to a scale
- Turn some gate switches off for rests

Result: a straightforward sequenced melody.

---

## Patch 2: Tangerine Dream style live-transposed sequence
- Patch as above
- Keyboard CV or precision voltage source → **TRANS A**
- Use external clock for tempo sync
- Use 8 or 16 steps
- Keep the programmed pattern intervallic rather than absolute

Result: the same sequenced pattern can be moved harmonically in performance.

---

## Patch 3: Bassline + lead
- A CV/GATE → bass voice
- B CV/GATE → lead voice
- Same external clock to both, or use **SLAVE B>A**
- A length = 8, B length = 5 or 7
- A in FW, B in PND or RND

Result: interlocking melodic layers with different repetition cycles.

---

## Patch 4: Addressed melody map
- Program each step to notes in a scale
- Set mode to **CV** or **CLK**
- External modulation source → **RST/CV input**
- CV OUT → oscillator pitch
- GATE OUT → envelope

Result: incoming voltage selects notes from your programmed set instead of stepping linearly.

This is excellent for controlled generative melody.

---

## Patch 5: Random but musical notes
- Set A to **RND**
- Tune active steps to chord tones or scale tones
- Shorten sequence length to 4–6 steps
- Use gate switches to create sparse rhythms
- Add transpose on TRANS A

Result: constrained random melodic movement.

---

## Patch 6: Long-form 16-step phrase
- Set Sequencer A length above 8 to enter **16-step mode**
- Program first half as phrase
- Program second half as variation
- Clock externally
- Use reset to realign with your song structure

Result: a longer, more song-like melodic sequence.

---

## Important technical/musical considerations

## Output range matters
Orbitals has rear jumpers for output range selection.

From the manual:

- **Bipolar ON, 5V jumper**: -2.5V to +2.5V
- **Bipolar ON, 10V jumper**: -5V to +5V
- **Bipolar OFF, 5V jumper**: 0V to +5V
- **Bipolar OFF, 10V jumper**: 0V to +10V

### For melodic use
If you’re driving oscillator pitch directly:
- the larger ranges can span many octaves
- this makes precise tuning harder by ear

So musically, a smaller range is often easier for tonal sequencing unless you want wide interval leaps.

## Safety note
The manual is explicit:
**Never adjust the jumpers with the module powered on.**

---

## Clocking considerations for melody

Orbitals can use:
- its own internal clock
- an external clock

For music systems with drums, master clocks, or song structure, external clocking is usually the better choice.

The module expects about:
- **1V logic high** for clock/reset/run inputs

It can also run quite fast — up to low audio range internally and about **1kHz clock input** reliably — which means it can blur into audio-rate or pseudo-oscillator behavior, though for melody the sweet spot is obviously much slower.

---

## Best musical strengths of Orbitals

Orbitals is particularly strong when you want:

- **hands-on pitch programming**
- **classic analog sequencing**
- **easy melodic transposition**
- **two related melodic lanes**
- **non-linear voltage-addressed note selection**
- **simple but powerful performance variation**

It is especially good for:
- Berlin-school sequences
- basslines
- looping motifs
- generative melodic patches
- interlocking two-voice patterns

---

## Limitations to keep in mind

Based on the manual, a few practical melodic limitations:

- No built-in quantizer is mentioned, so tuning notes to exact scales may need care or an external quantizer.
- Output range can be broad, which may make fine pitch dialing sensitive.
- Voltage-addressed modes are powerful, but they are not the same as a dedicated quantized note memory system.

Still, the combination of **manual step programming + transpose + addressable steps + dual lanes** makes it very musically flexible.

---

## Bottom line

Hexinverter Orbitals is a very capable melodic sequencer for eurorack because it can cover both:

- **traditional note sequencing**
and
- **more experimental CV-addressed melody generation**

Its standout melodic features are:

- dual 8-step / single 16-step operation
- per-step pitch and gate programming
- transpose input
- random/reverse/pendulum modes
- CV-addressed step selection
- easy synchronization between the two sequencers

In a patch, it can act as:
- the main melody source
- a bassline sequencer
- a harmonized second voice
- a transposable phrase generator
- a programmable note bank for generative composition

If you want, I can also turn this into:
1. a **patch cookbook**
2. a **beginner-friendly quickstart**
3. a **“best companion modules” guide** for Orbitals

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)