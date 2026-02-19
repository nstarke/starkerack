# Sound Machines — Modulor 114

- [Manual PDF](../../manuals/MODULOR114-MANUAL-SEP16-V01.pdf)

---

[Download the MODULÖR114 Owner’s Manual (PDF)](https://www.sound-machines.it/wp/wp-content/uploads/MODULOR_114_manual_1.0.pdf)

---

# Using the Soundmachines MODULÖR114 for Polyrhythmic, Hyper-Complex Percussion

The MODULÖR114 is not just a standard monosynth; it’s a multi-functional modular platform that can be used as a full percussion laboratory. Here’s how to tap into its rhythmic and percussive possibilities, pushing complexity, punch, and character.

---

## 1. **Clocking: Complex and Polyrhythmic Sources**

- **Clock Divider / Digital Modules**
  - The built-in **CLKDIV** offers four independent division outs and a reset input. Use an LFO or MIDI clock as input, then patch different CLKDIV outputs (/2, /4, /8, /16) to trigger S&H, envelopes, or gate percussion events at ratios that set up polyrhythms and complex time signatures.
  - Combine **outputs** using the **Logic Gates** (AND, NAND, XOR, NOT) to derive evolving, cross-rhythmic patterns. An XOR of /4 and /6, for example, can produce a cycle that only lines up every 12 steps.

- **Manual Trigger Buttons**
  - The two manual buttons can be AND'ed with LFO/clock pulses for performance “fills” or live variation.
  
---

## 2. **Percussive Voice Patching Techniques**

- **Oscillators as Drum Sources**
  - **VCO1 & VCO2/LFO1**: Patch the SAW/TRI outputs through the VCF at high resonance (self-oscillating), triggered with short envelopes, for snappy analog kick or tom sounds.
  - **Noise Source**: Use WHITE or PINK noise output into the VCF and then VCA (envelope-controlled) for hi-hats, snares, and noise-based percussion. Short ENVs for punch, longer for metallic texture.

- **Envelope Use**
  - Use the modulator’s **ADSR** for short, fast attacks and decays (“plink” shapes). Loop mode creates cycling envelopes that operate as secondary LFOs for additional layers of rhythmic modulation.
  - **Inverse/Offset**: Patch the ENV through the ADDSUB module to subtract the envelope from CV or audio, inverting contours to find unique percussive gestures.

- **Slew and S&H Variation**
  - **Sample & Hold (S&H)**: Feed random or periodic triggers (from CLKDIV or logic gates) and noise/oscillator to S&H. Use resulting stepped voltages to modulate pitch, cutoff, or FX parameters for irregular, glitchy patterns.
  - **Slew**: Insert after S&H for “glide” or ghost note effects, especially interesting when modulating filter cutoff or drum pitch.

---

## 3. **Generating Musical Complexity**

- **Quantizer**: Route S&H or LFO through the quantizer and use its scales (major, dorian, minor, etc) to ‘constrain’ random CV into melodic percussion, simulating pitched drums or tuned percussion polyrhythms.

- **Logic Gates as Pattern Generators**
  - Input multiple CLKDIV outputs into the logic gates; patch logic outputs to ENV triggers or S&H triggers, producing interlocking, never-repeating patterns.
  - XOR can also approximate ring modulation for audio: input two square waves for clanging, metallic drum tones.

---

## 4. **Effects as Percussive Shapers**

- **FX Module**: Use tempo-synced delay or modulated chorus for percussive echoes and punch. Route CV from logic modules, S&H, or LFOs into FX parameter CV jacks for dynamically shifting, glitchy, or granular effects that accentuate or disrupt the drum patterns.
- **CLIP LED**: Overdrive into FX for distorted, industrial percussion.

---

## 5. **Performance and Live Manipulation**

- **Ribbon Controller**: Use the ribbon’s CV and GATE outs as live velocity, pitch, or rhythm modulators. “Tap” rhythms into the ribbon while patching its output to S&H or directly to pitch/VCF for expressive fills and breaks.
- **Manual Buttons**: Use live as accent triggers routed through logic gates for on-the-fly pattern changes, ratchets, or stutters.

---

## **Patch Example Outline: Polyrhythmic Modular Percussion**

1. Set LFO2 as master clock source.
2. Send LFO2 to CLKDIV.
3. Route CLKDIV outputs (/3, /4, /5, /6, e.g.) to trigger:
    - ENV1 (for VCA: kick drum decay envelope)
    - ENV2 (for VCF: snare snap)
    - S&H (random percussion mod)
4. Noise → VCF (resonance high, cutoff modulated by ENV2 or S&H) → VCA → FX.
5. VCO1 SQU → ADDSUB (waveshaping) → MIX1 with noise for hybrid drum sounds or metallic hits.
6. Logic gates combine various triggers for surprise hits, fills, or polyrhythmic accents.
7. Modulate effect parameters (especially delay time or chorus rate) with S&H or logic for chaos.
8. Manual Buttons and Ribbon for performance-driven fills and surprises.

---

## **Summary Checklist: Percussive/Polyrhythmic Techniques**

- Multi-layered clocks via CLKDIV—use different divisions for each percussion element
- Logic gate patching for emergent, complex triggers
- S&H and Quantizer for irregular timing and pitch
- Ribbon/Manual Buttons for human intervention/variation
- FX modulation for evolving texture, glitch, punch
- Creative voice shaping via ADDSUB and VCF resonance, ENV inversions, and VCO sync/ringmod

---

Read the full [MODULÖR114 Manual (PDF)](https://www.sound-machines.it/wp/wp-content/uploads/MODULOR_114_manual_1.0.pdf) for more in-depth reference, and **refer to patch diagrams on pages 26–29 for concrete examples**.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)