# Mutable Instruments — Plaits

- [Manual PDF](../../manuals/Mutable Instruments - Plaits.pdf)

---

[Plaits Official Manual (PDF)](https://mutable-instruments.net/modules/plaits/manual.pdf)

---

# Creative Modulation Techniques for Mutable Instruments Plaits

Mutable Instruments Plaits is an eminently versatile macro-oscillator that thrives on creative modulation. Below, you'll find practical patches and patching strategies to help you coax **distorted percussive sounds**, **crazy basslines** (à la dubstep or drum and bass), and **haunting atmospheric pads** from Plaits, using CV and modulation.

---

## 1. Distorted Percussive Sounds

### Patch Ideas

- **Model Selection:**  
  Use the **second bank** of models (activated with the right button) for noisy and percussive synthesis algorithms—things like the *Kick, Snare, Hi-hat, and Metallic modes*.
- **Distortion through Harmonics/Timbre:**
  - **HARMONICS** often controls overdrive, attack sharpness, or the mix of harmonic/noisy content (especially in drum models).
  - **TIMBRE** typically sweeps brightness, sample rate, or decay sharpness—use extreme settings for punch/overdrive.
  - **MORPH** adjusts decay or mode blends; fast modulation here creates glitchy, broken textures.
- **CV Modulation:**  
  Patch envelopes to **TIMBRE** and **MORPH** for snappy, dynamic percussive punches.
  - Use a sequencer or random generator to the **MODEL CV input** for morphing drum sounds per hit.
- **Internal Envelope for Extra Grit:**  
  If not using external CV, set the **CV attenuverters** past 12 o’clock. The internal envelope will modulate the parameters, adding evolving distortion and movement.
- **Aux Output:**  
  The **AUX** output on drum models often offers an alternative, more aggressive drum synthesis—combine with OUT and use both for layered/complex drums.
- **Patching Ideas:**
  - Route Plaits OUT into a dedicated wavefolder, distortion, or bitcrusher module for even more wildness.
- **Feedback:**  
  Take the AUX out and process it through an external effect (like overdrive or analogue filter), then re-introduce some of that signal as audio-rate FM to **FM input** or use as a sidechain source.

---

## 2. Dirty, Crazy Basslines (Dubstep/Drum & Bass Style)

### Patch Ideas

- **Model Selection:**  
  Choose models like *Virtual Analog, Wavefolder, FM, or Granular Cloud* for bass.
- **V/Oct Sequencing:**  
  Use a CV/gate sequencer or an arpeggiator through the **V/OCT** input to get classic bassline motion.
- **Wobble & Modulation:**
  - **Massive Dubstep Wobble**: Patch a synced LFO (or envelope generator with a long decay and fast attack) into the **TIMBRE** or **MORPH** CV inputs. Open the attenuverters for deep parameter sweeps.
  - **FM Grit:** At audio-rate, send another oscillator or the internal AUX output into Plaits' FM input for brutal, syncopated grit.
  - Use quantized random/LFOs on **HARMONICS** for unpredictable bass movement.
- **Distortion/Resonance:**
  - Use models that are easily driven to gnarly territory, such as *Noise, Metal, or Granular* algorithms.
  - Push the **HARMONICS** and **MORPH** parameters hard to access brash or resonant peaks.
- **Combo Output:**  
  Blend the OUT and AUX signals for stacked, wide bass. Center OUT, AUX left/right for stereo spread.

---

## 3. Haunting Atmospheric Pads

### Patch Ideas

- **Model Selection:**  
  *Additive, String, Chord, Wavetable, Or Formant* models create lush, evolving harmonic textures.
- **Slow Modulation:**  
  - Use a pair of cycling LFOs, very slowly modulating **TIMBRE** and **MORPH** for spectral movement.
  - Subtle pitch modulation from sample-and-hold LFO on **FREQUENCY** or **V/OCT** for drifting pads.
- **Granular Models:**  
  - Clouds/grain models with high grain overlap (MORPH fully CW), low HARMONICS for density.
- **Envelope/LPG:**
  - Use Plaits’ **internal LPG** in VCF mode (see settings) for organic decay and filtering.
  - Patch slow envelopes to **LEVEL** and **FM** inputs for movement.
- **Spatial FX:**
  - Feed Plaits outputs to stereophonic delays, reverbs, or shimmer modules to bathe in space.
- **Chord Model:**  
  - Select chord type with **HARMONICS**, change inversion/transpose with **TIMBRE**, and scan through waveforms with **MORPH**.
  - Subtly animate these via CV for pads that shimmer and shift timbrally.

---

## Tips & Advanced Tricks

- **Attenuverters:**  
  Use the onboard attenuverters to dial in just the right amount of modulation from CV for each parameter. After tweaking modulation, reset to 12 o’clock if you want the internal envelope to take over.
- **Model Morphing:**  
  Send stepped/random or smooth CV to the MODEL input, for evolving or glitchy blends between different synthesis engines (ex: drum to synth, synth to pad).
- **FM and Audio-rate Modulation:**  
  Run fast LFOs or even external oscillators into the FM input for wild, audio-rate timbre changes, especially effective in FM/wavefolder models.
- **Envelope Follower:**  
  Route external audio through an envelope follower and use the extracted envelope to modulate Plaits for reactive, dynamic sounds.

---

## References

- **[Plaits Official Manual (PDF)](https://mutable-instruments.net/modules/plaits/manual.pdf)**
- **[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**

---