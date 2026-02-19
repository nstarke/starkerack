# ADDAC Systems — ADDAC-402 Heuristic Rhythm Generator

- [Manual PDF](../../manuals/ADDAC402_UsersGuide_A_0_web_6500.pdf)

---

[ADDAC402 USER'S GUIDE PDF](http://media.addacsystem.com/firmwares/manuals/ADDAC402%20User%20Guide.pdf)

---

# Advanced Rhythmic Techniques with the ADDAC402 Heuristic Rhythm Generator

The ADDAC402 is a powerful Eurorack module for generating advanced, algorithmic trigger/gate sequences across four independent channels. Leveraging its diverse modes, flexible configuration, and extensive CV controllability, you can create percussive sequences that are densely packed, polyrhythmic, and hyper-complex. Below is a strategic guide to using the ADDAC402 for such experimental and high-level rhythmic musical purposes:

---

## 1. **Building Polyrhythms & Odd Time Signatures**

### **Euclidean Mode**
- **Core Idea:** Assign each channel a different number of steps & fills (e.g., 5 steps/2 fills, 7 steps/3 fills, 11 steps/4 fills, etc.)
- **Polyrhythm Construction:** Let each voice output different classic divisions—e.g., Channel 1 = 5 steps, Channel 2 = 7 steps, Channel 3 = 9 steps, Channel 4 = 12 steps.
- **Result:** The interplay of these step counts produces evolving polyrhythms and cross-rhythms.
- **Tip:** Use the ‘Skip Step’ buttons to rotate patterns in phase, adding further complexity.

### **Gate Sequencer Mode**
- **Odd Time Signatures:** Use up to 32 steps per channel with independent bar length for each channel, sculpting freely from micro-polyrhythms to extended, non-repetitive sequences.
- **Dense Programming:** Activate many steps with selective gaps, or stagger channel bar lengths for “never-repeating” meta-rhythms.

---

## 2. **Maximizing Pattern Complexity**

### **Game of Life Mode**
- **Generative Chaos:** Let the automaton create evolving, complex patterns that you can “reset” or “evolve” with the reset buttons.
- **Live Variation:** Use the Master Reset for major “scene changes” or individual resets for instant randomization.

### **Golomb Rulers Mode**
- **Aperiodic Patterns:** Each ruler produces mathematically unique, non-overlapping trigger distances—great for unpredictable polyrhythmic grooves.

### **Probabilistic Footwork/Pong Modes**
- **Controlled Randomness:** In probabilistic mode, set each channel with a different percent to “eat up” or leave space for other events. Footwork mode exploits buggy, organic triggers for ultra-intricate, ‘broken’ percussive output.
- **Pong Mode:** Exploit ball-bounce events and left/right “pad” controls for percussive lines that rarely repeat precisely.

---

## 3. **Swings, Shuffles, and Grooves**

- **Swing/Assign Knob:** Default assign adds micro-shuffle to all triggers, but you can re-assign this to steps, skips, or resets.
- **Parameter-Locking:** Use CV input to modulate swing, rotate patterns, or reset channels based on external voltage/program changes.
- **Extreme Swings:** Try uppermost swing settings for hard-offset, stuttery/jittery grooves.

---

## 4. **Advanced Patch Ideas**

- **Layered Sequences:** Mult and mix outputs to trigger multiple drum voices. Route inverted outputs to alternate envelopes for ghost notes or fills.
- **CV Control:** Feed random, LFO, or envelope CVs into steps/fills/skips, so your patterns morph over time.
- **Gate/Trigger Toggling:** Use the switches and configuration menu to alter output length and shape, creating crisp triggers, heavy gates, or stuttering machine gun effects.
- **Preset Recall:** Sequence or punch in different preset patterns for rapid variation in live sets.

---

## 5. **Post-Processing for Percussive Uniqueness**

- **Further Modulation:** Run the outputs into slew/noise/random modules to modulate decay, pitch, or filter per drum hit.
- **FM/AM Tricks:** If using voices rather than only drum modules, experiment with modulating pitch or amplitude by sending gates to VCA or FM inputs.
- **Punch & Snap:** Pair gated outputs with fast DA/AD envelopes, and explore chaining with distortion/wavefolding/filter modules to create unique, punchy percussive impacts.

---

## General Tips

- **Don’t hesitate to randomize resets or step-skips for ever-evolving rhythms.**
- **Exploit the ‘inverted’ outputs for fills, ghost notes, or “response” patterns.**
- **Experiment with clock rates and divisions for everything from rapid-fire glitches to staggered polyrhythms.**
- **Use the module with other logic, sequential switch, or clock manipulator modules for maximum rhythmic density and interplay.**

---

## References
- [ADDAC402 USER'S GUIDE PDF](http://media.addacsystem.com/firmwares/manuals/ADDAC402%20User%20Guide.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)