# Mutable Instruments — Marbles

- [Manual PDF](../../manuals/Mutable Instruments - Marbles.pdf)

---

[Marbles Original Printed Manual (PDF)](https://mutable-instruments.net/modules/marbles/manual.pdf)

# Mutable Instruments Marbles Cheat Sheet

Marbles is a random sampler and generator designed for creating organic and musical gates and CV patterns, with looping and quantization options. Use it for innovative rhythms, melodies, and lively random modulations.

---

## Panel Overview

**Sections:**

- **t Section (Clock & Gates) — Left**
- **X Section (Random Voltages) — Right**

---

## Input & Output Reference

### Inputs

| Jack          | Section  | Function                                         | Voltage Range           |
|---------------|----------|--------------------------------------------------|-------------------------|
| Clock IN      | t        | External clock                                   | -5V to +5V (max: +8V)   |
| Jitter CV     | t        | Controls clock jitter                            | -5V to +5V              |
| Bias CV       | t        | Rhythm generator bias                            | -5V to +5V              |
| DejaVu CV     | t/X      | Loop/shuffle probability                         | -5V to +5V              |
| Spread CV     | X        | Distribution spread of random voltage            | -5V to +5V              |
| Bias CV       | X        | Skew random voltage up/down                      | -5V to +5V              |
| Stepping/Slew CV | X     | Quantization/Slew amount                         | -5V to +5V              |
| X External CV | X        | Replaces internal random voltage (loopable)      | -5V to +5V              |

### Outputs

| Jack             | Section | Function                                      | Voltage Range            |
|------------------|---------|-----------------------------------------------|--------------------------|
| t1, t2, t3 OUT   | t       | Clock/gate outputs                            | 0V (low) to +8V (high)   |
| X1, X2, X3 OUT   | X       | Random CV outputs                             | 0 to +2V / 0 to +5V / -5V to +5V (settable) |
| X4 (Varies)      | X       | Auxiliary/random output (depends on settings) | same as above            |

---

## Controls Reference

| Name             | Type                 | Section  | Function                                                     |
|------------------|----------------------|----------|--------------------------------------------------------------|
| CLOCK            | Knob                 | t        | Set internal clock rate (or divide/mult ext. clk w/button)   |
| JITTER           | Knob + CV            | t        | Add timing randomness to clock                               |
| BIAS             | Knob + CV            | t        | Distribute rhythm b/w outputs                                |
| GATE LENGTH      | Knob                 | t        | Gate/trig duration; can be randomized per step               |
| STEPS            | Knob + CV            | X        | Steps/Quant (CW = more quant, CCW = more slew)               |
| SPREAD           | Knob + CV            | X        | Adjust output voltage distribution (bell, uniform, etc.)      |
| BIAS             | Knob + CV            | X        | Pushes CV up/down                                            |
| OUTPUT RANGE     | Button               | X        | Selects CV output voltage: 0-2V, 0-5V, or -5V/+5V            |
| QUANTIZE SCALE   | Programmable         | X        | Play in samples to teach scale (6 scales storable)           |
| DEJAVU           | Knob + CV            | t/X      | Probability looping/replaying/shuffling material              |
| LOOP LENGTH      | Button (Shift)       | t/X      | Selects loop length (1-16 steps)                             |
| DIV/MULT RANGE   | Button               | t        | Sets clock division/multiplication factor                    |
| GENERATION MODE  | Button               | t        | Switches between routing, division, drum pattern models      |
| FOLLOW/PREDICT   | Rhythm Follower      | t        | Locks to complex external patterns automatically             |

---

## Quick Feature Rundown

- **Random Gate Generator:** Generates three gate streams with related or independently randomized timing.
- **Master Clock:** Internal or external synchronization, with division/multiplication and jitter.
- **Random Rhythm Models:** Random routing, division, or "Grids-style" drum patterns.
- **Random Voltage Generator:** Up to three simultaneous CVs, clocked by t outputs or external clock, with flexible distribution and range.
- **Quantization/Slew:** Step or smooth outputs; programmable scales learned by playing them in.
- **Random Looping (DejaVu):** Loop/reorder random sequences; up to 16 steps, looped or randomly shuffled.
- **CV Post-processing:** All CV transformations (spread, bias, quant, slew, deja vu, etc.) can be applied to external signals.
- **Output Diversity:** Each output (t/x) can operate with shared or complementary randomness.
- **High Quality Spec:** 14-bit DAC (error <1mV), 12-bit CV capture, Computer Modern typeface.

---

## Typical Use Flow

1. **Patch t OUT(s) to trigger your envelopes/drums/sequencers.**
2. **Patch X OUT(s) to pitch, filter, CV, or other destinations.**
3. **Dial in clock rate, jitter, and rhythm model for desired groove.**
4. **Select voltage range and spread/bias for melody/CV flavor.**
5. **Set STEPS for classic steps or turn CCW for smooth modulation.**
6. **Use DEJAVU to create loops or variations in the randomness.**
7. **Quantize to a scale by teaching it the notes (jam in the scale via buttons as described in full manual).**
8. **Inject external clock/CV for interactive or synced results.**

---

## Reference

- **HP:** 18
- **Power:** +12V 80mA, -12V 20mA
- **Depth:** 25mm
- **CV Input Range:** -5V/+5V
- **CV Output Range:** 0-2V, 0-5V, -5/+5V (selectable)
- **Gate Output:** 0V to +8V

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)