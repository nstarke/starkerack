# 2hp — Blur

- [Manual PDF](../../manuals/2hp_Blur.pdf)

---

[2hp Blur Manual PDF](https://www.twohp.com/modules/blur)

---

# 2hp Blur Eurorack Module Cheat Sheet

**Description:**  
Blur is a spectral processor that transforms audio by smearing frequency content, enabling reverb-esque pads and time-stretched textures.

---

## Panel Overview

| Jack/Control | Type    | Description                                                                | Range         |
|:-------------|:--------|:---------------------------------------------------------------------------|:--------------|
| `IN`         | Input   | Main audio input                                                           | 10Vpp         |
| `TIME`       | Knob    | Amount of spectral time stretch; x1 at center, up to x16 to the right      | -             |
| `TIME` (CV)  | CV In   | Controls Time parameter                                                    | -5V to +5V    |
| `VIBE`       | Knob    | Spectral spread/frequency wash; left = clear, right = smeared/washed out   | -             |
| `VIBE` (CV)  | CV In   | Controls Vibe parameter                                                    | -5V to +5V    |
| `MIX`        | Knob    | Dry/Wet blend; left = dry, right = wet                                     | -             |
| `MIX` (CV)   | CV In   | Controls Mix balance                                                       | -5V to +5V    |
| `OUT`        | Output  | Audio output                                                               | 10Vpp         |

---

## Quickstart

1. **Patch audio into `IN`.**
2. **Patch from `OUT` into your system.**
3. **Set `TIME` to control stretch:**
   - Left = normal/short playback
   - Center = original speed
   - Right = up to x16 stretch
4. **Set `VIBE`:**
   - Left = original timbre
   - Right = washed spectral pad
5. **Set `MIX`:**
   - Left = dry (original signal)
   - Right = wet (processed)
6. **Modulate with CV:**
   - Patch CV (−5V to +5V) into `TIME`, `VIBE`, or `MIX` for dynamic control.

---

## Voltage Reference

| CV Input      | Voltage Range   | Function                        |
|:--------------|:---------------|:--------------------------------|
| `TIME` (CV)   | -5V to +5V     | Spectral time-stretch amount    |
| `VIBE` (CV)   | -5V to +5V     | Frequency spread/smear          |
| `MIX` (CV)    | -5V to +5V     | Dry/Wet blending                |
| Input Audio   | ~10Vpp         | Line/Eurorack level             |
| Output Audio  | ~10Vpp         | Line/Eurorack level             |

---

## Power & Physical

- Width: **2HP**
- Depth: **46mm**
- Power: +12V 85mA, -12V 7mA, +5V 0mA

**Connect the power cable with the red stripe aligning with the module's white line marking!**

---

## Patch Ideas

- **Pad/Pluck:** Pair with transient-rich sources (e.g. Pluck) for ambient pads
- **Layered Ambience:** Use before or after reverb for wider pads (e.g. 2x Blur → Verb)
- **Pitch Processing:** Chain with pitch shifting for harmonic textures
- **Super Saws/Pulse:** Hyper saws (Swarm) sound lush when blurred

---

**[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**