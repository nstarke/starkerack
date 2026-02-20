# Vermona — Melodicer

- [Manual PDF](../../manuals/melodicer manual en 1.1 web.pdf)

---

[Download the Vermona meloDICER User Manual (PDF)](https://www.vermona.com/manuals/meloDICER_UserGuide_v11_EN.pdf)

# Creative Sound Design with Vermona meloDICER

As a Eurorack musician, the Vermona **meloDICER** offers powerful tools to inspire your patches—especially when you push its stochastic sequencing into unique rhythmic, melodic, and timbral territory. Below you’ll find strategies and patch ideas focusing on:

- **Distorted Percussive Sounds**
- **Wild, Modulated Basslines**
- **Haunting Pads & Atmospheres**

## 1. Distorted Percussive Sounds

**Patch Strategy:**
- Pair meloDICER with a noise source, drum synth, or highly resonant filter for your percussive sound.
- Use **GATE OUT** to trigger both fast envelopes and external modules (for example, distortion or wavefolding).
- Use the **rest**, **variation**, and **note value** controls to inject unpredictability.

**Advanced Tips:**
- **Variation**: Increase to introduce glitch, ratchet, and off-beat percussive effects. Enable triplets and 1/32 notes via the edit menu (see “NOTE VARIATION”), or limit them for tight, machine gun fills.
- **Legato**: Push to high settings to randomly extend note lengths, creating ties or pseudo–rolls for metallic or scraping snare sounds.
- Use **external CV modulation** (CV IN 2) to modulate **NOTE VALUE** or **VARIATION**—automate with random CV/LFOs for percussive unpredictability.

**Distortion/Processing:**
- Route GATE OUT to a drum voice patched through an external distortion/wavefolder.
- Use meloDICER’s unpredictable gates/triggers to activate effect units only on certain hits for dynamic, distorted accents.

---

## 2. Wild, Modulated Basslines (Dubstep/DnB)

**Patch Strategy:**
- Use meloDICER’s **1V/OCT** out to control a complex oscillator or rich analog synth voice with plenty of overdrive/distortion downstream.
- Focus on the **melody section’s faders:** Raise odd intervals for instability; modulate the **octave range** (faders 2 and 8) for big pitch jumps and slides.

**Bass Tricks:**
- **CV IN 1 modulation**: Patch in an envelope, LFO, or another sequencer. Assign to “TRANS SEQ” (edit menu): external CV selects the root/octave transposition, excellent for evolving, shifting bass lines.
- **Additive mode**: “ADD SEQ” allows for FM, slews, and bends (useful for growly basses if patched through a waveshaper).
- For “wobble” bass, patch an LFO to **CV IN 1** (mode B: “TRANS SEQ” for semitone snap, or A: “ADD SEQ” for smooth glides between notes).

**Rhythmic Drive:**
- Set **UNOCTAVE** and **LEGATO**: heavy legato for sliding “glitch” bass, rest and variation for syncopated, jumpy DNB style.
- Use **external clock** for tight sync; manipulate clock speed for stutter/break effects.

---

## 3. Haunting Atmospheric Pads

**Patch Strategy:**
- Use the **melody faders** to include several adjacent notes (for cluster chords or modal scales).
- Set **rest** low, so notes sustain; **legato** high for long, overlapping, evolving phrases.
- **Gate output** triggers slow envelopes or vactrol-controlled VCAs/filters for gently shifting textures.

**Ambient Tricks:**
- Use **CV IN 1**: Assign to “LO” and “HI” faders (edit menu: C and D)—patch slow LFOs, S&H, or evolving function generators to gradually expand and shrink the pitch range.
- Use **CV IN 2**: Modulate “LEGATO” and “REST” via slow random voltages—this will subtly morph how the pattern breathes.
- **Dice buttons**: Switch to realtime mode for continuous variation; lock rhythmic pattern while keeping melody stochastic (or vice versa) for generative “never repeating” pads.
- Activate **LOCK mode**: Tweak the melody sliders and rhythm controls without instantly applying, then switch settings in at the perfect moment for subtle or dramatic change.

---

## Bonus: Modulate the Modulators

- Patch a random CV source (like a Turing Machine, Wogglebug, or S&H) into **CV IN 1 or 2**, dynamically reassigning which aspect of the sequence it affects using the edit menu.
- Send rhythmic gate streams (from manual taps, other sequencers, or Euclidean generators) into **GATE IN 1/2** to trigger randomization on command, or even toggle mute/restarte the sequences.

---

## Quick Reference Table

| Target Sound        | meloDICER Function(s)                          | External Modulation                    |
|---------------------|------------------------------------------------|----------------------------------------|
| Distorted Percussion| NOTE VALUE, VARIATION, LEGATO, REST, Dice mode| CV IN 2 for rapid changes; GATE OUT to distortion; lock pattern for fills |
| Basslines           | Melody faders, CV IN 1 (ADD/TRANS SEQ), LEGATO | LFO/envelope to CV IN 1, external clock/gate for chop/sync    |
| Atmospheric Pads    | Melody faders, LO/HI, LEGATO/REST, Dice/Lock   | Slow LFO/Random to CV IN 1 & 2, hold notes with envelope/fx    |

---

For the most versatility, combine meloDICER’s rich pattern generation with aggressive external effects (distortion, filtering, wavefolding) and creative patch routing. Its stochastic engine, plus the ability to externally modulate or morph almost every key parameter, makes it a generative powerhouse for evolving, complex modular performances.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)