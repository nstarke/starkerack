# Vermona — Melodicer

- [Manual PDF](../../manuals/melodicer manual en 1.1 web.pdf)

---

[Manual PDF](#)

# Vermona meloDICER — creating melodic components in a Eurorack system

meloDICER is a **stochastic melodic sequencer / advanced control-voltage quantizer**. In practice, it excels at generating **musical pitch streams and phrase-like melodic motion** that sit between fixed sequencing and controlled randomness.

If your goal is to build **melodic parts** in a modular patch, meloDICER can serve as:

- a **main melody generator**
- a **pitch randomizer with repeatable patterns**
- a **quantizer for incoming CV**
- a **melody processor for externally supplied rhythms**
- a **transposition target for modulation and performance control**

---

## What the module does best for melody

The manual makes clear that meloDICER separates musical output into two domains:

- **RHYTHM**
- **MELODY**

For melodic creation, the most important idea is that **you do not program exact notes step by step**. Instead, you define:

- which notes are allowed
- which octaves are allowed
- how likely each note is
- whether phrases repeat or continuously evolve

That makes it ideal for:
- generative leads
- ambient motifs
- Berlin-school style repeating phrases with variation
- probabilistic basslines
- evolving tonal accompaniment
- melodic layers that stay musical without being rigid

---

## Core melodic controls

## 1. Semitone probability faders

The melody section uses faders for semitones. These define the **probability** of each note appearing.

### Musical use
This is the heart of melodic shaping.

For example:

- raise only **C** → melody outputs only C across the chosen octave range
- raise **C, E, G** → creates a C major triadic pitch pool
- raise **C, D, E, G, A** → pentatonic melody source
- raise more dissonant tones at lower levels → occasional tension notes

### Why this is powerful
Instead of programming a sequence, you define a **harmonic field**. meloDICER then draws from it stochastically.

This is especially useful for:
- tonal improvisation
- quickly finding hooks
- staying in-key during live performance
- generating accompaniment that follows a harmonic identity

---

## 2. Octave range faders

Two faders define the low and high pitch boundaries.

### Musical use
This lets you shape register very quickly:

- narrow range → bassline or motif
- wide range → more expressive melody
- high-only range → lead voice
- low-mid range → ostinato or counterline

Because pitch probability interacts with range, the same note selection can feel very different depending on octave span.

### Patch ideas
- **1-octave range** for bass
- **2–3 octaves** for melodic arpeggiation
- **high narrow range** for glassy plucks
- **wide range** for wandering ambient lines

---

## 3. Dice mode vs realtime mode

This is one of meloDICER’s most important compositional features.

### Dice mode
Pressing DICE generates a new random pattern for melody and/or rhythm, then repeats it.

This is ideal when you want:
- a phrase that loops
- a motif you can keep
- a melody you can save as a pattern
- controlled experimentation

### Realtime mode
Holding DICE switches that section into realtime generation, where notes are continuously re-randomized.

This is ideal when you want:
- endless evolving melodies
- generative ambient motion
- non-repeating tonal drift
- controlled instability

### Best musical strategy
A very strong use case is:

- keep **rhythm in dice mode**
- put **melody in realtime mode**

This gives you a stable rhythmic phrase with continuously shifting pitches.

Or reverse it:

- fixed melody pool
- changing rhythm

That’s excellent for melodic variation without losing identity.

---

## 4. Pattern length

Pattern length can be set from a sub-range within 16 steps of 1/16-note resolution.

### Musical use
This matters a lot for melody because phrase length shapes memorability.

Examples:
- **16/16** = standard 1-bar phrase
- **7 steps** = asymmetrical looping motif
- **5 or 11 steps** = polymetric melodic cycling against other modules
- shifted start/end range = altered phrase contour without changing probabilities

This makes meloDICER useful not only as a melody generator but also as a **phrase architecture tool**.

---

## Rhythm controls as melodic articulation

Although the question is about melody, the rhythm section strongly affects how the melody is perceived.

## NOTE VALUE
Sets the base rhythmic subdivision.

For melody this means:
- 1/8 → singable motif
- 1/16 → sequencer-like line
- slower values → sparse melodic statements

## VARIATION
Adds longer or shorter note values around the base.

For melody this creates:
- phrase irregularity
- rhythmic life
- occasional syncopation or expansion

## LEGATO
Determines the probability that pitches change without a new gate.

For melody this is huge:
- low LEGATO → articulated, sequenced notes
- medium LEGATO → phrased and lyrical
- high LEGATO → slurred motion, especially good with portamento or sustained envelopes

## REST
Introduces silence.

For melody, REST is not just rhythmic absence; it creates:
- breathing room
- motif clarity
- syncopated phrasing
- call-and-response feeling

A melody with carefully chosen note probabilities and moderate REST often sounds much more intentional than a fully dense stream of notes.

---

## Best ways to use meloDICER with other modules

Below are the most practical ways to combine it with the rest of a Eurorack system to make melodic components.

---

## 1. As a full melodic voice source

### Patch
- **1V/OCT OUT** → oscillator 1V/OCT
- **GATE OUT** → envelope gate input
- envelope → VCA CV
- oscillator → filter → VCA

### Result
meloDICER becomes the complete melody brain for a voice.

### Best for
- lead lines
- basslines
- generative motifs
- melodic arpeggios

### Tips
- use a waveform with clear pitch identity, like saw, pulse, or triangle
- add slight filter movement for phrase dynamics
- keep note selection sparse for more memorable melodies

---

## 2. As a duet generator with two oscillators

Because meloDICER outputs one pitch CV, you can mult it to multiple oscillators.

### Patch
- **1V/OCT OUT** → mult → oscillator A + oscillator B
- tune osc B to a fixed interval, e.g. +5th or +octave
- **GATE OUT** → envelope(s)

### Result
A harmonized melodic line.

### Best for
- unison leads
- octave bass
- fifth-based techno melodies
- rich ambient lines

### Variation
Use separate envelopes/VCAs so one oscillator is longer or quieter than the other. That gives a layered melodic contour from one CV source.

---

## 3. As a melody source for sampled or plucked voices

meloDICER pairs especially well with:
- LPG-based voices
- plucks
- FM voices
- wavetable oscillators
- physical modeling modules

Because the note stream is probabilistic, timbres with strong transient identity make the melody feel intentional and expressive.

### Great patch style
- medium note variation
- moderate rest
- some legato
- restricted note set like minor pentatonic

This produces very musical plucked patterns quickly.

---

## 4. As a constrained improviser over a harmonic center

Set only notes that belong to a scale or chord.

### Example scales
- minor pentatonic for safe melodic wandering
- dorian for moody but flexible lines
- major triad + 2nd + 6th for bright pop-like movement
- chromatic plus weighted chord tones for jazzy tension/release

### Result
The module improvises **inside your harmonic rules**.

This is one of the strongest ways to use it: let the machine “compose,” but only from your curated note world.

---

## 5. With an external clocked rhythm source in Mode B (Seq + Gate)

Mode B is very useful musically.

In this mode, meloDICER stops generating its own rhythm and instead takes gate signals at **GATE IN 1**, while still generating pitch from the melody section.

### Why that matters
You can use another module for rhythm while meloDICER handles pitch choice.

### Patch
- trigger/gate sequencer or rhythm generator → **GATE IN 1**
- **1V/OCT OUT** → oscillator pitch
- external gates also drive the envelope, or derive articulation from your patch

### Result
External rhythm + meloDICER pitch intelligence.

### Best companions
- trigger sequencers
- Euclidean rhythm modules
- random gate sources
- clock dividers
- logic-generated rhythms

### Strong musical use
Pair a complex but repeating drum/trigger pattern with meloDICER’s melody engine for **tight but non-programmed melodic phrasing**.

The manual even suggests pairing it with another rhythm module for altered rhythms or duophonic ideas.

---

## 6. Use CV IN 1 for melodic transposition

CV IN 1 can affect pitch in two major ways:

- **ADD SEQ** = adds incoming CV unquantized
- **TRANS SEQ** = adds incoming CV quantized to semitones

### Best melodic use
Use **TRANS SEQ** for clean musical transposition.

### Patch ideas
- sequencer row → CV IN 1 for chord-root changes
- precision adder-like transposition source
- keyboard CV → transpose generated melody live
- slow stepped random voltage → phrase-level modulation

### Result
Your melody keeps its interval/probability character but shifts harmonically.

This is extremely effective for:
- verse/chorus movement
- bassline root progression
- live harmonic changes
- generative composition that still follows song structure

### ADD SEQ use
Use **ADD SEQ** when you want looser, more analog movement:
- LFO vibrato-ish pitch motion
- slewed CV drift
- experimental microtonal wobble

---

## 7. Modulate pitch range with CV IN 1 LO and HI

CV IN 1 can also modulate the low and high range boundaries.

### Musical use
This changes melodic register over time.

### Patch ideas
- slow LFO to HI → melody gradually expands upward
- envelope to LO → notes jump out of the bass range temporarily
- sequencer CV to range bounds → different sections occupy different registers

### Result
A melody that feels like it “opens up,” “climbs,” or “contracts.”

This is great for arrangement within a live patch.

---

## 8. Quantize external CV in Modes C and D

meloDICER has two quantizer modes, which makes it useful even when it’s not your main sequencer.

## Mode C — Quantizer 1
- external CV enters **CV IN 2**
- quantization occurs on quarter notes / clock basis
- melody faders define the scale and note weighting

## Mode D — Quantizer 2
- external CV at **CV IN 2**
- quantization happens while **GATE IN 2** is active

### Why this matters musically
The faders do not just define scale membership; they define **quantization range weighting**. That means you can bias external voltages toward certain notes.

### Great patch sources
- sample & hold
- random CV
- chaotic generators
- sequencer rows
- LFOs
- pressure / controller voltages

### Result
You can turn raw modulation into:
- in-key melodies
- weighted tonal contours
- playable harmonic textures

This is a very elegant way to generate melodies from “non-musical” CV sources.

---

## 9. Use meloDICER for bass + lead relationships

One practical way to use the module in a system is to derive a **bass-focused melodic line**, then mirror or support it elsewhere.

### Patch
- meloDICER pitch to bass oscillator
- mult same CV to second voice through offset/transposition
- second voice processed differently (higher octave, longer envelope, more reverb)

### Result
You get coherent melodic layering because both voices share a pitch source.

### Best musical outcomes
- bass + octave lead
- bass + shimmering counter shimmer
- mono line + sub
- motif + drone accent

---

## 10. Save patterns as melodic scenes

meloDICER stores patterns that include:
- rhythm and melody settings
- available note values for variation
- pattern length
- DICE button states
- current random values

That means saved patterns can function like **melodic snapshots**.

### Musical use
Store:
- bass pattern
- verse motif
- chorus motif
- sparse ambient line
- highly active climax phrase

Then recall them as composition states.

### Important performance note
Loading activates **lock-mode**, preventing current physical control positions from immediately overwriting the loaded pattern. That’s useful on stage.

---

## 11. Lock mode for preparing melodic changes

LOCK is very performance-friendly.

### Why it matters
Normally, moving faders instantly affects output. In LOCK mode, you can set up:
- new scale
- new octave range
- new pattern length

without hearing the change yet.

### Performance use
While one melody plays, prepare the next one, then exit LOCK to apply it at once.

This is excellent for:
- transitions
- breakdowns
- harmonic pivots
- building tension before a melodic reveal

---

## 12. Gate-input control for melodic performance

Gate inputs can be configured for:
- toggling dice/realtime
- re-dicing rhythm or melody
- restart
- mute

### Melodic uses
- trigger new melody generation from a manual gate button
- re-dice at bar boundaries from a clocked trigger source
- restart phrases for arrangement alignment
- switch between looping and evolving modes with logic or performance gates

This makes meloDICER highly patchable inside a larger generative ecosystem.

---

# Musical patch recipes

## Patch 1: Generative lead line
**Use when:** you want an evolving top melody

- set note faders to a pentatonic or modal scale
- set octave range to 2–3 octaves
- NOTE VALUE around 1/8 or 1/16
- moderate VARIATION
- medium LEGATO
- some REST
- rhythm in dice mode
- melody in realtime mode

**Result:** a coherent but always-changing lead.

---

## Patch 2: Repeatable hook finder
**Use when:** you want to discover catchy melodic loops

- choose 3–5 notes
- use a narrow octave range
- keep rhythm simple
- press DICE repeatedly until a memorable phrase appears
- save the pattern

**Result:** fast hook generation without step programming.

---

## Patch 3: Probabilistic bassline
**Use when:** you want moving low-end that stays musical

- choose root, fifth, octave, maybe minor/major third
- narrow the range low
- reduce VARIATION
- low to medium REST
- low LEGATO
- dice both rhythm and melody until it grooves

**Result:** bass movement with human-like irregularity.

---

## Patch 4: Externally driven melody
**Use when:** you already have a rhythm sequencer you like

- switch to **Mode B**
- rhythm sequencer / Euclidean trigger source → GATE IN 1
- melody faders define harmonic pool
- 1V/OCT to oscillator

**Result:** your external rhythm gains an intelligent pitch layer.

---

## Patch 5: Random CV to tonal melody
**Use when:** you want chaos disciplined into music

- random stepped CV → CV IN 2
- switch to quantizer mode C or D
- raise scale-note faders
- use clock or gate source as required by the chosen mode

**Result:** unstable source material becomes structured melody.

---

## Patch 6: Section transposition
**Use when:** you want song-like harmonic movement

- set CV IN 1 to **TRANS SEQ**
- send stepped CV from sequencer or keyboard
- keep one melodic pattern running
- transpose roots over time

**Result:** a consistent melodic identity across chord/root changes.

---

# Important operational notes from the manual

## External clock behavior
meloDICER syncs its internal clock to external clock, but does **not** behave like a classic “advance one step per pulse” sequencer. Starting and stopping external clock won’t hard start/stop the sequence in the traditional way.

For arrangement control:
- use **mute**
- use **restart**
- use configured gate inputs

This matters if you are trying to align melodies tightly with other sequencers.

---

## Firmware limitation noted in the manual
In firmware **R19**, the edit-parameter assignments for **CV IN 2 controlling NOTE VALUE and VARIATION** are noted as **not working**.

So for melodic rhythm modulation via CV IN 2:
- LEGATO and REST are more reliable based on the manual note
- be cautious expecting NOTE VALUE / VARIATION modulation in that firmware

---

## Voltage and interfacing notes
Useful integration details:

- **1V/OCT output:** 0–5 V
- **GATE OUT:** +10 V
- **CV inputs:** 0–5 V active, up to +12 V tolerated
- **clock/gate inputs:** threshold +2 V

So it should integrate well with most Eurorack voices, modulation sources, and trigger sequencers.

---

# Best companion module types

meloDICER works especially well with:

- analog or digital VCOs
- envelope + VCA voice chains
- LPGs for plucky melodic articulation
- quantized transposition sources
- Euclidean / probabilistic trigger generators
- clock dividers and logic
- random voltage sources
- sample & hold
- precision adders
- filters with strong character
- delay/reverb for generative ambient output

If you are building a melodic system around it, the most synergistic pairings are:

1. **A voice module or oscillator/filter/VCA chain**
2. **A clock or master timing source**
3. **A trigger sequencer or gate generator**
4. **A CV source for transposition**
5. **Effects for spatializing the result**

---

# Bottom line

Vermona meloDICER is best understood not as a traditional note-entry sequencer, but as a **musical probability engine** for pitch and phrasing.

Used with other Eurorack modules, it can create melodic components by:

- generating complete melodies and basslines
- constraining randomness to chosen scales/chords
- repeating or continuously evolving pitch patterns
- accepting external rhythms for pitch generation
- quantizing random or sequenced CV into weighted scales
- transposing live for harmonic development
- storing melodic states as recallable patterns

Its real strength is that it lets you **compose by defining musical boundaries rather than exact events**. In a Eurorack system, that makes it incredibly effective for patches that feel alive, tonal, and performable.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)