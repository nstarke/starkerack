# Korg — Volca FM2

- [Manual PDF](../../manuals/volca-fm2_OM_EFGSCJ3.pdf)

---

[**Korg volca fm2 Manual PDF**](https://cdn.korg.com/us/support/download/files/8300ee49b8df8126d7be6cba2e735620.pdf)

---

## Using Korg volca fm2 for Dense, Hyper-Complex Percussion & Polyrhythms in Eurorack Context

While the **Korg volca fm2** is not a native Eurorack module, its compact design, sync capabilities, and extensive MIDI support make it very compatible as a polyrhythmic AI-driven percussion voice/controller in a modular setup. Here’s how you can get the most rhythmically intricate sequences and percussive textures with it:

---

### 1. **Create Percussive FM Drum Voices**

**FM Synthesis is Ideal for Drums**: FM excels at producing metallic, clicky, bell-like, and punchy percussive tones.  
- **Edit mode**: Dive into the envelopes (EG ATTACK and DECAY) for each operator:
  - Use *short attack* and *very fast decay* for sharp transients (think: kick, snare, rimshot, claves).
  - Experiment with **feedback** in an algorithm for more aggressive, noisy snares and hats.
  - Assign operators as *modulators* for unusual overtones—great for clangorous or zappy percussion.

**Velocity Slider & Motion Sequence**:
- Use *motion sequencing* to automate envelope, pitch, or algorithm changes step-by-step, resulting in evolving percussion hits.

---

### 2. **Dense, Polyrhythmic Sequencing Techniques**

**Step Sequencer and Polyrhythm**:
- The volca fm2’s **16-step sequencer** can run polyrhythms by chaining uneven-length patterns (e.g., sequence lengths of 5 and 7 steps for hemiola/complex cycles).
- Use the **CHAIN function**: Hold MEMORY and select non-consecutive sequences for odd metrical groupings.
- **Active Step mode**: Disable (skip) steps at strategic points to create polymetric loops (e.g., making a 12-step loop against a 16-step master clock).

**Time Signature Manipulation**:
- **FUNC + WARP ACT.STEP**: Even if you have fewer than 16 steps, the sequencer will "stretch" the pattern across 16-step time, which can yield cross-rhythms.
- Chain different length patterns for Euclidean/polyrhythmic cycles.

---

### 3. **Complex Modulation & Parameter Locking (Motion Sequencing)**

- **Motion Sequence ON/OFF/SMOOTH**: 
  - Use motion sequencing for rapid parameter jumps or gradual morphs (SMOOTH).
  - Record LFO, Algorithm, Envelope, Velocity, and TRANSPOSE changes per step to sharply differentiate each hit.
  - “Parameter lock” type behavior: use it for evolving timbres within a rhythm for rich, IDM-like or experimental textures.

---

### 4. **Sync & Modular Integration**

- **SYNC OUT/IN**: Clock Eurorack sequencers or drum modules from volca fm2 for tight integration.
  - Use multi-channel triggers/gates in your modular to fire off the volca at unusual points.
- **MIDI IN/OUT**: Utilize an external sequencer (like Hermod, Torso, etc.) to send polyrhythmic sequences or clock-synced LFOs for deeper pattern complexity.

---

### 5. **Live Unpredictability: Program Random, Chaining, and Effects**

- **FUNC + PROGRAM RANDOM**: Randomizes the loaded program—use this for unpredictable per-step drum violence; lock to a pattern for semi-chaotic structures.
- **Effect Section**:
  - *Chorus*: Smeared metallic hats/claps or blurring kick attacks—automate chorus level or combine with motion sequence for ghost notes or varied hit widths.
  - *Reverb*: Smear snares, toms, or hats for big room percussion; automate reverb amount/freeze for dubby breaks.
- **Algorithm Morphing**: Switch algorithms per-step for wildly different attack tones and body.

---

### 6. **Advanced Patterns: MIDI, Modular, and External Sync**

- Use **odd step patterns** (lengths like 11, 13, 17, chained to 16 or 8) for tuplet-based polyrhythms.  
- **Active Step** plus *muting/unmuting* steps on the fly = “live fills,” evolving glitch, or burst rhythms.
- **Sending MIDI CC from Eurorack/CV-to-MIDI module**: Modulate volca parameters with envelope followers, random generators, or LFOs from your rack.

---

## **Example: Building a Hyper-Rhythmic Drum Pattern**

1. **Program a snare ‘drum’ on Operator 2, tight attack/decay, algorithm favoring feedback/modulation.**
2. **Set step length to 7 steps, chain it with a 5-step “kick” pattern.**
3. **Active Step mode:** Drop every 4th snare for odd syncopation.
4. **Motion Sequence:** Randomize velocity and reverb.
5. **Sync OUT to modular, clocking a 5-step burst sequencer driving a hats module.**
6. **Chain a 13-step pattern for metallic FM blips, syncopated against the snare.**

Repeat, combine, and mutate for ongoing generative, dense percussion storms.

---

### **For Further Exploration**
- [Korg volca fm2 Manual PDF](https://cdn.korg.com/us/support/download/files/8300ee49b8df8126d7be6cba2e735620.pdf)

---

[**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)