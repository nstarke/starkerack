# Mutable Instruments — Branches

- [Manual PDF](../../manuals/branches_quickstart.pdf)

---

[Branches Manual PDF](https://mutable-instruments.net/modules/branches/manual/branches_manual.pdf)

---

## Using Mutable Instruments Branches for Eurorack Song Form & Structure

Mutable Instruments Branches is a **dual Bernoulli gate** module, meaning it’s a utility for probabilistic routing of gates/triggers—essentially a coin-toss controlled switch that can add variety and movement to your modular patches. This might seem “subtle,” but in modular music, controlled randomness and switch logic are crucial for transforming loops and short phrases into dynamic song structures.

Below are strategies, patch ideas, and techniques for using Branches to help turn great loops or sketches into full-length pieces.

---

### 1. **Song Section Transitions (A/B Structure)**
Use Branches to probabilistically or deterministically switch between different voices, subsequences, drum patterns, or effect chains. Feed your master clock or trigger into IN, choose two destinations (say, two different drum patterns, or two melodic/sequencer rows), and use the **probability knob/CV input** to control how often a section happens. Modulate the probability with an LFO, envelope, or slow CV manual movement to fade between sections over time.

#### Example Patch:
- Clock source triggers Branches IN1.
- OUT A → Drums Pattern 1, OUT B → Drums Pattern 2.
- Probability CV from a sequencer or manually via knob through the song.

This creates evolving, algorithmic song sections, like verse/chorus/verse.

---

### 2. **Generative Builds & Drops**
Take advantage of toggle and latch modes:
- **Latch mode:** Once a section appears, it persists (“holds”) until the other output gets activated. You can use this for dramatic builds or drops—e.g., send all triggers (hi-hats, ride, percussion layers) to OUT A and then after some time, all to OUT B for a sudden change such as a breakdown or drop. Control this with slow modulation, manual button holds, or an external sequence.
- **Toggle mode:** Causes triggers to alternate their routing with each input. Use this to slowly evolve patterns—odd/even measures, alternating fills, or morphing sequences.

---

### 3. **Fill, Variation, and Humanization**
Insert Branches between a rhythm generator (like a clock divider or trigger sequencer) and a percussion module. Tune the probability so some hits are “skipped” occasionally, making patterns less robotic, introducing surprises, and creating variation and “fills” during performance.

#### Example Patch:
- Every 8th step, send a clock pulse to Branches, OUT A to your snare, OUT B to a rim or ghost hit.
- Modulate probability over time for evolving fills.

---

### 4. **Melody Line Variation**
Feed a quantized random source or two sequencers into both outputs. Use Branches to switch which note sequence is active with each trigger. The probability control can fade between lead lines or motifs, enabling automatic or hands-on A/B theme development.

---

### 5. **Song Automation and Macro Moves**
Patch a slow LFO, envelope, “macro controller,” or random CV into the probability CV input. Over several minutes, this shape will subtly—then dramatically—change the probabilities, automating song sections or evolving patterns in a musical, non-repetitive way.

---

### 6. **Dynamic Effects Routing**
Send gate/trigger events to Branches, then route OUT A/B to effect sends, different reverb/delay tails, or modulation sources. Randomly or cyclically, this can mutate the feel of instruments and create fresh textures over a song.

---

### 7. **Performance Control**
- *Manual switches*: Tap the switch on Branches for “live” intervention, enabling toggle or latch modes for sudden changes—drop in new layers, mute parts, or cue up breakdowns.
- *Memory*: Toggle/latch states are remembered, ensuring reproducible yet flexible performance setups.

---

## Summary Table

| Use Case               | Patch Suggestion                                          | Song Use              |
|------------------------|----------------------------------------------------------|-----------------------|
| Section Transitions    | Gates to two rhythmic voices or sequencers               | Verse/Chorus Switch   |
| Fills/Variation        | Random skipping/humanizing percussion                    | Fills & Evolution     |
| Melodic Mutation       | Switch between two quantized melodies                    | Theme/Motif Variation |
| Macro Moves            | Modulate probability CV with LFO/envelope over song      | Dynamic Evolution     |
| Effects Morphing       | Random/directed FX routing                               | Texture Variation     |
| Live Performance       | Manual/latch for big drops or buildups                   | Instant Control       |

---

### General Tips
- Combine Branches with clock dividers, step sequencers, random voltage generators, and logic modules for the richest results.
- Use the outputs to control not just audio, but also modulation and events (e.g., opening/closing VCAs, switching effect sends).
- Remember: Subtlety pays off—small, probabilistic routing changes can drastically increase the “song-like” feel of your patch!

---

For the full manual, see [Branches Manual PDF](https://mutable-instruments.net/modules/branches/manual/branches_manual.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)