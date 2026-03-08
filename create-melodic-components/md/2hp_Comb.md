# 2hp — Comb

- [Manual PDF](../../manuals/Comb_Manual.pdf)

---

[Manual PDF](attachment)

# Using the Comb module to create melodic material

Based on the manual, this is a **2hp Comb** module: an **IIR peaking comb filter** with:

- **Audio input / output**
- **FREQ** control and CV
- **RES** control and CV
- **DAMP** control and CV
- Ability to go into **self-oscillation**
- A **dampening filter in the feedback path**

That means it can work not just as a tone-shaping effect, but as a **pitched resonator**, a **self-oscillating voice**, or a **melodic exciter/filter** when paired with other Eurorack modules.

---

## What the module does musically

A comb filter imposes a series of harmonic peaks onto incoming audio using a very short delay line. In practice, this gives you a few musically useful behaviors:

1. **Resonant pitch emphasis**
   - The **FREQ** control sets the comb’s cutoff, which the manual describes as **inversely proportional to delay time**.
   - Example from the manual: **500 Hz = 2 ms delay**.
   - As you tune FREQ, the harmonic spacing changes, often producing a perceived pitch.

2. **Feedback-based ringing**
   - **RES** increases feedback in the delay line.
   - At high settings, the module can **self-oscillate**, meaning it can generate a tone on its own or sustain resonant tones from tiny transients.

3. **Brightness and decay shaping**
   - **DAMP** controls a **1-pole filter in the feedback path**.
   - More dampening = darker, more muted resonance.
   - Less dampening = brighter, more extended upper harmonics.

So in a patch, Comb is ideal for turning:
- clicks into notes,
- noise into strings,
- simple oscillators into tuned harmonic material,
- modulation into animated melodic textures.

---

## Important module details from the manual

### I/O and CV
- **IN**: audio input, **10 Vpp**
- **OUT**: audio output, **10 Vpp**
- **FREQ CV**: ±5 V
- **RES CV**: ±5 V
- **DAMP CV**: ±5 V

### Controls
- **FREQ**
  - Sets cutoff frequency / comb tuning
  - Lower delay time = higher frequency
- **RES**
  - Sets feedback amount
  - Controls strength of resonant peaks
- **DAMP**
  - Controls cutoff of the filter in the feedback path
  - Left = darker / more damped
  - Right = brighter / less damped

---

# How to use it for melodic components

## 1. Turn impulses into pitched notes

This is the most direct “melodic” use of a comb filter.

### Patch idea
- Send a **triggered click**, short envelope pop, or sharp transient into **IN**
- Raise **RES** until the comb rings audibly
- Tune **FREQ** to the desired pitch area
- Adjust **DAMP** to shape how bright or natural the ring sounds

### Result
Each transient excites the filter like striking a string or resonant body. This creates:
- plucked tones
- tuned percussion
- pseudo-karplus voices
- melodic pings

### Best companion modules
Use with:
- trigger source / sequencer
- envelope with very short attack/decay
- VCA or transient generator
- noise source for more “string” texture

### Musical use
Sequence the transient source rhythmically, and use CV into **FREQ** to change the note for each step. This gives you a playable resonator voice.

---

## 2. Use self-oscillation as a sine-like melodic voice

Since the manual states the module is **capable of self oscillation**, you can use it as a sound source.

### Patch idea
- Leave **IN** unpatched or feed a tiny amount of noise/transient
- Increase **RES** until the module begins to ring or self-oscillate
- Tune **FREQ** by ear
- Use **FREQ CV** from a sequencer or quantizer

### Result
You can get a pitched tone that behaves like a resonant oscillator. Depending on settings, it may be:
- sine-like
- hollow
- metallic
- unstable in a musically interesting way

### Melodic role
This works well for:
- lead lines
- drones with pitch motion
- ghost melodies
- tuned feedback voices

### Tip
Because comb filters are not always calibrated for precise **1V/oct** tracking, treat this as an **experimental pitched voice** unless you confirm stable scaling in your system. A quantizer before the CV input can still help create musical intervals.

---

## 3. Karplus-Strong style plucked string patches

The manual specifically hints at “lustrous string sounds from white noise,” which is exactly where a comb filter shines.

### Patch idea
- Patch **white noise** or a very short burst of noise into **IN**
- Trigger the noise with a VCA or low-pass gate
- Set **RES** fairly high
- Tune **FREQ** to the perceived note
- Use **DAMP** to control how bright or muted the string feels

### Result
You get a synthetic plucked-string or harp-like voice.

### How to make it melodic
- Send sequenced CV into **FREQ CV**
- Trigger one short burst per note
- Use different DAMP values per phrase for articulation

### Performance angle
- Lower **DAMP** (more dark) = muted plucks
- Higher **DAMP** (brighter) = sharper, more metallic strings
- Modulating **DAMP** per note gives a very expressive melodic line

---

## 4. Process an oscillator into harmonically animated melodies

Comb can also reshape an already-pitched oscillator into something more complex.

### Patch idea
- Patch a VCO waveform into **IN**
- Sequence the VCO normally for pitch
- Use Comb after the oscillator
- Sweep or sequence **FREQ** independently
- Add modulation to **RES** or **DAMP**

### Result
This creates:
- phaser-like thickening at subtle settings
- tuned harmonic reinforcement
- metallic doubling
- shifting overtone emphasis

### Why this is useful melodically
The base oscillator carries the note, while Comb adds a second layer of pitch-related coloration. This can make simple sequences feel:
- more animated
- more acoustic
- more vocal
- more “played”

### Strong use cases
- basslines needing edge
- leads needing shimmer
- arpeggios with moving overtones
- drones that bloom into chords of harmonics

---

## 5. Create melodic percussion

Comb is excellent for tuned percussion because it naturally rings at a frequency related to the delay time.

### Patch idea
- Feed short triggers, clicks, or filtered noise into **IN**
- Moderate to high **RES**
- Tune **FREQ** to notes in a scale
- Keep **DAMP** lower for wood-like sounds or higher for metallic sounds

### Result
You can create:
- tuned toms
- claves
- mallet tones
- synthetic marimba / string-hit timbres

### Musical benefit
This is especially useful if you want a rhythm track that also contributes pitch content.

---

## 6. Use CV modulation to animate melodies

The module has CV over all three important parameters, which makes it much more than a static filter.

## FREQ CV for melodic motion
Patch:
- sequencer CV
- quantized random
- sample & hold
- slow envelope
- keyboard CV

Use it for:
- changing notes
- glides and bends
- subtle detuning around a fixed center
- pseudo-arpeggiation

## RES CV for articulation
Patch envelopes or velocity-like CV into **RES CV**.

Use it for:
- stronger resonance on accented notes
- notes that bloom into feedback
- dynamic contrast between dry and singing tones

## DAMP CV for timbral phrasing
Patch an envelope, LFO, or sequencer lane into **DAMP CV**.

Use it for:
- brighter attacks, darker tails
- alternating muted/open notes
- evolving harmonics over a phrase

This is especially effective for making repeating sequences feel alive.

---

# Practical melodic patch recipes

## Patch 1: Plucked string sequencer
**Goal:** melodic plucks

**Patch**
- Noise source → VCA → **Comb IN**
- Trigger sequencer → envelope → VCA CV
- Pitch CV sequencer → **FREQ CV**
- **Comb OUT** → mixer / VCA / effect

**Settings**
- **RES**: high but below runaway oscillation
- **DAMP**: middle to high
- **FREQ**: set to a useful note range

**Sound**
- Harp-like
- Koto-like
- Synthetic string plucks

---

## Patch 2: Self-oscillating lead
**Goal:** use Comb as a voice

**Patch**
- Minimal excitation or none at input
- Raise **RES** until self-oscillation starts
- Sequencer / quantizer CV → **FREQ CV**
- Optional envelope or VCA after output

**Settings**
- **RES**: very high
- **DAMP**: to taste
- **FREQ**: tuned by ear

**Sound**
- Hollow sine-ish lead
- Fragile resonant melody
- Feedback flute / wire tone

---

## Patch 3: Tuned percussion line
**Goal:** rhythm and melody at once

**Patch**
- Trigger pulse or click source → **IN**
- Sequencer CV → **FREQ CV**
- Accent envelope → **RES CV**
- Output → reverb

**Settings**
- **RES**: medium-high
- **DAMP**: lower for darker percussion, higher for metallic ringing

**Sound**
- Tuned pings
- Bellish percussion
- Resonant hits that imply a melody

---

## Patch 4: Harmonic enhancer for a bassline
**Goal:** enrich a simple mono sequence

**Patch**
- VCO → **Comb IN**
- Pitch sequencer → VCO
- Slow LFO or secondary sequencer → **FREQ CV**
- Envelope or accent CV → **DAMP CV**

**Settings**
- **RES**: low to medium for subtlety
- **DAMP**: medium
- **FREQ**: tuned to support the bass register

**Sound**
- Thicker bass
- Moving harmonics
- Phaser/physical resonance hybrid

---

## Patch 5: Noise-to-melody texture
**Goal:** convert noise into playable pitched texture

**Patch**
- White noise → **IN**
- Quantized CV → **FREQ CV**
- Slow modulation → **DAMP CV**
- Gate-controlled VCA before or after Comb

**Settings**
- **RES**: high
- **DAMP**: experiment from dark to bright

**Sound**
- Bowed/string-cloud textures
- Shimmering melodic beds
- Atmospheric tonal textures

---

# How it fits in a larger melodic Eurorack system

Comb works especially well in these roles:

## As a voice
If pushed into self-oscillation or excited by transients, it can become:
- a lead
- a pluck voice
- a tuned drone

## As a resonator
Placed after:
- noise
- impulses
- short envelopes
- percussive clicks

…it becomes a melodic resonant body.

## As a harmonic processor
Placed after an oscillator, sampler, or drum voice, it adds:
- pitch-focused coloration
- ringing overtone structures
- animated resonance

---

# Strengths for melody

From the manual, the most important melodic strengths are:

- **Self oscillation** means it can generate tones
- **FREQ CV** means you can sequence or modulate its pitch center
- **RES CV** means you can shape note intensity and sustain
- **DAMP CV** means you can articulate timbre over time
- **Feedback path filtering** makes it more expressive and acoustic-feeling than a plain static comb

---

# Limitations and expectations

A few practical points:

- The manual does **not** specify precision pitch tracking, so don’t assume perfect oscillator behavior.
- It may work best for:
  - tuned-by-ear melodic lines
  - quantized approximate pitches
  - resonant/acoustic melodic parts
  - experimental tonal textures
- For very controlled tonal music, pair it with:
  - a quantizer
  - attenuator/offset on pitch CV
  - stable transient source
  - VCA for note articulation

---

# Best “used together” scenarios

Since only one module manual is attached here, I can only analyze **Comb** directly. But in a typical melodic Eurorack setup, this module works especially well together with:

- **Sequencer** → for pitch changes into FREQ CV
- **Quantizer** → to constrain comb tuning to scales
- **Noise source** → to excite string-like resonances
- **Trigger / gate source** → to create note events
- **Envelope + VCA** → to shape excitation and output dynamics
- **LFO / random CV** → for evolving harmonic movement
- **Reverb / delay** → to turn resonant plucks into lush melodic atmospheres

If you upload the other module manuals too, I can give you a much more specific **module-by-module combined patching guide** for creating basslines, leads, plucks, drones, arps, and chord-like textures from the whole set.

---

## Quick takeaway

The **2hp Comb** is very effective for melodic work when used as:

- a **pitched resonator** for triggers/noise
- a **self-oscillating voice**
- a **Karplus-style plucked string generator**
- a **harmonic enhancer** for existing melodic lines

For melody, the key move is:  
**excite it with short sounds, tune with FREQ, sustain with RES, and shape brightness/decay with DAMP.**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)