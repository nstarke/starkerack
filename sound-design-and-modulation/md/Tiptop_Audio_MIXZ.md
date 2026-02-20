# Tiptop Audio — MIXZ

- [Manual PDF](../../manuals/Tiptop_Audio_mixz.pdf)

---

[Tiptop Audio MIXZ Manual (PDF)](https://tiptopaudio.com/manual/MIXZ_Manual_Web.pdf)

---

## Creative Modulation & Sound Design With Tiptop Audio MIXZ

The Tiptop Audio MIXZ is a **low-noise dual mixer** with the innovative Tiptop Bus Mix system. While the MIXZ is primarily a flexible, clean analog mixer, there are a number of creative ways to use its routing and gain-staging features to shape and distort sounds, glue together harsh percussive elements, and design heavy basslines or spooky textures.

Below are approaches and tips for three sound design goals, using modulation, gain-staging, and creative patching techniques:

---

### 1. Distorted Percussive Sounds

**Goal:** Gritty, hard-hitting drums for techno, breaks, DnB.

#### Techniques & Patch Ideas:

- **Gain Overdrive:** 
  - Crank the channel gain controls for Mixer A channels with your drum sound sources (e.g., Tiptop BD909, SD808, or external drum modules or samplers).
  - Increase gain until you hit the internal headroom, causing saturation or clipping. MIXZ is designed for clean mixing, but pushing the analog circuit can yield subtle analog distortion.

- **Cascaded Mixing/Feedback:**
  - Take MIXER A’s output and patch it into an external distortion or wavefolder, then return it into a MIXER B channel for parallel dry/wet blending.
  - Alternatively, try patching MIXER B’s output back into a MIXER A channel *very gently* to create internal feedback distortion (be careful with levels!).

- **CV Over Audio (AM/Distortion):**
  - Use one channel for audio, another for a slow LFO or high-velocity envelope, and mix both. The CV input will amplitude-modulate the audio, adding AM/ring-mod style artifacts.

- **Bus Mix Layering:**
  - Selectively enable only certain drum modules on the Bus Mix, then flip the BUS MIX switch on MIXZ to layer multiple drum hits internally—this concentrates their signals and increases natural bus "grunge" and glue.

- **Noise Exploitation:**
  - Some modules (like the CP909) introduce noise into the Bus Mix. Crank their levels up for noisy, distorted snare or hi-hat artifacts. Use this controlled noise for crunch.

---

### 2. Dubstep/Drum & Bass Basslines

**Goal:** Heavy, modulated, aggressive bass with movement and character.

#### Techniques & Patch Ideas:

- **Oscillator Layering:**
  - Patch different oscillators (e.g., two Z3000s as in the manual’s example) into Mixer A’s channels for detuned, thick basses.
  - Use Mixer A’s gain controls and pan them before a filter (like the Z2040), then run into Mixer B for final summing.

- **Mixer CV as Sidechain/Mod Source:**
  - Insert a fast envelope or LFO into a Mixer A or B channel along with your oscillator. The modulation can cause amplitude spikes/distortion when mixed with audio, producing dirty bass growls.
  - Set up a dummy channel with the mixer turned up and feed it sharp attack CV to “sidechain” other parts as they mix.

- **Saturation & Headroom Tricks:**
  - Use the Bus Mix to add several sub-bass sources and push the overall level into the mixer's max headroom for analog saturation/clipping.
  - Use a filtered noise (high-resonance bandpass) on one channel and mix it with raw bass for "reese" or movement.

---

### 3. Haunting Atmospheric Pads

**Goal:** Deep, evolving textures and haunted ambient sounds.

#### Techniques & Patch Ideas:

- **Layered Textures:**
  - Mix several slow-moving sound sources/pads (e.g., complex oscillator, filtered noise, granular synth outputs) via Mixer A and/or B.
  - Use Mixer B’s master gain to gently balance everything without clipping.

- **CV + Audio Blends:**
  - Mix slow LFOs, envelopes, or random voltages into Mixer B along with pad audio signals. This subtle CV bleed can randomize amplitude, creating evolving drone beds or tape-like “flutter.”

- **Bus Mix Ambient Bus:**
  - Enable several subtle ambient sources at low level on the Bus Mix, then fade in via the Bus Mix switch on Mixer B. Sudden ghostly layers and drones can be introduced or removed “hidden” from front-panel jacks.

- **Reverb/FX Routing:**
  - Run Mixer B’s output into a stereo reverb or delay (like Tiptop’s Z-DSP), with slow, cross-mixed pads, for lush textures.
  - Use unused mixer channels for feedback loops into effects—patch FX returns into open Mixer A/B channels and regulate with mixer level.

---

## Modulation Bonus Tips

- **Use External VCAs/Envelope Generators:** While MIXZ itself is passive on the CV side, using the mixer post-VCA makes it easier to amplitude-modulate or CV-mix signals.
- **Feedback Abuse:** Looping mixer outputs back into their inputs (with caution) can create otherworldly, aggressive, or unstable modulated sounds.
- **Extreme Layering:** The Bus Mix allows you to stack many voices with minimal cabling—selectively enable noisy, atonal, or non-musical sources for evolving soundbeds.

---

## Reference/Manual

- [Tiptop Audio MIXZ Manual PDF](https://tiptopaudio.com/manual/MIXZ_Manual_Web.pdf)
- [Tiptop Audio Website](https://tiptopaudio.com)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)