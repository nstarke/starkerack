# Humble Audio — Quad Operator

- [Manual PDF](../../manuals/Quad Operator Manual.pdf)

---

[Quad Operator Manual PDF](https://www.dropbox.com/paper/doc/print/JsIQoU7GbeAboEJku9ZgE?print=true)

# Humble Audio Quad Operator (+ Algo) for Melodic Eurorack Use

The **Humble Audio Quad Operator** is a 4-operator digital FM voice platform for Eurorack. With the **Algo expander**, it becomes a programmable FM algorithm morphing system. Used together, these modules are especially strong for building **melodic voices, harmonic layers, animated leads, plucks, bells, basses, and evolving sequence timbres**.

## What these modules are

### Quad Operator
A 4-operator oscillator/FM synthesis module with:

- 4 operators
- Variable operator waveshape:
  - sine
  - triangle
  - square
  - saw
- Per-operator:
  - ratio
  - detune
  - shape
  - gain CV
  - 4 modulation sends
  - independent output
- Global controls:
  - coarse / fine tune
  - VCO/LFO mode
  - 1V/oct
  - LF FM
  - AR FM external mod input
  - reset

### Algo expander
Adds:

- 3 saved FM matrix snapshots: **A, B, C**
- **Live** state
- Crossfade between algorithms/states

In practice, the Algo turns the Quad Operator into a **morphable FM melody engine**.

---

# Why they work well for melodic music

For melodic use, the key strengths are:

1. **Operators can stay in harmonic ratios**
   - In **lock state**, each operator follows integer multiples/divisions of the master pitch.
   - This is ideal for stable, tonal FM sounds.

2. **You can treat it like one voice or several**
   - One complex FM voice
   - Layered intervals
   - Four separate oscillators when operators are in **free state**

3. **You get timbral motion without changing pitch**
   - FM depth changes via modulation sends
   - Shape morphing per operator
   - Gain CV controlling both loudness and modulation intensity

4. **Algo adds performance-ready timbre recall**
   - Store one matrix for a mellow tone, another for a bright attack, another for a metallic variation
   - Crossfade between them while sequenced pitch remains stable

That makes it very good for **musical, melodic phrasing** instead of only harsh experimental FM.

---

# The most important concept: lock vs free

## Lock state
In **lock**, each operator is tied to the master pitch in integer ratios from **1/11 to 11x**.

Use this when you want:

- tuned FM voices
- harmonic overtones
- stable melodic tracking
- classic FM bass/lead/bell sounds
- chords built from related intervals

For melodic music, this is the default mode.

## Free state
In **free**, each operator becomes its own oscillator:

- ratio knob becomes coarse tune
- ratio CV becomes 1V/oct for that operator

Use this when you want:

- 4 separate melodic oscillators
- interval stacking by ear
- independent counterpoint voices
- drones plus a lead
- pseudo-paraphonic patches

This is less naturally harmonic for FM, but very useful compositionally.

---

# Best melodic workflows

## 1. Use it as a single FM voice
This is the most obvious melodic application.

### Basic patch
- Sequencer pitch CV -> **1V/Oct**
- Gate/envelope elsewhere in rack -> VCA or LPG after one chosen operator output
- Start with:
  - VCO mode
  - all operators in **lock**
  - detune at 12 o'clock
  - shapes fully CCW (sine)
  - all modulation sends off

Then:

- Choose one operator output as your audible output
- Use one or more other operators primarily as modulators
- Increase selected modulation sends slowly

### Result
You get:

- plucks
- keys
- FM bass
- glassy leads
- electric piano-like tones
- tuned percussive melody lines

This is exactly the patch style the manual encourages for harmonic FM.

---

## 2. Build layered melodic intervals from multiple outputs
Because each operator has its own output, the Quad Operator can generate **multiple related melodic layers** from one pitch source.

### Patch idea
- Same pitch CV to Quad Operator **1V/oct**
- Keep all operators in **lock**
- Set ratios to musically useful values, for example:
  - Op1 = 1
  - Op2 = 2
  - Op3 = 3
  - Op4 = 4 or 1/2 depending on patch
- Take multiple outputs to separate VCAs/filters/mixers

### Musical use
- Op1 as the fundamental melody
- Op2 an octave-up reinforcement
- Op3 a fifth-ish/upper harmonic color
- Op4 a sub or additional color tone

Strictly speaking these are harmonic partial relationships, not equal-tempered chord voicings. But in a mix they can function as:

- organ-like layering
- registral reinforcement
- pseudo-unison stacks
- overtone voices that track melody tightly

This is very effective for **melodic hooks** that need presence without sounding like a simple saw oscillator.

---

## 3. Use one operator as the audible carrier and animate the others as hidden modulators
This is where the module becomes especially musical.

### Patch idea
- Listen only to **Op1**
- Use Op2, Op3, Op4 as modulators by raising their sends into Op1
- Modulate their **Gain CVs** with envelopes or slow CV

Because gain affects both:

- operator output level
- modulation intensity sent to others

you can make the modulators “enter” dynamically.

### Musical result
This creates:

- note attacks that brighten then settle
- velocity-like timbral articulation
- evolving melodies where each note has internal movement
- expressive basslines with attack transient complexity

This is one of the strongest melodic uses of the Quad Operator.

---

# How to make musical FM sounds instead of noise

The manual gives a very clear starting recipe. For melodic material, begin here:

- **VCO mode**
- all operators in **lock**
- all **detune** at noon
- all **shape** fully counterclockwise (sine)
- all **modulation sends** fully counterclockwise

Then add complexity one step at a time.

## Good order of operations
1. Tune the root melody with **coarse/fine** and **1V/oct**
2. Set operator ratios
3. Bring up one mod send only
4. Add another modulator if needed
5. Then experiment with shape changes
6. Add slight detune last

## Why this matters
FM gets dissonant quickly when you combine:

- non-sine waves
- multiple modulators
- detuning
- free-running operators

For melodic use, restraint gives much better results.

---

# Practical melodic patch recipes

## A. FM lead voice
**Goal:** expressive mono lead

### Setup
- All operators in lock
- Shapes = sine to slightly triangular
- Op1 = carrier
- Op2 ratio = 2
- Op3 ratio = 3
- Op4 ratio = 1 or 4 depending on brightness

### Patch
- Sequencer CV -> 1V/oct
- Gate -> envelope -> external VCA for Op1 output
- Envelope or modulation source -> Gain CV on Op2 or Op3
- Raise Op2 -> Mod1
- Optionally raise Op3 -> Mod1 slightly

### Result
- bright attack
- vocal or brass-like movement
- stable pitch
- classic melodic FM lead behavior

If using Algo:
- Save mellow matrix to A
- bright lead matrix to B
- metallic/aggressive matrix to C
- crossfade during performance

---

## B. FM bassline
**Goal:** punchy, melodic low-end

### Setup
- All operators in lock
- Op1 audible
- Op2 ratio = 2
- Op3 ratio = 1
- Minimal modulation

### Patch
- Sequencer -> 1V/oct
- Gate -> short envelope -> VCA on Op1
- Raise Op2 -> Mod1 a little
- Use very slight Gain CV on Op2 for attack transient
- Keep shapes mostly sine/triangle

### Result
- solid low fundamental
- clickless but articulate attack
- good tracking
- easy to fit in a melodic sequence

For cleaner bass, avoid too much saw/square shape.

---

## C. Bell or mallet melody
**Goal:** tuned metallic melody

### Setup
- Lock state
- Op1 carrier
- Op2 and Op3 as modulators at higher ratios
- Slightly more FM depth than bass/lead patch

### Patch
- Sequencer -> 1V/oct
- Fast-decay envelope -> VCA for output
- Additional short envelope -> Gain CV of modulator operator
- Use a somewhat higher ratio on one modulator

### Result
- struck bell tones
- gamelan-like lines
- metallic arps
- digital mallet melodies

This is a natural use case for FM and fits the Quad Operator well.

---

## D. Evolving melodic timbre with Algo
**Goal:** one sequence, multiple harmonic colors

### Patch
- Create 3 modulation matrices:
  - **A** = almost no FM
  - **B** = moderate harmonic FM
  - **C** = brighter/denser FM
- Sequence pitch into 1V/oct
- Listen to one operator or a mix of several outputs
- Move Algo crossfade manually or via CV

### Result
The melody remains the same, but the tone evolves through:
- pure
- bright
- metallic
- dense

This is excellent for:
- verse/chorus changes
- live transitions
- long-form melodic techno or ambient development

This is probably the most performance-friendly reason to pair Quad Operator with Algo.

---

## E. Four-oscillator melodic bank
**Goal:** multiple melodic roles from one module

### Setup
Put some or all operators in **free state**.

### Patch ideas
- Op1 = lead
- Op2 = bass drone
- Op3 = countermelody
- Op4 = LFO or modulation source in LFO mode

Since in free state:
- ratio knob becomes coarse tune
- ratio CV becomes 1V/oct

you can patch separate pitch CVs to operators.

### Result
You can use the Quad Operator as:
- a compact 4-oscillator composition hub
- a semi-polyphonic source
- a layered melodic machine

This is less “classic FM voice” and more “digital oscillator cluster,” but very useful musically.

---

# Using the AR FM input musically

The **AR FM** input lets you bring in an external audio-rate signal and route it to any operators via its own modulation sends.

This is a huge melodic feature.

## Melodic uses for AR FM

### 1. External oscillator as modulator
Patch a tuned external VCO into AR FM.

- Keep Quad Operator tracking a melody
- Tune external oscillator to a related interval
- Send AR FM to one or more operators

Result:
- richer sidebands
- harmonically shifting timbre
- cross-module FM melodies

### 2. Feedback-like patches
The manual specifically suggests feedback-related experimentation, especially with locked operators.

Patch one Quad Operator output externally and return something into AR FM.

Result:
- more aggressive but still pitch-centered timbres
- animated sustained notes
- unstable but expressive melodic tones

### 3. Use another voice to articulate timbre
Patch a drum, another sequence, or an oscillator into AR FM.

Result:
- melody timbre reacts to external rhythm
- pseudo-sidechain timbral sync
- melodic line that changes character based on another voice

For melodic patching, keep the AR FM gain conservative to preserve pitch clarity.

---

# Shape control as a melodic tool

Each operator can morph continuously:
- sine -> triangle -> square -> saw

This matters a lot for melodic use.

## Best practices
### Sine
Best starting point for:
- clean FM
- harmonic patches
- stable melodic tone

### Triangle
Good for:
- slightly richer leads
- rounded basses
- soft animated timbres

### Square / Saw
Good for:
- bright leads
- edgy basses
- harmonically dense melodic lines

But with FM active, these can introduce:
- noise
- aliasing
- harshness

So for melodic clarity:
- start sine
- move brighter only when needed

---

# Gain CV is secretly one of the most musical controls

The manual notes that **Gain CV affects both output level and modulation intensity**.

That means each operator behaves somewhat like it has a built-in modulation VCA.

## Why this is great for melody
You can use envelopes, LFOs, or sequencer CV to make FM depth become dynamic per note.

Examples:
- short envelope on modulator gain = percussive attack
- slow LFO on modulator gain = timbral vibrato-like evolution
- sequencer row into gain CV = different timbre on each step

This is one of the best features for turning static pitch sequences into **melodic phrases with articulation**.

---

# Reset input for melodic precision

The **Reset CV** resets all operators’ phase.

For melodic music this can help with:

- consistent attack transient
- repeatable plucks
- cleaner modulation when using LFO mode
- phase-locked rhythmic modulation

If your notes feel slightly inconsistent on repeated triggers, reset can tighten behavior.

---

# Using VCO vs LFO mode for melodic composition

## VCO mode
Use for:
- pitched voices
- melodies
- basslines
- harmonic stacks

## LFO mode
Use for:
- phase-locked modulation sources
- slow complex modulation of filters, wavefolders, VCAs, or FM depth
- creating melodic animation indirectly

A strong technique is:

- Put Quad Operator in **LFO mode**
- Use operators as complex, related modulation sources
- Patch outputs to:
  - Gain CVs
  - Shape CVs
  - filter cutoff
  - external VCA level

This won’t directly generate melody, but it can create **coherent motion around a melody**.

---

# How Algo makes melodic performance better

Without Algo, Quad Operator is already flexible. With Algo, it becomes much easier to use in songs.

## What Algo stores
It stores the modulation matrix:
- the positions of all **Mod x** knobs for all 4 operators
- and the AR FM input sends

So Algo is essentially storing your FM routing/depth “algorithm.”

## Musical applications

### 1. Instant timbre presets for the same sequence
Store:
- A = bass
- B = lead
- C = bell

Then run the same melody and swap character.

### 2. Morphing between phrases
Crossfade from simple to complex FM over 8 or 16 bars.

### 3. Build song sections
- Verse = A
- Chorus = B
- Breakdown = Live
- Fill = C

### 4. Animate a static drone into a melody voice
Use saved matrices as macro-structure controls.

This is particularly powerful because FM patches are often hard to recreate exactly by hand.

---

# Suggested melodic strategies

## Strategy 1: Start with one carrier only
Use one operator output as your main voice first. Don’t listen to all outputs at once immediately.

## Strategy 2: Use simple ratios
Begin with:
- 1
- 2
- 3
- 4

These usually give more musically grounded results.

## Strategy 3: Keep detune subtle
The manual says detune is available even in lock mode. For melody:
- tiny detune = warmth/motion
- large detune = inharmonicity

## Strategy 4: Add modulation one send at a time
This module can get chaotic quickly. Small send amounts go a long way.

## Strategy 5: Save usable states with Algo
Once you find:
- a sweet bass
- a good lead
- a bright accent

save them immediately.

---

# Limitations to keep in mind for melodic use

Based on the manual:

- CV inputs for most control are sampled at **6 kHz**
- Audio I/O is at **48 kHz**
- More overtone-rich waveshapes plus heavy FM can create aliasing/noise
- Free-state FM is often more inharmonic
- There is no built-in envelope/VCA for final amplitude shaping, so external utilities help a lot

So for best melodic results, pair it with:
- envelopes
- VCAs
- filters
- sequencers
- mixers

---

# Best use cases in a musical rack

The Quad Operator + Algo combo is especially good for:

- **FM mono lead voice**
- **Melodic bass voice**
- **Bell/pluck/arpeggio generator**
- **Evolving techno sequence timbre source**
- **Harmonic drone with moving overtones**
- **4-oscillator melodic utility bank**
- **Crossfading timbral preset machine**

It is less about instant “DX7 preset nostalgia” and more about a **hands-on modular FM instrument**.

---

# Simple starter melodic patch

If I were dropping this into a patch for immediate musical payoff, I’d do this:

## Patch
- Sequencer CV -> 1V/oct
- Gate -> envelope -> VCA
- Op1 output -> VCA -> mixer
- All operators in lock
- Ratios:
  - Op1 = 1
  - Op2 = 2
  - Op3 = 3
  - Op4 = 1
- All shapes = sine
- All detunes = noon
- Raise Op2 -> Mod1 slightly
- Envelope or slow CV -> Gain CV on Op2
- Save to Algo A
- Make a brighter version with some Op3 -> Mod1 and save to B
- Make a metallic version with more FM and save to C

## Outcome
You now have:
- a playable tuned melodic FM voice
- dynamic note articulation
- three performable timbral states
- crossfading between them with Algo

That’s enough for an entire melodic part in a track.

---

# Bottom line

The **Quad Operator** is best understood as a **modular 4-op FM engine** that can be either:

- a single rich melodic voice,
- a bank of harmonically related oscillators,
- or four independent oscillators.

The **Algo expander** makes it far more practical in actual music by letting you **save, recall, and morph FM routing states**. Together, they are very strong for melodic work because they let you separate:

- **pitch** from
- **timbre evolution**

That means a simple sequence can become expressive, articulate, and song-structured without changing the notes themselves.

If you want, I can also turn this into:
1. a **patch cookbook** with 10 specific melodic patches, or  
2. a **quick-start guide** organized by genre: ambient, techno, electro, and IDM.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)