# 2hp — Freez

- [Manual PDF](../../manuals/Freez_Manual.pdf)

---

[Read the Full Manual PDF Here](#)  
*(Replace with actual link if available)*

---

# Freez 2HP Eurorack Looper — Quick Reference Cheat Sheet

## Module Purpose
**Freez** is a voltage-controlled looper/freezer for capturing and mangling audio.  
- Loop size and sample rate (pitch/bitcrush/grain effects) are voltage controllable.  
- Switchable momentary/latching capture.  
- Range: from granular/micro loops to 3s buffers.  

---

## Panel Controls Overview

| # | Name             | Type      | Description                                                                                | Voltage Range         |
|---|------------------|-----------|--------------------------------------------------------------------------------------------|-----------------------|
| 1 | **IN**           | Jack      | Audio input                                                                                | 10Vpp                 |
| 2 | **SIZE CV INPUT**| Jack      | CV input for buffer size. Added to knob position                                           | ±5V                   |
| 3 | **SIZE**         | Knob      | Sets buffer length (max CCW = largest, max CW = smallest, range 9ms–3s, depends on S. RATE)| -                     |
| 4 | **FREEZ LED**    | LED       | Indicates if buffer is frozen (lit = frozen; unlit = passthrough/unfrozen)                  | -                     |
| 5 | **MODE TOGGLE**  | Switch    | Up: Momentary freeze; Down: Latching freeze                                                | -                     |
| 6 | **BUTTON**       | Button    | Press to (un)freeze audio according to toggle setting                                      | -                     |
| 7 | **TRIG**         | Jack      | Trigger input for freeze/unfreeze (matches button behavior)                                | -                     |
| 8 | **S. RATE CV IN**| Jack      | CV input for sample rate (added to knob)                                                   | ±5V                   |
| 9 | **S. RATE**      | Knob      | Sets sample rate of recording/playback (CCW = lowest, CW = highest, 2.36k–96kHz)           | -                     |
|10 | **OUT**          | Jack      | Audio output                                                                               | 10Vpp                 |

---

## Reference Summary: Inputs, Outputs, and Controls

**Inputs**
- **IN**: Main audio input (10Vpp max)
- **SIZE CV INPUT**: Voltage control for SIZE, ±5V (sums with knob)
- **S. RATE CV INPUT**: Voltage control for S. RATE, ±5V (sums with knob)
- **TRIG**: Trigger or gate for (un)freeze control (matches button toggle mode)

**Outputs**
- **OUT**: Processed/frozen audio output (10Vpp max)

**Knobs/Switches/Buttons**
- **SIZE**: Adjust buffer (loop) length (min 9ms - max 3s, changes pitch/timbre)
- **S. RATE**: Adjust sample rate (2.36kHz–96kHz, reduces quality/granulates lower)
- **MODE TOGGLE**:  
  - Up = Momentary (freeze held while pressed or while gate high)  
  - Down = Latching (toggle freeze with each press or trigger)
- **BUTTON**: Manual freeze/unfreeze
- **FREEZ LED**: Lights when module is in freeze (held/latched) mode

---

## Usage Tips
- **Freeze/Unfreeze:** Use BUTTON or TRIG to capture a slice of audio.  
- **Sculpt Texture:** Change SIZE and S. RATE for drastic time/pitch/grain shifts.  
- **Voltage Control:** Sequence/automate CV inputs for dynamic glitching or granular effects.  
- **Modes:** Use momentary for stutter, latching for “tape stop” or creative live-capture loops.


---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)