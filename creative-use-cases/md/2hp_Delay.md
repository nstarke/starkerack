# 2hp — Delay

- [Manual PDF](../../manuals/Delay_Manual.pdf)

---

[2hp Delay Manual PDF](https://2hp.com/wp-content/uploads/2hp-delay-manual.pdf)

---

## Creative Patch Ideas for 2hp Delay in a Eurorack System

The 2hp Delay is a compact yet powerful module with CV control over time, feedback, and mix. Here are some creative ways to integrate it with other modules to unlock unique sonic possibilities:

---

### 1. **CV Automation with LFOs and Envelopes**
- **What:** Patch an LFO or a looping envelope into the TIME CV or FDBK CV.
- **Result:** Modulate delay time for chorus/flanging effects or modulate feedback for evolving echo textures.
- **Modules:** Make Noise Maths, Intellijel Quadrax, or any function/LFO generator.

### 2. **Karplus-Strong Synthesis**
- **What:** Feed short bursts (clicks, noises, or very short envelopes) into the IN. Set delay time to very short and feedback high to create "plucked string" tones.
- **Modules:** Noise source or envelope generator (e.g., Mutable Instruments Peaks, 2hp EG).
- **Tip:** Modulate TIME CV for dynamic, pitch-bending string effects.

### 3. **Voltage-Controlled Rhythmic Echoes**
- **What:** Use a clock sequencer or trigger source to modulate either the TIME or MIX CV in sync with drum patterns for evolving rhythmic delays.
- **Modules:** Pamela’s New Workout (clock source), Erica Synths Drum Sequencer.
- **Bonus:** Modulate feedback for synced dub-style delay throws.

### 4. **Delay as a Sound Design Tool**
- **What:** Patch complex audio sources (granular, wavetable, or FM voices) into the delay for dense, shifting soundscapes.
- **Modules:** Mutable Instruments Plaits, Make Noise Mimeophon, or similar.
- **Bonus:** Process the delay output with filters (e.g., Mutable Instruments Ripples) or wavefolders for even more timbral variety.

### 5. **Self-Oscillation FX and Drones**
- **What:** Crank the feedback (FDBK) to maximum until self-oscillation occurs. Use the TIME parameter as a pitch control.
- **Result:** The delay becomes a raw sound source! Use external VCAs or filters to sculpt the drone further.

### 6. **Stereo Delay & Doubling (With Two Delays)**
- **What:** Use two Delay modules, routing to left and right. Slightly offset TIME controls for stereo widening and classic ADT (automatic double-tracking) effects.
- **Modules:** Another 2hp Delay, or any compact delay.

### 7. **Creative FX Chains**
- **What:** Insert the Delay after a distortion (e.g., 2hp Distortion) for aggressive echoes or before reverb (e.g., Mutable Instruments Clouds, Erica Synths Pico DSP) for ethereal, cavernous echoes.
- **Chain Ideas:** Voice → Distortion → Delay → Reverb

### 8. **Resampling and Feedback Networks**
- **What:** Route the output of Delay back into itself via a mixer or crossfader (e.g., ALM Busy Circuits HPO + Fader), or into a pitch shifter for glitched, evolving textures.
- **Modules:** Cubusynth Crossfader, 2hp Mix.

### 9. **Delay as a Performance Parameter**
- **What:** Use manual CV sources, like a joystick (Intellijel Planar2) or expressive controller (Make Noise Pressure Points) to play the delay as a tactile instrument live.

### 10. **Processing External Audio**
- **What:** Run drum machines, guitars, or field recordings into the delay for lo-fi tape/echo textures.
- **Requirement:** Use a module like ALM S.B.G. or Intellijel Audio Interface II for line-level interfacing.

---

**Pro Tip:** Because all parameters are CV-addressable, complex automation is possible—use sequencers, stepped random modules (e.g., Wogglebug), or even gate to trigger random echoes for glitch effects!

---

**For further experimentation and patch sheet generation, check out this repo:**  
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)