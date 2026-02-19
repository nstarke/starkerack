# 2hp — Unity

- [Manual PDF](../../manuals/2hp_Unity.pdf)

---

[2hp Unity Manual (PDF)](https://2hp.com/wp-content/uploads/2018/12/unity_manual.pdf)

---

## Using the 2hp Unity Mixer to Create Dense, Hyper-Complex Percussion in Eurorack

The **2hp Unity** module is not a voice or sound-shaping effect but a highly useful dual unity mixer. In the context of polyrhythmic, complex, and densely rhythmic Eurorack music, the way you sum and combine modulation or rhythmic signals can be the key to unlocking intricate percussion patterns.

### Key Features for Rhythmic Complexity
- **Six-to-one or Dual Three-to-one Mixing:** Merge up to six signals for dense modulation or grouping signals for processing.
- **Averaging/Unity/Split Modes:** Set mixer gain behavior for either audio (to avoid clipping) or CV (for full amplitude modulation).
- **Normalling Behavior:** Without a cable in the first output, both mixers sum to the second output, letting you cascade or recombine sources.

---

## **Techniques for Hyper-Complex Percussion and Rhythms**

### 1. **Merging Multiple Gate/Rhythm Sources**
Combine up to six rhythm/gate sequences or trigger streams (from sequencers, Euclidean rhythm generators, or clock dividers/multipliers):
- **Unity Mode:** All gates pass through at full amplitude. Sum irregular patterns for unpredictable bursts and ‘max density’ percussion triggers.
- **Averaging Mode:** Use to tame overly busy patterns and prevent false triggers from multiple stacked gates.

#### **Patch Idea: Polyrhythm Combiner**
- Generate 3–6 polyrhythmic triggers (e.g., from different clock-divided patterns: 3, 5, 7, etc.)
- Combine using Unity mode for maximal output.
- Send to a percussive voice (e.g., drum module, sample player) for machine-gun, nearly stuttered hits, or use as accent triggers.

### 2. **Creating “Composite LFOs” for Percussive Modulation**
Layer several LFOs, envelopes, or stepped random voltages:
- Merge multiple LFOs with different rates/phases in Averaging Mode for organic, evolving amplitude/pitch envelopes of percussion voices.
- Use Split Mode: Top mixer handles control voltages for pitch, while the bottom averages audio FM or amplitude modulation signals for a crunchy, dynamically shifting percussion timbre.

#### **Patch Idea: Dynamic Transient Design**
- Patch three envelopes (from different rhythm sources) into Mixer 1.
- Output to the VCA controlling your drum sound for hybrid, ever-mutating transients.
- Use Mixer 2 for modulating pitch decay, timbre, or noise amount.

### 3. **Cascading Mixers for Advanced Variations**
Take advantage of normalling: If OUT 1 isn’t patched, its sum flows into Mixer 2.
- Use first set of inputs for ‘base rhythm’, second set to add fills, microtiming, or rare events.
- Process OUT 2 into clockable logic or burst generators for secondary rhythmic layers.

### 4. **Unpredictable Accent and Fill Generation**
Summing bursts, shuffled gates, and Euclidean patterns guarantees that every downbeat, offbeat, and microbeat can be addressed, allowing for accent patterns that create machine-like or complex jazzy percussion.

---

## **Creative Manipulation for Percussive Character**

- **Mix Percussive Audio Sources:** Use Averaging Mode to layer snare, clap, and hat samples for conglomerate percussion hits.
- **Drive/Distort Downstream:** Because summing voltages increases amplitude, follow Unity with a wavefolder or overdrive for punchy, clipping transients.
- **Animate Panning/FX:** Use merged modulation signals from Unity to automate panning, delay effect parameters, or filter sweeps in uniquely timed ways.
- **Unique Splits:** Use Split mode to send tight CV control to drums and simultaneous audio mixing to FX, keeping transients sharp and animated.

---

## **Summary Patch Example**

**Goal:** Create a shuffling, polyrhythmic hi-hat groove.
- Patch three out-of-phase LFOs (triangle, square, stepped random) into Mixer 1.
- Mixer 1 OUT to hi-hat module decay/VCAs.
- Patch three euclidean gates of different steps (e.g., 5, 6, 7) into Mixer 2.
- Mixer 2 OUT triggers hats.
- Use Split mode: Top mixer is full-strength CV, bottom is averaged for consistent amplitude.
- Add light analog distortion downstream.

---

Harnessing the **2hp Unity** in this way, you turn a simple mixer into a deep generator of percussive complexity and rhythmic inventiveness!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)