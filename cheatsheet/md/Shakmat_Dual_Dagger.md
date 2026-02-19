# Shakmat — Dual Dagger

- [Manual PDF](../../manuals/DD-User_Manual.pdf)

---

[👉 **Shakmat Dual Dagger Manual (PDF)**](https://www.shakmat.com/products/DUAL_DAGGER/User_manual_Dual_Dagger.pdf)

---

# **Shakmat Dual Dagger Cheat Sheet**

**Type:** Dual Stereo (4-pole) Filter / Stereo Bandpass  
**Size:** 6HP | **Depth:** 29mm | **Power:** +12V: 65mA, -12V: 80mA  
**Audio Input Range:** ±5V

---

## **Panel Controls & I/O Reference**

### **Knobs/Potentiometers**
- **A. LPF:** Low-pass filter cutoff (stereo)
- **C. RES:** Resonance (assignable: LPF, HPF, or both)
- **F. HPF:** High-pass filter cutoff (stereo)

### **Switches**
- **B. LINK:** Links filters for stereo bandpass mode
- **D. LPF Resonance Switch:** Assigns resonance control to LPF
- **E. HPF Resonance Switch:** Assigns resonance control to HPF

### **CV Inputs** *(all DC coupled)*
| Label   | Function         | Voltage Range                     |
|---------|------------------|-----------------------------------|
| 1 (LPF) | LPF cutoff CV    | -5V to +5V                        |
| 2 (RES) | Resonance CV     | -5V to +5V                        |
| 3 (HPF) | HPF cutoff CV    | -5V to +5V                        |
| 4 (PANLP, PANHP) | Panning LPF/HPF cutoff CV | -5V to +5V      |

- **PANLP:** Offsets L/R LPF cutoff in opposite directions with voltage
- **PANHP:** Offsets L/R HPF cutoff in opposite directions with voltage

### **Audio Inputs & Outputs**
| Label | Function             | Voltage Range   |
|-------|----------------------|----------------|
| IN1   | Audio Input 1 (L)    | -5V to +5V     |
| IN2   | Audio Input 2 (R)    | -5V to +5V     |
| OUT1  | Audio Output 1 (L)   | -5V to +5V     |
| OUT2  | Audio Output 2 (R)   | -5V to +5V     |

---

## **Quick Start**

### **Filtering Basics**
- **LPF/HPF knobs:** Adjust stereo low/high-pass cutoffs.
- **RES knob:** Control filter resonance. Assign to LPF, HPF or both with toggle switches.
- **LINK switch:** Engaged = bandpass mode. HPF = band edge (start freq), LPF = bandwidth.

### **Voltage Control**
- All primary functions (LPF, HPF, RES, PANLP, PANHP) are voltage controllable with ±5V.
- PAN inputs let you offset cutoff oppositely on L/R for powerful stereo effects.

### **Stereo Bandpass**
- **LINK on:** HPF cutoff is lower band edge, LPF sets bandwidth. Resonance applied at band edges via switches.

### **Resonance Jumpers (on rear)**
- **"Lo":** Safer (no self-oscillation)
- **"Hi":** Allows self-oscillation (VCO uses!)

---

## **Essential Patch Ideas**
- **Stereo Filtering/Animation:** Standard stereo filtering and animated stereo panning via PAN inputs.
- **Double Peaks:** Mono in, both outs mixed = double peak filter. PAN controls separation between peaks.
- **Sine VCO:** One channel can self-oscillate as a sine VCO (in Hi jumper mode).
- **Kick Drums:** Envelope FM the cutoff for snappy drum sounds.
- **Mid/Side Filtering:** Combine with M/S modules (e.g. Shakmat SumDif) for creative stereo processing.

---

## **Summary Table**

| Control/Jack     | Function                        | Voltage Range             |
|------------------|---------------------------------|--------------------------|
| A. LPF           | LPF cutoff knob (stereo)        | Manual & CV (-5V/+5V)    |
| B. LINK          | Bandpass mode toggle            | -                        |
| C. RES           | Resonance knob                  | Manual & CV (-5V/+5V)    |
| D. LPF Res SW    | LPF resonance assign            | -                        |
| E. HPF Res SW    | HPF resonance assign            | -                        |
| F. HPF           | HPF cutoff knob (stereo)        | Manual & CV (-5V/+5V)    |
| 1. LPF           | LPF cutoff CV in (stereo)       | -5V to +5V               |
| 2. RES           | Resonance CV in                 | -5V to +5V               |
| 3. HPF           | HPF cutoff CV in (stereo)       | -5V to +5V               |
| 4. PANLP/PANHP   | Pan LPF/HPF offset (L/R)        | -5V to +5V               |
| 5. IN1, IN2      | Audio inputs                    | -5V to +5V               |
| 6. OUT1, OUT2    | Audio outputs                   | -5V to +5V               |

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)