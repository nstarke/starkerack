# 2hp — Brst

- [Manual PDF](../../manuals/Brst_Manual.pdf)

---

[Brst Manual PDF](https://2hp.com/pages/brst-downloads)  
*(Link for reference, as manual source images are provided)*

---
# 2hp Brst Eurorack Module — Cheat Sheet

## Module Purpose
**Brst** is a voltage-controlled burst generator and trigger delay. When receiving a gate at **TRIG**, it outputs a user-defined burst of triggers with control over speed (rate) and number (pulses). Ideal for rhythmic bursts, fills, and generative percussion.

---

## Reference Summary

### Inputs
| Jack/Control     | Function                                            | Voltage Range     |
|------------------|-----------------------------------------------------|-------------------|
| **TRIG (Jack 1)**       | Trigger/Gate input to start a burst stream           | Threshold: 2.5V   |
| **PULSES CV (Jack 2)**  | CV input for # of pulses; adds to knob position      | 0–5V              |
| **RATE CV (Jack 4)**    | CV input for pulse speed; adds to knob position      | 0–5V              |

---

### Outputs
| Jack/Control    | Function                            | Voltage Range   |
|-----------------|-------------------------------------|-----------------|
| **OUT (Jack 8)**       | Burst output: stream of triggers            | 0–5V            |

---

### Controls
| Knob/Toggle           | Function                                                        | Range/Position    |
|-----------------------|-----------------------------------------------------------------|-------------------|
| **PULSES (Knob 3)**   | Sets number of triggers per burst                               | 1 (left) — 32 (right)  |
| **RATE (Knob 5)**     | Sets delay between triggers in a burst                          | 10ms (left) — 500ms (right) |
| **TRIG TOGGLE (Switch 6)** | Include/omit the initial trigger in the output           | Left: included; Right: omitted |
| **BURST LED (7)**     | LED: indicates burst activity                                   | —                 |

---

### Quick Use Steps

1. **Patch a gate/trigger signal** into **TRIG** jack (top).
2. **Set the number of pulses** per burst using the **PULSES** knob (far left: 1, far right: 32).
3. **Set burst rate** (time between triggers) using the **RATE** knob (far left: fast/10ms, far right: slow/500ms).
4. **Optional**: Modulate pulses and/or rate with CV by patching into **PULSES CV** or **RATE CV** (0–5V).
5. **Use the TRIG TOGGLE** to include (left) or omit (right) the initial input trigger as part of the output burst.
6. **Burst output** comes from the **OUT** jack (bottom).
7. **Monitor the BURST LED** for burst activity feedback.

---

### Power Consumption & Specs
- **Width:** 2 HP
- **Depth:** 47mm (Skiff friendly)
- **+12V:** 26mA / **-12V:** 7mA

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)