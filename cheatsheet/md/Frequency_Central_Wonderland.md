# Frequency Central — Wonderland

- [Manual PDF](../../manuals/Wonderland-Build-Document.pdf)

---

[Wonderland Manual PDF](http://www.frequencycentral.co.uk/wp-content/uploads/2022/06/Wonderland-build-doc.pdf)

---

# Wonderland Eurorack Matrix Mixer / Patchbay Cheat Sheet

## Overview

- **Type:** 8 x 8 Patchbay/Matrix Mixer/Switcher
- **Features:**  
  - 8 inputs (with micro-attenuators)
  - 8 normal outputs (in-phase; A–H)
  - 8 inverted outputs (180° out-of-phase; A–H)
  - 64 pushbutton switch matrix (patch any input to any output)
  - Passive signal routing (no voltage control)

---

## **Jack Reference**

### **Inputs (1–8)**
- **Location:** Top row
- **Type:** 3.5mm mono jack
- **Function:** Accepts audio or CV signals (any modular level)
- **Attenuation:** Each has a micro-attenuator (trimpot; screwdriver adjustable, factory set to 50%)
- **Voltage Range:** ±10V typical modular level (no specific limits stated, passive matrix)

### **Outputs (Per Output Column, A–H)**
For each output A–H, there are:
- **Normal Output Jack (3.5mm mono):**
  - In phase with input signal(s)
- **Inverted Output Jack (3.5mm mono):**
  - 180° out of phase with input signal(s)
- **Voltage Range:** Follows input voltage (subject to mix summing & attenuation; no amplification or limiting—watch for clipping if summing many signals)

---

## **Controls**

### **Buttons (Switch Matrix)**
- **Quantity:** 64
- **Type:** Pushbutton (latching, push on/push off)
- **Function:**  
  - **Press to connect input (row) to output (column)**
    - Example: Pressing the button at row 2, column C connects Input 2 to Output C.
  - Multiple switches ON = mix/sum several inputs to same output OR one input to multiple outputs

### **Micro-Attenuators (Trimpots, Input 1–8)**
- **Location:** One per input; accessible via small screwdriver
- **Adjustment:** Set gain/attenuation for each input
  - *Note:* If mixing many inputs to one output, reduce gain to prevent clipping.

---

## **Cheat Sheet for Use**

1. **Patch signals into one or more of the 8 input jacks (top row).**
2. **Adjust micro-attenuators as needed** (screwdriver in each input trimpot, default at 50%).
3. **Press switches at intersections to make connections** from any input to any output (outputs A–H).
   - One input can feed many outputs.
   - Many inputs can be summed to one output (attenuate as needed to avoid distortion).
4. **Patch from either the normal or inverted outputs (A–H columns).**
   - "Normal Out" = in phase
   - "Inverted Out" = 180° out of phase
5. **Monitor and tweak as needed.**  
   - Use for audio, CV, trigger/gate signals.
   - No active processing; strictly passive/analog matrix management.

---

## **Quick Reference Table**

| Jack/Control Type | Quantity | Label     | Location     | Notes/Range                      |
|-------------------|----------|-----------|--------------|----------------------------------|
| Input Jack        | 8        | 1–8       | Top row      | DC-coupled, modular signal ready |
| Micro-Attenuator  | 8        | (trimpot) | By inputs    | Screwdriver slot, range 0-100%   |
| Normal Out Jack   | 8        | A–H       | Side columns | In phase w/ input(s)             |
| Inverted Out Jack | 8        | A–H       | Side columns | 180° out of phase                |
| Switch Buttons    | 64       | Matrix    | Central grid | Latching, patch routing          |

---

## **Notes**

- **No voltage control, external CV/automation not supported**
- **Passive mixing—no level compensation or normalization**
- **If summing many signals, consider external attenuation** to avoid clipping/distortion

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)