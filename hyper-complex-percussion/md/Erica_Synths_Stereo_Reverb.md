# Erica Synths — Stereo Reverb

- [Manual PDF](../../manuals/black_stereo_reverb_Manual.pdf)

---

[Erica Synths Black Stereo Reverb Manual (PDF)](https://www.ericasynths.lv/media/Black_Stereo_Reverb_manual_1.01.pdf)

---

# Using the Erica Synths Black Stereo Reverb for Dense, Complex, & Percussive Rhythmic Music

**Context:**  
This module is an effects unit designed primarily for powerful, high-fidelity reverb. However, as a eurorack musician pursuing hyper-complex, densely rhythmic and percussive music (especially with polyrhythms and sophisticated time signatures), you can creatively repurpose many of its features for *unique, punchy, percussive, and rhythmic* effects.

Below are tips and techniques tailored to your goals:

---

## 1. **Percussive Reverb as a Rhythmic Voice**

While a reverb is not inherently a percussive *sound source*, the _Erica Synths Black Stereo Reverb_ offers features that let you use it as a rhythmic modulating element:

- **FREEZE Function as a Rhythmic Clock Divider / Buffer:**  
  - **Technique:** Patch a series of sharp, percussive triggers (e.g. from a Euclidean sequencer or polyrhythmic gate generator) into the FREEZE trigger input.  
  - **Why:** The FREEZE instantly grabs whatever's in the buffer.  
  - **Result:** If you FREEZE on percussive transients, the repeated fragment can become a texture or act as a rhythmic element in itself.
  - **CV Tricks:** Use a trigger pattern that’s a different division than your main clock to 'chop' the reverb at polyrhythmic points, creating complex interlocking layers.
  - **Variation:** Automate the release of FREEZE with a different rhythm or use logic modules to rhythmically alternate between frozen and non-frozen states.

- **SIZE Control and SIZE CV Input:**
  - **Technique:** Patch a sequencer, stepped random CV, or even audio-rate modulation into SIZE CV.  
  - **Why:** In FREEZE mode, SIZE not only controls space but also acts as a *playback frequency* for the buffer—a bit like a re-pitcher or granular tool.
  - **Result:** Fast, stepped modulation sync’d with percussion can render the reverb as a percussive, rhythmic digital artefact.
  - **1V/oct Tracking:** Play the buffer at quantized intervals, sync’d with your musical divisions.

- **Feedback as Percussive Burst:**  
  - Extreme feedback can be used as a quick echo burst by modulating FBK CV with a short envelope or gate tied to percussion events, so the reverb itself “resonates” with each drum hit.

---

## 2. **Polyrhythmic & Complex Modulation**

You can use this module as a live performance effect with complex time structures:

- **CV Control Over Multiple Parameters:**  
  - Assign *different* step/rhythmic CV sources to SIZE CV, FEEDBACK CV, and TONE CV (e.g. three channels of a polyrhythmic sequencer such as Pamela’s New Workout, Zadar, or Marbles).
  - Slowly modulate TONE/SPN with a rhythmic LFO, so the stereo field is animated in a polyrhythm against the primary percussion.

- **DRY/WET as a Performance Tool:**  
  - Cut sharply to full wet or dry in time with rhythmic variations to use the reverb like a punchy, “stutter” effect.

---

## 3. **Preset Switching and “Morphing”**

- **PATCH CV Input:**  
  - Sequence this input with a rhythmic voltage source to jump between saved reverb presets as part of your drum programming.  
  - If each preset is a dramatically different reverb (e.g. short/tight for snare, huge for kicks), you can morph the room/space around individual drums or pulses, adding extreme complexity.

---

## 4. **Stereo Imaging as a Rhythmic Parameter**

- **TONE/SPN as Spin:**  
  - In SHIFT+turn mode, TONE/SPN spins the reflections in stereo.
  - Modulate with stepped/pulse signals to match rhythm divisions, so spatial movement becomes percussive and syncopated.

- **MODE Switch on Rhythmic Boundaries:**  
  - Automate or manually perform changes in the early/late delay mix to accentuate off-beats or particular moments in a polyrhythm.

---

## 5. **Creative Patching (Examples)**

### Example Patch: “Rhythmic Chopper”
- Drum sequence into L(MONO) IN.
- Logical pattern generator outputs polyrhythmic pulses into FREEZE.
- Stepped sequencer (dividing main clock by 7, for example) into SIZE CV.
- Short, snappy envelopes linked to drum triggers into FBK/TONE CV.
- PATCH CV and MODE switched/ridden by hand or sequencer—constantly shifting reverb character and space.

### Example Patch: “Percolating BBD Textures”
- Use “Dirty BBD” mode with high feedback, but make the FBK CV respond to a fast, clocked sequencer (irregular pattern).  
- Modulate TONE/SPN with a rhythmic stepped source for tick-tock, stereo-swapped echoes.

---

## Uniqueness, Punch, and Character

- Push SIZE and FEEDBACK into territories where the module self-oscillates briefly when hit with percussive triggers.
- Exploit the lo-fi “Dirty BBD” algorithm for grainy, digital transients—especially sharp-sounding with short percussive hits.
- PLAY WITH PRESET MORPHING: Change the space/rhythm per drum hit, or every bar, for constantly shifting complexity.

---

For more inspiration and to learn techniques for modular rhythm manipulation, you might also want to explore the following repository:  
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)