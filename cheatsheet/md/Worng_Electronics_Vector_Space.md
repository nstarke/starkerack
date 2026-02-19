# Worng Electronics — Vector Space

- [Manual PDF](../../manuals/Vector Space Manual v1.00.pdf)

---

[WORNG Electronics Vector Space Manual (PDF)](https://www.worngelectronics.com/manuals/WORNG_Vector_Space_Manual.pdf)

---

# WORNG Electronics Vector Space  
**Eurorack Cheat Sheet**

---

## Overview

**Vector Space** is an analog CV/mixing processor that combines 3 input sources into 17 unique, interrelated outputs for complex modulation and voltage processing.

- **Maximum input/output voltage:** ±10V  
- **Accepts and generates CV/audio signals**

---

## Quick Reference

### Inputs

| Jack | Function                | Voltage Range | Switch | Switch Function          |
|------|-------------------------|--------------|--------|-------------------------|
| i    | Main CV/Audio Input 1   | ±5V or 0–10V | ++ / +- | Choose bipolar (+/-5V) or unipolar (0–10V) operation. Switch acts as an offset when toggled. |
| j    | Main CV/Audio Input 2   | ±5V or 0–10V | ++ / +- | As above                |
| k    | Main CV/Audio Input 3   | ±5V or 0–10V | ++ / +- | As above                |

- **Switches ("++/+-")** above each input select unipolar or bipolar range for that channel.
- **Offset:** Switching also offsets voltage regardless of unipolar/bipolar for live use/performance.

---

### Outputs

#### Cube Outputs (8 total)
- **Location:** Corners of the "cube" graphical diagram  
- **Signal:** In- and out-of-phase combinations of i, j, k  
- **LEDs:** Green (positive), Red (negative)  
- **Voltage Range:** Typically within ±10V  
- **Usage:** Quadrature LFO, panned audio, logic combinations

#### Plane Outputs (6 total)
- **Location:** Centers of the cube's faces/intersections  
- **Signal:** Mix of 2x rectified inputs + one in/out of phase input  
- **LEDs:** Gold (positive), Red (negative)  
- **Special:** Outputs are always skewed positive, can double modulation frequency if input oscillator is bipolar  
- **Voltage Range:** 0–10V typical (rectification skews toward positive)

#### Sphere Outputs (3 total)
- **Location:** Center column, with special LED indicators  
- **Outputs:**  
  - **Sphere:** Sum of all rectified inputs (maximal "distance from center")  
      - **LED:** Pink/purple nearby  
      - **Voltage Range:** 0–10V typical    
  - **NegSphere:** Inverted Sphere output (negative sum)  
      - **Voltage Range:** 0 to –10V typical  
  - **UnSphere:** "Distance to closest edge"; +5V when inputs are zero, drops as point moves outward  
      - **LED:** White  
      - **Voltage Range:** +5V (center), drops towards 0V (edges)  
- **Usage:** Randomization, audio, special morphs/envelopes

---

### Controls

- **3 Input Switches (labelled ++/+-):**  
  - Set for unipolar (0–10V) or bipolar (–5V to +5V) range for each input jack (i, j, k).
  - Act as live offset for additional performance modulation.

---

## Voltage Ranges

- **Input:** ±5V (bipolar) or 0–10V (unipolar) for all three input jacks
- **Output:** Up to ±10V (audio or CV) for all 17 outputs

---

## Patch Tips

- **Generative counterpoint:** Three sequencers/randoms into i/j/k, Plane outs → quantizers → VCOs.
- **Ultimate LFO logic:** Three LFOs into inputs, use Plane/Cube/Sphere outs for complex modulations.
- **Spatialization (Quad/Cubic):** Joystick to i/j, Cube outs to VCAs for quad panning; add k for cubic.
- **Vector Synthesis:** Five VCO waveshapes → VCAs → mixer, VCAs modulated from Cube/UnSphere/joystick for timbre morphing.
- **Timbral garden:** Three close-frequency VCOs into i/j/k, audition all outputs for rich combinations/panning.

---

## Installation Notes

- Fits any Eurorack case with +12V/-12V supply.  
- **Current draw:** ~150 mA per rail  
- **Ribbon cable:** Red stripe DOWN (marked "STRIPE")  

---

## Resources

[WORNG Electronics Vector Space Manual (PDF)](https://www.worngelectronics.com/manuals/WORNG_Vector_Space_Manual.pdf)  
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
