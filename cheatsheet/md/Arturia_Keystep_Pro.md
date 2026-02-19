# Arturia — Keystep Pro

- [Manual PDF](../../manuals/keystep-pro_Manual_1_1_0_EN.pdf)

---

[Arturia KeyStep Pro – Full User Manual PDF](https://manuals.arturia.com/pdf/KeyStep_Pro_EN.pdf)

---

# Arturia KeyStep Pro – Eurorack Cheat Sheet

*(Controller/Sequencer for Modular & MIDI Gear - Essentials Guide)*

---

## Hardware Overview

- **Type:** 37-key MIDI/CV controller & sequencer
- **Power:** 12V DC, 1.0A (Center Positive)
- **Computer Connection:** USB MIDI Class Compliant  
- **Standalone:** Yes (DC power jack)

---

## I/O Connections

### **Analog Voice Outputs (for Modular)**
- **Voice Outs (1–4):**
  - **Pitch CV (1V/Oct, 1.2V/Oct, or Hz/V)**
    - **Range:** 0–10V (assignable per voice)
    - **Set in Utility/MIDI Control Center**
    - **Default:** 1V/Oct for Eurorack
  - **Velo/Mod CV (velocity or aftertouch, assignable)**
    - **Range:** 0–10V (max settable 1–10V)
    - **Default:** Velocity
  - **Gate CV**
    - **Range:** 0 or +5V/+10V (V-Trig, S-Trig selectable)
    - **Default:** +5V (V-Trig)

### **Drum Gates (Track 1/Drum Mode)**
- **Outputs 1–8:**  
  - **Trig/Gate:** 0V/+5V (or +12V, S-Trig assignable)
  - **For triggering modular drums or EGs**
- **Drum outputs map to the lowest 8 keys**  
- **MIDI Note assignment customizable**

### **Clock Section**
- **In:** Accepts 1 pulse/step, 2/step, 24ppq, 48ppq (0–5V)
- **Out:** Outputs settable clock types (same rates, 0–5V)
- **Reset Out:** +5V, 4ms pulse (when STOP/RESET sent)

### **MIDI Section**
- **MIDI In:** 5-pin DIN
- **MIDI Out 1/Out 2:** 5-pin DIN (x2)
- **Can send/receive all MIDI notes, CCs, sync, transport**

### **USB MIDI**
- **Type B port**
- Class compliant – driverless. Can power via USB but hardware recommends using power supply for modular/CV use.

### **Power**
- **12V DC**, center positive, 1A, barrel connector

---

## Controls

### **Knobs/Encoders**

**Main Encoders (x5, touch-sensitive):**
  1. Pitch
  2. Gate length
  3. Velocity
  4. Time Shift
  5. Randomness

- **Function depends on mode:**  
  - **Seq/Drum:** Encode step parameters  
  - **Control Mode:** Send MIDI CCs (assignable)

**Tempo/Fine**  
- Set project/global tempo, or shift for fine adjust

**Swing/Offset**  
- Set swing per-sequence/project (+track offset with Shift)

**Metronome Level (back panel)**  
- Retractable knob

---

### **Buttons**

- **Transport:** PLAY, STOP, RECORD/QUANTIZE
- **Step (16):** For programming, selecting, copy, page select (for steps 1–64)
- **Track (1–4):** Select sequencer/track
- **Seq/Arp/Drum:** Toggle track mode (Track 1 = Drum, 2-4 = Arp)
- **Pattern, Scene, Chain:** Pattern and arrangement management
- **Mute/Solo:** Per-track
- **Overdub, Tie/Rest/Chord, Hold, Transpose, Shift**
- **Looper touch strip:** Live loop length & position

---

### **Keybed**
- 37 SlimKeys, velocity + aftertouch
- **Oct +/−, Pitch strip, Mod strip:** Touch controls

---

## CV/Gate, Input/Output Reference & Voltage Ranges

| Jack Name        | Type   | Signal          | Voltage Range            | Notes                          |
|------------------|--------|-----------------|-------------------------|--------------------------------|
| Voice 1–4 Pitch  | Output | CV (1V/Oct, etc)| 0–10V (default)         | Eurorack, Buchla, Hz/V assign. |
| Voice 1–4 Velo/Mod | Output| CV              | 0–10V (default)         | Velocity or Aftertouch         |
| Voice 1–4 Gate   | Output | Trigger/Gate    | 0/+5V (default), +10V   | V-Trig/S-Trig select           |
| Drum 1–8         | Output | Trigger/Gate    | 0/+5V (default), +12V   | For modular drum triggers      |
| Clock In         | Input  | Sync Pulse      | 0–5V (typical, TTL)     | 1step to 48ppq                 |
| Clock Out        | Output | Sync Pulse      | 0–5V (typical, TTL)     | Configurable ppq               |
| Reset Out        | Output | Gate            | +5V/4ms pulse           | Step/sequence reset            |
| MIDI In          | Input  | MIDI DIN        | —                       | Standard MIDI                  |
| MIDI Out 1/2     | Output | MIDI DIN        | —                       | Standard MIDI                  |
| USB              | Bi-dir | USB MIDI        | —                       | Sends/receives MIDI            |
| Sustain          | Input  | Footswitch      | —                       | Momentary                      |
| Metronome Out    | Output | Audio (click)   | Line level              | For click track                |
| Power            | Input  | 12V DC, 1A      | —                       | 2.1mm ID, 5.5mm OD, C+         |

---

## Key Performance Functions

- **Four Sequencers or three + drum sequencer**
- **Poly sequencing:** Up to 16 notes per step  
- **Step input, realtime input, overdub**  
- **Arpeggios:** 3 tracks, multiple modes, scales/octave/patt
- **CV Assign:** Route any track to any CV out
- **Drum Triggers:** Track 1 only, polymeters possible
- **Instant pattern change, pattern chains/scenes**
- **Flexible clocking:** MIDI, DIN, analog
- **SHIFT shortcuts everywhere:** Step operations, scale, root, CV assignment, pattern ops, time division...

---

## Programming & Performance Quick Tips

- **Connect to Modular:**
  - CV/Gate as described above; set correct standard (1V/Oct, V-trig, etc) in Utility or MIDI Control Center
  - Use Drum Gate outputs for triggering modular drums
- **Split keyboard:** Two tracks, upper/lower split (hold two Track buttons, set split note)
- **Assign CV:**
  - `SHIFT + G#/A/A#/B` (top octave): Route track to any CV voice(es)
- **Set scales quickly:**  
  - `SHIFT + Key` (upper row, blue text) for scale select, root, and custom scales
- **Polyrhythms:**  
  - Track length, polymeter per Drum track (Drum mode Poly)
- **Pattern management:**
  - Copy, paste, clear, undo, chain, scenes all accessible with dedicated/shift + buttons.

---

## Control Summary (Knobs, Buttons, Controls)

- **Knobs/Encoders:**
  - 5x Encoder (Pitch, Gate, Velocity, Time Shift, Random), 1x Tempo, 1x Swing
  - Metronome level (back panel)
- **Switches/Buttons**
  - Per above - Transport, Track select/mode, Pattern, Scene, Chain, Step, Mute, Solo, Utility, Control, Overdub, Hold, Chord, Tie/Rest, Octave, Looper
- **Touchstrips:** Pitch, Mod, Looper (horizontal)

### **SHIFT + [Key]**
- Pattern direction, scale, root, time division, chord mode, CV routing, clear, nudge, quantize, transpose, step skip, etc.

---

## Useful Links

- [Full Manual PDF (Arturia)](https://manuals.arturia.com/pdf/KeyStep_Pro_EN.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---

### **Modular Setup Reminder**

- Always power off before connecting CV/Gate!
- Confirm voltage/trig standard with your synthesizer's documentation.
- Use MIDI Control Center or Utility menu for advanced configuration.

---

*This cheat sheet covers essentials for modular/Eurorack users. For deep dives (scenes, DAW integration, firmware-specific features), refer to the full manual above.*