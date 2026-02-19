# 2hp — Rnd

- [Manual PDF](../../manuals/2hp_Rnd.pdf)

---

[Download the Rnd Manual PDF](https://2hp.com/manuals/Rnd.pdf)

---

# 2hp Rnd Module - Cheat Sheet

2hp Rnd is a compact dual random generator for Eurorack—perfect for modulation and unpredictable rhythmic sources.

---

## Panel Overview

**Top to Bottom:**
1. **INT/EXT Switch**  
2. **CLOCK Jack**  
3. **RATE Knob & LED**
4. **GATE Output**
5. **SMOOTH Attenuator & Output**
6. **QUANT Attenuator & Output**

---

## Controls & Jacks Reference

| Label          | Type     | Description                                                    | Range / Function      |
|----------------|----------|----------------------------------------------------------------|----------------------|
| INT / EXT      | Switch   | Selects clock source: Internal (L) or External (R)             | -                    |
| CLOCK          | Jack     | - INT: CV for internal clock rate<br>- EXT: Clock input        | CV Input: 0V-10V     |
| RATE           | Knob & LED | - INT Clock: Internal clock rate<br>- EXT Clock: Gate randomness rate<br>- Smooth: Rate of change| Slow (L) → Fast (R)     |
| GATE           | Output   | - INT: 50% duty cycle clock output<br>- EXT: Random gate output| 0V (low), 10V (high) |
| SMOOTH Attenuator | Knob | Sets output level of Smooth random voltage                     | 0V–10V               |
| SMOOTH         | Output   | Continuously changing random voltage, rate set by Rate knob    | 0V–10V               |
| QUANT Attenuator | Knob  | Sets output level for Quant output                             | 0V–10V               |
| QUANT          | Output   | New random voltage at every clock pulse (stepped)              | 0V–10V               |

---

## Quick Operation Guide

- **Internal Clock Mode**: (Switch left)
  - Use RATE to set clock speed. GATE outputs steady clock, QUANT changes every tick.
  - CLOCK jack can take CV to modulate clock rate.

- **External Clock Mode**: (Switch right)
  - CLOCK jack receives external clock.
  - GATE outputs random gates ("eruptions"); RATE sets probability/rate of rand gates.
  - QUANT outputs new stepped random voltage every external clock pulse.

- **SMOOTH Output**
  - Continuously changing random voltage.
  - Rate of change and output level set via RATE and SMOOTH ATTEN.

- **QUANT Output**
  - New value each time the module is clocked (internal/external).
  - Output level set via QUANT ATTEN.

---

## Voltage Ranges

- All outputs (GATE, SMOOTH, QUANT): **0V–10V**
- CLOCK CV Input: **0V–10V**

---

## Patch Tips

- Use **GATE** to trigger envelopes or events unpredictably.
- Use **SMOOTH** for organic, flowing modulations (filters, FM, etc).
- Use **QUANT** for stepped random sequences or pitch modulation.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
