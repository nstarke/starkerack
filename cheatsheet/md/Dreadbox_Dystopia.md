# Dreadbox — Dystopia

- [Manual PDF](../../manuals/Manual_DreadBox_Dystopia.pdf)

---

[**Download the Dreadbox Dystopia Manual PDF**](https://dreadbox-edu.com/manuals/DYSTOPIA_MANUAL.pdf)

---

# Dreadbox Dystopia Eurorack Module Cheat Sheet

## Panel Overview

The Dystopia is a versatile 10HP noise and bit-processing module with multiple filter options and external audio processing capability.

---

## Controls & Patch Points

### **Outputs**
- **SCATTER (Top Output Jack)**
  - Default: Noise (White Noise) output, bit crushed.
  - With EXT IN: Negative voltage slicer of EXT IN signal.
  - Voltage: ±5V

- **ODDS (Middle Left Output Jack)**
  - Gate signal based on ODDS knob/CV.
  - Voltage: 0–5V

- **PINK (Middle Center Output Jack)**
  - Pink noise (filtered output).
  - With EXT IN: 12dB/oct low pass filter on EXT IN.
  - Voltage: ±5V

- **BLUE (Middle Right Output Jack)**
  - Blue noise (filtered output).
  - With EXT IN: 12dB/oct high pass filter on EXT IN.
  - Voltage: ±5V

---

### **Inputs**
- **EXT IN (Top Left Input Jack)**
  - Cancels internal noise when patched; processes external audio or CV.

- **ODDS CV IN (Below ODDS knob)**
  - CV control for ODDS (gate probability).
  - Voltage: ±5V

- **BITS CV IN (Below BITS knob)**
  - CV control for BITS (bit crush rate).
  - Voltage: ±5V

- **PINK CV IN (Below PINK knob)**
  - CV for pink noise filter rolloff (low pass).
  - Voltage: ±5V

- **BLUE CV IN (Below BLUE knob)**
  - CV for blue noise filter rolloff (high pass).
  - Voltage: ±5V

---

### **Knobs**
- **ODDS**
  - Sets probability of gate events on ODDS output.

- **BITS**
  - Controls bit crusher clock frequency (effect on white noise or EXT IN).

- **PINK**
  - Adjust LPF rolloff for pink output (12dB/oct).

- **BLUE**
  - Adjust HPF rolloff for blue output (12dB/oct).

---

## **Special Functionality**

> **Patching anything into EXT IN disables all internal noise and processes your external audio:**  
> - **SCATTER:** Negative voltage slicer  
> - **ODDS:** Gate from external audio (distortion based on BITS)  
> - **CRUSH:** Bit crusher  
> - **PINK:** Low Pass Filter (12dB/oct)  
> - **BLUE:** High Pass Filter (12dB/oct)

---

### **I/O Reference Table**

| Jack Label | Type   | Function (Default / EXT IN)              | Range     |
|------------|--------|------------------------------------------|-----------|
| SCATTER    | Out    | Bitcrushed Noise / Sliced EXT IN         | ±5V       |
| ODDS       | Out    | Gate based on ODDS / Distorted EXT IN    | 0–5V      |
| PINK       | Out    | Pink Noise (LPF) / LPF EXT IN            | ±5V       |
| BLUE       | Out    | Blue Noise (HPF) / HPF EXT IN            | ±5V       |
| EXT IN     | In     | Replaces internal noise, injects audio/CV|           |
| ODDS CV    | In     | ODDS control voltage                     | ±5V       |
| BITS CV    | In     | BITS control voltage                     | ±5V       |
| PINK CV    | In     | PINK filter CV                           | ±5V       |
| BLUE CV    | In     | BLUE filter CV                           | ±5V       |

---

## **Quick Tips**
- **No patch in EXT IN:** Classic noise and bit crusher behavior.
- **Patch to EXT IN:** Turns module into an audio/CV processor (filters, slicing, distortion, bit crushing).
- **CV accepts full modular levels:** ±5V on all CV inputs.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
