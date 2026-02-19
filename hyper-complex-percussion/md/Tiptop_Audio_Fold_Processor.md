# Tiptop Audio — Fold Processor

- [Manual PDF](../../manuals/Tiptop_Audio_foldprocessor.pdf)

---

[Tiptop Audio Fold Processor Manual (PDF)](https://tiptopaudio.com/manuals/Tiptop_Audio_Fold_Processor_Manual.pdf)

---

## Using the Tiptop Audio Fold Processor for Dense, Hyper-Complex Percussion

The Tiptop Audio Fold Processor is a deeply creative tool for adding intricate timbral complexity and aggressive punch to any audio source, including percussive sounds and rhythms. Here are strategies to realize densely rhythmic, polyrhythmic, and highly nuanced percussive sequences with this module:

---

### Core Concepts

- **Type:** Effect processor (wavefolder + octave subdivider)
- **Main Features:**  
  - Serge-inspired diode wavefolder (analog waveshaping)
  - Unique "Square & Divide" section creating octave-divided pulse layers
  - Extensive CV control over folding and signal offset ("Inject") parameters

---

### Percussive & Rhythmic Techniques

#### 1. **Complex Percussion Source Processing**
- **Input:** Feed **dry drum samples**, modular percussion, or complex looped patterns (from samplers or drum machines like Tiptop ONE) into the **IN1** or **IN2** input.
- **Wavefolding:** Use the **FOLD** and **INJECT** knobs (or their CVs) to aggressively shape transients and add nonlinear harmonics — this makes kicks snappier, snares more metallic, and hats explosively clicky.
- **Voltage Sequencing:** Modulate FOLD and INJECT parameters with rhythmic CV sources (e.g. stepped random, clocked LFOs, trigger sequencers, Euclidean or magneto rhythmic gates) to create percussive morphing timbres that transform each hit.

#### 2. **Polyrhythmic Octave Division**
- **Subdivide Section:** Patch OUT into SUBDIV IN and manipulate the **octave division knobs** (÷1, ÷2, ÷4, ÷8) to layer subharmonic pulses over your drums.
- **Even/Odd Time:** Divide a fast rhythm (5–7 hits per bar) and overlay directly with another module creating a different division (e.g. 3, 4, or 7 hits per bar) — the different octaves form the backbone of a *polyrhythmic* drum pattern.
- **Division Automations:** Sequence or CV-modulate the SUBDIV gain knobs on or off using a rotosequencer, random gates, or trigger patterns to create shifting, constantly evolving pulse density.

#### 3. **Hyper-Complex Patterns**
- **Automation:** Use a CV sequencer, logic/inverter gates, or voltage-addressed switches to rapidly change the state of FOLD, INJECT, and DIVISION knobs, breaking out of regular repeating patterns.
- **FM Feedback:** Route the OUT or SUBDIV OUT into FM or AM inputs of other oscillators or percussion voices, making each percussive hit dynamically timbrally unique (e.g. for metallic hits, digital clicks, glitch snares).
- **Cross-patching:** Send wild LFOs, envelopes, or stepped randoms to FOLD/INJECT CVs rhythmically related but out of sync with the main clock for extreme polyrhythmic modulation.

#### 4. **Unique, Punchy Character**
- **Pre/Post FX:** Use the Fold Processor before or after core drum module audio paths or even in *parallel* for "wet/dry" blending — this lets you preserve punch while adding analog destruction.
- **Feedback Loops:** Route the OUT or SUBDIV OUT to the audio input of a delay (e.g. Tiptop Z-DSP), and/or set up feedback from the delay back into the Fold Processor for saturated, shifting, semi-chaotic rhythmic textures.
- **Velocity/Accent Control:** If your sequencer outputs velocity, use this CV to modulate the amount of folding or inject, translating per-step dynamics directly into unique timbral punch.

---

### Pattern Suggestions

- **Euclidean Sequencer** – Use with primary drum triggers; route output audio into Fold Processor.
- **Odd Meter LFOs** – E.g. a 5-step LFO modulates FOLD, 7-step LFO modulates INJECT CV — making each repeat cycle hyper-complex.
- **Clock Division** – Subdivide a main clock and trigger the DIVISION knobs at shifted intervals for offset, phase-shifting percussion.

---

### Patch Example: Hyper-Complex Mod Drum Stack

1. Patch a mixed drum loop or percussion VCO to Fold IN1.
2. FOLD OUT to filter or delay for further sculpting.
3. Simultaneously, SUBDIV OUT to second audio channel for layered sub pulses or metallic overtones.
4. Use CV sequencer outputs (random, Euclidean, or polyrhythmic clocked modulation) into FOLD CV and INJECT CV with variable ATTEN for dynamic morphing.
5. Modulate SUBDIV GAIN knobs with rhythmic gates for evolving subdivisions.

---

> **Pro Tip:** Layer the processed signal with the dry original to emphasize attack, or resample multiple passes of the Fold Processor for multi-layer “meta-rhythmic” drums!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)