# Doepfer — A-121-3

- [Manual PDF](../../manuals/A-121-3 12dB Multimode Filter (slim version).pdf)

---

[Doepfer A-121-3 12dB Multimode Filter Manual (HTML source)](https://doepfer.de/a1213.htm)

---

# Creative Patch Ideas for Doepfer A-121-3 12dB Multimode Filter

The **A-121-3** is a compact, voltage-controlled 12dB/octave multimode filter offering simultaneous Lowpass (LP), Highpass (HP), Bandpass (BP), and Notch (N) outputs. With flexible CV options and resonance up to self-oscillation, it’s an extremely versatile tool in a Eurorack system. Here are creative ways you might use it:

---

### 1. **Classic Subtractive Synthesis**
- **Patch:** Oscillator (VCO) → A-121-3 Audio In, use LP output to VCA, then to output.
- **Tip:** Modulate the cut-off with an LFO or Envelope Generator (e.g. Doepfer A-140, Maths) via CV1 or CV2 for movement and dynamics.
- **Enhancement:** Modulate resonance (CQ) with another LFO for evolving harmonics.

---

### 2. **Parallel Multimode Filtering**
- **Patch:** Use all four outputs (LP, HP, BP, N) simultaneously.
- **Mix:** Send the outputs into a mixer such as Mutable Instruments Veils or Doepfer A-138.
- **Result:** Morph between filter types in real time, or process parallel bands differently (e.g. stereo spread, effects processing).

---

### 3. **Filter as a Sine Oscillator/Modulator**
- Self-oscillate the filter (resonance full CW, no audio input) and patch the outputs to:
  - **Audio Path:** Use as a precise sine oscillator for FX or FM (e.g. to modulate another filter or VCO).
  - **CV Path:** Use the oscillating signal as an LFO by controlling frequency at lower ranges.

---

### 4. **Distortion Tricks**
- Increase the input level (Level knob past 5) to push the filter into soft clipping/distortion.
- **Patch:** Try simple waveforms (triangle, sine) and then complex/dense sounds (chords, noise).
- **Enhancement:** Follow with a wavefolder (e.g. Befaco Chopping Kinky) or wave multiplier for aggressive timbres.

---

### 5. **Dynamic Filter Modulation (Wobble/Basslines)**
- **Setup:** Use CV2 with attenuator (FCV2) and patch in a complex CV source, such as:
  - Envelopes with wiggly end-of-cycle feature (e.g. Intellijel Quadrax).
  - Stepped random (e.g. Wogglebug, Turing Machine).
- **Result:** Create 'wobble' filtered basslines or morphing sound textures.

---

### 6. **Evolving Resonance**
- **Idea:** Modulate CQ input with a slow LFO or random source (e.g. Make Noise Wogglebug).
- **Result:** Evolving, organic filter peaks—great for drones, pads, or generative compositions.

---

### 7. **Dual Filter Crossfading and Animation**
- Use two A-121-3s or another filter (e.g. Doepfer A-121-2 or Ripples), patch outputs to a crossfader (X-PAN, Happy Nerding PanMix).
- **Result:** Animate transitions between different filter shapes in real time.

---

### 8. **Notch Filtering Rhythmically**
- **Performance:** Patch the Notch output to an effect like delay or reverb. Modulate the cutoff rhythmically with a gate sequencer (e.g. Pamela’s New Workout, Varigate).
- **Result:** Sweeping notches with rhythmic motion, creating movement in pads or loops.

---

### 9. **Filter Feedback Patching**
- Patch the filter output (e.g. LP or BP) back into the filter input through an attenuator/VCA.
- **Result:** Self-modulating, unpredictable results—great for experimental and noise music.

---

### 10. **Multimode Percussion Synthesis**
- Use self-oscillation with fast VCAs/envelope generators to ping the filter. Vary the outputs for different percussion archetypes (kick -> LP, snare -> BP/N, hats -> HP/Noise).
- **Enhancement:** Modulate cutoff and resonance per hit for dynamic percussion sounds.

---

#### **Module Pairing Ideas**
- **Complex LFOs:** Mutable Instruments Tides, Make Noise Maths
- **Stepped/Sample&Hold:** Doepfer A-148, Wogglebug
- **Mixers/VCAs:** Mutable Instruments Veils, Doepfer A-138, Intellijel Quad VCA
- **Random/Chaos CV:** Turing Machine, Marbles
- **Envelopes:** Intellijel Quadrax, Doepfer A-140
- **Crossfaders:** Happy Nerding PanMix, Xaoc Devices Samara II

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)