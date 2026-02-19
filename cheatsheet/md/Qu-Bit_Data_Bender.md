# Qu-Bit — Data Bender

- [Manual PDF](../../manuals/QB_Data_Bender.pdf)

---

[Download the Data Bender Manual PDF](https://qubitelectronix.com/manuals/Data_Bender_Manual.pdf)

---

# Qu-Bit Data Bender Cheat Sheet

_Data Bender is a circuit bent digital audio buffer module for Eurorack, with high-fidelity 96kHz/24-bit audio, stereo I/O, and extensive real-time control for lo-fi, glitch, "bent" audio manipulation._

---

## I/O Reference

### Inputs

| Jack      | Function               | Voltage Range / Notes                        |
|-----------|------------------------|----------------------------------------------|
| left      | Audio In, Left (normals to right if empty) | Modular/Line Level*                       |
| right     | Audio In, Right        | Modular/Line Level*                          |
| clock     | External Clock In      | Standard modular gate/trigger                |
| time      | Time (buffer length) CV| -5V to +5V (adds to knob)                    |
| repeats   | Repeats CV             | -5V to +5V (adds to knob)                    |
| bend      | Macro: Bend on/off (Gate/Trig), Micro: playback reverse (Gate/Trig) | Modular gate/trigger  |
| break     | Macro: Break on/off (Gate/Trig), Micro: Traverse/Silence select (Gate/Trig) | Modular gate/trigger  |
| corrupt   | Corrupt on/off (Gate/Trig, or secondary: Reset Input) | Modular gate/trigger  |
| freeze    | Freeze buffer on/off (Gate/Trig) | Modular gate/trigger      |
| mix       | Mix CV                 | -5V to +5V (adds to knob)                    |

> *Input is modular level (up to ~10Vpp), accept line level but beware of extra loud outputs if saturation is introduced.

### Outputs

| Jack      | Function                | Voltage Range / Notes                  |
|-----------|-------------------------|----------------------------------------|
| left      | Audio Out, Left         | Modular level, typically up to 14Vpp   |
| right     | Audio Out, Right        | Modular level, typically up to 14Vpp   |

---

## Panel Controls

### Knobs

| Control   | Function                                               | CV Response |
|-----------|--------------------------------------------------------|-------------|
| time      | Sets buffer length/sample period; Internal: 16s – 80Hz / External: clock div/mult | -5V to +5V  |
| repeats   | Divides buffer for "stutter"; 0 = off, more = faster stutter | -5V to +5V |
| mix       | Dry/Wet blend: input/live vs. bent audio               | -5V to +5V  |
| corrupt   | Decimate: Bit-reduce/downsample<br>Dropout: Glitch/mute sections<br>Destroy: Saturate/clip<br>Selected by button | -5V to +5V  |
| bend      | Macro: tape/vinyl actions; Micro: playback speed/range/reverse | -5V to +5V  |
| break     | Macro: CD skips/stutter/silence; Micro: select buffer fragment or silence amount | -5V to +5V  |

### Buttons & LEDs

| Button    | Function / LED                                            |
|-----------|------------------------------------------------------------|
| shift     | Access secondary (edit) actions (hold) / blue when held   |
| clock     | Toggle Internal/External clock mode / LED blue (int), white (ext) |
| mode      | Macro (blue)/Micro (green) toggle                         |
| bend      | Enable/disable macro bend or reverse(micro); disables at knob min |
| break     | Macro: enable/disable; Micro: Traverse/Silence toggle     |
| corrupt   | Step through Decimate/Dropout/Destroy modes; color-coded  |
| freeze    | Freeze buffer (latch or momentary, edit menu)             |

---

## Core Functions Summary

- **Time**: Sets main buffer window (memory period).  
    - *Int*: 16s–80Hz (knob sweep)  
    - *Ext*: Clock div/mult (-16x to +8x), selected at detents. LED briefly gold when crossing div/mult border.  
    - CV (-5V–+5V) applies to knob.
- **Repeats**: Divides buffer (repeat/stutter), more = smaller subsections. CV (-5/+5V) applies to knob.
- **Mix**: Dry/wet blend from live input (left) to max buffer effect (right). CV (-5/+5V).
- **Corrupt**: Three modes toggled by button (hold Corrupt):
    - **Decimate (Blue)**: Bitcrush/downsample.  
    - **Dropout (Green)**: Random silences, adjust length/density.  
    - **Destroy (Gold)**: Soft/hard saturation; full right = hard clipped.  
- **Freeze**: Toggle "freeze" (buffer is locked/all parameters still editable); latching or momentary set in edit mode.
- **Bend** (Macro Mode):  
    - Simulates tape/vinyl: random playback speed, reverse, stops/pops/clicks.  
    - Knob affects probability/depth and complexity.
    - Gate/button toggles on/off.  
- **Break** (Macro Mode):  
    - CD skip style: glitches, stutter, buffer jumps, silence.  
    - Knob controls repeat probability and silence fraction.  
    - Gate/button toggles on/off.
- **Bend** (Micro Mode):  
    - Precise playback speed set (±3 octaves), press for reverse.
    - LED color: blue-forward, green-reverse, cyan/gold at integer octaves.
- **Break** (Micro Mode):  
    - Knob/Repeats choose buffer subsection (Traverse).
    - Press to toggle Traverse/Silence (LED on = silence duty control).

---

## Secondary (Shifted) Controls

_Hold Shift + press below for extra features:_

- **Shift + Time**: Glitch Windowing (ramps/click smoothing, indicated by Shift LED brightness/color).
- **Shift + Bend**: Stereo Mode — auto effects unique (blue) or shared (green) per channel.
- **Shift + Break**: Factory Reset (Break LED pulses white/blue confirm).  
- **Shift + Corrupt**: Corrupt jack toggles from Corrupt Gate (blue) to Reset Input (green), resets buffer clock.
- **Shift + Freeze**: Freeze latching (blue) or momentary (green).
- **Shift + Clock**: All gate inputs latching (blue) or momentary (green).

---

## Example Quick Start: "Lo-Fi Tape"

- Mode: Micro (Mode LED green)
- Mix: 100% (all the way up)
- Time: ~30% (set buffer window)
- Repeats: 0% (single buffer)
- Bend: ~45% (for tape effects)
- Corrupt: ~45% (for subtle noise/dropouts)
- SHIFT + TIME (Glitch Window): 0% (hard/no ramp for clicks & pops)

---

## General Specs

- **Width/Depth**: 14HP / 28mm
- **Power**: +12V: 58mA, -12V: 60mA
- **Sampling**: 96kHz, 24-bit, >1 min stereo memory

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)