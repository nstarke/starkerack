# ADDAC Systems — ADDAC-207 Quantizer

- [Manual PDF](../../manuals/ADDAC_207_Quantizer_REV05.pdf)

---

[ADDAC207 Intuitive Quantizer Manual PDF](https://addacsystem.com/Manuals/ADDAC207.manual.pdf)

---

# ADDAC207 Intuitive Quantizer — Cheat Sheet

#### **Quick Start**
- **Outputs 1–4 → VCOs**
- **Tune VCOs**: Use Keyboard Mode ([Hold Button 1](#hardware-overview--controls)) → All notes ON except active key
- **Quantize**: Exit Keyboard Mode ([Hold Button 1] again), patch CV to Note 1 IN, play C major by default; patch Note 2–4 for more voices

---

## **Panel Overview**

### **Jacks (Left to Right, Top to Bottom)**
| Jack         | Function                                             | Voltage Range          |
|--------------|------------------------------------------------------|------------------------|
| IN 1 – 4     | CV inputs for each voice/quantizer                   | ±5V                   |
| OUT 1 – 4    | Quantized pitch CV outs for each voice               | 0 to +10V              |
| GATE IN 1–4  | Trigger/Gate input for each voice (external timing)  | 0 or +5V               |
| GATE OUT 1–4 | Quantized note triggers/gates                        | 0 or +5V               |
| ASSIGN       | CV input for menu assignment controls                | 0 to +5V (rectifies –V)|

---

### **Knobs & Switches**
| Control              | Function                                                     |
|----------------------|-------------------------------------------------------------|
| Rotary Switch        | Select Key/Octave (“KEY/OCTAVE”)                            |
| MINOR/MAJOR Toggle   | Set scale type                                              |
| b/N/# Toggle         | Select root note accidental (flat/natural/sharp)            |

---

### **Illuminated Buttons (12, numbered 1–12)**
| Button      | Function (short press = activate note, long press = enter menu)   |
|-------------|-------------------------------------------------------------------|
| 1           | Toggle note 1 / Enter Mode Selection/Keyboard Mode                |
| 2           | Toggle note 2 / Set Note 2 interval/chord setting                 |
| 3           | Toggle note 3 / Set Note 3 interval/chord setting                 |
| 4           | Toggle note 4 / Set Note 4 interval/chord setting                 |
| 5           | Toggle note 5 / Quantization Type                                 |
| 6           | Toggle note 6 / Gate Length Menu                                  |
| 7           | Toggle note 7 / Trigger Repeat Menu                               |
| 8           | Toggle note 8 / Reaction Time                                     |
| 9           | Toggle note 9 / Octave Offset                                     |
| 10          | Toggle note 10 / Tuning & Fine Tune Menu                          |
| 11          | Toggle note 11 / Scale Mode, Tuning +, Assign                     |
| 12          | Toggle note 12 / Preset Menu, Tuning –, Assign                    |

#### *Multi-button and hold combinations* enter/exit menus, assign CV, or store/load presets. Color coding for function (Black: overall, Yellow: chord/gen, Blue: scale/temper, White: scale mode).

---

## **Operation Modes**

### **Quantizer Mode**
- CV Input is quantized to closest active note.
- LEDs light up for active scale notes.
- [Long press Button 1] toggles between Keyboard/Quantizer mode.

### **Keyboard Mode**
- User selects note manually—acts as simple keyboard.
- ALL LEDs ON except active note (the played note).
- Useful for tuning & manual play.
- **Voices 2–4:** can only play notes active in Quantizer Mode for chords.

---

## **Menu Navigation**

- **Long press (1s) any Button**: Enters its menu
- Change option by pressing a button, confirm with a second press.

### **Key Menu Functions**
- **NOTE 2/3/4 (Buttons 2–4):** Set output intervals for Voice 2/3/4 (Root/3rd/5th/etc.)
- **Q.TYPE (Button 5):** Quantization type (Above/Ignore/Below, Buttons 3/5/6)
- **GATE LENGTH (Button 6):** Set Gate Out length: 10–10240ms (Buttons 1–11), Button 12 for "Gate Off Condition"
- **TRIG REPEAT (Button 7):** Re-triggering, Voice 1 Master/Slave, auto Gate In detection (Buttons 2/3/4/7)
- **REACT TIME (Button 8):** Menu Hold Time (500ms–2700ms)
- **OCTAVE OFFSET (Button 9):** Output offset in octaves (-3 to +8, Buttons 1–10)
- **TUNING (Button 10):** Scale Temperament, Moog/Buchla standard (1V/Oct or 1.2V/Oct), Fine tuning per voice
- **SCALE MODE (Button 11):** Ionian/Dorian/etc. (Usually bypassed)
- **PRESETS (Button 12):** 11 user presets (Buttons 1–11, hold Button 12 to save)

### **ASSIGN (CV Input Routing):**
Patch CV to ASSIGN jack, press [hold Buttons 4+7], select destination:
- Button 1: Input Transpose
- Button 2–4: Voice 2/3/4 interval
- Button 5: Quantizer Type
- Button 6: Gate Length
- Button 7: Trigger Repeat
- Button 9: Octave Offset
- Button 11: Scale Transpose
- Button 12: Preset Change

---

## **Input/Output Reference**

| Function                | Jack                  | Voltage Range            | Details                           |
|-------------------------|-----------------------|-------------------------|------------------------------------|
| Note CV Input           | IN 1–4                | ±5V                     | 1 for each voice                   |
| Quantized Pitch Output  | OUT 1–4               | 0 to +10V               | 1 per voice, 1V/oct or 1.2V/oct    |
| Gate In                 | GATE IN 1–4           | 0 or +5V                | Triggers quantization              |
| Gate Out                | GATE OUT 1–4          | 0 or +5V                | Trigger on new note                |
| CV Menu Assignment      | ASSIGN                | 0 to +5V (rectifies –V) | Assignable by menu                 |

---

## **Other Key Features**
- **Microtonal Mode**: Fine tune 1V/oct to support >12 notes/octave
- **Temperaments**: Equal, Just, Well Tuned, Bohlen-Pierce, Exotic
- **Moog/Buchla CV Compatibility**: Switchable 1V/oct or 1.2V/oct
- **Nonvolatile Memory**: Fine tunings, menu settings, 11 user presets
- **Gate, Trigger, and Chord Functions**: Multi-voice quantization and interval setting
- **Tuning Reset**: Hold [SET KEY] for 5 seconds

---

## **Specs**
- **Format**: Eurorack, 10HP
- **Depth**: 6cm
- **Max Current**: 150mA
- **Bus**: Standard 16-pin

---

## **Major/Minor Scale Reference**
- See manual pages 33–34 for all major and minor scale layouts.

---

For full functionality and troubleshooting details, [consult the full manual PDF](https://addacsystem.com/Manuals/ADDAC207.manual.pdf).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)