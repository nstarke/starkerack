# ADDAC Systems — ADDAC-207 Quantizer

- [Manual PDF](../../manuals/ADDAC_207_Quantizer_REV05.pdf)

---

[ADDAC207 Intuitive Quantizer User’s Guide (PDF)](https://www.addacsystem.com/sites/default/files/2021-04/ADDAC207_UsersGuide_Rev05.pdf)

# Using the ADDAC207 Intuitive Quantizer to Create Melodic Components

The attached manual is for the **ADDAC207 Intuitive Quantizer**, a 4-channel quantizer/keyboard/chord generator for Eurorack. Since only this module’s manual is included, I’ll treat the “modules used together” as:

- the **4 internal quantizer voices** of the ADDAC207,
- the **scale, keyboard, transpose, gate, and assign functions** working together,
- and how you would patch it with typical Eurorack companions like **sequencers, random CV, LFOs, envelopes, oscillators, and switches**.

## What this module does musically

The ADDAC207 is best thought of as a **melodic control center**. It can:

- quantize up to **4 CV sources** to the same scale,
- generate **harmonies/chords** from a single source,
- act as a **manual keyboard**,
- output **gates** for note events,
- support **transpose** from an external CV,
- save **presets** for scales/settings,
- and even do **alternate temperaments** and microtonal-style tuning tricks.

That makes it useful for creating:

- melodies,
- basslines,
- harmonized leads,
- arpeggio-like structures,
- chord voicings,
- modal shifts,
- transposed sequences,
- and playable keyboard parts.

---

## Core architecture relevant to melody

## 1. Four quantizer voices

Each voice has:

- **CV IN**
- **CV OUT**
- **GATE IN**
- **GATE OUT**

This means each voice can be:

- an independent pitch stream, or
- linked to **Voice 1 as master** when Voices 2–4 have no CV patched.

That “Voice 1 master” behavior is one of the most musically important features in the module.

### Practical meaning
You can patch:

- one sequencer/random CV into **Voice 1**
- leave **Voices 2–4 unpatched at input**
- define interval offsets for Note 2/3/4

…and suddenly the module becomes a **scale-aware chord generator**.

---

## 2. Scale selection and note masks

You can define the active note set in two ways:

- with the **Key / accidental / major-minor controls** plus **SET KEY**
- or manually by turning individual note buttons on/off

So the ADDAC207 can function as:

- a normal key quantizer, or
- a custom scale/mode quantizer, or
- a restricted note collection generator for motifs.

### Why this matters musically
A quantizer is not just a tuning aid. It shapes melodic identity.

For example:

- **major scale** gives conventional brightness
- **natural minor** gives darker tonal material
- a custom note mask like **C, D, F, G, A** creates pentatonic melodies
- a sparse note selection like **C, Eb, F#, A** creates angular, cinematic material

This module is very good for “composing with omission.”

---

## 3. Quantizer vs Keyboard mode

The ADDAC207 has 2 main modes:

- **Quantizer Mode**
- **Keyboard Mode**

### Quantizer Mode
Incoming CV is quantized to the active note set.

This is the main mode for:

- sequencers
- random voltages
- slewed modulation
- sample-and-hold
- LFO-derived pitch lines

### Keyboard Mode
The buttons become a **monophonic keyboard**.

Important detail from the manual:

- **Voice 1 plays all notes**
- **Voices 2–4 only play notes allowed by the quantizer scale**, useful for chord generation

### Musical use
This makes the module perform like:

- a playable live pitch controller,
- a harmonic improvisation tool,
- a way to audition scales/chords before sequencing them.

---

# Best musical patch strategies

## Patch Strategy 1: Single melody line from random or sequencer CV

### Patch
- CV source -> **IN 1**
- **OUT 1** -> oscillator 1V/oct
- **GATE OUT 1** -> envelope trigger/gate
- envelope -> VCA
- oscillator -> filter/VCA/audio path

### Result
You get a pitch stream forced into the chosen scale.

### Best source types
- stepped random
- sequencer row
- sample-and-hold from noise
- slow triangle/sine LFO for repeating contour melodies
- pressure/joystick CV for manual melody creation

### Useful settings
- **Q.TYPE Above** for always pushing notes upward into the scale
- **Below** for grounded/downward-feeling resolution
- **Ignore** for sparse/event-style behavior when only exact scale voltages should pass meaningfully

### Musical character
- Above = more rising/aspirational
- Below = more weighted/stable
- Ignore = glitchy/minimal/selective

---

## Patch Strategy 2: One source into 4-part harmony

This is probably the most powerful melodic use.

### Patch
- Sequencer/random CV -> **IN 1**
- Leave **IN 2–4 unpatched**
- Turn **Voice 1 Master** ON in the TRIG.R menu
- Set Note intervals:
  - **NOTE 2** = 3rd
  - **NOTE 3** = 5th
  - **NOTE 4** = 7th
- Patch **OUT 1–4** to 4 oscillators, or 4 voices in a polyphonic patch

### Result
The module derives harmonized outputs from one melodic root.

Because intervals are interpreted **according to the active scale**, the harmony is diatonic rather than fixed-chromatic.

### Why this is musically strong
If you choose:
- C major scale
- root melody on Voice 1
- intervals 3rd / 5th / 7th

then the resulting harmony follows the scale, producing musically coherent chords.

For example:
- over C you might get C–E–G–B
- over D you might get D–F–A–C
- over E you might get E–G–B–D

So the chord quality shifts naturally with scale degree.

### Great uses
- 4-voice pads
- stacked oscillators
- chord stabs
- organ-style harmonies
- modal drones with moving tops
- generative harmony

---

## Patch Strategy 3: Bass + lead + chord tones from one source

Instead of treating all 4 outputs equally, split their roles.

### Patch idea
- **OUT 1** -> bass oscillator
- **OUT 2** -> mid voice
- **OUT 3** -> lead/pluck
- **OUT 4** -> upper shimmer/FM mod oscillator

Set intervals for 2/3/4 to create voicings like:
- root / 3rd / 5th / 7th
- root / 5th / octave / 10th
- root / 4th / 6th / 9th

### Musical benefit
One CV source becomes a complete tonal ecosystem.

This is especially effective if:
- each oscillator has a different envelope length,
- different filter brightness,
- different stereo placement.

---

## Patch Strategy 4: Four independent melodies in one key

### Patch
- 4 independent CV sources -> **IN 1–4**
- 4 separate oscillators or voices on **OUT 1–4**
- optionally 4 different trigger streams to each **GATE IN**

### Result
You get four separate melodic lines constrained to the same scale.

### Great for
- contrapuntal patches
- generative ensembles
- bass / lead / arp / drone divisions
- percussion tuned to scale tones
- four sequencers made harmonically compatible

### Why it works
Instead of harmonizing one source, you harmonically **unify multiple independent sources**.

This is often more interesting than strict chord following, because each line retains its own rhythm and contour.

---

## Patch Strategy 5: Use GATE IN for rhythmically controlled melody updates

Each voice can quantize from CV changes alone, but **GATE IN** allows external timing control.

### Patch
- flowing CV -> Voice IN
- trigger pattern -> corresponding **GATE IN**
- **OUT** -> oscillator pitch
- **GATE OUT** -> envelope

### Result
Pitch only updates when a trigger arrives.

### Why this matters
This lets you separate:
- **pitch source behavior** from
- **note rhythm**

So you can use:
- slow random drift as pitch material
- fast clocked triggers for rhythm

Or:
- a sequencer CV row
- irregular trigger pattern for syncopated note extraction

### Musically this enables
- sampled melodic gestures
- rhythmic arp-like slicing of continuous voltages
- stable timing from unstable pitch sources

---

## Patch Strategy 6: Manual keyboard performance with harmonized outputs

### Patch
- Enter **Keyboard Mode**
- Use buttons as notes
- **OUT 1–4** to multiple oscillators/voices
- **GATE OUTS** to envelopes

### Result
You play the module directly as a mini performance keyboard.

### Particularly useful for
- live improvisation
- quickly testing voicings
- drone harmonies
- melodic sketching
- hands-on modal playing

### Important behavior
In keyboard mode:
- Voice 1 can access all notes
- Voices 2–4 still respect the selected scale and interval logic

That makes it very good for **safe live harmony playing** without accidentally hitting bad chord tones.

---

# Transposition as a musical system

The ASSIGN input is a big compositional feature.

You can assign the external CV input to several functions, especially:

- **Input Transpose**
- **Scale Transpose**
- Note 2/3/4 offsets
- Quantization type
- Gate length
- Trigger repeat
- Octave offset
- Preset change

## 1. Input Transpose

This adds incoming assign CV to the incoming melodic CV before quantization.

### Musical effect
The melody shape is preserved, but moved up/down within scale behavior.

### Good use cases
- transpose a sequence by keyboard CV
- use a second sequencer for phrase transposition
- use pressure/joystick to shift motif center
- use slow CV for evolving harmonic drift

---

## 2. Scale Transpose

This transposes the **scale itself**, not the incoming melody CV.

### Musical effect
The same input voltage is now interpreted against a different root.

This is a very different result from input transposition.

### Why it’s musically interesting
Input transpose = “move the melody”
Scale transpose = “move the harmonic world under the melody”

That makes scale transpose especially useful for:
- chord progressions
- key changes
- modal shifts
- harmonic cycling in generative patches

### Example use
Keep a repeating contour at Voice 1 input.
Use a slow or sequenced CV into ASSIGN mapped to **Scale Transpose**.
Now the contour remains similar while the harmonic context changes.

This is excellent for:
- ambient
- Berlin-school
- generative tonal music
- soundtrack work

---

# Chord construction ideas using NOTE 2/3/4 intervals

The module lets you define interval relationships for Voices 2–4 relative to Voice 1.

Since these are scale-aware, you can create many musically useful textures.

## Traditional tertian harmony
- Note 2 = 3rd
- Note 3 = 5th
- Note 4 = 7th

Use for:
- jazz-ish chord color
- lush pads
- generative harmony

## Open harmony
- Note 2 = 5th
- Note 3 = 8th
- Note 4 = 10th

Use for:
- cinematic openness
- less muddy lower registers
- wide melodic stacks

## Quartal-ish/modal flavor
- Note 2 = 4th
- Note 3 = 7th
- Note 4 = 9th

Use for:
- suspended/modal harmony
- less tonal certainty
- modern ambient textures

## Parallel melodic doubles
- Note 2 = 3rd
- Note 3 = 6th
- Note 4 = 8th

Use for:
- folk-like doubles
- contrapuntal melodic blooms
- denser lead lines

---

# Scale design for melody writing

The manual makes clear you can manually toggle note buttons on/off. This is where the module gets especially compositional.

## 1. Diatonic scales
For conventional melodic work:
- major
- natural minor

Good for:
- tonal basslines
- hooks
- chord progressions
- voice-leading patches

## 2. Pentatonic extraction
Instead of using all 7 notes, choose 5.

Good for:
- fewer clashes
- stronger melodies from random CV
- easy layering over drones
- “everything sounds good” generative patches

## 3. Sparse custom scales
Choose only 3–6 notes.

Good for:
- motif control
- minimalist patterns
- gamelan-like reduction
- pseudo-arpeggiation from random CV

## 4. Modal use with Scale Mode
The module supports scale modes like:
- Ionian
- Dorian
- Phrygian
- Lydian
- Mixolydian
- Aeolian
- Locrian

This is useful when you want:
- the same basic key center,
- but different emotional color.

### Examples
- **Dorian** for minor but hopeful
- **Phrygian** for dark/tension
- **Lydian** for floating/bright
- **Mixolydian** for dominant/bluesy repetition

---

# Gate functions and melody shaping

## Gate Length
Gate length can be set from very short to very long.

This directly affects articulation.

### Short gate
- plucky notes
- arpeggios
- percussive basslines

### Long gate
- legato envelopes
- sustained drones
- tied melodic phrases

## Gate Off Condition
There’s an option to only quantize a new note when gate out is off.

### Musical use
This can force phrase clarity and prevent too-fast note updates.

Good for:
- monophonic synth lines
- clean phrasing
- reducing chatter from unstable CV sources

## Trigger Repeat
If ON, re-hitting the same quantized pitch still outputs a gate.

### Important use
This is excellent for:
- repeated notes with fresh envelope articulation
- rhythmic ostinatos
- percussive lead lines

If OFF:
- same pitch won’t retrigger unnecessarily

That is useful for:
- smooth legato behavior
- less repetitive re-firing

---

# Presets as song structure tools

The module stores presets containing scale notes and many menu settings.

This means you can use presets to prepare different melodic states such as:

- verse scale
- chorus scale
- bridge mode
- alternate harmony interval set
- different gate or quantization behavior

Since ASSIGN can also be mapped to **change preset**, the module can potentially become a **song-section harmonic switcher**.

### Example
Preset 1:
- C major
- chord tones 3rd/5th/7th

Preset 2:
- A minor
- open intervals 5th/8ve/10th

Preset 3:
- custom pentatonic
- short gates

Preset 4:
- Lydian with longer gates

Then move between them in performance or by external CV assignment.

---

# Alternate temperaments and melodic identity

The tuning menu supports several temperaments, including:

- Equal
- Just
- Bohlen-Pierce
- Pure / Well Tuned
- Exotic

For most melodic Eurorack use, you’ll likely stay in **Equal**. But the others can be used intentionally.

## Just temperament
Can make intervals feel more resonant and consonant around a chosen root.

Good for:
- drones
- root-centered ambient harmony
- static harmonic fields

## Bohlen-Pierce / Exotic
More experimental territory.

Good for:
- alien melody systems
- non-standard tonal centers
- abstract generative composition

Important note from the manual: non-equal temperaments are more root-dependent, so they are best when the piece has a strong tonal center rather than constant transposition.

---

# Strong real-world melodic patch examples

## Example 1: Generative ambient chord cloud
### Patch
- Smooth random CV -> IN 1
- Clock divider trigger -> GATE IN 1
- Voice 1 Master ON
- Note 2 = 3rd
- Note 3 = 5th
- Note 4 = 7th
- OUT 1–4 -> four oscillators or four voices
- Slow envelopes from GATE OUTs
- Long gate length
- Major or Dorian scale

### Result
A slow-moving harmonized cloud with coherent tonal motion.

---

## Example 2: Bassline plus harmonized lead
### Patch
- Sequencer CV -> IN 1
- Trigger pattern -> GATE IN 1
- OUT 1 -> bass oscillator
- OUT 2/3/4 -> stacked lead oscillators
- Use different octaves externally at oscillators or via octave offseting elsewhere

### Result
The bassline drives the harmony while upper voices bloom into chords.

---

## Example 3: Four coordinated but independent melodic voices
### Patch
- 4 sequencer lanes / random sources -> IN 1–4
- Same key and scale across all voices
- Different trigger streams into GATE IN 1–4
- OUTs to 4 sound sources

### Result
A small ensemble that remains harmonically unified.

This is especially effective for:
- modular “string quartet” style patches
- tuned percussion ensembles
- minimal music phasing systems

---

## Example 4: Live playable harmonic controller
### Patch
- Keyboard mode
- OUT 1–4 to four oscillators/voices
- GATE OUTs to envelopes
- Set Note 2/3/4 intervals
- Use presets for different harmonic environments

### Result
Hands-on chord melody performance from the panel itself.

---

## Example 5: Harmonic progression engine with scale transpose
### Patch
- Repeating melodic sequencer into IN 1
- ASSIGN input mapped to **Scale Transpose**
- Slow stepped CV sequence into ASSIGN
- Voice 1 Master ON with chord intervals set

### Result
The melodic contour stays recognizable while the underlying harmonic key changes.

This is one of the best uses in the module for creating actual “progressions” in generative music.

---

# Best supporting modules to pair with the ADDAC207

Even though they’re not in the attached manual, this quantizer pairs especially well with:

## Sequencers
For intentional melodic structure:
- step sequencers
- CV sequencers
- Cartesian sequencers
- Turing/random-loop sequencers

## Random voltage sources
For generative melody:
- stepped random
- sample & hold
- fluctuating random
- chaos CV

## Clocks and trigger generators
To control note timing through GATE IN.

## Oscillators
Especially multiple oscillators, since the ADDAC207 shines as a chord source.

## Envelopes and VCAs
Because GATE OUT gives you note articulation.

## Switches/sequential switches
For alternating melodic sources into one voice or redistributing outputs.

## Mixers and precision adders
For layering additional transposition and interval structure.

## Joysticks, touch controllers, keyboards
Excellent with ASSIGN transpose functions and keyboard mode.

---

# Important practical observations from the manual

## Voice 1 as master is central
If inputs 2–4 are unpatched and master behavior is active, the module becomes much more than a quantizer — it becomes a **scale-aware harmony engine**.

## Trigger repeat changes phrasing dramatically
This matters a lot if you want repeated notes to retrigger envelopes.

## Reaction time can be adjusted
This is mostly UX-related, but helpful if you perform in keyboard mode and want to avoid accidental menu entry.

## Fine tuning is per voice
Very useful when driving multiple oscillators in stacked harmony patches.

## Presets do not store everything
Fine tunings and some global settings are in main memory, not preset memory.

---

# Best musical roles for this module

The ADDAC207 is especially strong as:

- a **master melodic quantizer** for a whole patch
- a **chord generator** from one CV line
- a **4-part harmony distributor**
- a **modal/generative melody shaper**
- a **manual playable keyboard quantizer**
- a **transpose/progression engine**

It is less just a utility and more a **compositional module**.

---

# Bottom line

If you use the ADDAC207 well, it can provide nearly all pitch organization for a modular patch:

- one source becomes a melody,
- one melody becomes a chord,
- multiple CVs become a coherent ensemble,
- external CV can transpose notes or entire harmonic spaces,
- and presets can organize different musical sections.

The strongest melodic workflows are:

1. **single CV -> harmonized multi-voice outputs**
2. **multiple CV streams -> shared scale coherence**
3. **assign CV -> transposition or scale movement**
4. **keyboard mode -> direct melodic/harmonic performance**

If you want, I can also turn this into:
- a **“patch cookbook” with 10 concrete patches**,
- a **cheat sheet for live performance**, or
- a **signal flow diagram** for using the ADDAC207 in a melodic Eurorack system.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)