# 2hp — Turing Machine

- [Manual PDF](../../manuals/TM_Manual.pdf)

---

[**TM 2HP Eurorack Module Manual (PDF)**](https://2hp.com/docs/tm_manual.pdf)  
*(Use this official link or [here](https://2hp.com/docs/tm_manual.pdf) if unsure—the above is a placeholder as there's no link in the image)*

---

# **TM 2HP Cheat Sheet**

TM is a probabilistic random sequence generator for Eurorack inspired by Turing Machine concepts. It is ideal for generative and evolving sequences or controlled random voltage sources.

---

## **Front Panel Reference**

|**#**|**Label**|**Type**|**Function**|**Voltage Range**|
|-----|---------|--------|------------|-----------------|
| 1   | TRIG LED      | Visual    | Indicates change in sequence | N/A     |
| 2   | TRIG          | Input     | Trigger/gate to advance/shift sequence | Threshold: 2.5V |
| 3   | PROB CV       | Input     | CV for probability (random/locked) | 0–5V    |
| 4   | PROB          | Knob      | Sets probability of random voltage change per step. Left = always new, Right = locked. | N/A     |
| 5   | STEPS CV      | Input     | CV for sequence length | 0–5V    |
| 6   | STEPS         | Knob      | Sets sequence length; Left = 1, Right = 32 | N/A     |
| 7   | AMP           | Knob      | Scales output amplitude; Left = 0V, Right = 5V | N/A     |
| 8   | OUT           | Output    | Random stepped voltage | 0–5V    |

---

## **Quick Operation**

- **Power:** 2HP, 47mm depth (Skiff friendly), +12V: 23mA, -12V: 7mA
- **Install:** Ensure red stripe = -12V (down in most cases).
- **Trigger:** Send trigger/gate ≥2.5V to TRIG; step advances and decides to create new random voltage based on PROB.
- **PROB (Probability):**
  - **Left (100%):** Always generate new random voltage per step.
  - **Right (0%):** Sequence "locks" to current voltages, advances steps without further randomness.
  - **CV:** Patch in modulation (e.g., LFO, envelope) to vary randomness dynamically.
- **STEPS (Sequence Length):**
  - Sets how many steps before looping (1–32). CV controllable.
- **AMP (Amplitude):**
  - Sets range of output voltage. Full right = up to 5V, full left = 0V.
- **OUT:** Output stepped random CV to pitch quantizer, filter cutoff, etc.

---

## **Patch Tips**
- For evolving melodies, patch OUT to a quantizer then to an oscillator pitch input.
- Use an LFO or random CV into PROB CV for dynamic randomness control.
- Adjust STEPS to taste for short or extended looping patterns.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)