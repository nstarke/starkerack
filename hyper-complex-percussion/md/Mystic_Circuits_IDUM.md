# Mystic Circuits — IDUM

- [Manual PDF](../../manuals/IDUM Manual Draft 7.pdf)

---

[IDUM Official Manual (PDF)](https://www.mysticcircuits.com/_files/ugd/ec9752_18d9a91bff2b4ed3b200a508d79e933f.pdf)

---

## Using Mystic Circuits IDUM for Hyper-Complex Percussive and Rhythmic Sequences in Eurorack

As a Eurorack user aiming for dense, hyper-complex rhythms filled with polyrhythms, odd meters, and intricate patterns, the **Mystic Circuits IDUM** is an exceptional tool. Below is a structured guide to maximize its potential for your creative, percussive ambitions:

---

### 1. **Module Nature & Workflow**

**IDUM** is an effect/processor for gate and trigger signals, not a voice itself. You patch sequenced triggers or gates into IDUM, which then transforms the rhythm in a playable, performative way. Treat it as a rhythmic effects unit for triggers.

---

### 2. **Generating Complex, Densely Layered Percussion**

#### **A. Patch Fundamentals**

- **Start:** Use several channels from a trigger/gate sequencer (especially ones running differing polymeter or polyrhythm lengths/clock divisions).
- **Input:** Patch four separate rhythm triggers (they can all be polyrhythmic/polymetric) into IDUM's four trigger inputs.
- **Output:** Route the four outputs to four different percussion voices (kick, snare, rim, hi-hat, glitches, or even synth voices treated percussively).

#### **B. Embrace IDUM's Modification Modes for Complexity**

##### **Key Modes for Complex Percussion:**

1. **BURST**: Each trigger generates a burst/ratchet (speed is a multiplier/divider of the incoming clock).  
   - _Tip_: Modulate the burst speed with CV for morphing complexity.
2. **MULTIPLY/DIVIDE**: Creates bursts tied to the timing between incoming triggers, allowing for deviations and anti-grid patterns.
3. **BOUNCING BALL**: Generates accelerating or decelerating bursts, mimicking decaying or ramping rhythms (excellent for glitchy fills and non-linear timing).
4. **BREAK**: Applies preset breakbeats to incoming triggers, transforming static rhythms into classic or twisted drum & bass patterns—rotate the `PARAM` knob for 16 wild variations.
5. **ROTATE**: Reroutes trigger assignments to outputs; use to shuffle drum parts around, introducing unpredictability and counterpoint.
6. **SKIP**: Alters the clock itself, skipping or ratcheting, pushing attached sequencers into new cycle lengths or generating off-kilter time signatures.

##### **Polyrhythm & Polymeter Technique:**

- Combine incoming trigger streams with different step lengths (e.g., 5, 7, 9 steps, interlaced with a 16-step sequence).
- IDUM accentuates complex interactions by ratcheting some triggers, skipping others, and rotating channels unpredictably—this can yield emergent polyrhythmic overlays.

---

### 3. **Using CV & Performance Controls for Rhythmic Complexity**

- **CV Everything:** Patch LFOs, random sources, or other sequencers to IDUM's CV inputs (mode, param, chance, length) to morph between different rhythmic transformations in real time.
- **Chance Slider:** Use for stochastic rhythm densities—set the probability for any modification (ratchet, skip, break, etc.) to trigger per beat.
- **Length Slider:** Short lengths produce frantic, glitchy patterns; longer lengths bring evolving motifs or extended fills.

---

### 4. **Live Manipulation & Looping for Structure**

- **LOOPER:** Capture the last 8 steps of dense rhythmic interplay and loop it. While active, you can scrub the position, resize the length (from 1 to 8 steps), and even morph loop playback speed—a powerful way to create complex fills, breakdowns, or "live remixes."
- **REMOVE MODE:** Drop in or out certain modes on the fly, focusing on bursty chaos for a section, switching to breakbeats for another, etc.

---

### 5. **Advanced Ideas**

- **Self-Patching:** Use one ouput to trigger additional events (e.g., modulate parameters or gates on itself or other modules) for even more intricate interdependencies.
- **Pair with Unique Voice Modules:** Since IDUM is agnostic to what your triggers fire, patch its outputs to exotic drum synths, LPGs (low pass gates), glitch modules, or sample players for timbral complexity as well as rhythmic.

---

### 6. **Example Patch for Maximum Complexity**

```text
TR1 IN: 5-step trigger pattern         → TR1 OUT: Kick Drum
TR2 IN: 7-step polyrhythm (different clock) → TR2 OUT: Snare
TR3 IN: Randomized Euclidean rhythm    → TR3 OUT: HiHat (with LPG)
TR4 IN: Stepped random or bursty clock → TR4 OUT: Metallik Perc/Glitch

- Set Mode to 'Multiply/Divide' or 'Burst.'
- CV the Mode and Param with a stepped random voltage or LFO.
- Length at 3-5 for evolving, not-too-short motifs.
- Flip the Cycle switch: Down for drift (free time), Up for synced sequences.
- Use Looper for immediate live remixing/fills.
```

---

### 7. **Make It Punchy, Unique, and Percussive**
- IDUM does not process audio, but by changing timing, density, and stochasticity, your drum voices will groove and stutter in unexpected ways.
- **Pairing Tips:**
  - Patch to VCAs with short envelopes for clicky, punchy hits.
  - Use LPGs for percussive plucks.
  - Gate different parameters on your drum voices or FX (e.g., pitch, decay) for dynamic timbral complexity.
  - Randomize or sequence the CV inputs to morph modes live for shifting feels and time signatures mid-performance.

---

By thinking of IDUM as a live rhythmic mutation engine, you can move far beyond boring quantized beats into the wildest territories of IDM, experimental techno, glitch, and far more.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)