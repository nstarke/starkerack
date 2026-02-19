# Earthquaker Devices — Afterneath

- [Manual PDF](../../manuals/EQD-EU-Afterneath-Eurorack-R1.pdf)

---

[**Download the Afterneath Eurorack Module Manual (PDF)**](https://www.earthquakerdevices.com/afterneath-eurorack)

---

# EarthQuaker Devices Afterneath Eurorack "Cheat Sheet"

## OVERVIEW
- **Type:** Reverberation Effect (Multi-delays → reverb-like echoes)
- **Audio Path:** Analog dry, digital wet
- **Width:** 16hp | **Depth:** 31.75 mm | **+12V:** 95mA, -12V/5V: 0mA
- **Skiff-friendly**
- **Input Level:** Instrument to modular (set by Input knob)

---

## CONTROLS SUMMARY

### Top Row (Left → Right):
- **Input (knob):** Adjusts gain for audio input (fully CW = instrument; fully CCW = modular)
- **Dampen (knob):** Wet signal tone (CW = darker, CCW = brighter)
- **Reflect (knob):** Feedback/regeneration (turn up for longer, self-oscillates at extremes; also an attenuator for Reflect Return)
- **Mix (knob):** Wet/dry mix (not fully wet unless Dry Kill engaged)
- **Dry Kill (toggle):** Kills dry signal (output = wet only)

### Middle Row:
- **Drag (knob):** Space/spacing for delay lines = “warp speed” effect (CW = shorter, CCW = longer delays; pitch shift when changed live)
- **Mode (knob):** Selects 1 of 9 Drag Modes (see below)
- **Diffuse (knob):** Smears/smooths repeats (CW = more diffuse & reverb-like, CCW = sharper)
- **Length (knob):** Controls reverb decay

---

## JACKS

| Type         | Function                                            | Notes/Voltage Range    |
|--------------|-----------------------------------------------------|------------------------|
| **Input**         | Main audio input                                    | Instrument to modular, adjustable via Input knob |
| **Reflect Send**  | Feedback loop send, for patching external FX etc.   | Signal always present, does not interrupt internal feedback |
| **Reflect Return**| Return for feedback loop; disables internal loop when patched | Doubles as 2nd audio input if feedback not needed; Reflect knob attenuates |
| **Output**        | Main audio output                                   |                       |

---

### CV INPUTS ***(All with Inverting Attenuators)***
- Each parameter with CV has a dedicated inverting attenuator:  
    - **Unity gain**: attenuator full CW  
    - **Inverted**: attenuator full CCW  
    - **Fully attenuated (off)**: at 12 o’clock

| Jack               | Modulates                | Voltage Range                      |
|--------------------|-------------------------|------------------------------------|
| **Drag CV**        | Drag spacing            | Responds only to +1.6V to +4.1V (**Caution:** Bipolar signals need offset) |
| **Mode CV**        | Mode selection          | Not specified (suggest ±5V standard; best results with 0-5V unipolar) |
| **Diffuse CV**     | Diffuse smearing        | Not specified (±5V typical, see above) |
| **Length CV**      | Reverb decay length     | Not specified (±5V typical, see above) |

**Note:**  
- Associated knobs act as offsets for incoming CV.  
- When self-oscillating, Drag CV supports 1V/oct tracking (see below).

---

## MODES (affect Drag CV/knob behavior)
1. **Unquantized:** Smooth, unquantized over full range
2. **Unquantized w/Slew:** Same as above, but with lag (varispeed tape effect)
3. **Unquantized 1V/oct:** Smooth, scaled to 1V/oct (melodic modulation; self-oscillation VCO)
4. **Chromatic Scale:** 1V/oct CV quantized to chromatic scale
5. **Major Scale:**      1V/oct CV quantized to major scale
6. **Minor Scale:**      1V/oct CV quantized to minor scale
7. **Pentatonic Scale:** 1V/oct CV quantized to pentatonic
8. **Oct & Fifths:**     1V/oct CV – only octaves and fifths
9. **Octaves:**          1V/oct CV – only octaves

*Use Mode knob or Mode CV to select. Mode LED displays current selection.*

---

## ADVANCED USAGE

- **Self-Oscillation:**  
  - With Reflect/Length >12:00, module can self-oscillate (“regenerated reverb” → turns into VCO)
  - In Modes 3–9, Drag CV input follows 1V/oct (for keyboard/sequencer tracking)
  - **Drag CV Input:** Only positively responds to 1.6-4.1V unipolar
  - To scale properly:
    1. Drag CV attenuator full CW, Drag knob at noon
    2. Modes 3-9
    3. Length/Reflect > 12:00
    4. Play octave CV source, find upper Drag knob limit, set just beyond
    5. Lower Length/Reflect to stop oscillation if needed

- **Pseudostereo:**  
  - Output main & Reflect Send to separate channels for spacious/multichannel effects.
  - Patch Reflect Send to mults → other outputs/processing → Reflect Return.

---

## TIPS
- Input knob: Turn up for guitar/synth, down for modular signals.
- Use Inverting Attenuators to fine-tune CV ranges—start with knob noon, attenuator fully CW for external CV.
- Diffuse: Higher for ambient, lower for clarity.
- Self-oscillation = creative oscillator, can track pitch (not perfectly tuned).

---

## QUICK REFERENCE: ALL CONTROLS & JACKS

| Knob/Button/Toggle  | Function                                          |
|---------------------|--------------------------------------------------|
| Input               | Sets input gain                                  |
| Dampen              | Sets wet signal brightness                       |
| Reflect             | Sets feedback amount                             |
| Mix                 | Wet/dry blend                                    |
| Dry Kill (toggle)   | Removes dry audio (true "wet-only" out)          |
| Drag                | Spacing/"warp" between reverb delays             |
| Mode                | Select Drag mode (9 choices)                     |
| Diffuse             | Amount of smearing/ambience                      |
| Length              | Reverb decay time                                |

| Jack                | Function/Modulates                               | Voltage Range                   |
|---------------------|--------------------------------------------------|---------------------------------|
| Input               | Audio In                                          | Instrument/modular level        |
| Reflect Send        | Feedback signal out                               | Audio                           |
| Reflect Return      | Feedback signal in (bypass internal loop)         | Audio                           |
| Output              | Main Audio Out                                    | Audio                           |
| Drag CV             | Modulates Drag                                    | +1.6 to +4.1V (offset needed)   |
| Mode CV             | Modulates Mode selection                          | (0-5V recommended)              |
| Diffuse CV          | Modulates Diffuse                                 | (0-5V recommended)              |
| Length CV           | Modulates Length                                  | (0-5V recommended)              |

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)