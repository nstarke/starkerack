# 2hp — Div

- [Manual PDF](../../manuals/Div_Manual.pdf)

---

[2hp Div Manual PDF](https://2hp.com/wp-content/uploads/Div_Manual.pdf)

---

## Using the 2hp Div for Hyper-Complex Rhythmic Percussion in Eurorack

Creating densely layered, hyper-complex percussion with polyrhythms and unusual time signatures is one of the most rewarding uses of the [2hp Div](https://2hp.com/modules/div/) in a Eurorack system. Here’s how to unlock that in your setup:

---

### Module Capabilities at a Glance

- **Dual Clock Processor:** Two independent channels, each with a dedicated division/multiplication knob and CV input.
- **Clock Division/Multiplication:** Each channel can divide or multiply an input clock by: 1, 2, 3, 4, 5, 6, 7, 8, or 16.
- **CV Control:** External voltage (0–5V) can sweep the division/multiplication ratios for real-time variety.

---

### The Heart of Hyper-Complex Rhythms: Polyrhythms and Unusual Patterns

#### **1. Build Polyrhythms with Odd Divisions**

- Patch a master clock (such as from a sequencer or dedicated clock module) into the **IN** jack.
- Set **RATE 1** to an odd number (e.g., 3) and **RATE 2** to an even or another odd (e.g., 4, 5, or 7).
- Send **OUT 1** and **OUT 2** to trigger different percussion voices.
- Example: Channel 1 = /5 (quintuplets), Channel 2 = /4 (quarter notes). Together, they create a 5:4 polyrhythm.

#### **2. Dynamic Complexity via CV Control**

- Use a slowly evolving LFO or sequencer to modulate **RATE 1 CV** or **RATE 2 CV** inputs.
- You can change clock divisions on the fly, morphing from simple to hyper-complex patterns.
- This hands-free variation is essential for achieving ever-shifting, intricate patterns.

#### **3. Multiply for Speed and Microtiming**

- Set one channel to multiply (e.g., x7, x8, or x16). 
- Use high-multiplier outputs for rapid triggers—great for ratcheting effects or fills.
- Combine these bursts of triggers with slower divisions for texture and contrast.

#### **4. Layered Patterns for Dense Grooves**

- Patch both OUT 1 and OUT 2 to different percussion modules, envelopes, or sample triggers.
- Combine two Div modules for even more intricate layers.
- Chain Div’s OUTs into each other's INs (e.g., OUT 2 -> another Div’s IN) for “nested” rhythms.

#### **5. Irregular/Complex Time Signatures**

- Experiment with odd-numbered divisions (7, 5, etc.) and multiplications.
- Sequence changes in RATE settings synchronized to musical phrases for rhythmic sophistication.
- Patch divided/multiplied outs into switch modules or logic (AND/OR) for even more nuanced patterns.

---

### Advanced Tips

- **Probability/Randomness:** Feed divided clocks into a sample-and-hold, logic, or probability skipper for glitchy, ever-changing rhythms.
- **Syncopation:** Use swing clocks or deliberately offset divisions with short gate delays.
- **Modulation Source:** Use the outs to drive not just drums but stepped modulators, creating polyrhythmic parameter changes elsewhere in your rack.

---

### Example Patch

1. **Clock Source → Div IN**
2. **OUT 1 (÷7) → Hi-hat Trigger**
3. **OUT 2 (×5) → Snare Trigger**
4. **RATE 2 CV** modulated by stepped random voltage for unpredictable snare placement.

Repeat with different voices/cv sources for a layered, polyrhythmic percussion system.

---

Explore, experiment, and you’ll find the 2hp Div is a secret weapon for percussionists and rhythmic synthesists alike!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)