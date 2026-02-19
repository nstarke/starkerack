# Mutable Instruments — Branches

- [Manual PDF](../../manuals/branches_quickstart.pdf)

---

[Branches Manual (PDF)](https://mutable-instruments.net/modules/branches/manual)

---

# Mutable Instruments Branches – Cheat Sheet

Dual Bernoulli Gate  
**Purpose:** Route incoming triggers/gates to one of two outputs with voltage-controllable probability, or as a toggle/latchable switch.

---

## Input/Output & Controls Reference

| Label        | Type         | Description                                              | Voltage Range          |
|--------------|--------------|----------------------------------------------------------|-----------------------|
| IN (1, 2)    | Input Jack   | Trigger/gate input (Section 2 normalled to Section 1)   | Standard trigger/gate |
| PROB CV (2)  | Input Jack   | CV for probability control (per section)                 | 0V–5V                 |
| OUT A (3)    | Output Jack  | Trigger/gate output "A"                                  | +5V                   |
| OUT B (4)    | Output Jack  | Trigger/gate output "B"                                  | +5V                   |

**Knob:**  
- **Probability Knob (A):** Adjusts probability between outputs A and B (higher = more to A).  
  - Counterclockwise: Output B only  
  - Center: 50/50 random  
  - Clockwise: Output A only

**Button:**  
- **Switch (B):**  
  - Quick press: Toggle "Toggle Mode" (output flips only when tails).  
  - Hold (>1s): Toggle "Latch Mode" (output stays high until next trigger on opposite output).

---

## Modes

- **Classic (Bernoulli) Gate:**  
  - Each input trigger randomly routed to OUT A or OUT B based on probability knob/CV.
  - In extremes, acts as a VC switch.

- **Toggle Mode:**  
  - Outcome decides whether to keep outputting to the same jack, or flip to the other.

- **Latch Mode:**  
  - OUT A or OUT B stays high (+5V) until the other output is activated.

---

## Power and Other Specs

- **Power:** +12V: 10mA, -12V: 1mA
- **Connect power cable so the red stripe (-12V) matches the marked side on the PCB!**

---

## Useful Links

- [Branches Full Manual](https://mutable-instruments.net/modules/branches/manual)
- [Mutable Instruments Forum](https://mutable-instruments.net/forum)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
