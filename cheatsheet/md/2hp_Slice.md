# 2hp — Slice

- [Manual PDF](../../manuals/2hp_Slice.pdf)

---

[2hp Slice Manual PDF](https://twohp.com/modules/slice)

---

# 2hp Slice (Beat Repeat/Glitch Engine) — Quick Reference Cheat Sheet

## **Jack Reference**

| Jack                | Function                                           | Voltage Range         |
|---------------------|---------------------------------------------------|----------------------|
| **Audio Input**     | Signal in for beat repeat/glitch                  | 10Vpp                |
| **Audio Output**    | Effected audio out                                | 10Vpp                |
| **Clock Input**     | External clock sets beat grid (from 10 BPM up)    | Audio rate possible  |
| **Trig/Gate Input** | Activates effect (latch or momentary selectable)  | Threshold: 0.4V      |
| **Size CV Input**   | CV control of repeat size (division/multiplier)   | -5V to +5V           |

---

## **Control Reference**

| Control               | Function                                                                              |
|-----------------------|---------------------------------------------------------------------------------------|
| **Trig Button**       | Manually activate beat repeat. Hold at boot to change mode (latch/momentary)         |
| **Trig LED**          | Shows gate mode, clock rate, buffer state:<br>• Green = Clock rate<br>• Dim White = Latch<br>• Dim Purple = Momentary |
| **Size Knob**         | Sets repeat size; range: 2 Bars, 1 Bar, 1/2, 1/4, 1/4 trip., 1/8, 1/8 trip., 1/16, 1/16 trip., 1/32, 1/64, 1/128, 1/256 |
| **Triplet Toggle**    | UP = Triplets included; DOWN = Remove triplet divisions/multiplications               |

---

## **Gate Behavior Modes**

- **Latching (Default)**: Effect stays on with gate HIGH, off with gate LOW.
- **Momentary**: Effect active only when gate is HIGH.
- **Change Mode:** Hold TRIG BUTTON while powering up to toggle between modes.

---

## **Installation Summary**

1. **Find 2HP space** in your rack.
2. **Connect power**: Align red stripe on cable with white line on PCB.
3. **Use either 5-pin row** on the connector (only 1 row on module).
4. **Mount module** with 2.5mm screws and supplied slide nuts.

---

## **Specs**

- **Width:** 2HP
- **Depth:** 45mm
- **Power:** +12V 85mA / -12V 7mA / +5V 0mA

---

## **Tips & Pairings**

- **Rnd:** Great for random/clock CV modulation.
- **Play:** Use for synced sample slicing.
- **Drum Machine:** Adds fills, triplets, and glitch to drum patterns.
- **Loop:** Loop and further manipulate glitch textures.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)