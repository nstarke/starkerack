# Erica Synths — Cowbell

- [Manual PDF](../../manuals/cow_bell_Manual.pdf)

---

[Erica Synths Cowbell Manual (Reference Images)](uploaded-file-link) <!-- Replace with actual PDF link if available -->

---

# Erica Synths Cowbell (Eurorack) Cheat Sheet

**Type:** Analogue Percussion (Cowbell) | **HP:** 6 | **Depth:** 30mm | **Power:** 14mA @ +12V, 10mA @ -12V  
**Decay:** 120ms – 1100ms  
**Audio Output Level:** ±5V  

---

## Panel Overview

| **Control**         | **Function**                                                                           |
|---------------------|----------------------------------------------------------------------------------------|
| **Tune (Knob)**     | Sets master pitch of the cowbell                                                       |
| **Decay (Knob)**    | Sets length of the sound (shorter/longer than vintage cowbells)                        |
| **Tune CV Lvl (Knob)** | Attenuates CV amount sent to Tune                                                    |
| **Manual Trigger (Button)** | Triggers cowbell manually—ideal for checking sound settings or jamming live    |
| **LED**             | Flashes to indicate incoming triggers                                                  |

---

## Jacks and Voltages

| **Jack**                | **Type**     | **Voltage Range**           | **Function**                          |
|-------------------------|--------------|-----------------------------|---------------------------------------|
| **TRIGG (In)**          | Input        | +5V gate/trigger            | Triggers the cowbell (1ms gate)       |
| **ACC (In)**            | Input        | 0–+10V CV                   | Accent—+10V = maximum volume          |
| **TUNE CV (In)**        | Input        | ±5V CV                      | Controls tuning (pitch); attenuated   |
| **OUT (Out)**           | Output       | ±5V audio                   | Main cowbell audio out                |

---

## Typical Patch Instructions

1. **Connect GATE/TRIG:**
   - Patch drums/sequence gate signal to **TRIGG** input (+5V percussive trigger required).

2. **Patch Tune Modulation:**  
   - Patch LFO, sequencer, or envelope to **TUNE CV** to modulate cowbell pitch.
   - Use **Tune CV Lvl** to set modulation depth.

3. **Patch Accent:**
   - Use envelope, trigger, or CV source to **ACC** for velocity/accented strikes. +10V = max.

4. **Get Audio Out:**
   - Connect **OUT** to your mixer, VCA, or effects.

5. **Manual Play:**
   - Tap Manual Trigger for finger-play/live fills or sound check.

---

## Reference

- **TRIGG IN:** +5V Gate/Trigger
- **ACCENT IN:** 0V–+10V (max vol = +10V)
- **TUNE CV IN:** -5V to +5V (attenuated)
- **AUDIO OUT:** -5V to +5V

**Other Notes:**  
- Wide decay time range (120ms–1100ms).
- Use in dry conditions only; keep original box for warranty.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)