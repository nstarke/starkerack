# WMD SSF — DPLR

- [Manual PDF](../../manuals/DPLRmanual1.3.pdf)

---

[Manual PDF (SSF DPLR)](https://wmdevices.com/pages/dplr-manual)

---

## Using SSF DPLR for Hyper-Complex, Densely Rhythmic Percussion

The DPLR is a **dual/stereo delay** module packed with features that can help you sculpt densely rhythmic, intricate percussion textures, polyrhythms, and complex time signatures in a Eurorack system. Here’s how you can push it into unique, punchy, and percussive sonic territory:

### 1. **Multi-Tap/Polyrhythmic Delays**
- Set main **DELAY AMOUNT** (A) to align with a base clock or division—for example, an 8th note in your tempo.
- Use the **SPREAD (B)** control to offset the B channel delay to a different rhythmic division (e.g. 3/16, prime multiples, triplets, or quintuplets). This achieves real polyrhythmic repeats from a single pulse or percussion hit.
- Modulate **DELAY A/B** and **SPREAD** via their CV inputs with independent, sequenced or polymetric clocked modulators (e.g., clock dividers, Euclidean sequencers) for shifting, evolving delay times.

### 2. **Complicated Patterns with XTALK Modes**
- Use **XTALK** (cross-talk) modes to crossfeed delay lines: in higher XTALK settings, see B feeding back into A and vice versa. This blurs, smears, and interlaces rhythmic patterns between the left and right (A/B), creating unpredictable, complex echo-cascades that evolve in time.
- Rapidly cycle XTALK modes using external gate triggers or manual button presses to change rhythmic complexity on the fly.

### 3. **Filter Settings for Percussive Punch**
- Lighter **FILTER SLOPE** settings allow more high-frequency artifacts and noisy, glitchy feedback—ideal for sharp, cutting percussion echoes.
- Heavier filtering makes the delays darker and cleaner, perfect for sculpting thumpy, subby, “body” percussion.
- You can automate filter mode changes (by holding the mode button), or switch modes between sequences for dramatic timbral/rhythmic contrast.

### 4. **Dynamic, Voltage-Controlled Feedback (REGEN)**
- Use stepped sequencers, random voltages, or clocked LFOs to modulate **REGEN**. This makes the delay trails shift from very sparse to densely packed, mechanically precise bursts—great for ratcheting fills or stutters.
- Push REGEN high for “fractal” self-oscillating repeats; pulse it low for “muted” single-echo snare-like hits.

### 5. **Rhythmic Stereo Movement & Ping-Pong**
- Exploit the stereo delay architecture: Route different percussion or “transient” voices to left/right inputs, and pan/recombine delays for moving, multi-layered grooves.
- With differing delay times and/or XTALK fed to both outputs, even simple trigger patterns will be “exploded” into rhythmic webs.

### 6. **Percussive Delay Input Techniques**
- Use percussive “clicks,” rim-shots, or even chopped-up vocal samples as input, “smearing” them into glitchy, metallic, or re-synthesized transients by experimenting with delay times, feedback, and filter modes.

### 7. **Self-Patching & Feedback Networks**
- Try patching one output back into the input, possibly through a VCA or filter modulated by your rhythms, to create controllable burst, comb-filter, or Karplus-Strong style physical modelling effects—a source of very rich, evolving percussion.

---

#### Quick Patch Example
1. Send a rapid, irregular trigger pattern into a short envelope + percussive VCO and then into DPLR's input.
2. **Delay A:** Set for a fast, clock-aligned repeat (e.g. 1/16).
3. **Spread B:** Modulate with a slow LFO for drifting micro-time offsets.
4. **XTALK:** Use a random gate to select mode every bar.
5. **Regen CV:** Sequence for rhythmic bursts (ratchets, retriggers, breakbeats).
6. **Filter:** Light for glitch mode in verse, heavy for breakdown.

---

The DPLR’s voltage-control possibilities, cross-channel bleed, and mix of delay/filter/feedback control make it ideal for transforming any trigger, percussion voice, or audio loop into fast-evolving, deeply intricate rhythms.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)