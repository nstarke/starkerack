# Arcus Audio — Unity Mixer

- [Manual PDF](../../manuals/Unity Mixer - Arcus Audio.pdf)

---

**[Manual PDF - Unity Mixer (Arcus Audio)](https://arcusaudio.com/product/unity_mixer/)**

---

## Using the Arcus Audio Unity Mixer for Complex Rhythmic Eurorack Music

As a Eurorack modular musician seeking dense, hyper-complex percussion sequences—polyrhythms, odd time, and intricate patterns—the Arcus Audio Unity Mixer can be a vital utility module in your system. Below is how you might integrate it most effectively in your rhythmic experiments.

### Understanding the Module

**Key Specs:**
- **2hp**, dual 3:1 unity gain summing, or single 6:1 mixer
- **DC coupled**: processes audio and CV with equal fidelity
- **Bi-color LEDs**: visually monitor signal presence and polarity
- **Inputs**: Summing operation (no attenuation, pure sum)

**This is not a voice or effect processor**, but a high-quality utility for combining (mixing) signals—crucial for advanced patching.

---

## Creative Uses for Dense Rhythmic Percussion

### 1. Polyrhythmic CV/Trigger Mixing

- **Combine Multiple Trigger Streams:**  
  Mix three separate trigger/gate streams (e.g., from clock dividers, Euclidean sequencers, or trigger sequencers) into one output. Use the second mixer for another set.  
  *Example*: 5-step, 7-step, and 3-step triggers into a single percussion voice for unpredictable polyrhythm.

- **Layered Modulation Sources:**
  Mix multiple LFOs or envelope outputs (at various rates, phases, or shapes) into one modulation destination, e.g., filter cutoff, percussion module pitch, or VCA. This produces evolving, 'hypercomplex' amplitude or timbral modulation.

### 2. Summing Multiple Percussion Voices

- **Percussion Bus:**  
  Mix the outputs of several independent drum modules (e.g., kicks, hats, claps) into one mixer channel for parallel processing (e.g., feeding a VCA, filter, or effect). Use each mix out for separate drum groups—apply effects or sidechain to the whole group.

### 3. Rhythmic CV Interference & Logic Patch

- **Gate Masking:**  
  Mix clock, burst generators, 'random' gates, and regular triggers. The resulting sum can create erratic micro-rhythms. Use in conjunction with analog logic modules or S&H to extract complex triggers.

### 4. Combining Audio for Clicks, Ticks, and Noised Percussion

- **Audio Rate Summing:**  
  Patch sharp, short waveforms or noise bursts from several sources, sum them at unity gain to create new percussive textures—unique, digital-style ticks and noise bursts.

### 5. Complex Accent and Velocity Patching

- **Accent Bus:**  
  Mix several accent/envelope CVs to a percussion voice’s accent input. Use different rhythmic patterns for each envelope—resulting in varied velocity/emphasis per hit.

---

## Performance Tips

- **Bi-color LED Feedback:**  
  Instantly visualize signal polarity and level. Use this for troubleshooting your complex patterns, especially when dealing with CV inversion/phasing for stereo or performance effects.
- **Patch for Connectivity:**  
  At 2hp, the Unity Mixer lets you dedicate minimal rack space to a function you’ll use in nearly every complex rhythm patch—always keep it patched for experimentation.

---

**Summary Table**

| Patch Scenario               | Inputs                                                     | Output Application               |
|------------------------------|------------------------------------------------------------|----------------------------------|
| CV Polyrhythm Mix            | Clock/LFO/Random CV                                        | Modulate drum params             |
| Trigger Sum                  | Multiple gate/trigger sources                              | Drum voice trigger input         |
| Audio Percussion Layer       | Noise, sharp waveforms, clicks                             | New percussive sound             |
| Percussion Bus               | Several drum modules' outputs                              | FX processing, mixing            |
| Accent/Velocity Merge        | Varied envelopes/accents                                   | Accent input of percussion       |

---

**Link:**  
**[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**
