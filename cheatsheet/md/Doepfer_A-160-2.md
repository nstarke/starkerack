# Doepfer — A-160-2

- [Manual PDF](../../manuals/A-160-2.pdf)

---

[Doepfer A-160-2 Manual (Source)](https://doepfer.de/a1602.htm)

# Doepfer A-160-2 Clock/Trigger Divider II  
**Cheat Sheet**

---

## Summary
The A-160-2 is an advanced clock/trigger/gate divider. It takes a clock input and produces seven simultaneous divided outputs (with selectable division patterns and output types). It’s useful for rhythm generation, clocking sequencers, and related timing duties in a Eurorack system.

---

## Inputs & Outputs

### 1. Clock In
- **Use:** Receives external clock, gate, or trigger.
- **Voltage Range:** Digital signal (logic) e.g. 0V = low, +10V = high.
- **Sources:** LFO, MIDI sync, MIDI-CV gate, etc.
- **Note:** Clock edge (rising or falling) can be set via PCB jumper.

### 2. Reset In
- **Use:** Resets output state according to mode.
- **Voltage Range:** High = >2.5V, Low = <1V.
- **Configurable by Jumpers:**
  - Level vs. edge trigger
  - Respond to positive or negative edge/level

### 3. Seven Clock Divided Outputs (per mode)
- **Voltage Range:** 0V (low), ≈ +10V (high)
- **Output Polarity:** Select non-inverted/inverted via PCB jumper

#### Output Division Types (selected via 3-way switch):
- **Powers of 2:** /2, /4, /8, /16, /32, /64, /128  
- **Prime Numbers:** /2, /3, /5, /7, /11, /13, /17  
- **Integer:** /2, /3, /4, /5, /6, /7, /8  

---

## Front Panel Controls

- **Division Set Selector (3-way toggle):**  
  Selects between:*Powers of Two, Prime Numbers, Integer Sequences*

- **Output Mode Selector (3-way toggle):**  
  - **Gate:** Each output stays "high" for half its division cycle.  
  - **Trig:** Each output is AND-wired with the incoming clock (follow clock pulsewidth).  
  - **"Cst" (Custom):** Not implemented in current firmware.

*No knobs, buttons, or sliders are present on the panel.*

---

## Internal Jumpers (on PCB, for advanced configuration)

- **Clock Edge:** Rising or falling edge triggers output state change.
- **Reset Behavior:** Level vs edge, positive vs negative.
- **Output Polarity:** Outputs normal or inverted.

For jumper locations/functions, see: [A160_2_jumpers.pdf (Doepfer)](https://doepfer.de/a1602_jp.pdf)

---

## Physical Specs

- **Width:** 4 HP (20mm)
- **Depth:** 35mm
- **Current:** +12V: 50mA, -12V: 0mA

---

## Key Usage Tips

- Connect your master clock source to "Clock In".
- Use "Reset In" for synchronized resets (e.g. when syncing rhythm to bar start).
- Use the top toggle to select which division family best fits your patch.
- Use the mode toggle to pick Gate or Trigger type outputs.
- All outputs are available simultaneously for creative patching.
- Unused center "Cst" output mode may offer new features with future firmware.

---

## Reference Links

- [Doepfer A-160-2 Product Page & Manual](https://doepfer.de/a1602.htm)
- [A160_2_jumpers.pdf (jumper config)](https://doepfer.de/a1602_jp.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)