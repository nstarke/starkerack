# WMD SSF — Chimera

- [Manual PDF](../../manuals/Manual_v1.2.pdf)

---

[Download the Chimera Manual (PDF)](https://wmdevices.com/pages/chimera-manual)

---

## Using the WMD Chimera for Hyper-Complex Rhythmic Percussion in Eurorack

The Chimera is a metallic percussion synthesizer module, ideal for generating nuanced, complex, and cutting-edge rhythmic elements. Here’s how to use it as a powerful voice for dense, polymetric, and highly unique percussion:

---

### 1. **Programming Complex Triggers & Polyrhythms**

- **TRIG Input:** Send a variety of trigger pulses to the TRIG input from different sources in your rack (e.g., Euclidean sequencers, clock dividers/multipliers, or random gate generators). 
- **Trigger Patterns:** For polyrhythms and complex time signatures, use multiple gate/trigger generators in odd and even divisions (e.g., 5:4, 7:8). Pair with a clock/trigger sequencer (Pamela's New Workout, Hermod, or similar).

---

### 2. **Nuanced Velocity and Accenting**
- **ACCENT Input:** Patch an accent signal, such as a stepped CV or random voltage, to modulate emphasis on select hits. The ACCENT input also resets the rhythm in FEEL mode 2; experiment with bursts or unpredictable resets for shifting patterns.
- **FEEL Modes:** 
  - Mode 1: Forces mechanical regularity (great for some polyrhythmic foundations).
  - Mode 2: Introduces subtle velocity and timing variations (morphs repetitive triggers into expressive grooves).
  - Mode 3: Engages full randomization—each strike evolves uniquely, perfect for unpredictable, evolving metallic textures.

---

### 3. **Density and Expressive Texture Control**
- **DENSITY Knob:** Turn up for rapid-fire grains—this is key for shimmering, densely packed sequences. Lower density for space or to isolate certain percussive events within the polyrhythmic structure.
- **SURFACE Selector:** Morph between the 11 surface types for timbral shifts or automate with external CV for ever-evolving metallic flavors.

---

### 4. **Punch, Clarity, and Dynamic Range**
- **DECAY Control:** Keep DECAY short for snappy, punchy percs or lengthen for washy metallic noise. CV the decay for evolving articulations in your sequence.
- **VCA Input:** Patch envelopes or stepped, sequenced voltages here to impose accenting, ducking, or dynamic swells—layering groove complexity.
- **CHOKE Input:** Use this creatively by sending streams of gates for rapid gating effects (excellent for ratchet patterns or sudden dropouts within dense polyrhythms).

---

### 5. **Pitch, Timbre, and Special FX**
- **PITCH Knob:** Modulate using external CV for shifting metallic tones, making each hit distinct or morphing across the range for pseudo-melodic rhythmic effects.
- **ENVELOPE Pitch Control:** Apply positive or negative settings to infuse each sound with falling/rising bends—these can suggest Doppler or sci-fi, laser-esque sounds for even more percussive variation.
- **FX & FX AMT:** Cycle/sample-rate reduction for crunchy, digital edges or comb filtering for resonant, pinging overtones. Modulate FX AMT for movement.

---

### 6. **Sequencing and Modular Integration Tips**
- Pair Chimera with complex trigger sequencers, logic modules, or CV sample & holds for extreme rhythmic diversity.
- Send random, probabilistic, or LFO-sourced voltages to PITCH, DECAY, SURFACE, DENSITY, and FX parameters to maximize chaos or organic variation in dense rhythmic beds.
- Layer multiple instances (if you own more than one unit) or parallel process the output for further complexity.

---

### 7. **Patch Idea: Polymetric Machine Groove**
```text
- Channel 1 Pamela’s New Workout: 3-step pattern triggers → Chimera TRIG
- Channel 2: 5-step pattern → Chimera ACCENT
- Euclidean Gate from Ornament & Crime → Chimera CHOKE (rapid cut-outs)
- Random stepped voltage from Turing Machine (locked loop mode) → Chimera PITCH and DECAY
- Slowly cycling LFO → Chimera SURFACE
- FX set to comb filter; random slew to FX AMT
Result: Unrepeatable metallic machine-funk full of cross-rhythm, accent, and evolving timbre.
```

---

#### **With strategic modulation and sequencing, the Chimera is a secret weapon for advanced, dynamic, and hyper-complex percussion textures in Eurorack.**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)