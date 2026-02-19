# Omnitone — Beatsi

- [Manual PDF](../../manuals/Beatsi_Information_Package.pdf)

---

**[Beatsi Eurorack Module Manual (PDF)](attachment-link-placeholder)**

---

# Beatsi Eurorack Cheat Sheet

> **Beatsi** is a compact, digital module for modular drum synthesis (not samples or physical modeling). Sounds are based on virtual drum-synth building blocks and organized into three "kits":  
> - **Orange:** Acoustic/Basic  
> - **Blue:** Low-fi  
> - **Green:** Alien

---

## 1. **Panel Controls & Navigation**

### **Encoders**
- **Parameter Encoder:**  
  - Turn: Scroll parameters (Timbre, Pitch, Decay, Level) for each drum piece.  
  - Short Press: Assign selected parameter to CV1.  
  - Long Press: Edit **attenuverting** for CV1 on selected parameter.
- **Value Encoder:**  
  - Turn: Adjust the value for the selected parameter.  
  - Short Press: Assign selected parameter to CV2.  
  - Long Press: Edit **attenuverting** for CV2 on selected parameter.  
  - **Press both encoders:** Mute selected drum piece.

### **Button**
- **Hit:** Plays (auditions) the selected drum voice.

### **Grid Section**
Navigate between pieces and parameters (white cursor). The color of the value bar = kit currently in use for the piece.

---

## 2. **Inputs & Outputs Summary**

| Jack      | Function                        | Voltage Range         |
|-----------|---------------------------------|-----------------------|
| KICK      | Trigger Input (Kick)            | Trigger: 2V–10V       |
| SNARE     | Trigger Input (Snare)           | Trigger: 2V–10V       |
| HI-HAT    | Trigger/Gate Input (Hi-hat)     | Trigger/Gate: 2V–10V  |
| TOM       | Trigger Input (Tom)             | Trigger: 2V–10V       |
| TOM CV    | 1V/Oct Pitch CV (Tom)           | CV: -5V to +5V        |
| CRASH     | Trigger Input (Crash)           | Trigger: 2V–10V       |
| CV1       | Assignable CV Mod Input         | CV: -5V to +5V        |
| CV2       | Assignable CV Mod Input         | CV: -5V to +5V        |
| OUT       | **All drum sounds (sum)**       | Audio out             |

---

## 3. **Parameter Control & CV Assignment**

- **Each piece** (Kick, Snare, Hi-hat, Tom, Crash) has parameters:
  - **Timbre**
  - **Pitch**
  - **Decay**
  - **Level**
- **CV Assignment:**
  - **CV1:** Assign by cursor + Parameter Encoder (short press)
  - **CV2:** Assign by cursor + Value Encoder (short press)
  - **Attenuverting:** Cursor on parameter + associated encoder (long press). Adjust range: +1 to -1 (top squares = normal, bottom = inverted)
  - **Multiple parameters:** Both CVs can be assigned to multiple params at once.

---

## 4. **Kit Selection/Timbre Mod**

- **Kits**: Orange (acoustic), Blue (low-fi), Green (alien)
- Switch kit for piece:  
  - Navigate timbre parameter to either end; value bar "rolls over," changing color.

---

## 5. **Saving & Reset**

- **Auto-save:** Wait 5 sec after last change/no trigger; cursor dims = settings stored.
- **Reset All Settings:** Hold Hit, Parameter, Value buttons while powering up.

---

## 6. **Drum Engine Theory (Quick Ref)**

- **Kick/Tom:** Modeled as VCO + envelopes (decay pitch, amp env.), plus optional noise/AM/FM for punch.
- **Snare:** Modeled with noise burst + drum VCO base.
- **Cymbals/Crash/Hi-hat:** Noise filtered, delays, fast amplitude env.  
  - **Hi-hat:** Trigger = closed, Gate = open.

---

## 7. **Cheat Sheet Quick Reference**

| Drum | Trigger | CV | CV Dest. (Internal)     |
|------|---------|-----|------------------------|
| Kick | KICK    | CV1/2| Any param.            |
| Snare| SNARE   | CV1/2| Any param.            |
| Hat  | HI-HAT  | CV1/2| Any param.            |
| Tom  | TOM     | TOM CV| Pitch, CV1/2         |
| Crash| CRASH   | CV1/2| Any param.            |

- **All drums out via OUT.**

---

## 8. **Tips**
- Use external LFOs, random, or sequencer CVs into CV1/CV2 for morphing/animation.
- Fast triggers on hi-hat = closed; gates or longer triggers = open.
- Save/backup settings by waiting for auto-save (no triggers/edits for 5 sec).

---

**[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**

---

**Note:** If you want the official manual PDF, please contact the manufacturer/distributor as an online URL was not provided in the image. Replace "attachment-link-placeholder" above with the correct link if available.