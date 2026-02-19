# Intellijel — MultiGrain

- [Manual PDF](../../manuals/multigrain_manual_v1.2_2025.09.02.pdf)

---

[**Intellijel Multigrain v1.2 — Manual**](https://intellijel.com/wp-content/uploads/2025/09/Intellijel-Multigrain-Manual-v1.2.pdf)

---

# Creative Eurorack Patch Ideas With Intellijel Multigrain

The **Intellijel Multigrain v1.2** is a next-generation, live stereo morphing granular sampler perfectly suited as the focal point of experimental, textural, and performance-based modular systems. Let’s dive into creative applications and inter-module pairings that unleash Multigrain’s full potential.

---

## 1. Live Granular FX Chain for Instruments & Modular Voices

**Workflow:**

- Use one or more channels of **Intellijel Multigrain** as Live Sounds, processing inputs in real time.
- **Feed source:** Acoustic instruments (mic’d), electric guitar/bass (via Intellijel’s HiFi I/O, Strymon AA.1, or Befaco Instrument Interface), or synth voices.
- **Send audio back out** post-processing for further external processing or reinforcement (e.g. via a stereo mixer with an effects send/return loop).

**Why?**
- Process audio through Multigrain’s Live Grain Engine, enabling evolving granular effects, freezing, and mutation with voltage control.
- Insert granular textures _after_ direct instrument input, for creative live ambient processing.

---

## 2. Granular Drum Layering & Electroacoustic Percussion

**Workflow:**

- **Load multi-sample percussion libraries** or drum stems into various Sound slots.
- Modulate grain Rate, Size, and Pitch via triggers/LFOs/randoms for glitch or swung rhythm.
- **Pairing:** Mutable Instruments Grids, Numeric Repetitor, or euclidean sequencers can sequence the GATE/NEXT/TRIG inputs for rhythmically controlled granular playback.
  
**Bonus:** Use morphing between Scenes A and B for per-step parameter morphing—think constantly shifting timbres with rhythmic CV addressing.

---

## 3. CV/Gate Sequencing & Sound Morphing

**Workflow:**

- **CV-address Sounds** using Select input (0–5V for Sounds 1–8), sequencing phrases and textures.
- Use **precision CV sequencers** (like Intellijel Tetrapad/Tête, Make Noise Pressure Points, or Malekko Voltage Block) to automate Scene morphs or grain parameters.
- Modulate the Morph fader (or Morph CV input) rhythmically for dynamic transitions.

**Creative Tip:** Animate Morph with function generators or random LFOs (Make Noise Maths, Stages, Buchla 281e) for organic scene blending.

---

## 4. Advanced Modulation: Attenuvert Everything!

**Workflow:**

- **Feed modulation sources** (random, LFOs, envelopes—e.g., ALM Pamela’s Pro Workout, Xaoc Zadar, or even pitch CV) into X/Y/Z modulation ins.
- Attenuvert and assign to unique parameters per Sound/Scene Random, Rate, Size, and Pitch for every new grain.

**Creative Variation:** Patch a **self-generated random** trigger (Noise Tools, SSF Ultra-Random Analog) to either humanize or introduce sudden timbral shifts.

---

## 5. Feedback, Resampling, and Recursive Granular Textures

**Workflow:**

- **Patch OUT L/R** back to IN L/R via a VCA or mixer to create controlled feedback.
- Enable resampling mode—Multigrain's internal recorder then captures the output, creating hall-of-mirrors, self-generative granularity.
- Pair with a mixer like Intellijel Mixup or Befaco Hexmix for blend/attenuation.

**Pro Tip:** Insert a filter, VCA, or distortion (e.g., Erica Pico DSP, Happy Nerding FX Aid) **in the feedback loop** for effect-ridden “granular clouds.”

---

## 6. Creating Ambient Soundscapes With External Effects

**Workflow:**

- Use Multigrain as a **granular source**, then route OUT L/R into rich external effects chains: Strymon Magneto, Make Noise Mimeophon, Happy Nerding FX Aid XL, or even external pedals (via an output interface).
- Use Multigrain’s Blur (reverb send) for initial atmosphere, then stack spatialization or tape delay.

---

## 7. Polyphonic/Layered Granular Voices

**Workflow:**

- Assign different vocal, synth, or instrument samples to multiple Sounds.
- Trigger multiple grains simultaneously using different GATE/NEXT/SELECT inputs.
- **Sequence multiple CVs** or triggers (from René, Pam’s, or Voltage Block).

**Optional:** Cross-fade between polyrhythmic granular streams by modulating BLUR/TONE/PITCH per row for immersive stereo imaging.

---

## 8. Performance Macros & Morph Automation

**Workflow:**

- Map MORPH CV to foot pedals (via Intellijel Pedal I/O), MIDI-to-CV converters, or fader banks for hands-free, gestural scene morphing.
- Use external controllers (like Planar2, Tetrapad, Soundmachines LS1 Lightstrip) to sweep between scenes, triggering “macro” sound changes in a live set.

---

## 9. DIY Granular Sampler/Looper

**Workflow:**

- Use the Looping Recorder mode as an 8-32 second looper, capturing external sources on the fly.
- Freeze/auto-freeze grains in performance, with a clock or input threshold.
- Combine with a looper pedal or sampler for recursive time-based layering.

---

## 10. Intellijel Multigrain + Video Synthesis

**Workflow:**

- Multigrain’s assignable MOD outputs (A/B) can clock or cross-modulate video modules (like LZX Vidiot, LZX VBM, or Syntonie VU007/VCF).
- Use random mod sources, grain triggers, or envelope followers to animate visuals based on granular sound events—true audio/visual synthesis!

---

## Bonus: Integration With Alternative Controllers

- **Touch/MPE to CV:** Use converters like Polyend Poly, Endorphines Shuttle Control, or Expert Sleepers FH-2 with MPE devices (Sensel Morph, Linnstrument) to modulate Multigrain’s X/Y/Z for gestural granular performance.
- **Pedal Inputs:** Use external expression pedals to blend or freeze grains in real time.

---

## Pairing Highlights

- **Random/LFO:** ALM Pamela’s Pro Workout, Mutable Instruments Marbles, Xaoc Batumi, DivKid Ochd
- **Sequencer:** Intellijel Metropolix, Make Noise René, Malekko Voltage Block, Mordax Data (for shaped modulation)
- **Processing:** Mimeophon, FX Aid XL, Z-DSP, Strymon Magneto
- **Recorder:** 4MS Stereo Triggered Sampler, Expert Sleepers Disting MK4 (for capturing grains into further processing)

---

These techniques transform **Intellijel Multigrain** into a central brain for generative, performative, and experimental modular rigs. The ever-changing grain landscape, paired with creative CV control and modular effects, opens an endless world of sonic morphogenesis.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)