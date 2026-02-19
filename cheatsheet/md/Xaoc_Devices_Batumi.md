# Xaoc Devices — Batumi

- [Manual PDF](../../manuals/xaoc_batumi2_poti2_manual.pdf)

---

[**Xaoc Devices Batumi II & Poti II Manual (PDF)**](https://xaocdevices.com/manuals/xaoc_batumi_II_manual.pdf)

---

# Xaoc Devices BATUMI II + POTI II  
**Quad LFO/OSC & Expander**  
Concise Cheat Sheet (2024/2.0, "Models of 1974")

---

## **Panel Reference**

### **Sliders (x4, illuminated)**
- **A (top):** Always controls Channel A Frequency (0.01Hz–100Hz unpatched; up to 5kHz w/ CV).
- **B, C, D:** Control Frequency, Phase, Divide, or Multiply depending on Global Mode.

### **Buttons**
- **MODE:** Cycles through main modes:  
  - **RED Free** – 4 indep. LFOs/VCOs  
  - **YELLOW Phase** – B, C, D follow A freq, w/ phase offset  
  - **BLUE Divide** – B, C, D = A’s freq divided by integer  
  - **TURQUOISE Mult** – B, C, D = A’s freq multiplied by integer
- **WAVE:** Cycles asgn waveform:  
  - Red: Triangle  
  - Yellow: Down Saw  
  - Orange: Up Saw  
  - Green: Trapezoid  
  - Blue: Stepped Random  
  - Turquoise: Smooth Random
- **MODE+WAVE (hold one, tap other):** Toggles **SYNC/RESET** for sync inputs.

---

## **Inputs & Outputs (per channel)**

| JACK            | TYPE              | VOLTAGE      | DESCRIPTION                                                              |
|-----------------|-------------------|--------------|--------------------------------------------------------------------------|
| **FRQ•PH•RTO**  | CV IN             | -10V/+10V    | Controls freq, phase, div/mult (V/oct in Free, ±5 cycles in Phase)       |
| **RESET•SYNC**  | Sync Trigger In   | 5V gate/trig | Resets or syncs the phase/freq; toggle mode per channel                  |
| **SINE**        | Output            | ±5V          | Anti-aliased sine wave output                                            |
| **ASGN**        | Output            | ±5V          | Assignable wave (see above)                                              |
| **RECT**        | Output            | ±5V          | Anti-aliased pulse/square output (fixed width in most modes)             |

> **All outputs are bipolar ±5V.**

---

## **Modes Overview**

1. **Free (indep. LFOs/VCOs, 1V/oct)**
   - All channels independent.
   - Sine, Rect, Asgn outputs.
   - Use CV and sliders for full frequency sweep.
   - Random asgn are truly independent.

2. **Phase (B-D = A freq, variable phase)**
   - Channels B-D are phase-shifted copies of A.
   - CV modulates phase ±5 cycles per input.
   - Random waves: same sequence delayed.

3. **Divide (B-D = A freq divided by 1/2/3/4/5/8/16/32)**
   - Division set by sliders & CV.
   - Random: Downsampled sequence from A.
   - Max cycle: up to 37.9 days at min freq/CV!

4. **Mult (B-D = A freq multiplied by 1/2/3/4/5/8/16/32)**
   - Integer multiples of A’s cycle set by sliders/CV.
   - Limited to 5 kHz max channel freq.
   - Random: Upsampled sequence from A.

---

## **Tempo Sync**
- **RESET:** Incoming trig/gate resets phase to 0.
- **SYNC:** Follows tempo of external source, quantized frequency division after sync (as in Divide).
- **NOTE:** All 4 channels can sync in Free; only A syncs in other modes.

---

## **Poti II (Expander, 4HP) Controls**

### **Knobs (per channel, selected by button/LED)**
- **FRQ•PH•RTO CV:** Input CV Attenuation (per channel, ALL mode also)
- **SINE OUT:** Sine output attenuation (per channel, ALL mode also)
- **ASGN OUT:** Asgn output attenuation (per channel, ALL mode also)

> **Rect outputs cannot be attenuated.**

### **Channel Button**
- **Cycles between A/B/C/D/All** (LED color changes). Stores settings per channel.  
- **Unplugging resets to default (no atten).**

### **Wave CV Inputs and Switches**
- **SHAPE (CV IN, ±5V):**  
  - **SINE:** Wavefold (with amp comp)  
  - **ASGN:** Morphs through assignable waveforms  
  - **RECT:** Modulates pulse width  
- **Switch:** Selects which output is modulated by CV for the selected channel.

---

## **Quick Reference**

| Control             | Function                                                 |
|---------------------|----------------------------------------------------------|
| **Sliders (x4)**    | A: frequency; B/C/D: freq/phase/div/mult by mode         |
| **Mode Button**     | Mode (Free/Phase/Divide/Mult)                            |
| **Wave Button**     | Sets (or morphs, with Poti II) asgn waveform             |
| **Mode+Wave**       | Toggles Sync/Reset (per channel, LED feedback)           |
| **FRQ•PH•RTO CV IN**| Voltage (-10V/+10V), 1V/oct in Free, phase, or div/mult  |
| **RESET•SYNC**      | Gate/Trigger for phase/freq reset/sync                   |
| **Sine/Asgn/Rect**  | Outputs, ±5V                                             |
| **Poti II Knobs**   | CV/sine/asgn attenuation, per channel, switchable        |
| **Shape CV + Switch**| Choose and modulate sine/asgn/rect per channel          |

---

## **Voltage Ranges**

- **Outputs:** ±5V
- **Input CV:** –10V to +10V (FRQ•PH•RTO inputs)
- **Shape CV:** ±5V

---

## **Useful Tips**

- **1V/oct tracking in Free mode only!** (use as quad VCO)
- **External Sync** disables continuous freq control (slider/CV = division factor).
- With **Poti II**, set attenuation per channel & modulate wave shapes.  
- **Reset/Sync jacks on each channel:** get polyrhythms/LFO sync tricks!

---

## **Physical Installation**

- **Batumi II:** 10hp, 45mm deep, 90mA/+12V, 50mA/-12V
- **Poti II:** 4hp, 32mm, 10mA/+12V (powered only via Batumi II)
- **DO NOT CONNECT Poti II TO BUS BOARD!** Use supplied ribbon cable.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
