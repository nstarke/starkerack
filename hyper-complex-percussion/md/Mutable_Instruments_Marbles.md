# Mutable Instruments — Marbles

- [Manual PDF](../../manuals/Mutable Instruments - Marbles.pdf)

---

[**Marbles Original Manual (PDF)**](https://mutable-instruments.net/modules/marbles/manual.pdf)

---

## Mutable Instruments Marbles: Creating Hyper-Complex Rhythmic/Polyrhythmic Percussion

Mutable Instruments **Marbles** is a powerhouse for generative rhythmic and melodic sequencing. To use it as a machine for densely rhythmic and hyper-complex percussion sequences, take advantage of these key features and workflow tips:

---

### **1. Random Gate Generator: Multi-Channel Rhythm**
- **Multi-Channel Output:** Use the three gate outputs (`t1`, `t2`, `t3`). Each can trigger different percussion modules or drum voices (like kick, snare, hats, etc.).
- **Generative Models:** Select between:
  - *Random routing/coin toss* for unpredictable splitting of pulse streams.
  - *Random division/reciprocal factors* for mechanical, evolving syncopation.
  - *Grids-inspired rhythms* for organic drum patterns and fills.
- **Adjust Jitter:** Increase the *Jitter* control for microtiming variation; this adds a human, alive feel, or twist it all the way up for a chaotic, glitchy groove.
- **Gate Widths:** Set short gates for clicks, sharp percussion; increase gate length or randomize it for bursts, rolls, or pseudo-flams.

---

### **2. Master Clock and External Synchronization**
- Use internal or external clocking—multiply/divide the clock, or let Marbles follow irregular external rhythmic material.
- Polyrhythm Generator: Send different clock divisions (with range selector) to each `t` output for instant polyrhythmic action.

---

### **3. DEJA VU: Probabilistic Looping and Shuffle**
- Increase **Deja Vu** to "lock in" fragments of random rhythm for looping patterns, then shuffle the sequence for further complexity.
- Change **Loop Length** dynamically—short for tight ostinatos, long for slowly shifting evolution.
- **Live Remix:** Use external CV as a basis for probabilistically remixed, mangled drum lines.

---

### **4. Random Voltage Generator for Modulation**
- Patch the `X` outputs to modulate percussion parameters: envelope decays, filter cutoff, or drum voice parameters for ever-evolving timbres.
- Use **Spread** and **Bias** to morph between subtle and wild expressive ranges.
- *Quantized Mode*: Can make X outputs step between specific values for FM rhythms (tuned percussion, pinged filters, etc.).
- *Slew Mode*: Use continuous voltages to generate gliding percussion parameters (think morphing metallic sounds or pseudo-LFOs for percussion design).

---

### **5. Quantizer/Scales: Rhythmic and Melodic**
- Program scales by playing in accents/rhythmic patterns—the machine will bias random steps to follow your principal rhythm, creating emergent structures.

---

### **6. External CV Processing**
- Run external sequences or LFOs into Marbles’ CV processing chain. Let Marbles buffer, loop, structure, and shuffle your external sources... then re-randomize. Great for remixing sequences and making "derived" patterns with a percussive edge.

---

### **7. Output Diversity for Complexity**
- Each output can respond differently (complementary/random/opposed) to the main controls—experiment with dialing in different Spread/Steppiness/Deja Vu for each channel.

---

### **Top Tips for Dense, Punchy, Unique Percussion**
- **Multitrack:** Send each gate output to a different sample/voice, modulate their parameters with X outputs.
- **Trigger Repeats/Flams:** Modulate gate length/randomization for bursts or flam-like effects.
- **Rhythm as Modulation:** Use clock, triggers, and random CVs to modulate effects (VCAs, filters, wavefolders, delay feedback) for percussive color.
- **Exploit Clock Divisions:** Use complex divisions/multiplications (with uneven settings) for asymmetric time signatures (e.g. 5 against 7, 3 against 4).
- **Layer Microtiming:** Jitter and random duration gives percussion a "drunken master" groove.
- **CV Processed Looping:** Pipe in a riff from another sequencer, let Marbles break and reshape it ad infinitum.

---

**Marbles is not a percussive voice itself** but a prime, generative source for clock/gate/CV patterns to feed your drum voices, channeling both mathematical and intuitive chaos for fresh, endlessly evolving beats.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)