# Bored Brain — EQx5

- [Manual PDF](../../manuals/EQx5-UserGuide_1.0.pdf)

---

[eqx5 Boredbrain Voltage Controlled Equalizer Manual (PDF)](https://boredbrainmusic.com/wp-content/uploads/2023/10/eqx5-User-Guide-v1.0.pdf)

---

# Creative Eurorack Patch Ideas with Boredbrain eqx5

The **Boredbrain eqx5** is a powerful and flexible 5-band fully analog stereo equalizer designed for the Eurorack format. Its voltage-controlled bands, flexible routing, and visual feedback make it much more than just an EQ—think of it as a creative sound-shaping and modulation hub!

Here are some creative patch ideas and module combinations to spark your inspiration:

---

### 1. **Animated Spectral Filtering:**
- **What to use:** 5 LFOs (for example, Xaoc Batumi, or Make Noise Maths for two LFOs + slopes),** and stereo audio source (e.g., Mutable Instruments Plaits, stereo drum loop)
- **How:** Patch different LFOs to each frequency band CV input. Use different waveshapes and periods for evolving, swirling or rhythmically synced filter sweeps that animate across the spectrum.
- **Bonus:** Run the signal through a stereo reverb after eqx5 to enhance movement.

---

### 2. **Rhythmic Gating & Transient Shaping:**
- **What to use:** Envelope generator like Intellijel Quadrax or Pam's New Workout
- **How:** Patch drum transients or percussive envelopes to one or more band CV inputs. Use the input level into eqx5 to amplify the effect of dynamic gating—highpass for hats, lowpass for kicks, etc.
- **Bonus:** Sequence per-band envelope triggers for complex “dynamic slicing” of loops.

---

### 3. **Stereo Imaging Madness:**
- **What to use:** Stereo field recorder or stereo synth voice + VCAs (e.g., ALM Tangle Quartet) + eqx5
- **How:** Use eqx5’s independent left/right CV ins to modulate the bands differently per channel. Pan or automate the modulation for spectral imaging and pseudo-wide effects.
- **Bonus:** Send the left and right bands to different effects chains (e.g., delay left, reverb right) before mixing back together.

---

### 4. **Spectral Vocoding & Cross-Patching:**
- **What to use:** A modulator signal and a carrier signal (e.g., voice recording + pad), additional VCA for each band output if possible.
- **How:** Patch the output of envelope followers or comparators (e.g., Mutable Instruments Stages or Doepfer A-119) to the band CV inputs, using your modulator to “carve” the frequency spectrum of the carrier dynamically.
- **Bonus:** Sum or cross-patch left and right channels for unique cross modulation.

---

### 5. **Spectral Feedback Loops:**
- **What to use:** Delay module (e.g., Make Noise Mimeophon or Strymon Magneto)
- **How:** Run a stereo signal into eqx5, feed outputs into your delay, then use the delay’s feedback send back into eqx5 before returning to the main mix. Modulate the bands for shifting, evolving feedback flavors.
- **Tip:** Keep feedback just below self-oscillation for the wildest, but controllable results.

---

### 6. **CV-Controlled DJ-Style Breaks**
- **What to use:** Performance controllers (e.g., Faderbank, Planar2), sequencers, or a joystick module
- **How:** Manually sweep or sequence the band levels over loops, samples, or full mixes. Mute bands for “DJ kills,” automate with CV for repeatable, performable tricks.

---

### 7. **Spectral Sidechaining**
- **What to use:** Envelope follower + drum sidechain source
- **How:** Detect drum hits with an envelope follower, then invert and send this CV to lower frequency bands to carve space for the drum every time it hits—the modular’s own “multi-band ducking” compressor!

---

## Module Type Recommendations

- **LFOs**: Xaoc Batumi, Pamela’s Pro Workout, Maths
- **Envelope Followers**: Mutable Stages, Doepfer A-119, Endorphin.es Gateway
- **Sequencers/CV sources**: Make Noise Rene, Malekko Voltage Block, Intellijel Tetrapad
- **VCAs/Mixers**: ALM Tangle Quartet, Intellijel Quad VCA
- **Stereo Effects**: Strymon Magneto, Mimeophon, Erica Synths Black Hole DSP 2
- **Controllers**: Make Noise 0-ctrl, Intellijel Planar2

---

*Remember: eqx5 is more than EQ—it’s a sculptural, performative spectral tool!*

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)