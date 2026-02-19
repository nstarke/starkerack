# Industrial Music Electronics — Piston Honda

- [Manual PDF](../../manuals/phmk3manual11.pdf)

---

[**Download the Industrial Music Electronics Piston Honda Mark III Manual (PDF)**](https://www.industrialmusicelectronics.com/manuals/Piston_Honda_MK3_Manual_Firmware_1_1.pdf)

---

# Using Piston Honda MK3 for Densely Rhythmic & Hyper-Complex Percussion

Piston Honda MK3 is primarily a dual wavetable oscillator, but given its extreme flexibility, CV addressability, morphing features, and preset morphing, it can be weaponized for advanced, percussive, rhythmically dense music—especially within Eurorack environments. Below are both **general strategies** and **patching specifics** for achieving polyrhythmic, complex, and punchy percussive voices using this module.

---

## Quick Recap: Percussive & Rhythmic Sound Design Features

- **Two digital oscillators** each with 3D morphable wavetables.
- Each oscillator has dedicated CV over frequency, waveform (X/Y/Z), FM, and mode.
- CV-controllable preset morphing and memory for 8 presets, which enables abrupt or smoothly shifted rhythmic changes.
- Nonlinear tone/distortion modes for extra punch or lo-fi grit.
- Audio-rate (thru-zero) FM and dynamic external signal processing.
- Locking and independent control for X/Y/Z morphing.
- MicroSD for custom wavetables—easy integration of percussive transients.

---

## Percussion & Rhythm Strategies

### 1. **Percussive Voice Programming**

- **Use One Oscillator Per Drum Voice**: Assign Osc A as your “kick/snare/bass” oscillator, Osc B for “hat/percs/metallics.” This allows layering and splitting via the Mix outs.
- **Wavetable Selection & Morphing**: Create custom wavetables emphasizing sharp attacks or percussive transients using **WaveEdit**. Use the X/Y/Z morph for subtle to extreme timbre changes under voltage control.
- **Disable Morphing for Glitch/Transient Attacks**: In the OSC MENU, disable morph on selected axes for “glitchy” instantaneous jumps between waveforms—encourages noisy, percussive, and digital transients.
- **Preset-scope Morphing for Rhythmic Macro Changes**: Use the **preset manager** as a rhythmic performance tool:
  - Sequence the preset CV input with stepped random, clocked, or polyrhythmic sequencers.
  - In **Morph Mode,** smoothly interpolate between drum timbres or complete percussion kits with CV.

### 2. **Rhythm, Polyrhythm, and Trigger Interaction**

- **CV Sequencing on X/Y/Z and Frequency**: Use multiple gate/trigger sequencers (e.g., Euclidean, probability, clock dividers) to modulate individual axes and frequency inputs.
  - E.g., Send a fast clock to X, multiply slower variations on Y and Z for polymetric timbre evolution.
- **Audio-rate FM**: Use the second oscillator, or external percussion or click sources, to FM the main oscillator. The normalled FM routing means you can have mutually interacting percussive FM without repatching.
  - Short envelopes (transient “plucks”) into FM create percussive “clang” or metallic drum sounds.
- **Sync Inputs for Hard-Hitting Attacks**: Use rhythmic triggers into SYNC for hard transient resets—especially effective for snares, rimshots, hats.

### 3. **Complex Modulation & Pattern Generation**

- **Preset Trigger as a Polyrhythmic Pattern Fader**:
  - In Global Options, set Preset CV to **TRIG + OFFSET**. Clock/trigger inputs then scroll through rhythmic “kits” or drum states. Use offset for accent/variation.
  - **TRIG RANDOM** mode can scramble percussion on every hit!
- **Nonlinear Attenuverter Response**: Fine-tune CV ranges for X/Y/Z to allow just a touch or wide swings with external envelopes, random voltages, Euclidean patterns, or probability-based LFOs.
- **Editable Tone (Distortion)**: For unique, punchy hits, engage the “tone” menu’s different nonlinear “vintage”/quantized/distorted curves—especially for snares, hats, and digital rim claps.

### 4. **External Input Abuse**

- **Waveshaping External Rhythms**: Route external percussion loops, clicks, or even other drum modules into FM/External In. The wavetable will dynamically reshape those signals, creating glitchy, metallic, or otherworldly percussion textures.
  - E.g., Send a noise burst or fast clocked envelope in—modulate what “file” is chosen on Z; create rhythmic “granular percussion kits.”
- **Feedback/Unstable Modes**: Set both oscillators to EXT IN but don’t patch an external audio source: the normalled routing will create chaotic, abrasive digital noise bursts—great for occasional “noise hits” in extreme rhythm tracks.

### 5. **Layering and Polyphony**

- **Oscillator Link for “Drum Chords”**: Use oscillator Link mode for staggered, slightly detuned percussive stacks (e.g., for clap or snare layering). Modulate fine-tune with CV/gate for pulsewidth-like or acoustic phasing effects.

---

## **Example Patch Recipes**

**A. “Polyrhythmic Metallic Kit”**
- Osc A: Custom wavetable designed for clangy, metallic attack (one axis, e.g. X, is a set of metallic partials).
- Osc B: Different wavetable—short digital clicks/noise.
- Fast clock on A's X morph, slower divided clock on Y morph, random stepped CV on Z.
- Envelopes into Osc A/B’s frequency for “hit”/body, FM input for transient snap.
- Both outputs to a rhythmically gated VCA or directly to mixer.

**B. “Randomized Snare Generator”**
- Set Preset CV to TRIG RANDOM.
- Clocked trigger to Preset CV In.
- Each trigger generates new snare/drum sound.
- Attenuator determines how “far” presets jump.
- Use tone menu for crush/bit reduction.
- Output to fast envelope-VCA for envelope-shaped percussion.

---

## **Pro Tips for Uniqueness & Punch**

- **Extreme Sample-CV**: Use stepped random or complex LFOs into morph axes for intense, rapid mini-percussion changes.
- **Envelope Follower** an existing drum sample, use its output to CV X/Y/Z or morph presets for responsive “meta-drumming.”
- **Sync Everything**: Send the same trigger/gate to multiple inputs (FM, Sync, preset change), so that every hit is a new sound.
- **Mult the module outputs**: Layer the Piston Honda with other drum modules, or use as the source into comb or wavefolder modules for further grit.

---

## **Summary Table**

| **Feature**        | **Percussive/Rhythmic Strategy**                        |
|--------------------|--------------------------------------------------------|
| X/Y/Z Morph CV     | Polymetric, random, or step-sequenced wave morphs      |
| FM/Sync Inputs     | Use for sharp transients & metallic/atonal drum impact |
| Preset Manager     | Advance or morph drum sounds per rhythm event          |
| EXT IN             | Waveshape other drums, clicks, or noise                |
| Tone Menu          | Add crispness, digital edge, or vintage bite           |
| Unison/Link        | Layer multiple "hits" or voices                        |

---

For further exploration, see more patch ideas and discussion at the [official thread on ModWiggler](https://modwiggler.com/forum/viewtopic.php?f=16&t=205585) and the [WaveEdit community](https://synthtech.com/waveedit/).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)