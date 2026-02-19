# Erica Synths and Gamechanger Audio — Plasma Drive

- [Manual PDF](../../manuals/Plasma_Module_Manual.pdf)

---

[Erica Synths Fusion Plasma Drive Manual PDF](https://www.ericasynths.lv/media/Plasma_Drive_manual_1_01_WEB.pdf)

---

# Erica Synths Fusion Plasma Drive – Eurorack Cheat Sheet

Unique high-voltage distortion for Eurorack, combining vacuum tubes and plasma discharges, with tracking oscillators and assignable EQ for over-the-top sound mangling.

---

## **Summary Table**

### **Inputs, Outputs, Controls & Their Functions**

| Name           | Type     | Function/Range                                              | Location               |
|----------------|----------|------------------------------------------------------------|------------------------|
| **INPUT**      | Audio In | Main audio input, up to 20V ptp                            | Bottom left            |
| **OUTPUT**     | Audio Out| Main processed output                                      | Bottom right           |
| **VOLTAGE CV** | CV In    | Controls distortion level, -10V to +10V                    | Bottom right           |
| **DRY/WET CV** | CV In    | Controls dry/wet mix, -10V to +10V                         | Bottom left            |
| **OCT TRIG**   | Trigger In| Toggles 1 octave up/down tracking oscillator              | Middle right           |
| **SUB TRIG**   | Trigger In| Toggles 2 oct/3 oct down sub tracking oscillator          | Middle right           |

### **Knobs**

| Name         | Function                                             |
|--------------|-----------------------------------------------------|
| **IN LVL**   | Sets input gain; critical for signal shaping        |
| **VOLTAGE**  | Manual distortion/overdrive amount (CV summed)      |
| **DRY/WET**  | Blend between clean/dry and wet/distorted signal (CV summed) |
| **TREBLE**   | EQ high frequency boost/cut (±10dB @ 1.5kHz)        |
| **BASS**     | EQ low frequency boost/cut (±9dB @ 600Hz)           |

### **Switches/Buttons**

| Name         | Type             | Function                                                        |
|--------------|------------------|-----------------------------------------------------------------|
| **OCT Switch** | 3-position      | Up = +1octave, Mid = +1 & -1octave, Down = -1octave (tracking oscillators)   |
| **EQ ON/OFF** | Toggle (Latching)| ON = EQ before and after distortion; OFF = EQ after only        |
| **OCT TRIGG**  | Button (lit)     | Manually engages/disengages tracking oscillator(s)              |
| **SUB TRIGG**  | Button (lit)     | Manually engages/disengages sub tracking oscillators (-2, -3 oct); only works if OCT switch is MID or DOWN |

---

## **Quick Start**

1. **Connect Audio Input** to `INPUT`.
2. **Set IN LVL** to avoid unwanted clipping or volume loss.
3. **Raise VOLTAGE** to increase distortion (use CV for modulation).
4. **Set DRY/WET** for desired blend (use CV for morphing).
5. **Use TREBLE/BASS** EQ for tone shaping.
6. **Experiment with OCT Switch** for extra harmonics. Engage with OCT TRIGG/SUB TRIGG or via external triggers.
7. **EQ ON** feeds EQ before and after distortion; **EQ OFF** is post only.
8. **Take your output signal** from `OUTPUT`.

---

## **Technical Specs**

- **Audio Input:** up to 20V ptp
- **CV Inputs:** -10V to +10V
- **Panel width:** 16HP
- **Depth:** 45mm
- **Power:** 135mA @ +12V / 87mA @ -12V

---

## **Tips**

- **Input Level is Crucial**: Hotter signals = more interaction with plasma tube.
- **Use CV for Animation:** Modulate `VOLTAGE` or `DRY/WET` for evolving distortion.
- **Tracking Oscillators**: Add wild octave-up or sub-octave buzz and analog-style grit.
- **Try Rhythmic Triggers**: Send rhythmic gates/triggers to `OCT TRIG` or `SUB TRIG` for dynamic distortion changes.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)