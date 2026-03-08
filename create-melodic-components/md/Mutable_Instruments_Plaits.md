# Mutable Instruments — Plaits

- [Manual PDF](../../manuals/Mutable Instruments - Plaits.pdf)

---

[Mutable Instruments Plaits Manual (PDF/manual page)](https://pichenettes.github.io/mutable-instruments-documentation/modules/plaits/manual/)

# Using Plaits to Create Melodic Components

Plaits is a very flexible **macro-oscillator voice** for Eurorack, and based on this manual, it can serve as the core melodic sound source in several different ways: as a conventional pitched oscillator, a chord generator, a plucked/struck physical model, a wavetable lead, or even a speech-like melodic texture.

## What Plaits gives you musically

Plaits contains:

- **16 synthesis models**
- **1V/Oct pitch input**
- **internal LPG (low-pass gate)**
- **internal decay envelope triggered from TRIG**
- **main OUT plus AUX output**
- CV control over:
  - model
  - timbre
  - morph
  - harmonics
  - frequency / FM
  - level

That means it can function either as:

- a **complete melodic voice** with only pitch and trigger required, or
- a **deeply modulatable oscillator** inside a larger patch.

## Best melodic uses from the available models

For melody writing, the strongest Plaits models are:

### 1. Virtual analog model
Great for:

- basslines
- mono leads
- arpeggios
- classic subtractive-style sequences

Controls:
- **HARMONICS**: detune between the two waves
- **TIMBRE**: pulse shape / hardsync formants
- **MORPH**: saw/triangle/notch variation

How to use melodically:
- Send a sequencer or keyboard into **V/OCT**
- Send gates/triggers into **TRIG**
- Use the internal LPG for instant articulation
- Modulate **TIMBRE** or **MORPH** slowly for evolving lead lines

This is probably the easiest “traditional synth voice” inside the module.

---

### 2. Waveshaping / wavefolding model
Great for:

- expressive leads
- brighter melodic hooks
- animated basses

Controls:
- **HARMONICS**: waveshaper waveform
- **TIMBRE**: wavefolder amount
- **MORPH**: waveform asymmetry

How to use melodically:
- Patch pitch CV to **V/OCT**
- Trigger the internal envelope via **TRIG**
- Add slow CV to **TIMBRE** for movement across phrases
- Use **AUX** as an alternate folded tone for layering or parallel processing

This model works well when you want melodic material that feels more modern and harmonically rich.

---

### 3. FM model
Great for:

- glassy melodies
- electric piano-like lines
- metallic but playable leads
- complex bass tones

Controls:
- **HARMONICS**: frequency ratio
- **TIMBRE**: modulation index
- **MORPH**: feedback/chaos character

How to use melodically:
- Keep **MORPH** near noon for more stable pitched tones
- Sequence pitch via **V/OCT**
- Use light CV on **TIMBRE** to animate note brightness
- Use **AUX** sub output to reinforce the fundamental for bass melodies

This is one of the best models for melodic lines that need more harmonic complexity without losing pitch definition.

---

### 4. Additive model
Great for:

- organ-like leads
- hollow melodic lines
- soft harmonic pads when externally enveloped
- clear, trackable tonal material

Controls:
- **HARMONICS**: spectral bump count
- **TIMBRE**: center harmonic
- **MORPH**: bump shape

How to use melodically:
- This model responds very musically to subtle modulation
- Use it for tonal sequences where each note should remain clear
- The **AUX** output gives a Hammond-like subset of harmonics, useful for second-layer melody doubling

This is a good choice when you want melody without too much harshness.

---

### 5. Wavetable model
Great for:

- evolving leads
- digital arpeggios
- melodic ostinatos
- retro/futuristic tones

Controls:
- **HARMONICS**: bank selection
- **TIMBRE**: row
- **MORPH**: column

How to use melodically:
- Sequence notes into **V/OCT**
- Modulate **TIMBRE** and/or **MORPH** with slow LFOs, random, or envelope CV
- Use **AUX** low-fi output for a doubled or contrast voice

This model is especially useful when the melody should change tone over time without changing pitch.

---

### 6. Chord model
Excellent for melodic-harmonic writing.

Controls:
- **HARMONICS**: chord type
- **TIMBRE**: inversion/transposition
- **MORPH**: waveform selection
- **AUX**: root note

How to use musically:
- Send 1V/Oct to **V/OCT** to transpose the entire chord
- Trigger with **TRIG**
- Sequence chord changes as if Plaits were a harmonic voice
- Use **AUX** root output separately as:
  - a bassline source
  - pitch reference
  - doubled melody

This is one of the most powerful “melodic component” tools in the module because a single pitch CV line can become full harmonic movement.

---

### 7. Speech model
Useful for:

- vocal melody fragments
- robotic hooks
- spoken textures integrated into pitched music

Controls:
- **HARMONICS**: vowel/speech algorithm/word bank
- **TIMBRE**: species/formant shift
- **MORPH**: phoneme or word segment

Musical use:
- Sequence pitch melodically for “singing synth” effects
- Trigger words/segments with **TRIG**
- Use CV over **MORPH** to scan phonemes rhythmically
- Use FM attenuverter to affect intonation when triggered

This is less conventional, but very effective for melodic ear candy or top-line motifs.

---

### 8. Resonator / string models
Great for:

- plucked melodies
- mallet-like sequences
- pseudo-acoustic lines
- ambient melodic figures

Controls:
- **HARMONICS**: inharmonicity/material
- **TIMBRE**: excitation brightness
- **MORPH**: decay

How to use melodically:
- Send note CV to **V/OCT**
- Send gates/triggers to **TRIG**
- Let the internal exciter and decay shape each note
- Use **LEVEL** as accent input for more expressive phrasing when using triggered physical models

These models are especially strong for melodic sequences that need natural attack and resonant decay.

---

## Using the internal envelope and LPG for melodic patches

One of the most important melodic features in Plaits is that you do **not** always need an external envelope + VCA.

### With TRIG patched:
Plaits can:
- trigger its own decaying envelope
- strike its internal LPG
- excite physical/percussive models
- sample-and-hold model CV

This means a minimal melodic patch can be:

- sequencer pitch CV → **V/OCT**
- sequencer gate/trigger → **TRIG**
- audio out → mixer

That alone creates a playable melodic voice.

### Why this matters
For melodic composition, this makes Plaits ideal for:

- compact live systems
- generative patches
- quick sketching of riffs and motifs
- multi-voice systems where you want to conserve VCAs/envelopes

## Important note about the attenuverters

The manual notes that when a corresponding CV input is **unpatched** and **TRIG is patched**, the attenuverters for **TIMBRE**, **FM**, and **MORPH** control the amount of internal envelope modulation.

This is extremely useful for melody because it gives you note-by-note timbral articulation without extra patching.

For example:
- internal envelope to **TIMBRE** = brighter attack on each note
- internal envelope to **MORPH** = shape changes per note
- internal envelope to **FM** = pitch sweep or transient movement

This is a major feature for expressive melodic phrasing.

## Simple melodic patch ideas

## 1. Classic mono lead
Use:
- virtual analog, waveshaping, or FM model

Patch:
- pitch sequencer → **V/OCT**
- gate/trigger sequencer → **TRIG**
- **OUT** → mixer/filter/effects

Technique:
- use internal LPG
- set moderate decay
- assign internal envelope to **TIMBRE** with attenuverter for dynamic attack brightness

Result:
- expressive lead line with minimal patching

---

## 2. Plucked melody
Use:
- string/resonator model

Patch:
- sequencer → **V/OCT**
- triggers → **TRIG**
- OUT → reverb/delay

Technique:
- short to medium decay
- increase excitation brightness with **TIMBRE**
- use **LEVEL** CV for accents on selected notes

Result:
- melodic plucks, kalimba-like lines, or modal sequences

---

## 3. Chord progression plus bassline from one module
Use:
- chord model

Patch:
- sequence → **V/OCT**
- gates → **TRIG**
- **OUT** → main mixer voice
- **AUX** → separate bass processing chain

Technique:
- OUT carries full chord sound
- AUX gives root note, which can become a bass component
- tune waveform with **MORPH**
- animate inversion using **TIMBRE**

Result:
- harmonic and melodic content from one module

---

## 4. Evolving arpeggio voice
Use:
- wavetable or additive model

Patch:
- arpeggiator/sequencer → **V/OCT**
- triggers → **TRIG**
- slow LFO/random → **TIMBRE** or **MORPH**

Technique:
- keep pitch sequence simple
- let timbre modulation create variation
- use AUX as contrasting secondary texture

Result:
- melodic line that evolves without becoming harmonically unclear

---

## 5. Expressive bass melody
Use:
- FM or virtual analog model

Patch:
- bass sequencer → **V/OCT**
- gate → **TRIG**
- **AUX** sub or alternate output mixed with main out

Technique:
- use AUX sub to support low end
- keep LPG response tighter and more VCA-like if you want punch
- shorter decay for rhythmic articulation

Result:
- bassline with both definition and body

---

## 6. Vocal top-line
Use:
- speech model

Patch:
- melodic CV → **V/OCT**
- trigger sequence → **TRIG**
- slow/stepped CV → **MORPH**

Technique:
- scan phonemes or words while notes change
- use reverb or delay after the module
- automate **TIMBRE** for different “vocal characters”

Result:
- unusual melodic hooks and vocal-style motifs

## Using OUT and AUX together for melody

A big compositional strength of Plaits is the relationship between **OUT** and **AUX**.

Depending on the model, AUX may be:
- a sub oscillator
- another timbral variant
- a low-fi version
- a raw exciter
- a root note
- filtered/noisy complement

This allows several melodic strategies:

### Layered melody
Mix OUT and AUX together for a fuller lead.

### Split roles
Send:
- **OUT** to main melodic chain
- **AUX** to another filter/VCA/effect path

### Bass + melody
On the chord or FM models, AUX can support the root or sub while OUT carries the more complex upper content.

### Parallel processing
Use different effects on OUT and AUX:
- dry OUT + wet AUX
- distorted AUX + clean OUT
- mono center OUT + stereo FX AUX

## Settings that matter for melodic use

## 1. FREQUENCY knob range
You can narrow the coarse tuning range to **14 semitones around a fixed octave** instead of the full 8-octave span.

This is very helpful for melodic work because:
- fine tuning is easier
- live pitch adjustment is safer
- it behaves more like a conventional oscillator tuning control

To do this:
- hold the **second model button**
- turn **HARMONICS** to select the range

For melodic systems, this is one of the first settings worth changing.

## 2. LPG response
You can adjust the internal low-pass gate from:
- **VCFA-like** response to
- **VCA-like** response

For melody:
- more **VCFA** = plucky, organic, darker tail
- more **VCA** = more neutral, direct articulation

If you want clean sequenced melodies, move it more toward VCA.
If you want West Coast plucks or softer note edges, stay more toward VCFA.

## 3. Decay / ringing time
Adjustable with the button + **MORPH** combo.

For melody:
- short decay = basslines, staccato sequences, arps
- medium decay = leads, plucks
- long decay = ambient lines, overlapping phrases

## Melodic role by synthesis family

### Best for stable tonal melodies
- virtual analog
- additive
- wavetable
- chord

### Best for animated expressive leads
- waveshaping
- FM
- formant synthesis
- speech

### Best for plucks and struck melodic material
- string/resonator
- physical/percussive models used tonally

### Best for bass melodies
- virtual analog
- FM
- chord model with AUX root
- filtered noise model if tuned carefully for synth bass textures

## Performance ideas

## 1. Model switching per phrase
The model CV input can be modulated, and if TRIG is patched, model changes happen only when a trigger is received. That means you can switch synthesis model on note boundaries.

Musically, this allows:
- verse lead on one model, chorus lead on another
- alternating timbres every step
- controlled phrase-by-phrase variation

Because model changes can be sampled on triggers, it can stay rhythmically coherent.

## 2. Accent-based phrasing
For physical/percussive models, **LEVEL** acts as an accent control when TRIG is patched.

This is great for:
- melodic percussion
- expressive plucked sequences
- more human phrasing in repeating melodic patterns

## 3. Internal envelope as timbral articulation
Instead of only opening amplitude, use the unpatched CV attenuverters to route the internal envelope to timbre-related parameters.

This gives each note:
- a brighter start
- a pitch transient
- a shape sweep

That makes simple sequences sound much more musical.

## Practical melodic patch recipes

## Recipe A: Minimal lead voice
- V/OCT from sequencer
- TRIG from gate sequencer
- OUT to mixer
- model: virtual analog or waveshaper
- short-medium decay
- envelope to TIMBRE via attenuverter

Use when you want: fast patching, clear melody

## Recipe B: Ambient pluck line
- V/OCT from sequencer or quantized random
- TRIG from clock divider or sparse gates
- model: resonator/string
- OUT to reverb
- AUX to separate shimmer/delay path

Use when you want: sparse melodic ambience

## Recipe C: Harmonic melody engine
- V/OCT from sequencer
- model: chord
- OUT for chordal body
- AUX for bass root
- TRIG for articulation

Use when you want: instant musical structure from one voice

## Recipe D: Digital arp
- fast sequence into V/OCT
- wavetable model
- slow LFO into MORPH
- random stepped CV into TIMBRE
- TRIG every note

Use when you want: animated, modern melodic motion

## Recipe E: Metallic tuned melody
- FM model
- tuned V/OCT sequence
- low to moderate modulation index
- MORPH near noon
- AUX mixed in lightly

Use when you want: bellish or electric melodic hooks

## Bottom line

Plaits is exceptionally strong for melodic duties because it combines:

- a wide range of **pitched synthesis models**
- proper **1V/Oct tracking**
- built-in **triggered articulation**
- internal **LPG + envelope**
- dual outputs for **layering or split roles**
- enough timbral modulation to make even simple note sequences sound expressive

In practice, Plaits can cover:

- basslines
- leads
- arpeggios
- chord progressions
- plucked lines
- tuned percussion
- vocal-like melodies
- layered harmonic/melodic textures

If you are building melodic patches, the most immediately useful models are:
- **virtual analog**
- **FM**
- **wavetable**
- **additive**
- **chord**
- **resonator/string**

And the single most important trick from the manual is this:

> With **TRIG** patched and the timbre CV inputs left unpatched, the attenuverters can apply the **internal envelope** to timbre parameters, giving every note built-in melodic expression.

That makes Plaits not just a sound source, but a very complete melodic voice.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)