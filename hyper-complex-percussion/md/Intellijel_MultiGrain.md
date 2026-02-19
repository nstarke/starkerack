# Intellijel — MultiGrain

- [Manual PDF](../../manuals/multigrain_manual_v1.2_2025.09.02.pdf)

---

[Download the Intellijel Multigrain v1.2 Manual (PDF)](https://intellijel.com/downloads/manuals/Multigrain_Manual_v1.2.pdf)

---

# Using Intellijel Multigrain for Dense, Hyper-Complex Percussive Rhythms

As a eurorack musician, **Intellijel Multigrain** is an extremely deep tool for granular sampling, morphing, and rhythmic exploration. To generate densely rhythmic, hyper-complex percussion with polyrhythms, odd time signatures, and intricate patterns, follow these strategies derived from the manual and your creative goals:

---

## 1. **Granular Percussion Voice: Sample Preparation**

- **Load a bank of short, percussive samples** (one-shots, drum hits, clacks, found sounds) across all 8 Sound slots. Use one channel (L or R) for dry drums and the other for treated hits to enable stereo complexity (p.55).
- **Make multisample files**: Load one file with rapid-fire percussion slices, then use granular Start/Wrap/Scan controls to jump between them.
- Normalize your samples to keep attack transients punchy and consistent (p.55).

---

## 2. **Complex Rhythm Generation: Triggers, Modulation & CV**

#### **A. Clocking & Triggering**

- **Patch independent rhythmic triggers into GATE/NEXT/SELECT/SYNC** for each Sound to generate polyrhythmic grain streams (pp.11, 18). For example:
    - **GATE**: Fires grains within active Sound based on panel settings.
    - **NEXT**: Step through the sample bank sequentially with every external trigger.
    - **SELECT**: Directly voltages address which Sound slot is being accessed. Use with stepped CV or random voltages for unpredictable sequences.

- **SYNC input**: Use external clocks with odd divisions or non-standard rhythms. RATE knob becomes a clock multiplier/divider, allowing you to align or offset grains—even with polymetric clock sources (pp.18–19).

#### **B. Modulation: X, Y, Z Inputs and Internal Random**

- **Assign CV modulation to granular parameters**: Send clocked CV to SIZE, RATE, WRAP, SCAN, PITCH, and BLUR for time-varying results.
    - Modulating **RATE** and **SIZE** at fast, independent rates (e.g., with LFOs or sequencers at different tempos) instantly produces polyrhythmic grain bursts.

- **Apply internal random (RAND) to parameters**: Use neg/pos amounts to introduce probabilistic envelope, position, or direction tweaks per grain (p.25).

#### **C. Per-Step Modulation (Live Complexity)**

- **Trigger grains via external triggers** for “manual” micro-programming (e.g., running GATE from a fast/clock-divided rhythm generator), or use CV-controllable grain generation by modulating RATE (p.18).

- **Assign modulation to REVERSE** for reversal “hits” mapped to a rhythmic pattern or random toggling (p.24–26).

---

## 3. **Morphing & Scenes: Instant Timbre/Pattern Changes**

- Create Scenes (A/B) with **wildly different grain shapes, lengths, pitch, or density** for the same percussion sample (pp.13–14).
- **Automate the Morph fader** with CV to interpolate between settings in sync with a rhythmic LFO, knob, or even incoming performance gestures.
- **Discrete parameters (SHAPE, REVERSE)** can be morphed probabilistically, so you can set up probability-based rhythmic variations as you crossfade between Scenes (p.14).

---

## 4. **Unique Percussive Voice Processing Techniques**

#### **A. Superimposed Polyphony**

- **Latch multiple Sounds** (use LATCH; p.9, 53) to let grains from several sample slots overlap. Employ per-Sound modulation for polymetric granulation layers.

#### **B. Ping-Pong SCAN and Reversal**

- **Enable Ping-Pong (long press REVERSE; p.20)**—instead of wrapping, your grains bounce back and forth within the sample memory, yielding mesmerizing, irregular rhythmic motion.
- Combine this with clever START/WRAP/SCAN settings to “cycle” through various parts of a drum loop at variable speeds.

#### **C. Envelope Randomization for Groove and Stutter**

- Assign **RAND to LEVEL and TONE**, with negative amounts for automatic panned randomization—makes each hit jump L/R in the stereo field and change its EQ (p.25).

#### **D. Pitch Quantizer + Modulation**

- Use the **Quantizer** to force granular pitch shifts to scale degrees, but modulate it with X/Y/Z at audio rates for melodic percussion (pp.32–33).
- Assign quantized PITCH to CV for melodic-rhythmic patterns.

#### **E. Blurring/Reverb for Density**

- Add per-grain reverb via BLUR; modulate per-grain for “clouds” of percussive clutter that ebb and flow with rhythm (p.21).

#### **F. Live/Looping Recorder Tricks**

- Use the **Looping Recorder** (v1.2) to record rhythmic material live. Freeze/unfreeze the buffer on the fly (by button or modulation) to “lock in” spontaneous loops mid-performance (pp.39–41).
- Use threshold-based auto-freeze for sample-accurate rhythmic looping.

---

## 5. **Algorithmic/Generative Control for Evolving Patterns**

- Modulate multiple parameters simultaneously for self-evolving complexity.
- Assign random (RAND) to alternative grains for pseudo-generative sequences (p.25–26).
- Use complex sources (logic, euclidean sequencers, bursts, etc) patched to GATE, NEXT, or CV for non-repeating hyper-complex rhythmic streams.

---

## 6. **Unique FX Processing**

- Use Multigrain as an **effect**: Patch in drums or complex rhythmic audio to inputs, set a Sound to “Live” mode (p.10), and granulate/morph wild output streams.
- Combine **thru/blur bypass** and CV-morphing to switch between dry, reverb-drenched, and glitched-out percussive FX.

---

## 7. **Performance Shortcuts & Workflow**

- Use quick button combos (p.52–54) to randomize, copy, and morph Sounds and Scenes in realtime—injects controlled chaos and new grooves on demand.

---

### **Pro Tip: Layer Multigrain with Dedicated Triggers and Accent Modulation**

Multigrain’s design lets you “address” separate layers in parallel, creating intricate polyrhythmic structures. Use external sequencers, trigger matrices, or generative CV for advanced control.

---

Explore, experiment, and let Multigrain’s granular engine warp your rhythmic ideas into intricate soundscapes!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)