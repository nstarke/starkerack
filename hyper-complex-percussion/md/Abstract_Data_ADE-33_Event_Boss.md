# Abstract Data — ADE-33 Event Boss

- [Manual PDF](../../manuals/ADE33_Manual_v1_0.pdf)

---

[Abstract Data ADE-33 EVENT BOSS Manual PDF](https://www.abstractdata.biz/files/ADE-33%20User%20Guide%201.01.pdf)

---

# Using the Abstract Data ADE-33 Event Boss for Hyper-Complex Percussion

The **ADE-33 Event Boss** is a Eurorack module tailor-made for innovative pattern and rhythm manipulation, making it ideal for musicians seeking dense, intricate, and hyper-rhythmic percussion. Below are targeted approaches and patch ideas specifically for maximizing polyrhythms, odd time signatures, and complex groove generation with this module.

---

## Core Strategies for Advanced Percussion

### 1. **Polyrhythmic Clocking & Input Feeding**

- **Multiple Inputs:** Feed two or more unrelated clocks (e.g., 3:4:5:7 divisions) into `IN: GATE A1`, `A2`, and even `B/CV` (in Logic Mode).
- **Irregular Clocks:** Use looping or random triggers/LFOs not aligned with common tempos—great for evolving polyrhythm and cross-rhythm feel.
- **Multiclock Patterns:** Use a master clock split and divided/multiplied by modules like ADE-33’s **Multiples Mode** for nested polyrhythms.

### 2. **Complex Time Signatures**

- **Multiplicity & Division:** In **Multiples Mode**, set division and multiplication factors (including nonstandard like ÷5, ×7, ×12) via CV for non-4/4 patterns.
- Trigger percussion voices with the ADE-33 output to create shifting/compound time signatures and pulses.

### 3. **Probability & Randomization for Evolving Sequences**

- **Probability Mode:** Insert slow LFOs into `GATE B/CV` to morph the probability, causing patterns to evolve, drop/hit notes unpredictably, or tie gates for rolling fills or bursts.
- **Flip-Flop & Inversion Modes:** Ideal for “glitch,” IDM, or breakcore-style percussive lines with unexpected reversals and inflections.

### 4. **Logic Mode for Pattern Complexity**

- **Boolean Combinations:** Patch two rhythmical signals into `A1`/`A2` and `B/CV`, then switch logic types (AND, OR, XOR, etc.)—perfect for generating new, computationally complex percussion triggers from simple inputs.
- **Dynamic Logic Switching:** Use CV to flip which input is active (A1/A2), introducing time-variant logic routing in mid-performance!

### 5. **Phase Shifting & Mark/Space for Groove**

- **Phase Mode:** Apply CV (envelopes, stepped LFOs) to shift triggers ahead/behind or change mark/space ratios for swing, offset, and “drunken” rhythms.
- **Non-Quantized Shifts:** Tweak phase in ms for extreme, microtimed, shuffled patterns—push percussion off-grid for maximal groove.

### 6. **Variable Gate Lengths for Percussive Voice Articulation**

- **Gates Mode:** Manipulate how long a gate stays high/low to trigger envelope shapes with punch or accent (long gates for ROOOOOLL, short for TICK).
- Use fast-moving CV on `GATE B/CV` for ratcheting and rapid-fire hi-hat/snare/backbeat triggers.

---

## Versatile Patch Ideas

### **Example 1: Complex Polyrhythm with Logic**
1. Patch a 5-step clock to `IN: GATE A1`, and a 7-step clock to `IN: GATE B/CV`.
2. Set to Logic Mode and try XOR or AND.
3. Output to a percussion module’s trigger; you’ll get a composite rhythm—perfect for metallic percussion or syncopated bass drums.

### **Example 2: Morphing, Evolving Beats**
1. Send clock to `GATE A1`, random triggers to `GATE A2`.
2. Use Probability Mode, morph percentage with random/s&H/CV into `GATE B/CV`.
3. Output to open hats or rimshot—watch as the pattern densifies and thins out organically.

### **Example 3: Polymetric Layers**
1. Master clock > clock divider (x5) > `GATE A1`.
2. Master clock > divider (x4) > `GATE A2`.
3. Multiples Mode, select mult/div factor for each local mode—assign different percussion voices to the ADE-33 outputs to create a shifting layered drum bed.

### **Example 4: Advanced Swing & Groove**
1. Patch clock to `GATE A1`, slow triangle or stepped random LFO to `GATE B/CV`.
2. Phase Mode, use Percentage or ms Shift, then output to closed hats or rimshots for off-grid, J Dilla-style “drunken” beats.

### **Example 5: Unique, Punchy Percussive Voice Shaping**
- Use Gates Mode’s variable length outputs to trigger VCAs/EGs tied to percussion modules (kick/snare) for super punchy attacks or unusual decays.
- **Logic Hold** can “mute” a drum channel with performance gestures or accentuate offbeats with probability logic.

---

## Further Tips for Maximum Percussive Uniqueness

- **Layer Multiple Event Bosses:** For extreme density, chain multiple ADE-33 units or cascade outputs through sequencers and other logic modules.
- **Modulate Everything:** Assign random, Euclidean, or chaos-based CV sources to all CV-controllable ADE-33 parameters for ongoing mutation.
- **Integrate with Effects:** Use the rhythmic gates/triggers to ping filters, VCA gates, or sync effects (delays, bitcrushers, etc.) for percussive textures beyond conventional drum machines.

---

**Reference: For complete details, see the [ADE-33 Event Boss User Guide PDF](https://www.abstractdata.biz/files/ADE-33%20User%20Guide%201.01.pdf)**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)