# Arturia — Keystep Pro

- [Manual PDF](../../manuals/keystep-pro_Manual_1_1_0_EN.pdf)

---

[Arturia KeyStep Pro User Manual (PDF)](https://downloads.arturia.net/products/keystep-pro/manual/arturia_keystep-pro_manual_en.pdf)

---

## How to Create Unique Modulation with the Arturia KeyStep Pro:  
**Distorted Percussive Sounds, Dubstep/Drum & Bass Basslines, and Haunting Atmospheric Pads in Eurorack**

As a dedicated Eurorack modular musician, modulating your synth voices is essential for injecting movement, character, and energy into your performances. The **Arturia KeyStep Pro** is a powerhouse for generating complex, performance-worthy modulation and sequencing. Here's how you can push your modular system into creative and extreme sonic territories with its advanced capabilities.

---

## 1. Creating **Distorted Percussive Sounds**

**Key Techniques:**
- **Drum Gate Sequencing**: Use Track 1 in Drum Mode to sequence up to 8 gate outputs for triggering percussion modules, drum voice modules, or triggering LPGs and VCAs with envelopes.
- **Gate Time Randomization**: Use the Randomness encoder in Step Edit mode to randomize the likelihood of each hit, creating skipping, glitchy, unpredictable rhythms.
- **Accent Through Velocity**: Map the Velo/Mod CV output to a distortion or waveshaper module's CV input, so strong strikes trigger harder distortion for punchy, aggressive results.
- **Advanced Polyrhythms/Polymeters**: In Poly mode, set different track lengths for drum triggers. This causes the percussion to phase and shift, yielding wild evolving patterns.
- **Modulate Sound Source Parameters**: Assign one of the main encoders to sequence CC# values mapped to filter cutoff, wavefolder gain, or drive parameters via MIDI→CV converters. This lets you automate gritty, resonant, or squelchy changes on every percussive trigger.
- **External Clock or Burst Modulation**: Use the Clock In to inject burst generators or complex clocks (from modules like Pamela's NEW Workout, Temps Utile, etc.) for time-warped, juttered effects.

**Patch Example:**
- Drum Gate Out 1 → Envelope → VCA controlling a metallic percussion sound.
- Velo/Mod Out 1 → Intellijel Bifold or Bastl Timber (wavefolder drive).
- Randomness: encoder up to 50-80% on key steps for glitch/skipping hits.
- Use SHIFT+Time Division for rapid, spiky rhythms.

---

## 2. **Dubstep/Drum & Bass Basslines**

**Key Techniques:**
- **Multi-Track Bass Control**: Split a heavy oscillator or voice (think: FM'd VCO into a lowpass filter with tons of resonance) between multiple tracks for layered basslines.
- **Sequence Steps with Overlapping Notes**: Use Poly mode to stack notes in a step for aggressive "stacked osc" effects.
- **Modulate Filter/Fold/Drive**: Route the extra Velo/Mod or CC# tracks to CV inputs on your filter or distortion/wavefolder modules. Automate cutoff sweeps, resonance, or distortion intensity step-by-step.
- **Envelope & LFO Groove**: Arpeggiators on Track 2-4 running in triplets or odd time divisions allow you to send CV to modulate the same or companion bass parameters for tight, wobbly syncopation.
- **Pitch/Mod Touch-Strips**: Live perform filter/pitch sweeps, sample-and-hold FX, or glide by assigning the pitch strip to modulate anything responsive to CV (like a PLL or MS-22 for twin filter chaos).
- **Randomness Encoder**: Create "machine-gun" rolls, gate ratcheting (short triggered notes), or varying probability for live, jittering bass rhythms.
- **Transpose + Scale Mode**: Play in a minor or Dorian scale, hitting Transpose as you perform for instant, key-corrected bass runs.
- **Slide/Glide Emulation**: Use long gate steps, time-shifts, or chained tied steps with overlapping notes.

**Patch Example:**
- Voice 1 Pitch Out → Complex VCO.
- Gate Out 1 → Envelope (for Freq/Resonance modulation on filter).
- Velo/Mod Out (set to aftertouch) → Filter CV input, automate grrrrrows.
- Use the Step Edit's Time Shift encoder for off-grid grooves.

---

## 3. **Haunting Atmospheric Pads**

**Key Techniques:**
- **Polyphonic Step Entry**: Enter lush, extended chords in poly mode on any sequencer track, then extend sequence length for slow-moving pads.
- **Rnd/Walk Sequence Directions**: Use SHIFT+Seq Pattern to evolve/obscure progression order; create generative unexpected pad evolutions.
- **Scale Quantization**: Engage Dorian, Mixolydian, or custom scales for modal, emotionally complex pads.
- **Modulate Pad Texture**: Use secondary tracks not as pitch CV, but as CC# modulation or Velo/Mod outputs patched to shimmer reverb/delay modules, warping filters, pseudo-random LFOs, granular engines.
- **Ribbon Looper**: Use the horizontal looper strip to spontaneously loop/hold chord snippets. In Control Mode, this can even send MIDI CCs to sweep through clouds or feedback.
- **Slow, Independent Division**: Let one track run an ambient pad with 64 steps, while another triggers subtle filter/ringmod modulation in a different time division.
- **Overdub/Advanced Step Edit**: Stack held notes, shift select notes in a chord, gently detune with the Pitch encoder, or offset their gates for evolving movement.
- **Ambient Percussion From Drum Sequencer**: Use the Drum Gates to gently "strike" LPGs patched with slow decay envelopes for shimmering, bell-like, or decayed gongs in the periphery.

**Patch Example:**
- Voice 1 Pitch/Velocity/Gate to stereo ambient voice (Rings/Clouds, ZDSP, Magneto).
- Voice 2/3/4 to additional voices or effects, with the CC track modulating reverb or delay time/freeze.
- Use the Step Edit feature to time-shift and randomize individual notes in the chord per step.
- SHIFT+Hold on arpeggiators for evolving, generative pad movement.

---

## **General Tips for Extreme Modulations**
- **Randomization (Per-Step and Global)**: The Randomness encoder is your best friend for generative, unpredictably modulated sequences, especially when used on both drums and melodic tracks.
- **Live Control**: Use the Mod and Pitch strips expressively during performance; assign their outputs dynamically to different functions using your modular system's matrix mixers or assignable CV attenuverters.
- **MIDI->CV Extensibility**: Don't limit yourself to just the four main CV outputs; with MIDI-to-CV modules (like Expert Sleepers, Yarns, or the Hermod), you can route KeyStep Pro's MIDI CC# tracks to modulate nearly any modular parameter.
- **Scenes and Patterns for Performance**: Build a bank of strange, evolving modulative patterns in KeyStep Pro, then use Scenes to recall elaborate, shifting worlds of sound mid-jam.

---

## Reference

- [Arturia KeyStep Pro User Manual (PDF)](https://downloads.arturia.net/products/keystep-pro/manual/arturia_keystep-pro_manual_en.pdf)

---

Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)