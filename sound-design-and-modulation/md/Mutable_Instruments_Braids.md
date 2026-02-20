# Mutable Instruments — Braids

- [Manual PDF](../../manuals/Manual - Mutable Instruments Braids Documentation.pdf)

---

[Mutable Instruments Braids Manual PDF](https://mutable-instruments.net/modules/braids/manual.pdf)

---

## Mutable Instruments Braids: Creative Modulation Tips

Mutable Instruments Braids is a powerful and versatile digital macro-oscillator. With 45 synthesis models and extensive modulation and CV capabilities, it’s a prime sound source for modern electronic music, especially for warped percussion, filthy bass, and eerie pads. Here’s how you can modulate Braids for maximum sonic impact:

---

### 1. Distorted Percussive Sounds

**Model Choices:**  
- **DRUM** (TR-808 metallic drum)  
- **KICK** (TR-808 bass drum)  
- **SNAR** (TR-808 snare)  
- **CYMB**, **BELL**, **PLUK**

**Modulation Techniques:**

- **TRIG Input:**  
  Use external gates/triggers (sequencer, clock divider) to excite physical models and fire envelopes. Set the TSRC (Trigger Source) to EXT for standard triggering or AUTO for self-triggering based on pitch changes.
- **Timbre & Color CV:**  
  Patch envelopes, LFOs, or stepped random sources into TIMBRE and COLOR to distort decay, brightness, or introduce glitch/artifacting. Fast envelopes = sharp, snappy hits; audio-rate signals = wild, bitcrushed/folder chaos.
- **FM Input:**  
  Patch in another percussion sound or fast random voltage (like a noised-up S&H) and set FM attenuverter for gritty, harsh transients.
- **AD Envelope (Internal):**  
  Use the internal Attack/Decay envelope generator to quickly modulate FM, TIMBRE, COLOR, or even output VCA (see |\FM, |\TIM, |\COL, |\VCA in Options). This adds dynamic shapes, movement, and snap to every hit.
- **Low Bit Depth (BITS)/RATE Reduction:**  
  Lower bit rate and sample rate produce crunchy, mangled transients and digital artifacts—ideal for lo-fi, industrial percussion.
- **SIGN Option:**  
  Enable for grungy distortion and unexpected waveform glitches.
- **CLOU/PRTC Granular Models:**  
  Modulate TIMBRE with gates or slow LFOs to smash textures from granular to dense, turbulent "grains".

---

### 2. Gnarly Dubstep/DnB Basslines

**Model Choices:**  
- **FM, FBFM, WTFM** (phase modulation, feedback, wild tonalities)  
- **/|/|-_-_, RING, VOSM, WTx4, HARM, WTBL** (aggressive, harmonically rich)  
- **TOY, TWNQ** (digital filth and resonant mayhem)  

**Modulation Techniques:**

- **V/OCT Input:**  
  Sequencer for pitch, or even audio-rate oscillator for brutal, “FM-fusion” low-end movement.
- **FM Input:**  
  Route an envelope, LFO, or another oscillator here. Use bipolar modulation (FM attenuverter) for frequency “wobble” that’s essential in dubstep. Extremely short envelopes give “growl”; slow LFOs give classic wobble.
- **TIMBRE and COLOR Modulation:**  
  Assign envelopes or stepped random CV. Patch a slow LFO to TIMBRE and a faster one to COLOR—or vice versa. Modulate in opposite polarity for wild crossfades through heavy distortion or formant shifting.
- **Model Morphing (META mode):**  
  Assign a random stepped source, S&H LFO, or manual control via a fader or sequencer to FM input while META is on. Sweep across synthesis models mid-note for brutal, hybrid tones.
- **Signal Folding (FOLD Model):**  
  Modulate TIMBRE (wavefold strength) with envelopes or wobbly LFOs, and COLOR to switch between sine/triangle.
- **Twin Peaks (TWNQ):**  
  Self-modulation via high feedback and aggressive Q values achieves spitting, resonant bass.
- **WTx4 (Quad Voice):**  
  Use COLOR for chordal "spread" or heavy unison basses; dial in microtonal detuning for a "swarm" effect.
- **Embrace AlIasing:**  
  Intentionally run at low RATE (DAC sample rate) for aliasing harmonics and teeth-grinding distortion.

---

### 3. Haunting Pads & Atmospheres

**Model Choices:**  
- **ZLPF/ZHPF/ZBPF** (filtered analog emulations)  
- **WMAP, WTBL, WLIN** (rich wavetables)  
- **CLOU/PRTC** (granular, textural)  
- **VOWL, VFOF** (vocal-like, formant-rich)  
- **HARM** (additive pads), **RING** (FM shimmer)  

**Modulation Techniques:**

- **Slow Modulation:**  
  Use multiple LFOs or long envelopes patched to TIMBRE, COLOR, and FM. Drift between waveforms, filter shapes, and harmonic structures.
- **Granular Models (CLOU, PRTC):**  
  Modulate COLOR and TIMBRE with slow random voltages, or a joystick, for evolving, shimmering sounds.  
- **Meta Mode + Random CV:**  
  Morph pad textures by slowly sweeping the FM input (when META is on) through models, wavetables, or filter settings.
- **FM Sideband "Shimmer":**  
  Patch reverb tails, ambient drones, or external synths to FM for subtle, spectral shifting.
- **Internal Envelope:**  
  Use a long attack & decay envelope to modulate output amplitude or timbral position, creating swelling, morphing tones.
- **Formant Models (VOWL/VFOF):**  
  Use slow LFO on TIMBRE for vowel sweeps; COLOR to simulate "gender/age".  
- **Noise Models (NOIS, TWNQ):**  
  Crossfade outputs or modulate filter resonance to blur between synthetic "wind" and haunted resonance.
- **Brightness/Detune:**  
  Use FLAT and DRFT for gentle detuning and instability for old tape/vintage synthetic character.

---

## Additional Pro Tips

- **Self-Modulation:**  
  Mult Braids' output back to FM, TIMBRE, or COLOR for feedback chaos and self-organizing movement.
- **Meta-Model Randomization:**  
  Use stepped random CV or a random looping sequencer on FM (in META mode) for living, generative textures.
- **All Modulation is Additive:**  
  Knob positions and CVs combine—consider scaling/offsetting to hit the "sweet spots".
- **Attenuverter Mastery:**  
  Fine-tune modulation range and polarity for expressive, performance-ready sounds.
- **Combine with Distortion or Waveshaper Modules:**  
  Push already-twisted Braids output through analog distortion or wavefolders for extra grit.

---

[Mutable Instruments Braids Manual PDF](https://mutable-instruments.net/modules/braids/manual.pdf)

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
