# Kaona Instruments — Zazou

- [Manual PDF](../../manuals/Zazou_manual_ENG_V1-0.pdf)

---

**[Zazou Eurorack Module Manual (PDF)](https://www.kaona.fr/manuel-zazou-en.pdf)**

---

# **ZAZOU Cheat Sheet**
_Eurorack Generative Sequencer (Firmware 1.0)_

---

## **Panel Overview & Controls**

### **Encoders**
- **Encoder 1:** Menu navigation (short click = enter, long click = special functions)
- **Encoder 2:** Select/adjust algorithms, sequences (short click = select, rotate = change value)
- **Encoder 3:** Fine parameter changes, confirmations (click = confirm/select)

### **Buttons (4, color-coded)**
- **Track selection (Red, Yellow, Green, Blue)**
  - **Base:** Activate/deactivate tracks for parameter edits
  - **Algorithms/Sequences:** Manual gate (play note from track)
  - **Live:** Mute/unmute each track

### **Transport Buttons**
- **Play/Stop:** Start/stop note generation (also via CV)
- **Reset:** Restart sequence from beginning (also via CV)
- **Change:** Advance sequence by one step (also via CV)

---

## **Input/Output Jacks (with voltages)**

### **Inputs (CV)**
- **Gate Inputs (x4, color-coded):**  
  - _4 Tracks, triggers note generation per channel_  
  - **Expected:** Standard Eurorack gates/triggers (0V = low, ≥3V = high)
- **Play/Stop In:** Gate input to globally start/stop sequences  
  - **Expected:** Gate/trig, ≥3V active
- **Reset In:** Gate input to restart all sequences  
  - **Expected:** Gate/trig, ≥3V active
- **Change In:** Gate input: advance steps  
  - **Expected:** Gate/trig, ≥3V active

### **Outputs**
- **Gate Outputs (x4):**  
  - _One per channel; pulses active when note is sounding_  
  - **Levels:** Standard Eurorack gate (0V = low, 5V = high)
- **1V/Oct Note Outputs (x4):**  
  - _Outputs pitch per note_  
  - **Range:** 1V/oct (transposable/octave range settable), up to 5V (default) or 8V max (set in config)
- **CV Outputs (x4):**  
  - _Outputs note velocity_  
  - **Range:** 0–5V (or 0–8V, configurable)
- **MIDI Out (TRS-A/B configurable):**  
  - _Poly/multitimbral MIDI note & velocity output, up to 4 channels_
  - **MIDI Channel:** Assignable per track

#### **Other Connections**
- **SD Card:** For saves, not needed to function but enables manual save/load
- **Gate Connector:** For dedicated cable link to Skippy (rhythm generator)
- **USB Port:** _Firmware updates only (never connect with power plugged in!)_
- **Expander Port:** Reserved for future use, do not connect anything!

---

## **Main Modes / Menus**

| **Section**    | **Entry**           | **Functions**                                      |
|----------------|---------------------|----------------------------------------------------|
| Base           | Short click Enc 1   | Set key/root, scale, global settings, per-track tuning |
| Algorithms     | Short click Enc 2   | Choose & parameterize melodic algorithm per track  |
| Sequences      | Long click Enc 2    | Set chord/note progressions, chain chords, steps   |
| Live           | Short click Enc 3   | Circle of fifths display, mute/unmute tracks       |
| Files          | Long click Enc 3    | Save/load presets/tracks/sequences (SD needed)     |
| Configuration  | Long click Enc 1    | Set MIDI channels, clock/ref BPM, output voltages  |

---

## **Quick Reference: Algorithms**
| **Algorithm**    | **Description/Style**                |
|------------------|---------------------------------------|
| RANDOM           | Random notes in scale/chord           |
| ARPEGGIO         | Many arpeggio styles & patterns       |
| WALKINGBASS      | Basslines (jazz, blues, boogie, etc.) |
| SERIAL           | Serialist (12-tone); chromatic only   |
| CANTOR           | Fractal; pattern via recursion        |
| FIBONACCI        | Fibo sequence; melodic propagation    |
| INTERVAL         | Repeated intervals (set multipliers)  |
| SIERPINSKI       | Fractal division/recurrence patterns  |
| MANDELBROT       | Complex → simple patterns             |
| JULIA            | Fractal, diverging/repetitive notes   |

_All algorithms have extensive parameters (chord, octave, duration, velocity, ornamentation, etc)._

---

## **Selections** 

### **Scales (20+)**
Major, Minor, Nat/Harm Melodic minors, Pentatonics, Blues (M/m), Jazz modes (Ionian, Dorian, etc), Chromatic, Bebop, etc.

### **Chord Types (selectable per algorithm)**
- Major (M), Minor (m), 6, 7, M7, m7, sus, dim, aug, add9, add11, add13, etc.
- “SCALE” chord: allows access to all notes in selected scale.

---

## **Other Settings**

- **Root Note:** Sets base key per track or globally
- **Sequences:** Choose progression (II-V-I, Circle of 5ths/4ths, blues 12-bar, etc.) or random/root etc.
- **Velocity CV Output Voltage Range:** 0–5V or 0–8V (set in Config)
- **1V/oct Note Output:** Octave and max voltage clamped (5V/8V, configurable)
- **BPM:** Fixed or measured from PLAY/STOP gate In

---

## **Tips**

- **All settings are per-track or global (when all track buttons active)**
- **All parameters are auto-saved. SD card enables manual save/load/recall.**
- **Muting/Unmuting in Live mode is instant via track color button.**

---

## **Troubleshooting**

- **MIDI TRS not working?** Set TRS-A/B switch accordingly (change only while module is off)
- **Note voltage or velocity too high?** Limit max output to 5V in config
- **USB use:** _Never connect USB while module is powered!_

---

## **Voltage Ranges Reference**

| **Jack**         | **Type**                | **Voltage Range**     |
|------------------|------------------------|-----------------------|
| Gate Inputs      | Input (per track)       | ≥3V = trigger         |
| Play/Reset/Change| Input                   | ≥3V = trigger         |
| Gate Outputs     | Output (per track)      | 0V or 5V              |
| 1V/Oct Output    | Output (per track)      | 0–5V (or 0–8V)        |
| CV Output        | Output (per track)      | 0–5V (or 0–8V)        |

---

## **Links**

- **[Official Manual PDF](https://www.kaona.fr/manuel-zazou-en.pdf)**
- **[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**
