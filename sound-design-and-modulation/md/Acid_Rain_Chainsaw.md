# Acid Rain — Chainsaw

- [Manual PDF](../../manuals/Chainsaw_Manual_1.1.pdf)

---

[Chainsaw Stereo Super-Oscillator Manual (PDF)](https://www.acidraintechnology.com/_files/ugd/665d09_6b9cf7f51ad94824a3fcfcdbb989fca9.pdf)

---

# Creative Sound Design with Chainsaw Stereo Super-Oscillator

Below is an analysis of how to modulate the **Chainsaw** module for unique sound design, with a focus on **distorted percussive sounds**, **crazy basslines** (dubstep/DnB), and **haunting atmospheric pads**.

## Understanding Chainsaw's Modulation Capabilities

### Relevant Controls & Inputs

- **Detune Knob (4) & CV Input (6):** Controls spread of 7 waves per voice; modulate for density & movement.
- **Waveform Morph (5) & CV Input (7):** Fades all waves from saw to square. CV morphing is very expressive.
- **Linear FM Input (9):** Linear frequency modulation affecting all voices, up to 2kHz CV.
- **1V/Oct Inputs (8, 10, 12):** Individual pitch control per voice for polyphony, chords, or stacked intervals.
- **Stereo Outs (11, 13):** Waves distributed for wide image; use both or just one for mono.
---

## Sound Design Techniques

### 1. Distorted Percussive Sounds

- **Patch Ideas:**
    - Feed a sharp envelope (e.g., Maths, Function) to **Detune CV (6)** for a rapid detune burst. This creates metallic, punchy attacks as all waves move out of unison.
    - Morph the waves quickly: Envelope into **Waveform Morph CV (7)** for a snap from saw to square or reverse.
    - For *extra bite*, patch a high-frequency oscillator (audio rate) to **Linear FM (9)**—this can yield clangorous, noisy timbres with digital edge.
- **Tips:**
    - Use a VCA after Chainsaw and trigger it with a short envelope for sharp transients.
    - Post-process the output with aggressive overdrive and fast envelopes on a filter for more impact.

### 2. Crazy Basslines (Dubstep/Drum & Bass)

- **Patch Ideas:**
    - Voltage sequence to main **V/OCT input(s)** for pitch slides & glides.
    - LFO or envelope into **Detune CV (6)** for evolving, thick bass movement. Try modulating just a bit or exaggerated for slurred, chorus-like swarms.
    - Use an envelope or LFO to morph between saw and square via **Waveform Morph CV (7)**. Many dubstep basses are made by dynamically wavetable-scrubbing/morphing.
    - Audio-rate modulation (e.g., another VCO) into **Linear FM (9)** for "formant" and dysphonic textures.
- **Tips:**
    - After Chainsaw, patch through a low-pass filter with high resonance for “wub” sounds. Modulate cutoff with a fast envelope or synced LFO.
    - Experiment with stereo image by using both outs and panning/filtering each further downstream for a wall-of-sound effect.

### 3. Haunting Atmospheric Pads

- **Patch Ideas:**
    - Slow random voltages (Sample & Hold, Wogglebug, etc.) into **Detune CV (6)** and/or **Waveform Morph CV (7)** for drifting, evolving pads.
    - Use all three 1V/OCT inputs for stacked chords (root/third/fifth, etc.) and send smooth modulations to each for subtle pitch drifting.
    - Subtle LFO or slow envelope to **Linear FM (9)** for unstable, eerie textures.
- **Tips:**
    - Blend the stereo outs for a wide image; follow with reverb and delay for atmospheric washes.
    - Modulate detune slowly for a chorus-like shimmering pad.

---

## Patch Example Tables

| Sound Type     | In 6 (Detune CV)            | In 7 (Morph CV)           | In 9 (FM CV)            | 1V/Oct (8/10/12)    |
| -------------- | --------------------------- | ------------------------- | ----------------------- | ------------------- |
| Percussive     | Envelope: fast, sharp burst | Envelope: short spike     | Audio rate VCO          | Triggers > VCA      |
| Bassline       | LFO (medium/fast sweep)     | Envelope or LFO (rhythmic)| Audio/LFO rate for growl| Pitch sequence      |
| Atmospheric    | S&H or slow LFO             | S&H, multiple LFOs        | Slow LFO or S&H         | Triads/Chords       |

---

**General Tips:**

- **All mod inputs** are bipolar (±5V), so unipolar sources (like envelopes) may need offset for symmetrical morphing.
- **Linear FM** is great for subtle vibrato or intense, digital atonality.
- **Detune** can go from sweet chorus to metallic, detuned madness—try automating it with slow CV for pads or fast for percussive shimmer.
- For *maximum impact*, post-process Chainsaw's output with envelopes, distortion, filters, and spatial FX.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)