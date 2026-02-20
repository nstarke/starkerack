# 2hp — Turing Machine

- [Manual PDF](../../manuals/TM_Manual.pdf)

---

[Download the 2hp TM Manual (PDF)](https://2hp.com/products/tm)

---

## Creative Use of the 2hp TM Eurorack Module  
The TM module is a compact, Turing Machine-inspired random voltage generator, letting you dial in continuous or locked random sequences. Below are ideas for modulating the TM to create the following sound types with examples for patching and external processing:

---

### 1. Distorted Percussive Sounds  

**Goal:** Use TM's stepped and evolving voltage sequences to trigger, shape, and distort percussion sources.

#### Patch Ideas:
- **Trigger random drum modules:**  
    - Patch a fast clock or gate to the TM `TRIG` input.
    - Use `OUT` to modulate the decay, pitch, or distortion amount on a drum synth (e.g., kick/snares). Insert TM’s random voltages into a VCA CV or distortion CV in.
    - Set `PROB` moderate (~50%) for semi-random results; for evolving breaks, automate `STEPS` (sequence length) with CV.

- **Voltage-controlled Distortion:**
    - Route TM `OUT` to control a wavefolder, bitcrusher, or distortion pedal/input.
    - Fast, short `STEPS` with high `AMP` will produce glitchy modulation.
    - Clock the TM with an audio-rate oscillator for audio-range random CV (for crunchy/sputtery distortion).

- **Granular-atmosphere Percussion:**  
    - Use a slow clock, short sequence (2–4 steps), and the `AMP` just above zero to subtly modulate reverb size/mix, delay time, or filter resonance on percussive sounds for lo-fi ambiance.

---

### 2. Crazy Dubstep/Drum & Bass Basslines  

**Goal:** TM generates ever-changing, stepped voltages driving growly, modulating bass sounds.

#### Patch Ideas:
- **Bassline Pitch & Timbre Generator:**
    - Mult a gate/trigger sequencer to the TM `TRIG` input (use the same gate as your main rhythm for synchronized random steps).
    - Use TM `OUT` to the 1V/oct or FM input of a bass oscillator, or as a wavetable index on a digital voice.
    - Set `PROB` 70-90% for an evolving pattern that sticks sometimes for that ‘wobble’ quality.
    - CV-control `AMP` and `STEPS` using LFOs or envelopes for morphing sequences and energy flow (swell into crazier patterns or lock them).

- **Modulate Effect Parameters for Growl:**
    - Run TM `OUT` into filter cutoff, distortion drive, or wavefolder amount.
    - For metallic bass, clock TM at high speed and set very short STEPS (1–3).
    - Experiment with post-TM quantizers set to minor or diminished scales for dark, aggressive basslines.

---

### 3. Haunting Atmospheric Pad Sounds  

**Goal:** Underlying unpredictably shifting voltages create evolving drones/textures.

#### Patch Ideas:
- **Slowly Shifting Textures:**
    - Set `TRIG` to a slow clock (less than 1Hz).
    - Long sequence (`STEPS` knob far right) and moderate `PROB` (~30%) ensure the pattern evolves without sharp bursts.
    - Patch `OUT` to subtle destinations: oscillator FM, wavefolder symmetry, reverb/delay feedback, or VCA amplitude CV.
    - Use `AMP` limiting for background lurches and slow tides rather than drastic jumps.
    - Mult out to several destinations—random stereo panning, evolving shimmer, filter sweeps, etc.

- **Artificial Lifeforms/Alien Voices:**  
    - Fast clock, short sequence, high PROB for stuttering modulation.
    - Route into granular synthesis or a wavetable morph input for glitchy, otherworldly atmospherics.

---

## Additional Tips:

- **External Modulation:**  
    TM CV inputs (`PROB CV`, `STEPS CV`) accept 0V–5V. Patch envelopes, LFOs, or sample & holds to these for dynamic, performable changes to randomness, locking, and sequence length on the fly.
- **Amplitude (`AMP`) as Texture Fader:**  
    Use an envelope on `AMP` for rhythmic, gated random voltages—e.g., pulsing random pads, noise bursts, or phased randomness.
- **Quantization:**  
    Running TM `OUT` into a quantizer produces in-scale, randomly evolving melodies or harmonies—useful for ambient, generative, and IDM music.

---

**Download the [2hp TM Manual PDF](https://2hp.com/products/tm) for further reference.**  
**Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)**