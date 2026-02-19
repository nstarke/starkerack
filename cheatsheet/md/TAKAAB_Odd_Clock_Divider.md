# TAKAAB — Odd Clock Divider

- [Manual PDF](../../manuals/TAKAAB OCD - Odd Clock Divider – Siam Modular.pdf)

---

[**TAKAAB OCD - Odd Clock Divider Manual**](https://siammodular.com/products/takaab-ocd-odd-clock-divider?srsltid=AfmBOopTsJBGyNaC6WtMfJJU3EFzdu1WvzDldMz3y6eA2c-lwQCE1iKj)

---

# TAKAAB OCD Odd Clock Divider — Cheat Sheet

## Module Quickstart

- **Type:** Clock Divider (Odd and uncommon divisions)
- **Width:** 2HP
- **Power:** Standard eurorack power

### How It Works
- Input a clock (2.5V–10V, up to 10KHz); module outputs divided clocks at 1/3, 1/5, 1/7, 1/9, and 1/10 (or by jumper: 1/3, 1/5, 1/7, 1/6, 1/10).
- All output clocks are 6V signals, 50% duty cycle, rounded down to the nearest pulse.
- Reset input or button restarts all divided clocks to the first step.

---

## Panel Controls & Connections

### Jacks
| Jack        | Type       | Function                                                  | Voltage Range  |
|-------------|------------|-----------------------------------------------------------|----------------|
| CLOCK IN    | Input      | Main clock input for division                             | 2.5V–10V, up to 10kHz |
| RESET       | Input      | Resets outputs to first pulse (trigger/gate/up-edge)      | 2.5V–10V, up to 10kHz |
| 1/3 OUT     | Output     | Outputs clock divided by 3 (HIGH:LOW = 1:2 for 1/3)      | 6V             |
| 1/5 OUT     | Output     | Outputs clock divided by 5 (1:4)                         | 6V             |
| 1/7 OUT     | Output     | Outputs clock divided by 7 (3:4)                         | 6V             |
| 1/9 OUT*    | Output     | Outputs clock divided by 9 (4:5) (*see jumper note)      | 6V             |
| 1/10 OUT    | Output     | Outputs clock divided by 10 (5:5)                        | 6V             |

\* By internal jumper, the 1/9 out can be set to 1/6 (ratio 4:2 HIGH:LOW).

### Panel Controls

| Control           | Type   | Function                                      |
|-------------------|--------|-----------------------------------------------|
| RESET Button      | Button | Manually resets all outputs to initial state  |

---

## Internal Jumpers/Headers

- **1/9 to 1/6 Jumper:** Onboard jumper changes 1/9 output to 1/6 (4:2 HIGH:LOW).
- **Normalize Headers:** 2-pin headers for chaining CLOCK IN/RESET signals between O/ECD modules (use Dupont jumper cable, one included).
- **Chained Reset:** Header for linking an adjacent unit’s reset with the manual RESET button.

---

## Usage Tips

- For clock divisions not covered by common modules (odd/prime/polyrhythms).
- Use the RESET input/button to keep multiple dividers in musical sync.
- Chain with Takaab UXS for front-panel jumper control.
- All outputs are pulse (square) at 6V max.

---

## Signal Reference Summary

- **CLOCK IN:** 2.5-10V, up to 10kHz, rising edge triggers.
- **RESET IN:** 2.5-10V, up to 10kHz, rising edge resets.
- **All OUTs:** 6V, square, 50% duty except 1/6 (4:2).
- **Manual RESET:** Button for instant sync.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)