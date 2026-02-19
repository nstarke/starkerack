# Erogenous Tones — Levita8

- [Manual PDF](../../manuals/l8-instructions.pdf)

---

[LEVIT8 Manual (PDF)](http://erogenous-tones.com/files/LEVIT8-Manual-1.0.pdf)

---
# **LEVIT8 (Erogenous Tones) – Cheat Sheet**

**Description:**  
8x Attenuator / Gain / Inverter / Mixer utility for Eurorack. Handles Audio, Gates, CVs, and mixes DC audio or modulation signals.

---

## **Jacks & Voltage Ranges**

| JACK        | FUNCTION                                             | VOLTAGE RANGE   |
|-------------|------------------------------------------------------|-----------------|
| INPUT 1–8   | Signal/CV/Gate input. Normalled to +5V if nothing plugged in.  | -10V to +10V (saturates here) |
| OUTPUT 1–8  | Channel output. Can be channel, sub-mix, or full-mix depending on switch state.| -10V to +10V |

---

## **Knobs, Switches & Controls**

| CONTROL            | DESCRIPTION                                                                       |
|--------------------|-----------------------------------------------------------------------------------|
| **8 x Attenuator/Gain Knobs** | Linear. Sets gain/attenuation (-2x to +2x with inversion). 0 = off.           |
| **4 x Invert Switches (CH2,4,6,8)** | Inverts polarity of their respective channels but not the others.            |
| **2 x MIX Switches (CH4 and CH8)**  | UP: Mixes first 4 channels to OUT4, and all 8 to OUT8 (when both up); see mixing modes below.  |
| **8 x Bi-LEDs**                   | Shows post-knob/switch signal polarity and level (Green = +ve, Red = -ve).  |

---

## **Mixing Modes**

- **All MIX Switches DOWN**:  
  > All 8 channels act as independent attenuators/gain/inverters.
- **CH4 MIX UP, CH8 MIX DOWN**:  
  > OUT4 = MIX of CH1–4; OUTS 1–3 = PASS-THRU; OUT5–8 = normal.
- **CH4 MIX UP, CH8 MIX UP**:  
  > OUT4 = MIX of CH1–4; OUT8 = MIX of CH5–8; OUT 1–3/5–7 = PASS-THRU.
- **CH4 MIX DOWN, CH8 MIX UP**:  
  > OUT8 = MIX of CH1–8; OUT 1–7 = PASS-THRU.
- **In All Modes**:  
  > Jacks with no cable receive +5V (can generate DC offset, 0–10V or -10V to +10V with inversion).

---

## **Tips & Tricks**

- Use as ±Gain, Attenuator, Inverter, Mixer, or DC Bias generator.
- Remove a channel from a mix (no signal) by setting its knob to zero (prevents DC offset in sum).
- Great for audio, CV, gates, logic signals.
- Channels saturate at ±10V.

---

## **Quick Reference**

- **Input range:** -10V to +10V (saturates here).
- **Max gain:** ≈2x (linear).
- **No cable = +5V normalized — great for offsets.**
- **CH2/4/6/8 have INVERT switches.**
- **CH4/8 have MIX switches for flexible summing/parallel use.**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
