# 2hp — Euclid

- [Manual PDF](../../manuals/2hp_Euclid.pdf)

---

[2hp Euclid Manual (PDF)](https://2hp.com/assets/files/euclid_manual.pdf)

---

# 2hp Euclid Cheat Sheet

Euclid is a 2hp rhythmic pattern generator based on Euclidean algorithms, producing cyclic and musical trigger patterns with flexible step and offset controls.

---

## I/O Jack Reference

| Jack / Control | Description                           | Voltage Range / Type     |
|:--------------:|:-------------------------------------:|:-----------------------:|
| **TRIG IN**    | Advances the pattern one step         | Trigger/Gate Input      |
| **RESET IN**   | Resets pattern to first step          | Trigger/Gate Input      |
| **LENGTH CV**  | CV control of pattern length          | 0–5V; summed w/ knob    |
| **STEPS CV**   | CV control of active steps            | 0–5V; summed w/ knob    |
| **TRIGGER OUT**| Output trigger when active step fires | +5V, 6ms pulse          |

---

## Control Reference

| Control          | Function                                     | Details                                               |
|------------------|----------------------------------------------|-------------------------------------------------------|
| **LENGTH (Knob)**| Sets pattern length (1–16 steps)             | Full Left: 1, Full Right: 16                          |
| **STEPS (Pot)**  | Sets # of active steps in pattern            | Min: 1 step, Center: ½ length, Max: full length       |
| **OFFSET POT**   | Sets pattern offset (initial step shift)     | Full Left: No offset, Full Right: Offset by Length-1   |
| **OUTPUT LED**   | Shows trigger output activity                | Lights when pattern fires an active step               |

---

## Quick Usage

1. **Connect** TRIG IN to your clock source. Each clock pulse advances the sequence.
2. **Connect** TRIGGER OUT to your drum(s) or destination module.
3. **Select pattern length** (LENGTH knob/CV) from 1 to 16 steps.
4. **Set active steps** (STEPS pot/CV) to distribute triggers within the pattern length.
5. **Apply offset** (OFFSET pot) to shift the starting point of the pattern.
6. **RESET IN** can be used to re-sync pattern start.

**All CV inputs accept 0–5V; values add to their respective knobs/pots.**

---

## Module Specs

- **Width:** 2hp
- **Current:** +12V 21mA / -12V 2mA
- **Depth:** 42mm

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)