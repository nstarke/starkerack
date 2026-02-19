# Instruo — Tona

- [Manual PDF](../../manuals/Tona-Manual-A5.pdf)

---

[Download the Instruō tòna Oscillator Manual PDF](sandbox:/mnt/data/instruo-tona-oscillator-manual.pdf)

---

# Creative Patch Ideas for Instruō tòna

Drawing from the manual, here are some creative ways to integrate the Instruō tòna with other Eurorack modules, elevating both classic and experimental synthesizer workflows.

---

### 1. **West Coast Complex Oscillator Patch**

*Combine tòna with a wavefolder, low pass gate, and envelope generators for a Buchla-inspired complex voice.*

- **Modules Needed:**  
  - [Instruō tòna]  
  - Dedicated wavefolder (optional, tòna’s internal is great, but for serial folding look at Instruō athrú, or Make Noise DPO’s folder section)
  - Low Pass Gate (e.g. Make Noise Optomix, Instruō traigh or tanh[3])
  - Function Generator/Envelope (e.g. Maths, Befaco Rampage)

- **Patch Ideas:**  
    - Use tòna’s sine or triangle output to feed its own wavefolder and an external wavefolder in series.
    - Modulate tòna’s Fold input using an envelope or audio-rate oscillator.
    - Route folded output through LPG for plucky, woody sequences.

---

### 2. **Audio-Rate Modulation Experiments**

*Leverage tòna’s Linear FM and Wavefold CV for rich, non-traditional timbres.*

- **Modules Needed:**  
  - Audio-rate Oscillator (e.g. Intellijel Dixie II+, Doepfer A-110)
  - CV Utility Attenuator/VCA (e.g. Mutable Instruments Shades, Doepfer A-132)
  - Step Sequencer (for pitch melodies/modulations)

- **Patch Ideas:**  
    - Patch an external VCO sine or triangle into tòna’s Linear FM input; use the FM attenuator to dial in subtle to clangorous inharmonic results.
    - Use tòna’s saw or square output patched back to its own Wavefold CV input—create audio-rate self-modulation for unstable, percussive, or evolving textures.
    - Put a VCA in between tòna and the modulator for dynamic FM depth (e.g. control the VCA with an envelope).

---

### 3. **Classic Subtractive and Hybrid Techniques**

*Bridge tonal East Coast and rich West Coast flavors with mutant subtractive voices.*

- **Modules Needed:**  
  - Analog Filter (e.g. Doepfer A-124, Mutable Instruments Ripples, Intellijel Polaris)
  - Mixer
  - VCA (Voltage Controlled Amplifier)
  - Envelope Generator/Sequencer

- **Patch Ideas:**  
    - Mix tòna’s triangle, saw, and square outputs—create hybrid waveforms before filtering.
    - Use Wavefold output before or after filtering for dynamic harmonic interest.
    - Sequence with a random source (e.g. Wogglebug, Turing Machine) for generative tones.

---

### 4. **Sync Sweep & Retro Tones**

*Oscillator sync yields aggressive sync sweeps, classic hard-edged leads, and laser-zap SFX.*

- **Modules Needed:**  
  - Fast LFO or second Oscillator with sharp-edged waveform
  - Envelope Generator

- **Patch Ideas:**  
    - Hard sync tòna to another VCO for metallic, tearing sounds – sweep tòna’s frequency with an envelope for sync sweeps.
    - Try syncing to a subharmonic (octave down) square for video-gamey tones.

---

### 5. **Percussive & Drum Synthesis**

*Wavefolder and FM are great for metallic or percussive voices (bells, kicks, snares).*

- **Modules Needed:**  
  - Fast Envelopes (e.g. Intellijel Quadra, Make Noise Maths)
  - LPG or VCA
  - Optionally: Noise Source

- **Patch Ideas:**  
    - Use tòna's wavefold out for metallic pings, FM’d with short envelopes for bells or hi-hats.
    - Mix tòna's sine or triangle at low frequencies with an envelope for deep, subby kicks.

---

### 6. **Random and Evolving Textures**

*Patch generative modulation sources into tòna for living, textural soundbeds.*

- **Modules Needed:**  
  - Random/Noise sources (e.g. Mutable Instruments Marbles, Doepfer A-118)
  - Cycling Envelope Generators/LFOs

- **Patch Ideas:**  
    - Modulate wavefold depth or FM with slow random voltages for evolving, shifting tones.
    - Cross-patch between tòna FM and wavefolder for unstable, animated drones.

---

### 7. **Stereo and Polyphonic Experiments**

*Pair two tòna modules—or tòna with another VCO—for wide stereo imaging or double-voice patches.*

- **Patch Ideas:**  
    - Pan each tòna output to opposite stereo channels, subtly detune or cross-modulate for lush stereo fields.
    - Hard sync or FM between the two for dynamic interplay.

---

### Special Module Suggestions (for tòna-based systems)

- **Instruō Scíon** – Biofeedback CV generator; great for organic FM or fold modulation.
- **Mutable Instruments Kinks** – Utilities for logic, rectification, great for modulating tòna in creative ways.
- **Make Noise Mimeophon** – Stereo delay/looping; combines brilliantly with tòna’s harmonically rich outputs.

---

## Pro Tip

Tòna’s wavefold output is “folded sine”—run this to a resonant filter for spectral sculpting, or to a delay for overtone layering. Try feedback patches looping folded output through reverb/delay and back into wavefold CV for self-generating soundscapes.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)