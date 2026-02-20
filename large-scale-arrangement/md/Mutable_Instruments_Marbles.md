# Mutable Instruments — Marbles

- [Manual PDF](../../manuals/Mutable Instruments - Marbles.pdf)

---

[**Marbles Manual PDF**](https://mutable-instruments.net/modules/marbles/manual.pdf)

---

# Using Mutable Instruments Marbles for Full-Song Creation in Eurorack

Mutable Instruments Marbles is far more than a random generator—it's a performative sequencer and idea machine for modular musicians looking to realize **full-length, evolving songs**. Let’s analyze its capabilities and outline song-creation strategies in modular synthesis, addressing the challenge of progressing beyond a simple groove or loop.

---

## Key Marbles Songwriting Features

- **Random Gate & Voltage Generation**: Multiple clocked rhythm and melody channels.
- **Master Clock/Tempo Source**: Internal or external, with tempo-following.
- **Quantization and Smoothing of CV**: From random notes to repeatable scales/melodies, or even smooth, drifting modulations.
- **Looping & Shuffling (DEJA VU)**: Probabilistic repeats and novel variations for “parts” or sections.
- **Scale Programming**: Tailor musical scales by teaching Marbles your preferred notes.
- **External CV Remixing**: Transform existing sequences into new material on the fly.

---

## Song Structure Strategies with Marbles

### 1. **Section Creation with Deja Vu**
- Use **DEJA VU** to set a high probability of looping (e.g., 95%) on both X (melodies) and t (gates/rhythm). 
    - This captures a “section” of material (e.g., 8 steps) for verses/choruses.
    - Assign looped random CV to a melodic voice; tie gates to percussion.
- Fade DEJA VU to reintroduce randomness—this makes a great “B section,” fill, or break.

### 2. **Automatic Song ‘Scenes’**
- Sequence or manually change Marbles’ settings for:
    - **Scale (quantizer)**
    - **SPREAD & BIAS**
    - **Gate Duration**
    - **Steppiness/Slew**
- Use CV control for these paramaters (from sequencers, LFOs, or manual voltage) to morph textures and density, automating “scene” changes: intro, verse, chorus, bridge, outro.

### 3. **Multi-Channel Song Layers**
- **X Section (Random Voltages):**
    - X1: Melodic Line (quantized), sent to a voice or oscillator.
    - X2: Bassline (different range or quantization/scale).
    - X3: Wiggling modulator, sent to filter, effects, etc.
- **t Section (Random Gates):**
    - t1: Kick patterns.
    - t2: Snare/hats, comping, or FX triggers.
    - t3: Modulation triggers (scene change cues).
- This division helps build songs with fully-interlocked rhythm, bass, melody, and modulation.

### 4. **External CV Processing (Remix Existing Patterns)**
- Send CV from a step sequencer (e.g., a traditional bassline or melody) through Marbles’ external CV input.
- Use Deja Vu, quantization, spreading, and shuffling to “recompose” your sequence for alternate song sections, fills, transitions, or breakdowns—without programming new patterns.
- Route Marbles’ output to several voices for complex interchanges and variations.

### 5. **Transitional/Bridge Sections**
- Randomize clock division or multiply rate for instant tempo and pattern change (stutter, slow down, speed up, double time).
- Morph from quantized melodies to smoothed/lagged curves for ambient, textural bridges or fades.

### 6. **Global Structure via Presets/CV**
- Use external sequencers or preset storage modules (or MIDI-to-CV from a DAW) to automate changes in Marbles’ settings in time with your song’s structure.
- Example: Voltage-address Marbles’ BIAS or DEJA VU with scenes timed to a grid, for hands-off song structure.

---

## Combining Marbles with Other Modules

- **Voices/Oscillators**: FM, analog, wavetable, etc., for melody/bass.
- **Drum Modules**: Patch Marbles gates to kick, snare, hats, and percussion.
- **Filters/Effects**: Use Marbles’ CV for vivid, evolving FX.
- **Mixers/Crossfaders**: Blend “A” and “B” sections, or create DJ-like transitions.
- **Sequencers/Controllers**: Use Marbles for remixing, not for basic patterns, or cross-sequence with external step sequencers.
- **VCAs/Envelopes**: Animate voice levels, effects, or CV destinations.

---

## Example Song Structure Patch

1. **Intro:** Random rhythm and melody, high SPREAD, no loop, BIAS toward high notes.
2. **Verse:** DEJA VU loop, programmed scale, tight quantization (“step”).
3. **Fill:** Less loop, add jitter, slow clock division, more smoothing.
4. **Chorus:** New loop, higher density (BIAS), greater melodic range or faster gates.
5. **Bridge:** External sequence remixed, filter sweep modulated by X3.
6. **Outro:** Return to random, fade out with steppy to smooth sweep.

---

## Critical Tips

- **Record Everything:** Marbles excels at happy accidents that won’t reoccur.
- **Use CV Automation:** Automate changes to parameters with LFOs, scenes, or knobs.
- **Sample Sections:** Loop and rearrange sections externally if needed.

---

By leveraging Marbles’ **random looping, scale quantization, section mutation, and external CV remixing**, it becomes the core of a generative, narrative, and full-length modular song workflow.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)