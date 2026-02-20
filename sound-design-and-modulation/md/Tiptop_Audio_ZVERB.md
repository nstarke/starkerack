# Tiptop Audio — ZVERB

- [Manual PDF](../../manuals/Tiptop_Audio_fx_manual.pdf)

---

[Full PDF Manual for Tiptop Audio ECHOZ / ZVERB / Z5000](https://tiptopaudio.com/manuals/ECHOZ-ZVERB-Z5000-Manual.pdf)

---

## Modulation Tips for Tiptop Audio ECHOZ / ZVERB / Z5000

These three effect modules are powerful sound manglers in Eurorack! All three modules are CV-controllable stereo multi-effects, distinguished by their algorithm banks—delays (ECHOZ), reverbs (ZVERB), and a wider multi-FX spread (Z5000). Here’s how to push these modules into unique territory, specifically for distorted percussion, wild basslines, and haunting atmospheres:

---

### 1. **Distorted Percussive Sounds**

- **High Feedback & Extreme Fidelity Mod:**
  - Crank the **FEEDBACK/MOD** knob and simultaneously reduce **FIDELITY** (turn left). The analog clocking will cause digital artifacts, degradation, and aliasing. With percussive sounds, this results in crunchy, destroyed reverbs or delays.
  - On **Tape Echo** or **Mono Tape Echo** programs, increasing feedback will saturate and self-oscillate. Turning up input gain can push the DSP into clipping, which is indicated by the **clipping light**; use this deliberately to add even more grit.

- **CV Modulation:**
  - Modulate the **FIDELITY** CV input with stepped or random voltages (sample & hold, random LFOs), ideally clocked to your beat. This introduces “bitcrushed,” pitch-shifting, and time-warped digital artifacts in time with your percussion.
  - Use short, snappy envelopes or triggers routed to the **TIME** or **FEEDBACK/MOD** CV inputs for machine-gun/repeat delay effects. Fast envelopes will punch the delay time, causing severe glitching and hard digital re-pitching.

- **Recommended Algorithms:**
  - **ECHOZ**: Short BBD, Mono Tape Echo, Wobbly Tape Echo, 3 Head Switch Echo (for metallic delays).
  - **Z5000**: Mono Tape Echo, Tape Multi-Head Blend.
  - **ZVERB**: Gated Reverb, Space Station, Gate.

---

### 2. **Crazy Basslines (Dubstep & DnB Flavor)**

- **Pitch-Shift Delays & Wild Feedback:**
  - Pick pitch-shifting delay patches such as **Mono Pitch Shift Delay**, **Chord Delay**, **Detuned Taps**, or **Dual Interval Delays**.
  - Use slow or audio-rate LFOs into the **TIME** or **FEEDBACK/MOD** CV inputs to create warbly, evolving sub-basslines or FM-like effects on bass riffs.
  - Modulate **FILTER** with an envelope or synced LFO to create moving formants or wah-type effects.

- **FIDELITY as a Weapon:**
  - Audio-rate modulation of **FIDELITY** can act as a brutal, digital down-sampling or ring-modulation effect. For “ripped” bass, try routing an oscillator or noisy LFO to the **FIDELITY** CV input.
  - Be careful: Negative CV to Fidelity may crash the DSP (as the manual notes). If it freezes, simply reload a program.

- **Stereo Tricks:**
  - Use “ping pong” or “chorus echo” modes for wide bass movement. Pan your bass dry signal center and wet left/right for stereo-extending.

- **Recommended Algorithms:**
  - **ECHOZ**: Mono Pitch Shift Delay, Chord Delay, Detuned Taps, Dual Microshift Delay.
  - **Z5000**: Stereo Flanger, Dual Microshift Delay, Warp Pong.
  - **ZVERB**: Downward Spiral, Shimmer Pitch Adjust, Pitch > Chorus.

---

### 3. **Haunting Atmospheric Pads**

- **Looooong Tails & Spaciousness:**
  - Choose super-long reverb or multi-tap delays like **Hall** (ZVERB and Z5000), **Void**, **Epic Mod Hall**, **Random Hall**, **Delay > Hall**, **Blooming**.
  - Modulate **TIME** with slow LFOs or random voltages for evolving spaces that bloom and contract organically.
  - Use **FIDELITY** CV with slow, gentle modulation for evolving, spectral changes and background shimmer/crunch.

- **Modulated Filters & Formants:**
  - Use **FILTER** for spectral motion—patch a shallow LFO or S&H for subtle movement, or an envelope follower from your sound source for dynamic spectral changes.
  - For ghostly, vocal pads: try **Formant Delay**, **Ahhhnsemble**, or **Formant Verb**—modulate filter for vowel sweeps.
  - For “shimmering” effects, use **Shimmer**, **Shimmer Taps**, **Shimmer Octave Up/Down**.

- **Feedback Clouds:**
  - High **FEEDBACK/MOD** settings will smear transients and create reverb/delay clouds. Try modulating **FEEDBACK** with very slow random voltages for unpredictable ambient swells.

- **Recommended Algorithms:**
  - **ECHOZ**: Multi-tap Diffuse Band Delays, Formant Delay, Shimmer Taps, Detuned Taps.
  - **Z5000**: Hall, Shimmer, Void, Shimmer, Stereo Chorus, Vintage Ensemble, Formant Delay.
  - **ZVERB**: Epic Mod Hall, Void, Downward Spiral, Formant Verb, Blooming, Pitch > Chorus.

---

### **General Modulation Routing Tips**

1. **Envelopes** to FEEDBACK/MOD and TIME for “pumping” or sidechain-like dynamic effects.
2. **LFOs** (slow = pad; audio-rate = mangled, broken digital artifacts) to any CV input.
3. **Random/Noise/S&H** to FIDELITY or FILTER for unpredictable, constantly shifting timbres.
4. **Audio-rate Oscillator** to FIDELITY for brutal digital scrambling, especially on bass and percussion.
5. **Multiple modulation sources** at low depths for complex, animated soundscapes.

---

**Key Manual Links:**
- [Full PDF Manual for Tiptop Audio ECHOZ / ZVERB / Z5000](https://tiptopaudio.com/manuals/ECHOZ-ZVERB-Z5000-Manual.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)