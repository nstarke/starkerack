# 2hp — Comb

- [Manual PDF](../../manuals/Comb_Manual.pdf)

---

[Comb 2hp Manual (PDF)](https://2hp.com/manuals/comb.pdf)

---

## Using the 2hp Comb Module for Densely Rhythmic, Hyper-Complex Percussion

The **2hp Comb** is an effect module—a versatile IIR peaking comb filter, not a sound source. However, its ability to **reshape transient content, add harmonics, punch, and metallic resonance** makes it an outstanding secret weapon for intricate percussion and complex rhythmic patterns in modular music.

Below are strategies for integrating Comb into a setup geared towards **densely rhythmic, hyper-complex percussion** featuring polyrhythms, unusual time signatures, and complex sequences.

---

### 1. Percussion Processing: Adding Harmonic Character

- **Input:** Patch drum or percussive sounds (kick, snare, hats, FM percussion, or even white noise bursts) to the **IN**.
- **Cutoff Frequency (FREQ):**  
  - Modulate the FREQ parameter with either clock-divided triggers or sequenced random CV (using the FREQ CV input).
  - This shifts the harmonic peaks, making each hit unique and “pitched” or metallic.
- **Resonance (RES):**  
  - Use high resonance settings to cause ringing and overtones—ideal for metallic, trashy snares/crashes, or tuned percussion (think log drums, agogo).
  - Modulate RES with random, Euclidean, or polyrhythmic patterns—each drum can “ring” differently within the rhythmic grid.

---

### 2. Creating Unique, Punchy, Percussive FX

- **Damp Control (DAMP):**  
  - Modulate with complex envelopes or LFOs sync’d/polyrhythmic to base clock: short, sharp (fully damped) = more clipped and thuddy; open (no damping) = more metallic and resonant.
  - Use “accent” triggers to momentarily brighten certain hits—great for ghost notes or syncopated events.
- **Self-oscillation:**  
  - Push resonance into self-oscillation, then trigger the filter with gates or bursts—Comb will act as a wild, pingable percussion voice of its own.
  - Vary FREQ CV input by using different divisions or clock sources for different polyrhythms.

---

### 3. Complex CV Modulation for Complex Rhythms

- **Sequence All CV Inputs:**  
  - Use sequencers or random sources (Turing Machine, Marbles, Pamela’s New Workout) to provide stepped or smoothly transitioning voltages to FREQ CV, RES CV, and DAMP CV.
  - Phase-offset LFOs or Euclidean pattern CVs provide ever-changing parameter shifts, imprinting rhythmic complexity and timbral movement onto percussive material.
- **Rhythmic Gate Processing:**  
  - Use logic modules to combine multiple rhythms and send short gates/envelopes to the FREQ or RES CV inputs for polyrhythmic flams, ratchets, or fills.

---

### 4. Sound Design Tips for Hyper-Complex Patterns

- **Layer Multiple Comb Instances:**  
  - Use more than one Comb (or mult’s with varied CV), processing different drums with different settings for dense, granular “comb-filtered drumkit” sounds.
- **Turn White Noise Into Claps:**  
  - Pulse white noise or crowd samples through Comb with modulated settings, resembling classic 808/909 “clap” machines—modulate FREQ for flams or roll effects.
- **Glitch and Stutter FX:**  
  - Rapidly switch parameter states (via fast gates or stepped CV) for hard, glitchy timbral jumps—a modern, IDM-friendly technique.

---

### 5. Integration for Maximum Rhythmic Density

- **Feedback and Damping:**  
  - Heavy feedback + rapid changes to DAMP allow you to “choke” and “release” the resonance per hit, mechanically accenting certain rhythms in a highly dynamic way.
- **Sync with Clocked CV:**  
  - Use clocked or phase-shifted LFOs/envelopes to rhythmically animate Comb’s parameters in non-repetitive ways, bridging polyrhythmic signals into something coherent and punchy.

---

### Summary of Patch Techniques

- **Drums → Comb In → Audio Out**
- Patch complex sequencer/clock dividers/LFOs/gate sources to FREQ CV, RES CV, and DAMP CV.
- Push resonance high for metallic/fx sounds, modulate for evolving timbral rhythm.
- Use damp for drum “accent”/tone/decay control.
- Self-oscillate Comb and “ping” it for hybrid drum sounds.

---

For sonic examples and workflow tools, visit the [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor) repository.

---

**Happy patching! Let the rhythms get as intricate as your imagination.**