# Tiptop Audio — RS808

- [Manual PDF](../../manuals/Tiptop_Audio_RS808_ns.pdf)

---

[RS808 Manual PDF](https://www.tiptopaudio.com/808-2)

---

# Tiptop Audio RS808 Cheat Sheet

**The RS808 is a TR-808 Rimshot/Clavs sound generator for Eurorack, offering expanded control over classic 808 percussion sounds.**

---

## Quick Start

1. **Connect GATE IN to a gate/trigger source.**
2. **Connect RS/CL OUT to your audio system.**
3. **Set LEVEL halfway, both toggle switches down (Rimshot).**
4. **Set SNAP ~30%, PITCH ~50%.**
5. **Flip both toggles up for Clavs; experiment with combinations for other sounds.**

---

## Panel Overview

| Control/Jack           | Function                                                                   |
|------------------------|----------------------------------------------------------------------------|
| LEVEL (Knob)           | Output volume of the module.                                               |
| SNAP (Knob)            | Height/strength of internal envelope (adds "snap" to sound).               |
| PITCH (Knob)           | Sets frequency/pitch of the sound (not on original TR-808).                |
| ACCENT (Knob)          | Adjusts dynamic accent/gain for triggered notes.                            |
| ACCENT IN (Jack)       | Gate/trigger for accent—sets loudness/attack dynamically.<br>Voltage Range: **0 to 10V** gate preferred.                                   |
| GATE IN (Jack)         | Main gate/trigger input to fire sound.<br>Voltage Range: **0 to 10V** gate/trigger.                 |
| RS/CL OUT (Jack)       | Main audio output. Output level: **Eurorack line level (~10Vpp or less)**.                      |
| Toggle Switches (2x)   | **Sound selection:**<br>- Both down: Rimshot<br>- Both up: Clavs<br>- Left up/Right down: Blend/Hybrid<br>- Left down/Right up: Short click |

---

## Sound Selection via Toggles

- **Both DOWN:** Classic 808 *Rimshot*
- **Both UP:** 808 *Clavs*
- **Left UP / Right DOWN:** Hybrid (mix of Clavs & Rimshot), nonlinear mix
- **Left DOWN / Right UP:** Short “click” sound

---

## Patch Reference

| Jack        | Type         | Expected Signal        | Function                         |
|-------------|--------------|-----------------------|----------------------------------|
| GATE IN     | CV input     | 0–10V gate/trigger    | Triggers sound                   |
| ACCENT IN   | CV input     | 0–10V gate/trigger    | Dynamic accent control           |
| RS/CL OUT   | Audio output | 10Vpp max (typical)   | Module output                    |

---

## Additional Notes

- **SNAP** and **PITCH**: New controls absent from original TR-808, enable deeper sound design possibilities.
- **Accent Routing:**  
   - With no ACCENT IN jack inserted, **GATE IN** is normalized to ACCENT for extra punch.
   - If ACCENT IN is patched, control accent dynamically via gates/triggers or CV.
- **ACCENT Knob**: Acts as gain fine-tune if no accent gate present; sets accent amplitude difference if ACCENT IN is used.

---

For more, visit the [RS808 product page](https://www.tiptopaudio.com/808-2).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)