# Rebel Technology — Stoicheia

- [Manual PDF](../../manuals/Stoicheia – Rebel Technology.pdf)

---

[**Download the Stoicheia Manual PDF**](https://raw.github.com/pingdynasty/EuclideanSequencer/master/EuclideanSequencerSchematic.png)

---

## Using the Stoicheia Euclidean Sequencer for Hyper-Complex Percussion & Polyrhythms

The Stoicheia by Rebel Technology is a powerful dual Euclidean sequencer, specifically designed to generate rhythmically dense and complex sequences from simple trigger inputs. By leveraging its pattern algorithms and flexible controls, you can push your percussive arrangements into the world of hyper-advanced polyrhythms, odd time signatures, and evolving rhythmic patterns.

### Key Features for Advanced Rhythmic Generation

- **Dual Independent Euclidean Sequencers:** Each with individual control over sequence length, fills, and rotation.
- **Chainable Modes:** For creating patterns longer than 16 steps and complex composite rhythms.
- **Flexible Trigger Modes:** Switch between trigger, alternating, and chained outputs.
- **Hardware Reset:** Perfect for synchronizing with other clocked modules.
- **All Controls Voltage-Addressable:** Immediate hands-on or modulated control.

---

## Strategies for Generating Dense, Complex Percussion

### 1. **Polyrhythms and Complex Time Signatures**

- **Independent Length & Fills:** Set each channel (α and β) to different sequence lengths and fills (e.g., Channel 1: 7 steps/3 fills, Channel 2: 12 steps/5 fills). Send each output to separate percussion voices. The resulting overlap forms true polyrhythms and non-standard time signatures.
    - Examples:
        - E(7,12): Central & West African patterns
        - E(5,8): Cuban cinquillo/Spanish tango
- **Odd Fills & Rotations:** Experiment with prime numbers (e.g., E(5,7), E(3,5), etc.), and use the rotation knob to offset the start point for each channel, further increasing rhythmic complexity.

### 2. **Chained Mode for Super-Patterns**

- **Extended Patterns:** Use chained mode to play both sequences consecutively (rather than concurrently), allowing for complex cyclical patterns: e.g., a 9-step chain followed by a 7-step chain equals a 16-step "macro-pattern."
- **Mega-Polyrhythms:** Use chained mode in conjunction with another Euclidean or clock divider to layer meta-patterns.

### 3. **Manual/External Reset for Syncopation**

- **Live Resets:** Patch a manual gate button or rhythmic pattern into the reset input, causing both sequences to restart in time with external or performance-based cues. This can create shifting accents and “phase music” effects.

### 4. **Glitch & Modulation: Patch Ideas**

- **VC Clock Sources:** Modulate the tempo using a variable clock/LFO for tempo bursts or slow-motion effects.
- **Pulse Width Modulated Clocks:** The output trigger width mirrors the input pulse—use this to generate "flam" or super-tight, punchy triggers.
- **Rotate Sequences Live:** Patch stepped random CV or a sequencer into the rotate control voltage to dynamically shuffle patterns.

### 5. **Percussive Voice Pairings**

- **Bass Drum / Snare Layers:** Send two polymetric patterns (e.g., E(2,5) and E(5,8)) simultaneously to different drum/sample modules.
- **Multiple Drum Voices:** If your drum modules have accent/gate length inputs, exploit the output pulse width from Stoicheia for dynamic gates.

### 6. **Creating Evolving, Non-Repeating Grooves**

- **Dynamic Parameter Morphing:** Slowly modulate sequence length, fills, or rotation with LFOs, random sources, or envelopes. This results in constantly morphing, ever-evolving rhythmic patterns.
- **Performance Tip:** Pair with additional Euclidean or random-sequence modules for even more interlocked/clashing rhythms.

---

## Bonus: DIY & Hacking Potential

- **Open Hardware/Software:** Customize, hack, or update firmware for bespoke rhythmic functions; all resources are on [Stoicheia's GitHub](https://github.com/pingdynasty/EuclideanSequencer).
- **Arduino/FTDI Support:** Reprogram the module for generative rhythms or sequence behaviors beyond Euclidean.

---

## Final Patch Example: "Hyper-Poly" Sequence
1. Set α Channel: Length 7, Fills 3, Rotation +2
2. Set β Channel: Length 12, Fills 5, Rotation -1
3. Engage Chained Mode
4. Clock from an external trigger sequencer or tempo LFO
5. Patch outputs to drum voices (e.g., BD and closed hat).
6. Use a slow LFO patched to “fills” CV or “rotation” for evolving rhythms.
7. Optional: Patch random triggers to the reset for syncopated pattern shifts.

---

### [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
