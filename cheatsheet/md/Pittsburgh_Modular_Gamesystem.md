# Pittsburgh Modular — Gamesystem

- [Manual PDF](../../manuals/game_system_manual.pdf)

---

# Pittsburgh Modular **Game System** — Cheat Sheet

[**Download Manual PDF**](https://pittsburghmodular.com/storage/manuals/GameSystemManual.pdf)  
*(Direct link to manufacturer PDF, use for full details and graphics.)*

---

## Quickstart Overview

**Game System** offers 6 sequencer "games" (5 CV/Gate sequencing, 1 Euclidean rhythm generator), joystick/button control, all fully CV/gate controllable.

---

## Panel Controls / Inputs / Outputs

### **Buttons**
| Button | Function |
|--------|----------|
| **GAME**       | Cycle "games"; hold 2s to enter settings menu |
| **MODE**       | Game-dependent mode (see below) |
| **RESET**      | Resets open game |
| **CLOCK**      | Tap tempo (internal clock), or clock divider (external clock) |

### **Joystick**
| Movement      | Function (Game Dependent) |
|---------------|--------------------------|
| All Directions| Steps cursor, selects steps/params, per game |
| Press         | Select/confirm/toggle step on/off; set last step (hold 2s) |

### **Inputs (CV/Gate)**

| Input    | Emulates                 | Action/Threshold |
|----------|--------------------------|------------------|
| BUTTON   | Joystick Button          | >threshold gate/CV = press |
| MODE     | Mode Button              | same             |
| RESET    | Reset Button             | same             |
| CLOCK    | External Clock           | Used in ExtClk mod|
| LEFT     | Joystick Left            | same             |
| RIGHT    | Joystick Right           | same             |
| UP       | Joystick Up              | same             |
| DOWN     | Joystick Down            | same             |

- **Trigger threshold not specified; expect typical eurorack gate logic (anything >+2V likely works).**

### **Outputs**

| Output   | Jack Type | Voltage Range         | Game Usage (See Game Summaries)               |
|----------|-----------|-----------------------|------------------------------------------------|
| OUTPUT 1 | CV or Gate| 0–5V CV; Gate         | Game-specific: CV (1V/Oct), gate, clock        |
| OUTPUT 2 | CV or Gate| 0–5V CV; Gate         | Game-specific: CV (1V/Oct), gate, clock        |
| OUTPUT 3 | Gate only | ~5V (typ.)            | Game-specific: gate only                       |
| OUTPUT 4 | Gate only | ~5V (typ.)            | Game-specific: gate only                       |

- **CV Outputs calibrated 1V/Octave, 0–5V (for melody CV, random CV, etc.)**
- **See individual game for which jack does what.**


---

## **Game Summaries**

| Game         | Description | Key Controls | Outputs    |
|--------------|-------------|--------------|------------|
| **1: Meteor Shower** | Arcade-style, dodge meteors; random voltage & gates from explosions | Joystick: Move; JBtn: # of meteors (hold); Mode: Autopilot | O1: Random CV (1V/oct, 0–5V) (on ship/meteor); O2: Gate (on ship/meteor); O3: Gate (meteor/ground); O4: Step clock |
| **2: Music Sequencer** | Classic 1–32 step CV/gate; per-step voltages | JS: Left/right: step, up/down: CV, JBtn: Toggle step (hold: set last), Mode: Dir | O1+O2: CV (1V/oct, 0–5V); O3: Gate on active step; O4: Step clock |
| **3: Drum Sequencer** | Four 16-step gate sequencers (percussion) | JS: Move cursor; JBtn: Toggle step (hold: set last); Mode: Flip seqs | O1: Top green seq gate; O2: Top red seq gate; O3: Btm green; O4: Btm red |
| **4: Time Traveller** | 4 outruns "grid", 2D clock divider (div 1–8, offset) | JS: Move select out; JBtn: Change selected out; Mode: Free roam (random movement) | O1–O4: Gate when given out overlays green clock div |
| **5: Probability Machine** | 2D probability field for complex/chaotic CV/gate | JS: Red arrow pos; JBtn: Complexity (1–4); Mode: Computer control | O1: Rand CV w/ O3 gate; O2: Rand CV w/ O4 gate (1V/oct, 0–5V); O3: Gate; O4: Gate |
| **6: Euclidean Rhythms** | Euclidean gate generator (geo patterns) | JS: L/R: seq len, U/D: # of beats, JBtn: Invert pattern; Mode: Dir | O1: Random CV (active step, 1V/oct, 0–5V); O2: Gate on active step; O3: Gate on inactive; O4: Step clock |

---

## **Settings Menu**

Press and hold **GAME** button (2s), use joystick to cycle, GAME to exit.
- **1. Clock Source:** Internal (tap tempo via CLOCK) / External (use CLOCK jack; CLOCK btn is divider)
- **2. Display Brightness**
- **3. Gate Length:** 40/80/160/240ms
- **4. Factory Reset:** JS UP ×3, explosion confirms
- **5. Static Voltages:** Select + calibrate CV outputs (adjust trim for 1V/oct 0–5V)

---

## **Voltage/CV Details**
- All CV outputs: **0–5V, 1V/Octave calibration** where applicable.
- Gates: **~0–5V typical**.
- CV/Gate input triggers: **Any voltage above trigger threshold (spec not given; typically >+2V in Eurorack).**

---

## **Links**

[Game System Manual PDF](https://pittsburghmodular.com/storage/manuals/GameSystemManual.pdf)  
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)