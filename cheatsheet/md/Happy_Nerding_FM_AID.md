# Happy Nerding — FM AID

- [Manual PDF](../../manuals/FM-AID-USERS-GUIDE_2020.pdf)

---

[Download the FM AID 2020 Manual (PDF)](https://happynerding.com/manuals/FM_Aid_manual_2020.pdf)

# Happy Nerding FM AID (2020) — Cheat Sheet

## **Overview**
FM AID is an analog Eurorack module for through-zero linear FM synthesis. Any signal can be used as Carrier or Modulator for wild, aliasing-free wave shaping and FM tones. Saw-tooth input recommended for "classic" FM outputs, but all source types yield unique results.

---

## **Panel Reference**

### **Top Controls**
- **FM Knob:** Sets modulation depth (FM index).
- **CV Knob:** Bipolar attenuator for CV input, mixes with FM knob.

### **Jacks**
1. **CV IN**
   - _Voltage Range:_ -5V to +5V (accepts AC or DC)
   - _Purpose:_ Controls FM depth (modulation index) via external voltage.
2. **MOD IN (Modulator)**
   - _Voltage Range:_ Preferably -5V to +5V (accepts -1V to +1V up to -12V to +12V with trimmer adjustment)
   - _Purpose:_ Signal input that frequency-modulates the Carrier.
   - _Note:_ Carrier is normalled to Mod if no patch present.
3. **CAR IN (Carrier)**
   - _Voltage Range:_ Preferably -5V to +5V (trimmable up to ±12V)
   - _Purpose:_ Main signal to be modulated.
   - _Note:_ Sawtooth gives most "classic" FM outputs.
4. **Outputs (All: -5V to +5V, 1kΩ impedance)**
   - **Sine:** Smoothest output, classic sine when fed sawtooth.
   - **Triangle:** Brighter than sine.
   - **Sawtooth:** Bright, reproduces saw input when fed saw.
   - **Square:** Brightest, gives square when fed saw.

---

## **Quick Start**

1. **Install in 4HP space, connect 10–16 pin power (red stripe = -12V).**
2. **Feed sawtooth to CAR IN for "classic" FM output shapes.**
3. **Plug MOD IN for external modulation, or use default (normalled) for wavefolding.**
4. **Use FM knob to set FM index (intensity).**
5. **Use CV knob to add/shape modulation from the CV input.**
6. **Patch outputs to get Sine, Triangle, Saw, or Square variants.**

---

## **Tricks**

- **Self-patch any output to MOD IN** for feedback tones and analog noise.
- **Patch velocity or pitch CV to CV IN** for dynamic, keyboard-driven timbres.
- **Hard-sync both carrier & modulator sources** to eliminate frequency beating.
- **Lower carrier/modulator octave or switch to sine/triangle to restore low end** if the main tone gets lost at high FM depth.

---

## **Calibration**
- Onboard trimmer adapts module for input voltage ranges from ±5V to ±12V.
- To calibrate: Feed saw into Carrier, set FM fully CCW, monitor Saw output, and trim for cleanest output.

---

## **Input/Output & Control Summary Table**

| Function | Jack/Control | Type | Typical Voltage Range | Description |
|----------|--------------|------|----------------------|-------------|
| FM depth | FM knob | Knob | Manual | Sets FM index |
| CV attenuator | CV knob | Knob | Manual | Mixes CV with FM knob |
| FM depth CV | CV IN | Jack | -5V to +5V | Modulates FM depth |
| Modulator | MOD IN | Jack | -5V to +5V (adj. up to ±12V) | Frequency modulation input |
| Carrier | CAR IN | Jack | -5V to +5V (adj. up to ±12V) | Source to be FM-modulated |
| Sine out | Output | Jack | -5V to +5V | Sine-like output |
| Triangle out | Output | Jack | -5V to +5V | Triangle-like output |
| Sawtooth out | Output | Jack | -5V to +5V | Sawtooth output |
| Square out | Output | Jack | -5V to +5V | Square output |

---

**[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**
