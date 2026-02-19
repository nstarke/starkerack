# ALM — ALM034 - Pam's Pro Workout

- [Manual PDF](../../manuals/alm034-manual.pdf)

---

[**Official Pamela’s Pro Workout Manual PDF**](https://busycircuits.com/alm034/manual/)

---

# Pamela’s Pro Workout Cheat Sheet

**Pamela’s Pro Workout** is a powerful programmable clocked modulation and trigger source for Eurorack—with deep parameter editing and extensive external CV modulation.  
This guide puts everything at your fingertips for fast, creative patching!

---

## Panel Reference

```
 ____________________________
|  Pamela’s Pro Workout      |
|                            |  
| [Clk] [Run] [CV1] [CV2]    | <--- Inputs (Top Row)
|                            |
| [Color LCD]                |
|                            |
| [Program Knob] [Start/Stop]| <--- Main Controls
|                            |
| 1 2 3 4 5 6 7 8            | <--- 8 Outputs (Bottom Row)
|____________________________|
```

---

## Jacks, Button, and Knob Reference

### Inputs (Top row, left to right)
| Label      | Function                                                                  | Voltage Range      |
|------------|---------------------------------------------------------------------------|--------------------|
| Clk        | External clock input, or assignable as CV in or bank switch               | 0–5V logic (edge 0.7V min) |
| Run        | Clock run/stop gate, or RESET, CV in, prev bank, or output rotate trigger | 0–5V logic (edge 0.7V min) |
| CV1        | Assignable analog CV input for parameter modulation                       | 0–5V (outside ignored)     |
| CV2        | Assignable analog CV input for parameter modulation                       | 0–5V (outside ignored)     |

> **NOTE:** CV inputs can be assigned as additional CV or trigger sources depending on settings.

---

### Outputs (Bottom row, 1–8 left to right)
- **8 outputs:** Each programmable with clocks, triggers, envelopes, modulation, LFOs, etc.
    - **Voltage Range:** 0–5V, 12-bit resolution, up to 3.8 kHz update frequency
    - **Dedicated green LED per output**

---

### Expander Connections (Rear)
- **Axon-1 / Axon-2:** Adds 4x extra CV ins (0–5V), assignable, with Axon-2 offering 2 assignable buttons
- **PPEXP1 / PPEXP2:** Adds external DIN Sync/MIDI clock outputs and fixed division triggers

---

### Main Controls

| Control                           | Action                                                           |
|------------------------------------|------------------------------------------------------------------|
| **Program Knob** (push/turn)       | Navigate/edit parameters, push to select, hold for ‘extended’ per-output params, long hold (in main screen) opens settings |
| **Start/Stop Button**              | Starts or stops the clock, resets on stop                        |

#### Shortcuts:
- **Hold Start/Stop and turn knob**: Quick-jump same parameter across outputs
- **Hold Start/Stop and click knob**: Mute/unmute current output

---

## Basic Operation Summary

1. **Set Clock BPM:**  
   - Main screen: Turn/push program knob to set BPM (10–330 BPM).
2. **Navigate Outputs / Select Output Modifier:**  
   - Without selecting, turning knob scrolls through 8 outputs.  
   - Push to highlight an output’s "modifier" (mult/divide/utility/triggered).
   - Turn to set time division or type. Push to exit.
3. **Edit Output Parameters (Waveforms & More):**  
   - With output selected, *push+hold* knob (>1 sec) to open parameter page.
   - Scroll & edit: Shape, Level, Width/Slew, Offset, Phase, Euclid, Probability, Loop, Cross-Op, Flex, Quantizer, Scope, etc.
   - Push+hold knob again to exit.

4. **CV Assignment:**
   - Many parameters: Scroll to CV in menu, assign to CV1, CV2 (or Axon if present).
   - Set attenuation/offset for each CV assignment (full bipolar/attenuverter logic).

5. **Save/Load Banks:**
   - Whole module or per-output, up to 64 banks.
   - All settings persist across power cycles.

---

## Output Waveforms & Parameters

| Parameter     | Description                                                               |
|---------------|---------------------------------------------------------------------------|
| **Shape**     | Pulse/square, ratchets, triangle, trapezoid, sine, hump, expo/log env, random, etc.  |
| **Width/Slew**| Changes width (pwm, ratchet density), slew makes wave more/less sharp     |
| **Level**     | Output voltage, 0–5V (in percent)                                         |
| **Offset**    | Adds DC offset (percent of 0–5V); with Level=0, can output fixed CV       |
| **Phase**     | Phase shift/moves start point of waveform                                 |
| **Probability**| Chance step will trigger/send output, 0–100%                             |
| **Euclidean** | Steps / Triggers / Pad / Shift for Euclidean rhythm generation            |
| **Loop**      | Output pattern or randomness can reset/repeat after X beats (incl. nap/wake)|
| **Cross Op**  | Combine output with another output/CV using logic, mix, sample+hold, etc. |
| **Flex Op**   | Micro-timing: Swing, Human, Ramp Up/Down, Hump, Delay, PWR2               |
| **Quantiser** | Quantizes to music scales (Chromatic, Major, Minor, User, etc.)           |
| **Invert**    | Invert output voltage                                                     |
| **Scope**     | Real time waveform view                                                   |

---

## Inputs/Outputs Voltage Ranges

| Jack Type          | Range           | Function                                |
|--------------------|-----------------|-----------------------------------------|
| Outputs 1–8        | 0 to +5V        | CV/triggers/LFO, 12-bit, 3.8kHz         |
| Inputs (CV 1,2)    | 0 to +5V        | Assignable analog CV                    |
| Clk/Run Inputs     | 0 to +5V logic, 0.7V rising| Clock/logic, can be used as assignable CV (0–5V, see above) |

---

## Settings Menu (press+hold encoder from BPM/main screen)

- **Clk/Run input assignment:** (Clock, CV, bank switching, rotation, etc.)
- **EXT PPQN:** Set expected clock pulses per quarter note (default 24)
- **UI theme** (visual style)
- **Encoder hold time** (customize hold duration)
- **Bank load/save**
- **Reset all**
---

## Expander Info (back panel)
- **AUX headers ONLY!** See manual for correct header usage.

---

## Useful Tips

- Any parameter with a % can be modulated by CV!
- Multiple parameters can be assigned to the same CV input, each with custom attenuate/offset.
- Utility output types: GATE (held high = playing), OFF, START (pulse on start), STOP (pulse on stop).
- Use 'Scope' to view your output wave and its shape in real-time.

---

## External Sync

- For precise sync: set PPQN to 24, use DIN Sync-standard clock/run (Run recommended for pre-sync).
- Supports CV control of BPM via clock input.

---

## Links

- [Official Manual PDF](https://busycircuits.com/alm034/manual/)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)