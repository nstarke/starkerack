# 2hp — Slice

- [Manual PDF](../../manuals/2hp_Slice.pdf)

---

[2hp Slice Manual (PDF)](https://www.twohp.com/_files/ugd/ccb147_aa7b64bff27740e98aba819b85c9578d.pdf)

---

## Generating Dense, Hyper-Complex Rhythmic Music with 2hp Slice

The **2hp Slice** is a beat repeat/glitch effect module, not a sound source/voice, but it can radically transform any rhythmic or percussive audio input. Its real strength in complex rhythm creation lies in its flexible clocking, advanced repeat/divide/multiply options, and ability to be voltage-controlled at audio rates. Here's how you can leverage it to create intricate rhythmic and percussive textures:

---

### Core Concepts

- **Effect, Not Voice**: Use Slice to process any audio—drum loops, percussion hits, synth lines, samples—turning straightforward materials into detailed, hyper-rhythmic patterns.
- **Clocking**: The clock input determines the base rhythmic grid. Feeding unusual or polyrhythmic clocks will radically alter the possibilities.
- **Size Control (Knob + CV)**: Sets repeat size from long bars to extremely tight micro-loops, all time-synced to the clock.
- **Triplet Toggle**: Expands subdivisions to include non-standard rhythmic groupings, excellent for tuplets, swing, and polyrhythms.
- **Gate/Trig Input & Manual Button**: Activate effect on demand or using sequencers/envelope-followers for "dynamic" glitching.

---

## Strategies for Hyper-Complex Percussive Sequences

### 1. **Polyrhythms with Multiple Clocks**

- Use a programmable clock or trigger sequencer capable of unusual time signatures or layered polyrhythms (e.g., sending a 5/4 clock from one source, a 4/4 from another, and switching/mixing between them).
- **Patch Example**:  
  - Clock input—mult two different clocks (with different divisions, e.g., 3 against 4) into a sequential switch or logic module, and then to the Slice input.
  - The irregular clocking will create beat repeat cycles that dance across rhythmic boundaries.

### 2. **CV Modulation for Nested/Complex Patterns**

- Use the **Size CV input** to modulate the repeat size in real-time.  
  - Random CV (from modules like 2hp Rnd, stepped random, or programmable sequencer) will cycle through divisions and multiplications in unpredictable rhythms.
  - For more musical results, use a dedicated sequencer tied to your overall meter, but programmed with offbeat, swung, or polymetric values.
- **Percussive Trick**:  
  - Route an envelope or LFO synced to a different clock division into Size CV. This can drive the repeats from long slices (chunky) to tiny audio-rate snippets (granular, percussive hits) throughout a phrase.

### 3. **Triplet & Non-Standard Subdivision Manipulation**

- **Triplet Toggle**: Activate triplets for odd groove divisions—great for 6/8 feels, 7/8, or mathy drum phrases.
- Combine the triplet function with polyrhythmic clocks for dense, overlapping textures.

### 4. **Momentary vs. Latching Gate for Dynamic Patterns**

- **Momentary Mode**: The beat repeat effect is only active while the trigger is held—feed in complex, irregular gates (from a rhythm source or custom logic patch) to glitch sections "on the fly."
- **Latching Mode**: Traditional on/off repeat; ideal for locking in stuttered or looped fills at key spots.

### 5. **Manual "Glitch" Performance & Live FX**

- Trigger the effect manually with the front panel button for live fills, improvised stutters, and drops.
- Combine manual triggering with quick shifts in Size or triplet toggling for hand-controlled, evolving rhythms.

---

#### *Advanced Percussive Sound Design Tips*

- **Punch/Impacts**: Input transient-rich audio (like percussion or snappy drum machine sounds) and use quick, tight slice segments for metallic, sharp glitch hits.
- **Granular Percussive Textures**: Set the Size very small and modulate at audio rate for granular timbres—turning ordinary samples into micro-percussive textures.
- **Multi-voice Routing**: Use multiple Slices on separate audio streams (e.g., one for kick/snare, one for hats) and cross-modulate their clocks/CVs for ultra-dense polyrhythms.
- **Layer with Samplers & Loopers**: As suggested in the manual, pair Slice with a sampler like 2hp Play or a looper. Mult the Size CV to both—the rhythmic slicing and the sample pitch together create melodic-rhythmic motion (e.g., “beat repeat” gets faster as pitch rises).

---

## Module Pairing Recommendations

- **Rnd/Random CV**: To modulate Size or trigger input for unpredictability.
- **Sequencer with odd divisions**: For polyrhythmic clocking.
- **Other glitch/process modules**: For multi-stage FX chains.

---

**Summary Table**

| Parameter        | Patch/Manipulation Tips |
|------------------|-------------------------|
| Clock Input      | Non-traditional clocks, polyrhythms |
| Size Knob/CV     | mod sequencer, random, envelopes   |
| Triplet Toggle   | Push/pull groove, tuplets          |
| Gate/Trig Input  | Irregular gates, logic, hands-on    |
| Audio Input      | Anything percussive or transient-rich|

---

For more info, check the [2hp Slice Manual (PDF)](https://www.twohp.com/_files/ugd/ccb147_aa7b64bff27740e98aba819b85c9578d.pdf)  
Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)