# Toadstool Tech — Ectocore

- [Manual PDF](../../manuals/ectocore_quickstart.pdf)

---

**[Ectocore Quickstart Guide PDF](https://github.com/nstarke/infinitedigits-ectocore/blob/main/docs/quickstart-v6.0.pdf)**

---

# Using Ectocore for Dense, Hyper-Complex Percussion & Polyrhythms

The Ectocore is a unique sample-based effects module that is perfect for highly rhythmic, complex, and percussive electronic music explorations. Here’s how you can use it to achieve hyper-complex percussion sequences, polyrhythms, and advanced time signatures:

---

## 1. **Sample Slicing & Randomization for Percussive Complexity**
- **Sample Knob**: Choose percussion-rich samples or one-shots from within a bank. Navigate using the LED ring for precise choices.
- **Amen Knob**: Acts like a Turing machine for slices; fully CCW = straight playback, but as you turn CW, it cycles and randomly jumps through slices (steps 1–16). This immediately creates intricate and unpredictable chopped beats.
    - **Fully CW** = new random slice pattern each loop, with a rhythmic FX fill to spice things up. For evolving rhythms, turn CW and then "reroll" by returning and turning again.
- **Amen Attenurandomizer**: Introduce controlled chaos—fully left = wild/random, fully right = subtle variation (drifts with playhead). Adding CV here lets you modulate the chaos or even lock it tighter to external clocks for cross-rhythmic interplay.

## 2. **Clocking & Polyrhythms**
- **Clock Input**: Sync Ectocore to any external sequencer, irregular clock, or another rhythm generator. For polyrhythmic action, send a clock in an odd time signature (e.g., 5/4, 7/8) from your main sequencer.
- **Clock Mult/Div**: Multiply for ratcheting, or divide for slower, stretching grooves, creating cross-rhythms or shifting phrases.
- **Tap Tempo**: Set the master tempo manually (even in real-time performance, count 2 taps). With an external clock, it acts as a reset for restarting patterns in phase.

## 3. **Trigger Output & Complex Patterns**
- **Trig Output**: Set to different modes to output triggers based on your sample patterns. Use this output to drive other drum voices, envelopes, or sequencers for modular interplay across voices with complex groove logic.
- **Trigger Mode**: Cycles through how/when triggers are generated in relation to the slices—great for gate-driven effects and intricate percussion layers.

## 4. **Effects as Percussive Tools**
- **Grimoire Knob**: Each glyph is a unique multi-FX combination. Selecting different glyphs changes the “shape” of your percussion—experiment here with FX exclusive to certain glyphs.
- **Break Knob**: Adjust the density of FX triggers. Turn up for filled, busy textures; down for sparser, more controlled fills.
- **FX Selection (Bank & Grimoire)**: Certain combinations will add crazy stutter/chop (Chopper), filtering (DJ Filter, HP/LP), and distortion (Drive), further morphing your percussive voices.
    - For punch and impact: use **Drive** and **Gated** FX for sudden rhythmic punch, or **DJ Filter** for dramatic bandpass sweeps on beats.

## 5. **Performance Hacks & Super Cool Functions**
- **Tap + Break, Tap + Amen, Tap + Sample**: These hidden combos may yield unique modulation, pattern shifting, or sampling tricks—not detailed here, but experiment for secret performance tools.
- **Volume**: Instant access to level boosting for standout percussive attacks.

---

## **Suggested Patches for Complex Percussion**

1. **Polyrhythmic Sliced Breaks**
   - Clock Input: Patch a weird clock (3/4, 5/8, swinging, etc.).
   - Amen: CW for maximum random slice junglism.
   - Amen Attenurandomizer: Modulate with LFO for drifting rhythm “jitter.”

2. **Dense FX-Fill Sequences**
   - Grimoire: Choose a glyph with Chopper + Drive.
   - Break: Turn up to increase FX density.
   - Mult/Div: Shift timing mid-sequence for “broken” loops.

3. **Self-Generating Percussive Patterns**
   - Trig Output: Send to other drum modules for unexpected polyphony.
   - Amen: Constantly “reroll” patterns during performance.
   - Tap Tempo: Use live for tempo jank/glitch transitions.

---

## **General Tips**
- Layer with other rhythm modules for meta-grooves.
- Use Trig output and Clock div/mult to generate rhythmic nested structures.
- Treat Ectocore as both a sound generator and a “groove brain” for your drum rack.

---

**[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**