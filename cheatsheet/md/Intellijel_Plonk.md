# Intellijel — Plonk

- [Manual PDF](../../manuals/plonk_manual_v1.16_2020.11.08.pdf)

---

[**Plonk Manual PDF**](attachment:Plonk_Manual_1.16.pdf)

---

# Intellijel Plonk Cheat Sheet

## Overview
Plonk is a physical modeling percussion synthesizer capable of creating both realistic and synthetic percussive sounds. It uses separate Exciter and Resonator sections, is duophonic (2-voice), and supports deep modulation and preset storage.

---

## **Inputs, Outputs, and Controls Reference**

### **Jacks/Input/Outputs**

| Jack      | Type | Purpose | Voltage Range | Notes |
|-----------|------|---------|---------------|-------|
| **A. X**      | CV In  | Modulate X-assigned parameter | ±5V | Summed with X knob/param. Attenuverter present. |
| **B. MOD**    | CV In  | Modulate MOD-assigned parameter or special control | ±5V | Attenuverter present. Gate >1.5V for gate-based. |
| **C. DECAY**  | CV In  | Offset DECAY knob/param | ±5V | Attenuverter present. |
| **D. Y**      | CV In  | Modulate Y-assigned parameter | ±5V | Summed with Y knob/param. Attenuverter present. |
| **E. PITCH**  | CV In  | 1V/oct pitch input | ±5V | Only updates while TRIG high. |
| **F. TRIG**   | Gate In | Triggers Exciter | Std. gate, >1ms | |
| **G. VEL**    | CV In  | Velocity/expression | 0 to +5V (norm. +5V) | Controls accent, dynamics, or volume by menu. |
| **H. OUT**    | Audio Out | Main mono audio | - | -

---

### **Knobs and Front Panel Controls**

| Control | Function |
|---------|----------|
| **PITCH** (knob)   | Base pitch of resonator. |
| **DECAY** (knob)   | Scales overall sound/resonator decay. |
| **X / Y** (knobs)  | Manual modulation for X/Y assigned parameter (bipolar). |
| **ENCODER**        | Menu navigation/value change (push+turn function). |

---

### **Buttons**

| Button    | Function |
|-----------|----------|
| **DISPLAY**   | OLED screen with activity LEDs for both voices. |
| **PITCH**     | Opens pitch menu (Octave/Quantize). |
| **TRIGGER**   | Manually fires exciter for preview. |
| **EXCITER**   | Opens exciter menu (mallet/noise/shaping/etc.). |
| **OBJECT**    | Opens resonator menu (model/decay/tone/etc.). |
| **MOD**       | Assign MOD CV input (+ depth). |
| **CONFIG**    | System config/output/FX/global. |
| **LOAD/SAVE** | Load/save presets and manage memory. |
| **X / Y**     | Assign X/Y CV input (+ depth). |

---

## **Quick Start**

1. **Default Patch:** Power on, output to system audio, set PITCH/X/Y (12:00), DECAY full CW.
2. **Trigger:** Press TRIGGER to play.
3. **Preset:** LOAD → scroll/select/preview with ENCODER → click to load.
4. **Sequencer:** TRIG from sequencer to TRIG; CV to PITCH; optionally VEL for velocity.
5. **Live Modulate:** MOD input for preset stepping/kits (factory presets 1/5/9/13 support).
6. **Edit Sounds:** Use EXCITER and OBJECT menus.

---

## **Menus and Modulation**

- **Exciter Parameters:** Mallet/Noise mix, Mallet stiffness, Noise attack/decay/density/filters/envelope type.
- **Object Parameters:** Resonator type (String/Beam/Marimba/Drumhead/Membrane/Plate), Decay, Tone, Position, Inharmonicity, Low Cut, Pitch Envelope amt/decay, Polyphony (1/2).
- **Modulation Destinations:** Most exciter/object parameters can be mapped to X, Y, or MOD, plus bitcrusher and saturation FX.
  - **Special MOD:** Choke (Res, Noise, Both), Preset Step, Morph, Randomize.

---

## **Preset Management**

- **128 memory slots.** Panel knobs are always live and override/offset preset values!
- **Load:** LOAD → ENCODER scroll → preview with TRIGGER → click to load.
- **Save:** SAVE → ENCODER pick slot → SAVE or click ENCODER to enter name → confirm with Y.
- **Transfer (USB-MIDI):** See manual for SysEx instructions.

---

## **Other Notes**

- **Calibration:** See CONFIG > Global Config.
- **Firmware/Changelog:** Many expanded FX/modulation since v1.10.
- **Size/Power:** 12hp, 44mm deep, 170mA @ +12V, 6mA @ -12V.

---

## **Parameter Modulation Depths**

- Depth settings: LOW (±16), MEDIUM (±32), HIGH (±64), FULL (±128) for X, Y, MOD.

---

## Links

- [Intellijel Plonk Manual PDF](attachment:Plonk_Manual_1.16.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---

**Tip:** Plonk is highly dynamic—experiment, assign modulation, and morph between presets for maximum variety!