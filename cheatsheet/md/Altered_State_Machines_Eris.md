# Altered State Machines — Eris

- [Manual PDF](../../manuals/Eris _ Altered State Machines.pdf)

---

[**Manual PDF: Eris 4x4 Matrix Mixer by Altered State Machines**](https://alteredstatemachines.net/eris)

---

# Eris 4x4 Matrix Mixer Cheat Sheet

## Overview
- **4x4 matrix mixer**: 4 inputs x 4 outputs, 12hp
- **Mixes and routes audio or CV signals** (DC coupled)
- Linear potentiometers control send level from any input to any output
- Each channel can **amplify up to 4x** input (makeup gain/overdrive)
- **Auxiliary input/output** with soft vactrol-based mute
- Toggle switch (rear): Aux input gain (Unity/x2)
- Suitable for mixing (audio, CV, FX send/return, feedback, modulation matrices)

---

## Controls & Jacks Reference

### Inputs (Jacks)
- **Inputs 1-4 (Top Row, Left)**
  - Accept **audio or CV** signals
  - Typical modular range: ±10V (not specified, but standard for Eurorack, module is DC coupled)
  - Each input may be summed to any output
  
- **Auxiliary Input**
  - Signal is summed with Output 1 before being routed to Aux Output
  - Gain: Switchable (Unity or x2 via rear toggle)
  - **Mute**: Vactrol-based soft mute (button or toggle on front panel)

### Outputs (Jacks)
- **Outputs 1-4 (Top Row, Right)**
  - Each receives mixed signal according to matrix settings
- **Auxiliary Output**
  - Sum of Aux Input and Output 1 (post-mix), subject to mute status

### Knobs / Potentiometers
- **16 Channel Level Knobs** (4 per input/output crosspoint)
  - Each knob controls send level from one input to one output (linear response)
  - Levels up to **4x** amplification of input signal
  
### Switches
- **Aux Input Gain Toggle (Back Panel)**
  - Selects between Unity Gain (1x) and high gain (2x) for Aux In
- **Aux Mute (Front Panel/Button)**
  - Soft vactrol-based mute for Aux Input (clickless)

---

## Typical Use Scenarios

- **Basic 4-Input Mixer:** Route all to Output 1 as main mix.
- **FX Send/Return Matrix:** Send Outputs 2/3/4 to effects, return effected signals to Aux In.
- **Modulation Matrix:** Route various CV signals to different destinations.
- **Feedback Networks or Cybernetic Circuits**
- **Kick Drum/Accent Mixing:** Use Aux channel for bringing in/out specific sounds.

---

## Power / Specs

- **Size:** 12 hp
- **Current Draw:** +12V 17mA, -12V 3mA, 0mA 5V
- **DC Coupled:** Handles audio & CV equally

---

## Compliance & Limitations

- **EU (RoHS):** Not currently shippable to EU (vactrol in Aux mute, RoHS version pending)

---

## Quick Links

- [Manual PDF](https://alteredstatemachines.net/eris)
- [ModularGrid](https://modulargrid.net/e/altered-state-machines-eris)
- [Etsy Purchase](https://www.etsy.com/listing/1814206182/eris-4-x-4-matrix-mixer)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)