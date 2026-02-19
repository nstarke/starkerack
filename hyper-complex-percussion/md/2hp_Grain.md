# 2hp — Grain

- [Manual PDF](../../manuals/2hp_Grain_Manual.pdf)

---

[2hp Grain Manual (PDF)](https://2hp.com/manuals/grain.pdf)  

---  

## Creating Dense, Hyper-Complex Rhythmic Percussion With 2hp Grain

The **2hp Grain** is primarily a granular audio processor, capable of wild transformation of incoming audio into clouds, textures, and stuttered fragments. It's not a drum module by itself, but with creative patching and modulation, it can **transform ordinary or percussive sounds into complex and punchy rhythmic textures**, perfect for experimental and complex percussion.

### 1. Signal Source: Feeding Percussive Material
- **Input Percussive Sounds:** Use a drum machine, percussion sample player (e.g., 2hp Play), or analog drum modules as inputs. Short, snappy percussive material works best for punchy textures.
- **Layering Material:** You can feed breaks, metallic hits, or even acoustic recordings to create a dense starting point.

### 2. Rhythmic Complexity via Density & CV
- **Polyrhythmic/Complex Triggers:** Patch complex CV sources (e.g., clock dividers, polyrhythmic LFOs, Turing Machines, random sources, or trigger sequencers) to the **Density CV** input.  
- **What This Does:** Density CV directly modulates the rate and position of grain generation. Using clocks or bursts not aligned to the master tempo will cause Grain to "chop" and stutter your input buffer in wild rhythmic patterns.
- **Stochastic/Periodic Modes:** Turn the Density Knob left (periodic) or right (stochastic/random) for more regular or unpredictable grain rhythms.
- **Layer Multiple CVs:** Try mixing two or more rhythmic CV sources for even greater rhythmic complexity.

### 3. Using the Freq and V/Oct Inputs for Percussive Variation
- **Modulating Freq:**  
    - Patch stepped or random CV sequence to FREQ for pitch-variant percussion (e.g. every 4th hit shifts up, or random percussive scales).
    - Use an envelope or fast LFO here for chirps/punchy, percussive tone sweeps.
    - Remember: Higher Freq = smaller grains + faster grain rate = snappier, tighter textures.
- **V/Oct Input:**
    - If you want tuned percussion, patch a sequence here in sync or cross-rhythm to your main pattern for per-grain pitch changes.
    - Modulating this with clocked stepper sequencer can introduce melodic/rhythmic interplay.

### 4. Sculpting Punch & Uniqueness via Mix
- **Mix Knob / CV:**  
    - Automate the blend between dry input and granular ‘wet’ effect via the Mix CV.
    - Fast modulation here (e.g. audio-rate or stepped LFO) can create gating, stuttering, or ‘glitch’ rhythmic effects, sharply toggling between clean hits and granulated bursts.

### 5. Additional Pro Tips
- **CV Range Awareness:** Most CV inputs respond to ±5V; attenuate your sources for dramatic or subtle effects.
- **Buffer Abuse:** Feed in a single hit, then freeze/hold the input with the Density knob or corresponding CV so you’re re-granulating a tiny fragment. This can generate granular ‘machine gun’ effects.
- **Patching Feedback:** Mult the output back into the input (with attenuation/limiting!) for self-layering chaotic patterns.
- **External Clocking:** Use external, non-standard clocks (e.g., odd meters, polyrhythm sources) to fire grains and drive unpredictable patterns.

### Example Patch

1. **Audio Source:** Hi-hat loop → IN.
2. **Density CV:** Clock divider (3/8, 5/16, 7/8, etc. for polyrhythms) and random stepped CV summed → Density CV.
3. **Freq:** Envelope follower from percussion envelope, or periodically stepped random CV → Freq.
4. **Mix CV:** Fast LFO or trigger pulses (not synced to main clock) → Mix CV.
5. **Output:** To mixer, maybe through a compressor or transient shaper for maximum punch.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)