# Noise Engineering — Basimilus Iteritas Alia

- [Manual PDF](../../manuals/Basimilus Iteritas Alia Manual - Noise Engineering Documentation.pdf)

---

[Basimilus Iteritas Alia Manual PDF](https://manuals.noiseengineering.us/bia/)

# Using Basimilus Iteritas Alia for melodic music

Basimilus Iteritas Alia (BIA) is presented as a **digital drum voice**, but the manual makes clear it can also function as a strong **melodic oscillator/synth voice**. In particular, it works well for **basslines, leads, stabs, supersaws, harsh FM-style tones, and sequenced pitched percussion**.

## Why it works melodically

From the manual:

- **Pitch input is calibrated for 1V/oct tracking**
- Pitch CV range is **-2 V to +5 V**
- There is a **Pitch encoder** for fine or coarse semitone tuning
- It has multiple synthesis modes:
  - **Skin**: additive, more tonal
  - **Liquid**: additive with pitch envelope, great for punchy melodic tones
  - **Metal**: phase-modulated, noisier and more inharmonic, but still useful for aggressive bass/lead sounds
- It includes an **Env Out**, which mirrors the internal envelope and can modulate other modules

This means BIA can be treated as a full synth voice when paired with:
- a **pitch sequencer**
- a **trigger/gate source**
- optional **modulation**
- optional **filter, VCA, effects, or wave shaping**

---

## Best melodic roles for BIA

## 1. Bassline voice

BIA is especially strong for bass.

### Recommended setup
- Send a **pitch sequence** to **Pitch**
- Send a **gate/trigger pattern** to **Trig**
- Take **Out** to your mixer, filter, or effects
- Use **Bass** range switch to place it in bass register
- Start with **Skin** or **Liquid**

### Good controls for bass shaping
- **Morph**: moves through sine, triangle, saw, square. Lower settings can give more solid low-end; more aggressive settings add bite.
- **Harmonic**: keep lower for simpler bass fundamentals, or increase for more overtone weight.
- **Spread**: low or harmonic settings help preserve tonal clarity.
- **Fold**: adds aggression and harmonics; useful for acid-like or distorted bass.
- **Decay**: controls note length.
- **Attack**: center or slightly right for cleaner onset; left of center adds noise, which is less typical for clean bass but useful for edge.

### Especially useful mode
- **Liquid** adds pitch envelope internally, which can make basslines feel more punchy and animated even without external modulation.

---

## 2. Lead voice

BIA can make sharp, cutting leads with a lot of harmonic motion.

### Recommended setup
- Pitch sequencer to **Pitch**
- Trigger/gate sequence to **Trig**
- Use **Alto** or **Treble**
- Patch **Out** to delay/reverb for space

### Good approaches
- **Skin** for brighter, more stable melodic leads
- **Metal** for aggressive industrial or experimental lead timbres
- Moderate **Spread** gives richer overtone spacing
- Increase **Fold** for growl and articulation
- Modulate **Morph** or **Fold** slowly with CV for evolving phrases

### Musical result
This works particularly well for:
- techno leads
- EBM/industrial hooks
- arpeggios
- distorted mono leads

---

## 3. Chord-like or supersaw-style melodic textures

The manual includes a **Supersaw** patch concept, which is very important melodically.

Because BIA uses multiple oscillators, **Spread** can create detuned or interval-rich textures that feel wider and more chordal than a simple single oscillator.

### Patch concept
- Pitch CV sequence to **Pitch**
- Trigger pattern to **Trig**
- Use **Skin**
- Increase **Spread**
- Adjust **Morph** toward brighter waveforms
- Use moderate **Harmonic**
- Use longer **Decay**

### Pair with
- stereo delay
- chorus
- reverb
- filter modulation

This can yield:
- unison-style leads
- pseudo-chord stabs
- trancey supersaw-ish lines
- big melodic riffs

---

## 4. Plucked or struck tonal sequences

Because BIA has an internal envelope and percussive architecture, it naturally excels at **plucks**, **mallets**, and **pitched strikes**.

### Best mode
- **Skin** for clean struck tones
- **Liquid** for kick-like plucked bass
- **Metal** for bells, clangs, and tuned metallic hits

### How to patch
- Clocked trigger source into **Trig**
- Quantized pitch CV into **Pitch**
- Short-to-medium **Decay**
- Tune with encoder
- Use **Attack** near center for a punchy transient

This is a strong method for:
- marimba-like sequences
- tuned tom patterns
- melodic percussion lines
- electro-style tonal hits

---

## 5. FM-like melodic bass and metallic melody

The manual explicitly includes a **“Not quite FM bass”** patch. That indicates BIA is very capable of FM-adjacent melodic sounds.

### Use **Metal** mode for:
- metallic bass
- alien leads
- tuned industrial percussion
- digital bell-like phrases

### Main sound design controls
- **Spread** changes interval relationships / inharmonicity
- **Harmonic** affects overtone envelope behavior
- **Morph** changes waveform foundation before modulation complexity
- **Fold** adds further density and harshness

This is ideal for:
- IDM
- industrial
- broken beat
- dark techno
- soundtrack design

---

## How to combine BIA with other modules for melodic systems

Even though only BIA is shown here, the manual strongly suggests how it behaves in a larger patch. Here are the most useful pairings.

## A. With a sequencer or quantizer

This is the most important pairing.

### What the second module should do
- Output **1V/oct pitch CV**
- Output corresponding **triggers/gates**

### Result
BIA becomes a playable mono synth voice.

### Best uses
- basslines
- riffs
- arps
- tuned percussion

Because BIA is trigger-based, the sequencer does not need to sustain notes traditionally; it just needs to trigger the internal envelope rhythmically.

---

## B. With an envelope or function generator

BIA already has an internal envelope, but external modulation makes it much more melodic and expressive.

### Patch external modulation to:
- **Morph**
- **Fold**
- **Spread**
- **Decay**
- **Attack**
- **Harm**

### Musical benefit
You can create:
- accent variation
- timbral phrasing
- note-to-note articulation changes
- evolving melodic loops

A slow envelope or random stepped CV to **Morph** or **Fold** is especially effective.

---

## C. With a filter

BIA does not need a filter to sound good, but a filter can make it sit more naturally in melodic roles.

### Why use one
- tame harsh highs from **Fold**
- shape bass emphasis
- animate leads with filter sweeps
- make metallic tones more tonal

### Strong use cases
- lowpass after **Metal** mode for aggressive but focused bass
- bandpass after **Skin** for vocal or nasal leads
- resonant lowpass after **Liquid** for punchy acid-adjacent lines

---

## D. With a VCA

Since BIA already contains its own envelope, a VCA is optional for basic use, but still useful.

### Why
- dynamic control from another envelope
- sidechain-style pumping
- amplitude automation independent of BIA’s internal contour
- ducking and mix placement

### Nice trick
Use **Env Out** to modulate another VCA or filter elsewhere in the patch while BIA plays melody.

---

## E. With effects

BIA becomes much more “synth-like” melodically when sent through effects.

### Best effect pairings
- **Delay**: for arps and lead echoes
- **Reverb**: for spacious melodic percussion and lead atmospheres
- **Chorus/ensemble**: for supersaw and widening
- **Distortion/saturation**: for industrial bass and lead
- **Phaser/flanger**: for animated metallic lines

---

## F. Using Env Out as a melodic patching tool

One of the biggest advantages of the Alia version over the original is **Env Out**.

The manual says it outputs an envelope mirroring BIA’s internal envelope, from **0 V to +5 V**.

### This lets BIA control other modules while playing melody
Examples:
- Open a filter on another oscillator in sync with BIA notes
- Modulate another VCA for layered synth attacks
- Trigger dynamic effect depth
- Animate wavefolder amount on another voice
- Create layered bass + click systems where BIA shapes another sound

### Very musical application
Use BIA as the main bassline, and route **Env Out** to:
- a filter cutoff on a second oscillator
- a VCA controlling sub bass
- effect send level for note-by-note dub-style echoes

This makes BIA not just a voice, but also a **performance modulation source**.

---

## Mode-specific melodic recommendations

## Skin
Best for:
- bass
- plucks
- supersaw-like textures
- synth stabs
- clearer melodic parts

Why:
- additive structure is more stable and tonal
- easier to tune musically
- better for conventional note sequences

## Liquid
Best for:
- punchy basslines
- acid-like stabs
- percussive melodic hooks
- tom-like tuned sequences

Why:
- built-in pitch envelope adds attack character
- great for lines that need movement and impact

## Metal
Best for:
- industrial melodies
- aggressive FM-ish bass
- bells and clangorous tuned sounds
- experimental lead work

Why:
- more inharmonic and complex
- phase modulation creates richer, noisier spectra

---

## Parameter strategies for melodic patching

## For clean tonal bass
- Mode: **Skin**
- Range: **Bass**
- Morph: lower to mid
- Harmonic: low to mid
- Spread: low
- Fold: low to moderate
- Attack: center
- Decay: medium

## For punchy techno bass
- Mode: **Liquid**
- Range: **Bass**
- Morph: mid
- Harmonic: low-mid
- Spread: low
- Fold: moderate
- Attack: center/right of center
- Decay: short-medium

## For bright lead
- Mode: **Skin**
- Range: **Alto/Treble**
- Morph: saw/square area
- Harmonic: medium-high
- Spread: medium
- Fold: moderate-high
- Decay: medium
- Add delay/reverb

## For metallic melody
- Mode: **Metal**
- Range: **Alto/Treble**
- Morph: experiment broadly
- Harmonic: medium
- Spread: medium-high
- Fold: low to moderate at first
- Decay: medium-long

## For tuned percussion line
- Mode: **Skin** or **Metal**
- Range: depends on register
- Decay: short
- Attack: center
- Harmonic: moderate
- Spread: adjust by ear for tonal center

---

## Important voltage and patching notes

From the manual:

- **Trig threshold**: around **+1.8 V**
- Modulation CV inputs: **0 V to +5 V**
- Pitch CV range: **-2 V to +5 V**
- **Env Out**: **0 V to +5 V**
- Audio output can reach about **14 Vpp**

This means:
- standard Eurorack sequencers and triggers should work fine
- attenuating modulation sources may help when patching into parameter CV inputs
- audio may be hot, so watch gain staging into external mixers, interfaces, or effects

---

## Best musical workflows

## 1. Single-voice melodic synth
- Sequencer pitch out → **Pitch**
- Gate/trigger out → **Trig**
- BIA **Out** → mixer/effects

Use for:
- mono bass
- lead
- stab line

## 2. Layered bass patch
- Same as above
- **Env Out** → filter cutoff or VCA on second oscillator/sub source

Use for:
- bass with synchronized transient shaping
- layered punch and sub

## 3. Melodic percussion engine
- Quantized random or sequenced CV → **Pitch**
- Rhythmic triggers → **Trig**
- Short decay
- Optional modulation to **Morph** or **Spread**

Use for:
- tuned toms
- bell patterns
- electro hits

## 4. Evolving lead
- Sequencer → **Pitch**
- Trigger pattern → **Trig**
- Slow LFO or envelope → **Morph**
- Random stepped CV → **Fold** or **Spread**
- Delay/reverb after output

Use for:
- animated melodies
- live performance variation
- generative hooks

---

## Overall takeaway

Basimilus Iteritas Alia is not limited to drums at all. Based on the manual, it is highly effective as a:

- **bass voice**
- **lead voice**
- **pitched percussion voice**
- **supersaw/unison-style synth**
- **metallic/FM-like melodic oscillator**
- **modulation source via Env Out**

Its strongest melodic advantage is that it combines:
- pitch tracking,
- rich multi-oscillator tone generation,
- internal transient/envelope behavior,
- aggressive timbral shaping,
- and patchable envelope output.

In a Eurorack system, that makes it excellent for **sequenced melodic lines with strong articulation**, especially in techno, industrial, electro, IDM, experimental, and hybrid drum/synth compositions.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)