# Doepfer — A-160-5

- [Manual PDF](../../manuals/A-160-5.pdf)

---

[Doepfer A-160-5 Voltage Controlled Clock Multiplier / Ratcheting Controller - Official Manual](https://doepfer.de/a1605.htm)

---

# Doepfer A-160-5 Cheat Sheet

## Overview

The A-160-5 is a **voltage controlled clock multiplier** with **ratcheting capability**. It takes an incoming clock source and outputs a clock at a multiplied rate. The multiplication factor is manually set or controlled via CV (0 to +5V), with different factor modes selectable. Ideal for creating rhythmic complexity, especially "ratcheting" patterns as used by Tangerine Dream.

---

## Quickstart

1. **Clock Input:** Patch your main clock/Gate source to `Clock In`.
2. **Clock Output:** Patch `Clock Out` to send multiplied clock pulses to sequencers, ADSRs, etc.
3. **Set Multiply Factor:**
    - *Manual*: Use the `Manual` knob (no CV patched).
    - *CV Controlled*: Patch 0…+5V CV to `CV In` (overrides manual).
4. **Select Mode:** Set the 3-way toggle to choose multiplication factors (Integers, Powers-of-two, or Mixed).
5. **Monitor LEDs:**
    - 8 LEDs: Show current multiplication factor.
    - 2 LEDs: Show live clock In and Out activity.

---

## Inputs & Outputs

| Jack/Control  | Type      | Details                                             | Voltage Range      |
|---------------|-----------|----------------------------------------------------|--------------------|
| **Clock In**  | Input     | Receives external clock/gate signal                 | Typical gate/clk   |
| **Clock Out** | Output    | Multiplied clock output                             | Same as input      |
| **CV In**     | Input     | Sets multiplication factor (overrides Manual Knob)  | 0 to +5V           |
| **Manual**    | Knob      | Sets multiplication (normalled to CV In if unpatched) | 0 to +5V (internally generated)|
| **Mode**      | 3-way Switch | Selects multiplication table:         |                    |
|               |           | - Left: Integer values (1,2,3...8)                 |                    |
|               |           | - Middle: Powers of two (1,2,4,8...)               |                    |
|               |           | - Right: Mixed values                              |                    |

---

## Reference – Controls

- **Manual Knob:** Adjusts multiplication factor (0V = mute).
- **Mode Toggle:**  
  - **Left** (Ganzzahlige Werte): 1–8  
  - **Middle** (2er-Potenzen): 1, 2, 4, 8  
  - **Right** (Mix): 1, 2, 3, 4, 6, 8, etc.
- **LED Matrix:** Indicates active multiplication factor (first LED = 1, up to 8).
- **"Clock In" LED:** Blinks with incoming clock.
- **"Clock Out" LED:** Blinks with outgoing (multiplied) clock.

---

## Tips

- **No Output at 0V:** If your Manual knob or CV input is fully CCW/0V, module mutes the clock output.
- **Dynamic Ratcheting:** Use sequencer CV lanes to automate ratchet counts for each step.
- **Allow Stabilization:** After sudden clock changes, the output clock may lag a few pulses as it recalculates multiplication.

---

## Technical Data

- **Width:** 4 HP (20mm)
- **Depth:** 35mm
- **Current:** +50mA (+12V), -0mA (-12V)

---

## Patch Example

- **Sequencer Clock:** Out from A-155/A-154 to `Clock In`.
- **Gate Multiplication:** `Clock Out` to envelope/trigger destination.
- **Ratchet Control:** Sequencer CV to `CV In` to vary pulse count per step.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)