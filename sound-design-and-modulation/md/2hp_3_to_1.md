# 2hp — 3 to 1

- [Manual PDF](../../manuals/3_To_1_Manual.pdf)

---

[3:1 Module Manual (PDF)](https://2hp.com/docs/3-1.pdf)

---

# Creative Modulation Ideas Using the 2hp 3:1 Eurorack Module

The **2hp 3:1** is a voltage-controlled gate switch/summer that can route or sum three gate/trigger inputs under manual or CV control. This module is a flexible tool for intricate patching strategies in both rhythmic and melodic contexts. Here are detailed ideas for using this module to sculpt **distorted percussion, wild basslines, and eerie pads** as heard in genres like dubstep, drum and bass, and dark ambient.

---

## Core Modulation Features

- **Voltage Control over Input Selection:** Route rhythmic gates/sequences with hands-free CV.
- **Selective/Summing Modes:** Either isolate a single input or combine multiple gate streams for polyrhythmic complexity.
- **Gate-to-Trigger Conversion:** Great for precision-triggering complex envelopes or percussive events.

---

## 1. Distorted Percussive Sounds

**Goal:** Drive drums or metallic hits with sharp, unpredictable gates to create "glitchy" or "broken" percussion.

### Patch Ideas
- **Rhythmic Chaos:**
  - Patch three different rhythmic gate sources (e.g., clock dividers, random triggers, or Euclidean patterns) into IN 1, IN 2, and IN 3.
  - Toggle to **SUM mode** (mode right). All simultaneous gate inputs will be summed to short triggers (5ms), rapidly retriggering downstream modules—perfect for noisy, layered percussion.
- **External Modulation:**
  - Send a stepped random CV (e.g., from a sample and hold) or a lively LFO into SEL CV to automate and “fracture” gate selection on the fly, making percussion stutter and shift.
  - Route OUT to a distortion/wavefolder and then to a drum sound generator for harsh, digital artifacts.

### Quick Tips
- Use **velocity-sensitive envelopes** triggered from 3:1 OUT to sculpt transients.
- For digital grit, clock an audio-rate square oscillator as a trigger source for metallic “clangs”.

---

## 2. Aggressive/Crazy Basslines (Dubstep, DnB)

**Goal:** Create switching basslines with gnarly rhythm and timbral switchups.

### Patch Ideas
- **Bassline Articulation:**
  - Patch gates from different bass step sequencer lines (even if programmed out of phase) to the three INs.
  - Use a sequencer or envelope follower from your drum hits to modulate SEL CV, allowing bass notes to “switch pattern” as the drums play—classic "talking" or "bouncing" dubstep effect.
  - OUT feeds an envelope or direct VCA controlling a bass oscillator or filter ping for *precisely-timed growls*.
- **Malfunctioning Wobble:**
  - In SUM mode, overlapping bass rhythm gates trigger retriggers—try sending this summed/triggered signal to a waveshaper for unpredictable, “broken voice” bass contours.
- **CV Trick:**
  - Use a quadrature LFO on SEL CV for cyclical, morphing riffs; fast LFO rates can “granulize” gates for bass stutters.

---

## 3. Haunting Atmospheric Pads

**Goal:** Evolve sustained pads by creatively gating multiple modulators or textures.

### Patch Ideas
- **Texture Weaving:**
  - Gate three “layers” of slow-moving modulation sources (random LFOs, envelopes, or drone oscillators) into IN 1–3, mix through SUM mode.
  - CV automate SEL with slowly drifting random voltages; this will fade layers in/out, making pads shift unpredictably.
  - OUT triggers VCA or CV inputs on reverbs/FX for ambient “echoes” that flicker in and out of existence.
- **Ghostly Pulses:**
  - Use sporadic trigger patterns from a random rhythm generator; output governs when certain pad layers or FX chains are active, creating ethereal movement.
- **Pad Animation:**
  - Gated triggers from 3:1 OUT can start envelope generators for filter sweeps or wavetable morphs—make atmospheric pads “breathe” and mutter with every switching event.

---

## Extra Patch Tips

- **Automation:** Treat the SEL control as a major timbre animator; slowly morph selection for morphing, fast for glitch.
- **Abusing Modes:** Toggle SELECT and SUM mode with clock/reset edges for extreme, performance-oriented scene changes.
- **Unusual FX:** The 5ms gate-to-trigger in SUM mode lets you precisely ping LPGs (Low Pass Gates) or make short, plucky FM percussion.

---

For further DIY patch generation and modular utilities, see  
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)