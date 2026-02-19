# 2hp — Pitch

- [Manual PDF](../../manuals/2hp_Pitch.pdf)

---

[2hp Pitch Manual PDF](https://2hp.com/wp-content/uploads/2020/12/2hp_Pitch_Manual.pdf)

---

## Using 2hp Pitch for Complex, Densely Rhythmic Percussion in Eurorack

**2hp Pitch** is a time domain pitch shifter with integrated "wow & flutter" (W&F) effects. Though primarily used for transposing signals and tape-like effects, you can leverage its feature set to create unique, punchy, and percussive textures—ideal for modern, micro-edited, hyper-complex rhythm music.

Below are strategies to make the most out of this 2hp effect in pursuit of intricate percussive patterns and polyrhythmic madness.

---

### 1. **Percussion Layer Enhancement via Pitch Shifting**

- **Feed drum or percussion voices** (such as kicks, hi-hats, glitches, foley, or physical modeling percs) into the `Audio Input`. 
- Use the **Pitch Knob and 1V/OCT Input** to transpose or modulate the sound. Rapid, clock-synced, or trigger-driven pitch modulation creates stuttering, ratcheting, or evolving timbral changes.
    - **Complex rhythms:** Use a polyrhythmic CV sequencer to drive 1V/OCT, 'retuning' each percussion hit differently in various time divisions.
    - **Modulate pitch with rhythmic LFOs:** Use multiplyable clocked LFOs, fed into the 1V/OCT input, at different polyrhythmic intervals.

---

### 2. **Pseudo-Tape Effects for Percussion Manipulation**

- Use the **W&F Knob** or input random CV via `W&F CV Input` to add random fluctuation/tape instability.
    - **Per-cussion punch:** Hard, quick modulation at rhythmically relevant moments (e.g. via fast, stepped random or S&H synced to triggers) can make each percussion hit slightly different.
    - **Swing/syncopation:** Use `W&F` with clocked but offset CV sources to introduce subtle off-grid timing and pitch artifacts, especially interesting with hi-hats, shakers, or FM percussion.

---

### 3. **Mix/Shaping per Hit for Dynamic Rhythm Complexity**

- The **Mix CV Input** allows dynamic blending between dry (original) and wet (pitch-shifted) signals. Patch a rhythmic CV source (clock divider, burst generator, trigger sequencer) into Mix CV.
    - **Patterned accents:** Use Euclidean or polyrhythmic gates as Mix CV for intricate patterns of “dry” and “wet” sounds throughout a bar, almost like automated send FX.
    - **Morphing timbres:** Automate Mix knob in time with your complex rhythm structures to add 'ghost' or shadow hits, echoes, or slurred effects.

---

### 4. **Advanced Patch Ideas**

- **Dual Pitch:**
    - If you have two percussion voices (or split a mono signal), run one through Pitch at +7 semitones, the other at -5, and recombine. Layer patterns for stacked, "digital polyrhythm" percussion lines.
- **Feedback/Buffer Hacks:**
    - Feed the output back to the input via a CV-controllable VCA for glitchy, unpredictable patterns. Wet signal detuning + feedback + W&F = complex, ever-changing digital percussion clouds.
- **Combo with Your Sequencer:**
    - Use a trigger sequencer (modular or external) to generate uneven divisions (e.g. 5/8, 7/16), and use these as CV sources for Pitch and Mix for polymetric movement.

---

### 5. **Make it Hyper-Modern and Punchy**

- **Sharp, Sync’d CV:**
    - Use stepped, quantized random CV (like a Turing Machine or Sample & Hold) into the 1V/OCT or W&F input, clocked by your master rhythm or at divisions thereof.
- **Accentuation:**
    - Accent certain hits by automating pitch jump (e.g., suddenly +2 octaves on every 9th step), or quick, harsh W&F burst on off-beats.
- **Chop and Glitch:**
    - Send granulated, micro-edited patterns into Pitch, modulate heavily, and crossfade fast between dry and wet for “granular drum machine” effects.

---

### 6. **In the Larger Patch**

- **Feed** micro-edited loops, glitch buffers, or sample-sliced drum kits (e.g. from sampler modules) into Pitch.
- **Combine** with sequential switches, logic, or complex gate processors to drive CV inputs in ever-shifting, polyrhythmic architectures.
- **Record** the output into a buffer/looper (e.g., 2hp Loop) for evolving, fractal-sounding percussion beds.

---

**Key Principles:**
- Treat 2hp Pitch as a rhythmic tool, not just a pitch shifter.
- Modulate everything with rhythmically interesting CV.
- Combine with clocked, random, or step-sequenced sources for non-repetitive drumming.
- Layer processed (wet) and unprocessed (dry) percussion for syncopation and drive.

---

**Continue reading the full manual:**  
[2hp Pitch Manual PDF](https://2hp.com/wp-content/uploads/2020/12/2hp_Pitch_Manual.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)