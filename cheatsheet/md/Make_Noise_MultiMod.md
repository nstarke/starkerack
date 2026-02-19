# Make Noise — MultiMod

- [Manual PDF](../../manuals/multimod-manual.pdf)

---

[**MultiMod Manual PDF**](#)  
*PDF link placeholder — please insert the actual link if available*

---

# MultiMod (Make Noise) Cheat Sheet

---

## **Overview**
- **MultiMod** takes one control signal, copies it to 8 outputs, and processes each with *independent* phase and speed adjustment.  
- Internal LFO allows usage with nothing patched to input.
- Key concepts: **Spread** and **Phase** provide complex modulation from a single source.

---

## **Inputs & Outputs Reference**

| Jack                  | Function                                                      | Voltage Range        |
|-----------------------|---------------------------------------------------------------|---------------------|
| **Signal IN**         | Main modulation source. Uses internal LFO if unpatched.       | ±10 V DC            |
| **HOLD IN**           | Gates to "hold" (freeze) current buffer.                      | >2 V (gate)         |
| **Phase CV IN**       | CV to automate phase (pot acts as attenuator).                | ±10 V (0–5 V = panel range, up to ±10 V extends range) |
| **Reset IN**          | Gate to re-align phase/positions (momentary reset).           | >2 V (gate)         |
| **TEMPO IN**          | Clock input; quantizes Time, Phase, Spread & Outputs          | >2 V (gate)         |
| **Spread CV IN**      | CV control over spread (with attenuverter).                   | ±10 V (±5 V = panel range; up to ±10 V extends range)  |
| **Time CV IN**        | CV control over time (global speed).                          | ±10 V (0–5 V = panel, beyond extends range)            |
| **CLK OUT**           | Clock output at current rate or division/multiple of external clock. | N/A                 |
| **Channel Outputs 1–8**| 8 phase/spread modulated copies of input or internal LFO.    | ±10 V (nominal)     |
| **Channel Index OUT** | 1–8 V, indicating currently 'highest' channel (useful as CV/gate source). | 1 V = Ch 1 ... 8 V = Ch 8 |

---

## **Knobs, Buttons, & Controls**

| Control                  | Description                                                                      | Notes |
|--------------------------|----------------------------------------------------------------------------------|-------|
| **Phase Panel Control**  | Manual phase offset for channel tap points                                       | Combo pot with CV |
| **Spread Panel Control** | Sets spread of playback speeds (x8 to /8 per channel, inversely on each end)    | Center (12:00) = no spread |
| **Shape Button**         | Selects read or LFO shape (Ramp, Saw, Triangle, Sine, Square, Stepped & Smooth Random) | Color-coded |
| **Time Panel Control**   | Sets global write/read speed or LFO rate                                         | Combo pot with CV |
| **Hold Button**          | Toggles HOLD function (freezes buffer)                                           | Latching button |
| **Reset Button**         | Resets all channels to current 'start' position                                  | Momentary button |
| **Spread CV Attenuverter**| Adjusts depth/inversion of external Spread CV                                   | -    |

---

### **Voltage Ranges Summary**

- **Input CVs**: Expect full-range support for ±10 V. Panel controls generally map to 0–5 V by default, beyond that increases range up to panel/digital limits.
- **Outputs**: All outputs are DC-coupled, ±10 V max per channel.

---

## **LED Color Reference**

**SHAPE (Shape Button/Window):**
- Red: Forward Ramp
- Green: Saw (backward)
- Blue: Triangle (Ping Pong)
- Purple: Sine (Ping Pong Wow & Flutter)
- Pink: Square (Staircase, in LFO mode = Square)
- Orange: Stepped Random
- Yellow: Smooth Random ("Ramplets")

**CLOCK (Clock Window):**
- Red/Orange/Yellow/Green/Purple/Blue: Various speed indicators; quantized divisions/multiples when clocked.

**CHANNELS:**
- Center Spread: White/Pink/Red/Purple (phase)
- Spread active: Aqua/Green/Blue/Hot Pink/Yellow (speed: faster/slower/multiplied/divided).

---

## **Quick Usage**

1. **Patch a Control Signal or Use Internal LFO**: Leave Signal IN open for internal LFO.
2. **Shape Selection**: Use Shape button to pick waveform/shape or read path for processed outputs.
3. **Spread**: Center for uniform speed; clockwise/counter-clockwise spreads channel speeds (extremes go up to x8 or /8, more with high CV).
4. **Phase**: Adjusts phase offset between channels. Use CV for animation or external control.
5. **Time**: Sets overall buffer length / LFO speed. Clock with TEMPO IN.
6. **Reset & Hold**: Use Reset for realignment, Hold to freeze/loop.

---

## **Patch Ideas**

- **"Shift Register"**: Spread @ noon, Phase full CCW, use for oscillator CV distribution w/ increased phase for staggered patterns.
- **"Snap Focus"**: Use TEMPO+RESET for periodic re-alignment of outputs.
- **"Noise Spectrum"**: Feed noise in, use outputs for colored/multispectrum noise.

---

## **Additional Resources**

- [**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)
