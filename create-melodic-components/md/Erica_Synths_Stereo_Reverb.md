# Erica Synths — Stereo Reverb

- [Manual PDF](../../manuals/black_stereo_reverb_Manual.pdf)

---

[Manual PDF](attachment)

# Using the Erica Synths Black Stereo Reverb to Create Melodic Components

This manual is for the **Erica Synths Black Stereo Reverb**. While it is primarily an effects module rather than a voice or sequencer, it can still play a strong role in building **melodic material** in a Eurorack system, especially when paired with oscillators, envelopes, sequencers, samplers, or other pitched sound sources.

## What this module contributes musically

The Black Stereo Reverb can shape melody in a few important ways:

- **Turn simple notes into spatial melodic phrases**
- **Freeze and repitch audio for drones and playable textures**
- **Use feedback to create tuned resonances and self-oscillating layers**
- **Recall presets to switch between different “melodic spaces”**
- **Use CV over size, tone, feedback, and patch selection to animate sequences**

## Features most relevant to melody

From the manual, the key melody-oriented features are:

- **Stereo reverb with Tape, BBD, and Dirty BBD character**
- **Room / Hall / Cathedral style spaces**
- **FREEZE**, manually or by trigger/gate
- **SIZE CV calibrated to 1V/oct**
- **Feedback capable of self-oscillation**
- **CV over size, feedback, tone, dry/wet, and patch selection**
- **10 savable presets**

These features make it useful not just as a reverb, but as a **playable sound processor**.

---

## Best ways to use it for melodic work

## 1. Add reverb to a melodic voice

The most straightforward use:

- Patch a **VCO, wavetable oscillator, sampler, or complete synth voice** into **L(MONO) IN**
- Take **L OUT / R OUT** to your mixer or output
- Set:
  - **TYPE** to Tape for smoother ambience
  - **MODE** to Room or Hall for tighter note definition
  - **DRY/WET** around 20–40% so pitch stays clear
  - **FEEDBACK** moderate to avoid washing out fast sequences

### Why this helps melody
For arpeggios, basslines, or leads, this gives notes depth without destroying articulation.  
Use:

- **Room** for plucks and rhythmic melodies
- **Hall** for lead lines
- **Cathedral-like larger settings** for sparse melodic phrases

---

## 2. Use FREEZE as a pitched texture generator

One of the most musical features is **FREEZE**.

According to the manual:

- FREEZE captures the reflected audio signal
- When frozen, the **SIZE knob or SIZE CV manipulates playback frequency**
- **SIZE CV tracks 1V/oct**

That means once you freeze audio, the module can act a bit like a **pitched buffer instrument**.

### Patch idea
- Send a short melodic sound into the reverb:
  - pluck
  - bell
  - vocal hit
  - noise burst through a filter
- Trigger **FREEZE**
- Now send a **sequencer CV** into **SIZE CV**

Because SIZE CV tracks 1V/oct, you can use a pitch sequencer or keyboard CV to play the frozen audio at different pitches.

### Result
You get:

- granular-ish tonal textures
- organ-like sustained harmony
- playable ambient leads
- repitched frozen chords or note tails

This is one of the strongest ways the module can directly create melodic content.

---

## 3. Build drones that follow a scale

A very effective melodic technique:

- Feed in a note, chord stab, or harmonic sound
- Freeze it
- Send **quantized CV** into **SIZE CV**
- Keep **DRY/WET** high or fully wet
- Adjust **TONE/SPN** to shape brightness
- Use **FEEDBACK** carefully to thicken the sustain

### Musical outcome
This turns the module into a **scale-following drone voice**.  
If your input is harmonically rich, the repitching can sound like:

- choir pads
- shimmer-like sustained tones
- lo-fi tape choir
- evolving harmonic beds

This works especially well in ambient, techno intros, cinematic music, and experimental melodic patches.

---

## 4. Make pseudo-melodies from feedback

The manual notes that:

- At full clockwise **FEEDBACK**, the module can go into **self-oscillation**

This means the reverb can become a sound source in its own right.

### Patch idea
- Feed a short click, trigger pulse, or tiny burst of noise into the input
- Raise **FEEDBACK**
- Tune the resulting resonant behavior using:
  - **SIZE**
  - **TONE**
  - **TYPE**
  - **MODE**

You may not get perfectly stable oscillator pitch like a VCO, but you can get:

- tuned ringing tones
- resonant melodic artifacts
- unstable lo-fi notes
- haunting feedback harmonics

If you then modulate **SIZE CV** with a sequencer or quantizer, you can coax the feedback network into more melodic movement.

### Best use
This is ideal for:

- dub-techno chords
- eerie melodic noise lines
- unstable tape-flavored lead textures
- background harmonic motion

---

## 5. Animate a sequence with CV

Even if another module is handling pitch, the Black Stereo Reverb can make the melody feel much more alive through CV modulation.

### CV destinations
- **SIZE CV**: changes virtual room size, and in freeze mode changes playback pitch/frequency
- **FBK CV**: changes the intensity and sustain
- **TONE CV**: darkens/brightens reflections
- **PATCH CV**: switches among 10 saved presets

### Musical use
You can patch:

- an LFO for slow phrase evolution
- an envelope for note-by-note reverb emphasis
- a sequencer row for different ambience per note
- a random voltage source for generative melodic variation

### Example
A simple 8-step melody becomes much more expressive if:

- every 4th note gets more feedback
- certain notes get brighter reflections
- preset changes occur at phrase boundaries

This does not change pitch directly, but it strongly shapes how the melody is perceived.

---

## 6. Preset switching as song structure

The module stores **10 presets** and allows **patch CV** to switch among them.

That means you can create several melodic environments, for example:

1. Tight room for bassline
2. Dark tape hall for verse lead
3. Huge cathedral wash for breakdown
4. Frozen repitched drone for intro
5. Dirty BBD feedback texture for transition

Then sequence **PATCH CV** from a CV sequencer, manual controller, or gate-to-CV source.

### Why this matters melodically
A melody can feel like an entirely different phrase depending on:

- reverb time
- tonal darkness
- stereo spin
- freeze state
- feedback amount

Preset switching lets one melodic line become multiple musical sections.

---

## 7. Stereo spin for width in lead lines

The manual says **TONE/SPN** controls either:

- tone of reflections
- or stereo spin when using SHIFT

This is useful for melodic parts that need width without losing the center.

### Use cases
- widen sustained leads
- create moving stereo motion in arpeggios
- make repeated motifs sound less static
- add life to frozen melodic layers

For mono melodic voices, patch into **L(MONO) IN** and let the module create stereo spread.

---

## Concrete patch examples

## Patch 1: Ambient playable frozen lead
**Goal:** turn one note into a playable melodic instrument

- Sound source: plucked VCO or bell sound
- Patch source to **L(MONO) IN**
- Set **DRY/WET** mostly wet
- Trigger **FREEZE** after the reverb tail blooms
- Send **1V/oct sequencer or keyboard CV** to **SIZE CV**
- Use a quantizer if needed
- Adjust **TONE** for brightness
- Keep **FEEDBACK** moderate

**Result:** a playable sustained lead made from the frozen reverb buffer.

---

## Patch 2: Melodic halo around a bassline
**Goal:** keep bass notes defined while adding harmonic space

- Bass voice into **L(MONO) IN**
- **TYPE** = Tape or BBD
- **MODE** = Room
- **DRY/WET** low
- **TONE** fairly dark
- Modulate **FBK CV** with an envelope tied to accents

**Result:** the bassline remains punchy, but accented notes bloom into a melodic tail.

---

## Patch 3: Dub chord machine
**Goal:** make chord stabs trail into tuneful space

- Chord voice or polyphonic source into stereo inputs
- **TYPE** = Dirty BBD
- **MODE** = Hall or Cathedral
- Medium/high **FEEDBACK**
- Modulate **TONE CV** slowly
- Occasionally trigger **FREEZE**
- Sequence **SIZE CV** during freeze

**Result:** dub echoes smear into harmonic pads and repitched melodic clouds.

---

## Patch 4: Generative melodic drone
**Goal:** autonomous evolving harmonic material

- Feed filtered noise or a struck resonant sound into the input
- Freeze the texture
- Send random stepped CV through a quantizer into **SIZE CV**
- Slow LFO to **TONE CV**
- Another slow CV to **FBK CV**

**Result:** evolving notes and harmonic motion from a static captured source.

---

## Patch 5: Preset-sequenced melodic arrangement
**Goal:** one sequence, multiple emotional spaces

- Melodic voice into reverb
- Save 4–6 presets with different:
  - TYPE
  - MODE
  - FEEDBACK
  - TONE
  - DRY/WET
- Send stepped CV to **PATCH**
- Change presets every bar or every phrase

**Result:** your melody changes character over time without changing the notes themselves.

---

## Important controls to learn first

If you want melodic results quickly, focus on these:

### SIZE
- Normal mode: room size and reverb feel
- Freeze mode: playback frequency/pitch behavior
- Most important control for melodic experimentation

### FREEZE
- Essential for creating sustained tonal material
- Can be manual or triggered by gate

### FEEDBACK
- Controls sustain and density
- Can push into self-oscillation for more tone generation

### TONE/SPN
- Shapes brightness or stereo motion
- Very useful for making melodic layers sit correctly in a mix

### PATCH CV
- Excellent for structured performance changes

---

## Musical strengths of this module

This module is especially good at:

- **ambient melody processing**
- **repitched frozen textures**
- **stereo widening of leads**
- **feedback-based harmonic effects**
- **preset-based arrangement changes**
- **turning short notes into sustained melodic material**

It is less suited to being a precise primary oscillator, but it is very strong as a **melodic enhancer and texture voice**.

---

## Best system partners

This module pairs especially well with:

- **quantizers** for playing frozen buffers musically
- **sequencers** sending pitch CV to SIZE CV
- **plucked or percussive voices** for interesting freeze captures
- **samplers and granular modules**
- **filters** before the input to control harmonic content
- **VCAs/envelopes** to control what gets fed into the reverb
- **switches/sequential switches** for changing sources into the freeze buffer

---

## Summary

The **Erica Synths Black Stereo Reverb** is not just a finishing effect. In a melodic Eurorack patch, it can serve as:

- a **spatial enhancer** for notes and sequences
- a **frozen pitched texture instrument**
- a **feedback-driven drone generator**
- a **preset-morphing performance tool**
- a **stereo animation processor** for melodic voices

Its most unique melodic trick is the combination of **FREEZE + SIZE CV with 1V/oct tracking**, which allows frozen reverb material to be repitched and played like an instrument.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)