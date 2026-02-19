# Free Modular — Boost

- [Manual PDF](../../manuals/boost_manual.pdf)

---

[**Download the Boost Module PDF Manual**](https://github.com/nstarke/eurorack-processor/raw/main/docs/boost.pdf)

---

## Using Boost for Complex Percussive Rhythms in Eurorack

Boost is a characterful distortion/overdrive module for Eurorack. While it isn’t a direct sound source (voice), it dramatically shapes audio, making it invaluable for percussive, rhythmic, and hyper-complex beats. Here’s how you can exploit its features for dense, intricate percussion and polyrhythms:

---

### 1. **Percussive Processing / Transient Shaping**

- **Punchy Percussion:** 
  - Route dry drum or percussion modules (sample players, synth voices, or analog drums) through **Boost** to aggressively accentuate transients using the Drive knob.
  - This will give your rhythms more presence, especially in dense patterns where clarity of hits is vital.

- **Transient Contrast in Polyrhythm Layers:** 
  - Use Boost on only select rhythmic layers (for instance, a 5/8 sequence of hi-hats vs. a 7/8 kick pattern). The module’s harmonic clipping will help each pattern “cut” through the mix, making cross-rhythms more distinct.

---

### 2. **Dynamic Control & Unpredictable Variation**

- **Automated Distortion:**  
  - Although Boost lacks CV, place a VCA (Voltage Controlled Amplifier) before it and modulate the VCA level with a rhythmic LFO, Euclidean generator, or envelope tied to a drum sequence.
    - This lets you “sidechain” the amount of distortion to rhythmic gates/triggers, so certain drum accents get suddenly dirtier/punchier within your polyrhythmic groove.

---

### 3. **Tone Sculpting for Rhythmic Emphasis**

- **Accent Highs or Lows Based on Pattern Density:**
  - Use the Tone control to tailor brightness:
    - **Low Tone**: Rounds off highs, ideal for dense, rapid-fire sequences where you want to avoid harshness.
    - **High Tone**: Emphasizes sizzle/crispness, particularly good for intricate hats, metallic FM percussion, or to brighten odd pulses in complex signatures.

- **Automated Tone Sweeps:**  
  - Use an external voltage-controlled filter after Boost and rhythmically modulate it, thus further animating percussive timbre shape in complex time patterns.

---

### 4. **External Sources / Unconventional Percussion**

- **Amplifying Line/Mic Signals for Modular Percussion:**
  - Use Boost to bring in external drum machines, found-sound percussion, or even dynamic mic’d objects. The 26dB gain makes even quiet sources punch through modular processing, with added grit for unique voices in your rhythmic ensemble.

- **Feedback for Glitch Rhythms:**  
  - Patch Boost’s output back into itself (with caution!) or use a mixer to route part of the output to the input. Tweak Tone/Drive at different rhythmic intervals for wild timbral glitches—set gates or clock dividers to “open” the feedback on certain pulses, adding complexity and unpredictability.

---

### 5. **Modular Routing Ideas for Hyper-Complex Beats**

- **Layering:**
  - Parallel process—run one sequence dry, another through Boost, then mix. This allows stacking rhythmic voices with different harmonic profiles that respond differently to time-based complexity.
- **Subtle Use for Accents:**
  - Occasionally gate Boost in only for “accent” hits in an otherwise clean pattern, creating dynamic emphasis in complex time signatures.

---

### 6. **Practical Example Patch:**

1. **Complex Drum Sequencer** (e.g. using a polyrhythmic trigger sequencer, Deluge, or Pam’s New Workout with pattern divisions)
2. **Multiple percussion voices**: Send “kick+snare” to dry, “hats, claps, or metallics” to Boost.
3. Insert a VCA before Boost, modulate it with a 16-step sequencer set to a different clock.
4. Shape Tone for crispness; overdrive for harmonics.
5. Use another VCA for level/sidechain ducking if needed.

Your result is a snarling, hyper-detailed, percussively animated wall of rhythm where the timbre, drive, and impact evolve and are tied to your polyrhythmic complexity.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)