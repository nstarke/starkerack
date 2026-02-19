# Schlappi Engineering — Angle Grinder

- [Manual PDF](../../manuals/angle_grinder_manual_20181022.pdf)

---

[Schlappi Engineering Angle Grinder Manual (PDF)](https://schlappiengineering.com/wp-content/uploads/2020/10/AngleGrinderManual1.1.pdf)

# Creative Uses of Schlappi Engineering Angle Grinder in Eurorack

The **Angle Grinder** is a unique and versatile quad sine oscillator, state variable filter, waveshaper, and feedback playground. Here are some creative patch ideas and module combos to unleash its full sonic potential in your rack:

---

## 1. **Quad Stereo LFOs & Panning**
**Use Case**: Patching quad LFOs for animated stereo/quadraphonic effects.

- **Patch**: Set Angle Grinder to LFO range. Use the 0°, 90°, 180°, 270° outputs to modulate four VCAs controlling signal levels in a stereo or quad setup.  
- **Suggested Modules**:  
  - Mutable Instruments Veils/Intellijel Quad VCA (for VCA duties)
  - Stereo mixers or quadraphonic outputs (Doepfer A-138s or Erica Synths Black Quad VCA)
- **Result**: Complex movement and panning of audio sources, quad modulation for multi-dimensional effects.

---

## 2. **Supersaw & Metal Sound Generation**
**Use Case**: Create a "supersaw" or metallic oscillator by using the GRIND out with external audio.

- **Patch**: Run a triangle or saw oscillator into the Angle Grinder's **IN**. Adjust the **GRIND** sliders and tune the internal oscillator higher/lower than the input frequency for cross-mod timbres.
- **Suggested Modules**:  
  - Any raw analog VCO (e.g., Make Noise STO, Doepfer A-110)
  - Optional: Animate GRIND sliders with CV from LFOs or sequencers (Pamela’s New Workout)
- **Result**: Hybridizing the input and Angle Grinder’s phase comparators yields powerful, animated “super-saw” or clangorous metallic timbres.

---

## 3. **Voltage Controlled Feedback Looper / Feedback Oscillator**
**Use Case**: Exploit the nonlinear GRIND->SPIN feedback for chaotic oscillations and unstable filtering.

- **Patch**: Turn up GRIND->SPIN and reduce DAMPING. Feed GRIND out into distortion, delay (chronoblob, Mimeophon), or reverb (Erica Synths Black Hole DSP), then route it back to the IN or INJECT for wild feedback trails.
- **Suggested Modules**:
  - Any effect module with CV input (for further wild modulation)
  - Distortion: Metasonix R-series, WMD Geiger Counter
- **Result**: Self-oscillating, feedback-driven drones that sweep from clean resonance to pure chaos.

---

## 4. **Phase Quadrature FM / Cross-Modulation**
**Use Case**: Use four phase-offset sine waves to FM other oscillators or filters for animated phase relationships.

- **Patch**: Take each SPIN out to modulate the FM, cutoff, or other CV inputs on multiple modules simultaneously.
- **Suggested Modules**:
  - Classic analog VCOs for FM (e.g., Verbos Complex Oscillator)
  - Multi-input filters or morphing VCAs (e.g., Four Pole, XAOC Belgrad)
- **Result**: Moving blur of FM tones, evolving resonances, and phase-shifting ghost harmonics across your system.

---

## 5. **Voltage Controlled Multimode Filtering & Rhythmic Gating**
**Use Case**: Use Angle Grinder as a quad filter (LP, BP, HP, Inv BP) and voltage-controlled comparator for creating rhythmic gates or morphing waveshapes.

- **Patch**: Patch audio into IN, and simultaneously take all four filter outputs to different VCAs, gates, or mixers for rhythmic sculpting.
- **Suggested Modules**:
  - Clocked or logic modules (Qubit Pulsar, Doepfer A-160 series) for gating/filtering
  - Wavefolders/Distortion for post-GRIND shaping
- **Result**: Highly animated filter sweeps and morphing with quad, offset responses—unique for percussive synthesis or carving up rhythmic textures.

---

## 6. **Phase-Driven Sine Chord-Oscillator Generator**
**Use Case**: Make dense textures or chords by precisely tuning and mixing the four phase outputs.

- **Patch**: Tune Angle Grinder to a musical frequency, process each SPIN output through different pitch shifters, quantizers, or waveshapers, then mix for harmonic clusters.
- **Suggested Modules**:
  - Make Noise Telharmonic, Expert Sleepers Disting (for pitch shifting)
  - Mutable Instruments Rings (as a resonator)
- **Result**: Lush sine clusters, organ-like drones, or evolving microtonal pads.

---

## 7. **Sync & Soft Sync Blizzard**
**Use Case**: Use the INJECT input for soft sync experiments.

- **Patch**: Patch a high harmonic source (another VCO’s square or saw) into INJECT with AC coupling. Tweak the coarse and fine tune, watch for spikes and phase resets.
- **Suggested Modules**:
  - Noisy intermediate: Plaits in noise or drum modes
  - Classic analog VCO for sync master (Doepfer, Pittsburgh, Moog, etc.)
- **Result**: Resonator spikes, wacky hard/soft sync tones, or drum-like transients.

---

## 8. **Quad Waveshaper with Sequenced CV Animation**
**Use Case**: Automate the GRIND sliders via sequencers or envelopes for shifting timbre effects.

- **Patch**: Patch pitch or modulation CV from a sequencer or envelope into the GRIND CV inputs. Each slider/phase can be independently modulated.
- **Suggested Modules**:
  - Intellijel Tetrapad, Doepfer A-140 for envelopes/sequencing
  - Any step sequencer or complex envelope
- **Result**: Rhythmic or evolving morphs between waveshapes, spectral animation, or dynamic phase cancellation.

---

### Extra Tip:
**The Angle Grinder excels at hybrid cross-patching!** Feed its outputs anywhere you’d use wild modulation, phase-offset sines, or distortion sources in your modular system. Its deep feedback structure rewards experimentation and “wrong” connections.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)