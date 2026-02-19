# Mutable Instruments — Clouds

- [Manual PDF](../../manuals/Mutable Instruments - Clouds.pdf)

---

[**Mutable Instruments Clouds Manual PDF**](https://mutable-instruments.net/modules/clouds/manual/)

---

# **Mutable Instruments Clouds – Cheat Sheet**

A quick-reference guide to the Clouds granular audio processor for Eurorack.

---

## **Quick Start**

1. **Patch audio** into L (and optionally R) input.
2. **Patch stereo output** (L/R) to mixer/output.
3. **Twist knobs** to manipulate grain position, size, pitch, density, texture.
4. **[Optional] Patch CV** into desired CV ins for dynamic modulation.
5. **Press FREEZE** to capture a sound, manipulate the buffer, or scan through frozen grains.

---

## **Controls Reference**

### **Knobs**
| Knob                 | Function                                                                         |
|----------------------|----------------------------------------------------------------------------------|
| POSITION             | Where in the buffer grains are sourced (back in time: CW = earlier)              |
| SIZE                 | Grain length                                                                     |
| PITCH                | Grain playback speed (12 o'clock = normal pitch)                                 |
| IN GAIN              | Audio input gain (-18dB to +6dB)                                                 |
| DENSITY              | Grain overlap/timing (CW = denser/random, CCW = denser/constant, noon = none)    |
| TEXTURE              | Morphs grain envelope shape; past 2 o'clock activates diffuser                   |
| BLEND                | Controls one of: Dry/Wet ↔ Spread ↔ Feedback ↔ Reverb (select via button B)      |

### **Buttons**
| Button                             | Function                                                                                 |
|-------------------------------------|------------------------------------------------------------------------------------------|
| FREEZE (A)                         | Capture/freeze buffer (toggle)                                                           |
| Blend Parameter/Audio Quality (B)   | Select parameter for BLEND knob/CV, or hold+tap to set audio quality                     |
| Load/Save (C)                      | Load or save frozen buffers; double-action, see manual for details                       |

### **LEDs**
- Bargraph: Input/output level, setting indicators, parameter values.
- Color indicates: blend parameter (green), buffer slot (red/green), calibration (orange).

---

## **Inputs & Outputs [**Voltage Range: All CV INs ±5V**]**

| Jack # | Label/Use        | Type       | Description                                                                         |
|--------|------------------|------------|-------------------------------------------------------------------------------------|
| 1      | FREEZE           | Gate In    | Gate high = freezes buffer (same as button).                                         |
| 2      | TRIGGER          | Trig In    | Generates a single grain per trigger (micro-sample playback at DENSITY noon).        |
| 3      | POS CV           | CV In      | Modulate grain buffer position (±5V)                                                 |
| 4      | SIZE CV          | CV In      | Modulate grain size (±5V)                                                            |
| 5      | V/OCT            | CV In      | 1V/Oct pitch tracking of grain playback (±5V)                                        |
| 6      | BLEND CV         | CV In      | Modulate selected blend parameter (±5V)                                              |
| 7/8    | IN L / R         | Audio In   | Stereo input (R normalled to L if unpatched)                                         |
| 9      | DENSITY CV       | CV In      | Modulate grain density/overlap (±5V)                                                 |
| 10     | TEXTURE CV       | CV In      | Modulate envelope/diffusion/texture (±5V)                                            |
| 11/12  | OUT L / R        | Audio Out  | Stereo output                                                                        |

---

## **Blend Parameters**
- **Dry/Wet**  
- **Stereo Spread** (random panning per grain)  
- **Feedback Amount**  
- **Reverb Amount**  
Select parameter using Blend Parameter/AQ button (B); indicator LED shows selection.

---

## **Freezing & Saving**
- **FREEZE:** Stops recording; process sound in memory.
- **Save/Load Buffer:**  
  - Hold Load/Save 1s, select slot (1–4), confirm to save.
  - Tap Load/Save, select slot, confirm to load.

---

## **Calibration**
- 1V/Oct calibration: See manual (requires accurate CV source).

---

## **Audio Quality**
- Hold Blend Parameter/Audio Quality button for 1s; tap to cycle:  
  - 32kHz/16-bit  
  - 32kHz/8-bit µ-law  
  - 16kHz/16-bit  
  - 16kHz/8-bit µ-law  

---

## **Tips**
- Add random modulation to Position or Pitch for lush textures.
- Use audio out as modulation noise source.
- Fast note sequences to V/Oct = chord grains.
- Short FREEZE pulses = capture micro-textures.

---

## **Troubleshooting**
- **No effect?**  
  - Dry/Wet blend may be fully dry. Use Blend Parameter/AQ button to select dry/wet, adjust BLEND knob.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)