# Doepfer — A-160-2

- [Manual PDF](../../manuals/A-160-2.pdf)

---

[Doepfer A-160-2 Manual PDF](https://doepfer.de/a1602.htm)

---

## Using the Doepfer A-160-2 Clock/Trigger Divider II for Dense, Complex, and Hyper-Percussive Rhythms

The A-160-2 is a **clock/trigger/gate divider**—not a voice or audio effect, but a powerful rhythm-generation and event-manipulation tool in your Eurorack system. Here’s how to maximize its potential for complex, polyrhythmic, high-density percussion:

---

### 1. **Generating Complex & Polyrhythmic Patterns**

#### **Three Division Modes**
- **Power of Two:** 2, 4, 8, 16, 32, 64, 128
- **Prime Numbers:** 2, 3, 5, 7, 11, 13, 17
- **Integers:** 2, 3, 4, 5, 6, 7, 8

**Polyrhythm and Polytime Strategy:**
- Feed a steady **master clock** (from another clock source, LFO, or sequencer).
- Patch different outputs to various percussion trigger inputs (kick, snare, hats, etc).
- Use the **prime number** mode: Assign e.g., /3 (triplets), /5 (quintuplets), and /7 (septuplets) outputs to different percussive voices. This immediately interlocks non-aligning subdivisions, generating dense polyrhythms impossible with standard binary divides.
- Combine the **integer mode** (includes /4, /5, /6, /7, etc.) for even denser, cyclically evolving patterns.

#### **Layer and Cross-Trigger**
- Send multiple outputs into logic modules (AND, OR, XOR) to generate even more complex, shifting patterns—especially if those logics are fed from different division sets.

---

### 2. **Playing with Clock and Output Modes**

#### **Gate vs Trigger Mode**
- **Gate mode:** Outputs are held high for the length of the divided period (stays “on” for half the cycle at /2, a quarter at /4, etc).
- **Trigger mode**: Outputs are AND-wired with the input clock—pulses are as short as the incoming clock pulse, which can add a sharp, percussive attack.

> **Tip:** Use **Trigger Mode** for ultra-snappy percussion, or patch to a fixed-envelope generator for punchy blips. Use **Gate Mode** for sustained triggers, or patch to drum voices/envelopes that like held gates.

#### **Jumper Options for Advanced Tweaks**
- **Edge Selection:** The divider can act on either rising or falling edges of the clock, letting you subtly offset or shift grooves.
- **Output Polarity:** Invert the outputs for “negative logic” percussive hits—not only do you double your pattern complexity, but can trigger “reverse” or opposite hits from the same stream.
- **Reset Behavior:** Using resets, you can either tightly lock patterns to bar cycles or intentionally disrupt pattern alignment for phase-shifting, Steve Reich-like polyrhythm structures.

---

### 3. **Unique Patch Ideas for Complicated Patterns**

- **Multi-Drum Programming:** Each output goes to a unique drum sound. With the prime or integer divides, you get complex, never-repeating sequences.
- **Accent/Fill Creation:** Use one output to reset or re-trigger another sequencer or modulator, introducing periodic “jumps” or fills in a pattern.
- **Self-Patching for Shifting Grooves:** Patch one divider output into the reset of another, causing divisions to phase or “gate skip” in unpredictable ways.
- **Layer Multiple A-160-2s:** Chain outputs between modules (with different division modes) for extremely long and evolving rhythmic cycles.

---

### 4. **General Tips for Punchy, Percussive Results**
- Use the **shortest possible triggers** (trigger mode, tiny input clocks) for crisp, clicky percussion.
- Use logic and switch modules to alternate between odd divisions for evolving, morphing grooves.
- Pair with random modules, switches, or dynamic modulation on the clock/reset lines for generative unpredictability.

**Remember:**
- The A-160-2 is not a voice or effect, but a trigger/gate generator. Its musical power comes from controlling when other modules “fire.”
- Combine several A-160-2s, logic, random, and analog trigger logic for Richter-level rhythmic density and modular “math.”

---

**Further Reading:**
- [Doepfer A-160-2 Website/Manual PDF](https://doepfer.de/a1602.htm)
- [A160_2_jumpers.pdf – Jumper Layout & Customization](https://doepfer.de/a1602_jumper.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)