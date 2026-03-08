# Intellijel — Plonk

- [Manual PDF](../../manuals/plonk_manual_v1.16_2020.11.08.pdf)

---

# [Intellijel Plonk Manual (English, Firmware 1.16)](https://intellijel.com/downloads/manuals/Plonk_Manual_1.16_2020.11.08.pdf)

## Using Plonk to create melodic components in a Eurorack system

Plonk is primarily presented as a **physical-modeling percussion synthesizer**, but the manual makes it clear that it can also do **pitched percussion, string-like tones, basses, guitar-like sounds, marimba/vibes, and other tonal material**. That makes it very usable for melodic roles, not just drums.

Because only one module manual is attached here, I’ll analyze **how Plonk itself can function as a melodic voice**, and how its inputs/modulation architecture let it interact with the rest of a Eurorack system to produce musical lines, tuned parts, and expressive melodic gestures.

---

## 1. Why Plonk works well for melody

Plonk has several features that make it more than a drum module:

- **1V/oct PITCH input**
- **Base pitch control** with octave and optional quantization
- **Resonator models** that include:
  - String
  - Beam
  - Marimba
  - Drumhead
  - Membrane
  - Plate
- **Internal pitch envelope** for attack transients or pitch sweeps
- **2-voice polyphony**
- **Velocity input**
- **Assignable X, Y, and MOD modulation destinations**
- **Preset storage and preset stepping/morphing**

That means Plonk can act like:

- a tuned mallet instrument
- a plucked string synth
- a metallic bell/chime voice
- a bass voice
- a semi-polyphonic melodic percussion voice
- a morphing “kit-to-melody” voice

---

## 2. Core patch for melody

### Basic melodic patch
Use Plonk like a standard tonal voice:

- Sequencer **pitch CV** → **PITCH**
- Sequencer **gate** → **TRIG**
- Optional accent/velocity CV → **VEL**
- **OUT** → mixer / VCA / effects / output

### Good starting settings
From the manual and from practical use:

- Set **PITCH knob** around noon
- Set a suitable **Octave** in the PITCH menu
- Turn **Quantize** on if you want semitone stepping from the front-panel pitch knob
- Set **DECAY** fairly high for sustained melodic notes
- Choose a resonator better suited to pitch:
  - **String** for plucks/bass/guitar-like sounds
  - **Marimba** for tonal percussion
  - **Beam** for bells and woody struck tones
  - **Plate** for metallic melodic material

---

## 3. Best resonator types for melodic use

## String
Best for:
- plucked melodies
- basslines
- pseudo-guitar parts
- bowed/sustained textures when using noise exciter creatively

How to use it:
- Use more **mallet** than noise for a plucked attack
- Adjust **Resonator Position** to shape harmonic content
- Use **Resonator Tone** to shift material feel from softer to brighter
- Try moderate **Resonator Decay** for plucks, longer for sustained tones
- Add a little **Pitch Envelope Amount** for a natural pluck transient

Musically:
- Great for arpeggios
- Works very well for modal or minimalist melodic lines
- Can become a bass voice with shorter decay and lower octave

---

## Marimba
Best for:
- mallet melodies
- ostinatos
- tuned percussion patterns
- marimba/vibraphone-like phrases

How to use it:
- Blend **mallet** and **noise** depending on how much attack detail you want
- Use **Mallet Stiffness** to sharpen or soften articulation
- Keep **Inharmonicity** moderate for more recognizably pitched notes
- Use longer **Resonator Decay** for vibes-like ringing

Musically:
- Excellent for repeating melodic figures
- Great with probability-based triggers or polyrhythmic sequencers
- Very strong for West African / minimal / gamelan-inspired melodic percussion

---

## Beam
Best for:
- bells
- claves/chimes
- tuned wood/metal struck melodies

How to use it:
- Use stiffer mallet settings
- Higher tone values often produce more metallic/glassy material feel
- Slight inharmonicity gives lovely bell-like complexity
- Moderate decay helps preserve pitch clarity

Musically:
- Strong for sparse melodic punctuation
- Great for upper-register motifs
- Useful in ambient and generative patches

---

## Plate
Best for:
- metallic tuned sounds
- gong-like pitches
- shimmering upper-register melodic parts

How to use it:
- Plate can get very inharmonic fast, so for stronger pitch identity keep modulation restrained
- Use **Low Cut** to clear mud and emphasize upper partials
- Works well with long decays and external reverb

Musically:
- Excellent for evolving melodic layers
- More about color and atmosphere than strict tonal precision

---

## Drumhead / Membrane
These are less obvious for melody, but still useful.

Best for:
- tom-like tuned lines
- electronic tuned percussion
- hybrid melodic-drum sequences

Musically:
- Great if you want melody that still feels percussive and rhythmic
- Particularly useful in techno, IDM, electro, and experimental music

---

## 4. Exciter design for melodic articulation

Plonk’s melody isn’t only about pitch; it’s also about **how notes speak**.

## Mallet exciter
Use for:
- clean attacks
- plucked and struck notes
- more traditional melodic articulation

### Mallet Stiffness
- Higher stiffness = sharper transient, more click/definition
- Lower stiffness = rounder attack

For melody:
- Use **lower to medium stiffness** for warm marimba/plucked tones
- Use **higher stiffness** for bells, claves, or articulate sequenced lines

---

## Noise exciter
Use for:
- breathiness
- scrape/bow textures
- snare-like articulation
- noisy attack emphasis

Key parameters:
- **Noise Attack**
- **Noise Decay**
- **Noise Density**
- **Noise LP/HP filters**
- **Noise Envelope Type**

For melodic use:
- Short filtered noise adds realism to attacks
- Medium density plus envelope shaping can suggest bowing or friction
- AHR mode can make longer, sustained articulated tones

### Nice trick
For expressive melodic lines:
- Use a little noise mixed with mallet
- Route velocity to excite the note more dynamically
- This makes notes feel more like performance gestures than static synth tones

---

## 5. Pitch behavior and tuning

## PITCH input
Plonk accepts **1 V/oct** at the **PITCH** input. This is the main path for melodic sequencing.

Important note from the manual:
- Pitch is updated **only while the TRIG input is high**
- If you want true audio-rate or continuous pitch modulation, use **X, Y, or MOD assigned to R Pitch**

This matters a lot musically:

### For normal sequenced melodies
- Use standard gate + pitch sequencing into TRIG and PITCH

### For vibrato / pitch bends / FM-like movement
- Assign **R Pitch** to **MOD** (or X/Y if available in your workflow)
- Then patch:
  - LFO for vibrato
  - envelope for pitch bend
  - random CV for unstable acoustic behavior
  - oscillator for FM-like clangorous tones

This is one of the most important “melodic unlocks” in the module.

---

## 6. Velocity makes melodies expressive

The **VEL** input can operate in three modes:

- **accent**
- **dynamics**
- **volume**

## Best options for melodic work

### Dynamics mode
This is the most performance-oriented melodic setting.

It makes the **strength of the exciter proportional to input voltage**. That means:
- harder notes feel brighter/more forceful
- softer notes feel gentler
- repeated notes become expressive

Use this with:
- MIDI-to-CV velocity output
- sequencer accent lane
- manually programmed CV contour

### Volume mode
Useful when you want:
- tremolo
- amplitude contouring
- fade-ins/outs
- more conventional amplitude phrasing

### Accent mode
Simple and effective for:
- alternating strong/weak notes
- rhythmic emphasis in melodic percussion lines

---

## 7. X and Y controls are extremely useful for melodic macros

Plonk lets you assign **X** and **Y** to a large range of exciter/object parameters. These act as macro controls and can also receive CV.

This is ideal for melody because you can tie expressive changes to performance movement.

## Strong melodic destinations for X/Y

### R Tone
Great for opening/closing timbral brightness across a melody.

### R Position
Changes where the resonator is “struck,” altering partial balance.
This can make a repeating melody feel alive.

### Mallet:Noise
Morphs between plucked/struck and noisy/frictional articulations.

### M Stiffness
Adds articulation variation across notes.

### R Inharmonic
Very useful for moving between:
- clear pitch
- bell-like complexity
- abstract metallicity

### R PEnv Amt
Controls how much pitch attack transient happens.
Excellent for expressive plucks and kicks-to-bass hybrids.

### Saturation / Bitcrusher
Useful if you want melodic lines to move from clean to aggressive.

---

## 8. MOD input opens advanced melodic behavior

The **MOD** input is especially powerful because it can do more than simple parameter modulation.

## A. Use MOD for R Pitch
One of the best melodic setups:
- Assign MOD destination to **R Pitch**
- Send an LFO or envelope into MOD

This creates:
- vibrato
- pitch bends
- expressive attacks
- pseudo-FM tones
- unstable acoustic drift

For melodic realism, subtle modulation here is gold.

---

## B. Preset Step for melodic kits and multisamples-in-spirit
**Preset Step** lets Plonk switch presets based on incoming CV at MOD whenever a trigger is received.

This means one pitch/gate sequence can produce:
- different resonator/exciter structures per note
- alternating melodic timbres
- pseudo-multisampled tonal sets
- melodic “kits” where different notes in a line have different instrument identities

For example:
- preset 20 = woody marimba
- preset 21 = metallic bell
- preset 22 = muted string
- preset 23 = noisy attack pluck

Then use CV into MOD to select among them before each note.

Musically, this is amazing for:
- call-and-response within one melodic sequence
- phrase-based variation
- different timbres across scale degrees
- generative melodic orchestration

---

## C. Morph between presets
This is one of Plonk’s best features for melody.

When MOD is set to **Morph**, incoming CV blends between:
- the current preset
- another destination preset

This does **not** morph resonator type, but it **does** morph the other exciter and object parameters.

This is ideal for:
- evolving melodic phrases
- changing a motif from muted to bright
- moving from mallet to noisy articulation
- slowly transforming a bassline into a bell sequence

Patch ideas:
- slow triangle LFO into MOD for cyclical timbral movement
- envelope into MOD for note-dependent timbre shaping
- random stepped CV into MOD for per-note changes
- pressure/manual controller into MOD for expressive live performance

---

## D. Randomize
Randomize is more experimental, but still melodic if used carefully.

A trigger at MOD with destination set to **Randomize** randomizes most exciter/object parameters.

Use with caution for melody:
- can create fresh timbres
- may reduce pitch clarity depending on resulting resonator settings

Best use:
- randomize until you find a compelling tonal voice
- save it as a preset
- build a melodic bank from curated random discoveries

---

## 9. 2-voice polyphony helps melodic phrasing

Plonk is **duophonic**.

That means:
- one note can ring while another begins
- melodic phrases can overlap
- long decays don’t always get cut off by the next note

This is especially useful for:
- marimba rolls
- bell/chime melodies
- legato-ish plucked lines
- ambient melodic ostinatos

## Polyphony setting
- **1 voice**: new note chokes previous note
- **2 voices**: previous note continues ringing

For melodic applications:

### Use 1 voice when:
- you want clean basslines
- you want tight mono articulation
- you want old notes cut off like a synth voice

### Use 2 voices when:
- you want natural resonance overlap
- you want idiomatic percussion melodies
- you want richer ambient/tuned percussion textures

---

## 10. Presets as melodic instruments, not fixed sounds

The manual emphasizes that Plonk presets behave differently from standard synth patches because the **panel knobs remain live**.

This is very important musically.

A preset on Plonk is better thought of as:
- an **instrument model**
- a performance-ready timbral state
- a family of sounds rather than one exact sound

For melody, this is a strength.

You can load a melodic preset, then perform with:
- **DECAY** for phrase length
- **X/Y** for articulation and timbre
- **VEL** for dynamics
- **MOD** for morphing or pitch behavior

So one preset can cover:
- muted notes
- accented notes
- bright notes
- sustained notes
- unstable/animated notes

That makes Plonk unusually expressive for melodic composition.

---

## 11. Good melodic patch recipes

## A. Marimba lead
- Resonator: **Marimba**
- Mix: mostly **Mallet**
- Mallet Stiffness: medium
- Resonator Decay: medium-long
- R Tone: medium-high
- Polyphony: 2
- VEL Mode: **dynamics**

Patch:
- Sequencer pitch → PITCH
- Gate → TRIG
- Accent/velocity CV → VEL
- Slow LFO → X assigned to R Tone

Result:
- expressive tuned percussion melody
- subtle tone drift over time

---

## B. Plucked bass
- Resonator: **String**
- Mix: mostly mallet
- Resonator Decay: short-medium
- Resonator Position: off-center
- Pitch Env Amount: slight positive
- Pitch Env Decay: short
- Polyphony: 1

Patch:
- Bass sequencer CV → PITCH
- Gate → TRIG
- Envelope or accent lane → VEL
- MOD assigned to R Pitch with tiny envelope modulation for bite

Result:
- physical-modeled bass pluck
- very musical in minimal techno, electro, downtempo

---

## C. Bell sequence
- Resonator: **Beam** or **Plate**
- Mix: stiff mallet with a little noise
- R Tone: high
- Inharmonicity: slight positive
- Decay: long
- Polyphony: 2

Patch:
- Sequencer → pitch and trig
- Random stepped CV → X assigned to R Position
- Slow LFO → Y assigned to R Tone

Result:
- evolving tuned bell melody
- ideal for ambient / generative music

---

## D. Hybrid melodic drumline
- Resonator: **Drumhead** or **Membrane**
- Tune to a scale via PITCH input
- Decay: medium
- Noise mixed in moderately
- Velocity active

Patch:
- Melodic sequencer → PITCH/TRIG
- Accent lane → VEL
- MOD set to Preset Step across a few tuned percussive presets

Result:
- line blurs between melody and rhythm
- especially good for IDM, tribal, experimental techno

---

## E. Morphing lead voice
- Create preset A: muted woody pluck
- Create preset B: bright metallic pluck
- MOD destination: **Morph**
- Choose preset B as morph target
- Slow or performance CV → MOD

Result:
- one sequence evolves through a phrase
- highly expressive for live sets

---

## 12. Practical sequencing advice

## Gate timing
The manual notes:
- gate must be at least **1 ms**
- pitch is sampled while **TRIG is high**
- if your sequencer sends gate before pitch has stabilized, use **Gate Delay** in Global Config

For melodic accuracy:
- keep Gate Delay low by default
- raise it only if notes are coming out wrong in pitch

This is especially relevant with quirky analog sequencers or some MIDI-CV interfaces.

---

## Quantization strategy
Plonk’s internal quantize affects the **PITCH knob**, not external pitch CV in the same way a dedicated quantizer module would.

For melodies:
- use an external quantized sequencer or quantizer if you need strict scales
- use Plonk’s pitch menu mainly to set **base octave** and knob behavior

---

## 13. Sound design advice for clearer melodic pitch

Physical modeling can become very complex. If you want a melodic part to read clearly in a mix:

- prefer **String**, **Marimba**, or **Beam**
- keep **Inharmonicity** moderate
- don’t overdo noise mix
- use **Low Cut** if the sound is muddy
- adjust **Resonator Position** to emphasize useful partials
- use moderate decay for fast passages
- shorten pitch envelope decay if attacks feel too bent or kick-like
- avoid extreme bitcrushing if pitch clarity matters

If you want more abstract melodic color:
- increase inharmonicity
- use Plate
- add noise
- modulate R Tone and Position
- use Morph between contrasting presets

---

## 14. Best roles Plonk can play in melodic music

Plonk can serve as:

### Primary melodic voice
For:
- marimba lines
- plucked leads
- bell melodies
- physical-model bass

### Secondary countermelody
Its percussive onset helps it cut through mixes without occupying huge sustained harmonic space.

### Tuned percussion layer
Excellent for doubling melodic lines with rhythmic identity.

### Generative melodic texture
With polyphony, morphing, preset stepping, and modulation, Plonk excels at semi-autonomous melodic movement.

### Bass/percussion hybrid
One of the most interesting uses:
- tune it melodically
- keep it punchy
- let it function as both rhythmic and tonal foundation

---

## 15. Bottom line

Plonk is not just a drum module. It’s a **highly expressive physical-modeling melodic voice** disguised as percussion.

Its strongest melodic advantages are:

- proper **1V/oct tracking**
- **pitched resonator models**
- **velocity response**
- **macro modulation via X/Y**
- **R Pitch modulation for vibrato and bends**
- **2-voice polyphony**
- **preset morphing and stepping** for phrase-level timbral movement

If you build patches around **String, Marimba, Beam, and Plate**, and treat exciter design as articulation rather than just “drum attack,” Plonk becomes a very musical source for:

- basslines
- mallet melodies
- bells/chimes
- plucks
- hybrid acoustic/electronic lead voices
- evolving generative melodic parts

---

## Suggested “together” use in a larger Eurorack patch

Even though only Plonk is included here, in a broader Eurorack system it pairs especially well with:

- **pitch sequencers** for melodic CV
- **quantizers** for tonal control
- **clocked modulation** for timbral motion
- **MIDI-CV interfaces** with velocity output
- **function generators / envelopes** into MOD or X/Y
- **LFOs** for vibrato and morphing
- **random stepped CV** for preset selection or articulation changes
- **reverb/delay** for bell and plate-based melodic textures
- **mixers/VCAs** for final phrasing and layering

If you want, I can also turn this into:
1. a **set of specific melodic patch recipes**,  
2. a **genre-based guide** (techno, ambient, IDM, house, electro), or  
3. a **parameter cheat sheet for tuning Plonk into bass, mallet, bell, and lead roles**.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)