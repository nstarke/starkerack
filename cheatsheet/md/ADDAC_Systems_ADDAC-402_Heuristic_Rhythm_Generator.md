# ADDAC Systems — ADDAC-402 Heuristic Rhythm Generator

- [Manual PDF](../../manuals/ADDAC402_UsersGuide_A_0_web_6500.pdf)

---

```markdown
[ADDAC402 User Manual PDF](http://addacsystem.com/sites/default/files/files/ADDAC402_USER_GUIDE.pdf)

# ADDAC402 Heuristic Rhythm Generator – Cheat Sheet

---

## **OVERVIEW**

**4 independent gate/trigger channels**. Generates rhythms with multiple algorithms, adjustable by knobs, buttons, and CV.  
Visual feedback via OLED screen and LEDs.

---

## **FRONT PANEL CONTROL SUMMARY**

**Jacks**
| Jack Number | Label/Type                        | Function                                 | Voltage Range        |
|:-----------:|:----------------------------------|:-----------------------------------------|:---------------------|
| 14          | Fills/Parameter B CV Inputs       | CV for Fills/Parameter B per voice       | 0-5V                 |
| 15          | Inverted Gate Outputs             | Inverted gate/trigger out per channel    | 0/5V (trigger/gate)  |
| 16          | Gate Outputs                      | Main gate/trigger out per channel        | 0/5V (trigger/gate)  |
| 17          | Play/Pause Trigger Input          | Clock in for play/pause toggle           | Gate/Trig 0-5V       |
| 18          | Clock Trigger Input               | Master clock                             | Gate/Trig 0-5V       |
| 19          | Master Reset Trigger Input        | Resets all sequences                     | Gate/Trig 0-5V       |
| 20          | Swing / Assign CV Input           | Assignable CV input (swing/etc.)         | 0-5V (assignable)    |

**Knobs & Encoders**
- **Preset Selector & Menu Scroll (3):** Select/load/save presets, scroll config menu
- **Swing/Assign (4):** Default = swing, assignable per config, acts as attenuator with CV in (0-5V)
- **Steps / Param A (7):** Adjust steps/parameter A (per channel/algorithm)
- **Fills / Param B (8):** Adjust fills/parameter B, attenuator when CV jack used (0-5V)

**Buttons**
- **Mode Info/Menu/Enter (2):** Short = info/menu select; Long (3s) = open config menu
- **Play/Pause (5):** Start/stop transport
- **Skip Step (10):** Skip/rotate current channel pattern
- **Resets (11):** Reset individual voice sequence to start
- **Master Reset (12):** All voices reset to step 1
- **Mode Select (13):** Advance to next mode

**Toggles**
- **Gate/Trigger Switches (9):** Per-voice, sets output as gate or trigger per channel

**Visual**
- **OLED Display (6):** Parameters and current pattern feedback
- **LEDs (1):** Per-channel gate state

---

## **ALGORITHMS / MODES**

Cycle with Mode Select button, in this order:
1. **Euclidean:** STEPS = total steps, FILLS = # of "on" steps, SKIP rotates, RESET resets.
2. **Gate Sequencer:** Up to 32 steps/channel. STEPS = pattern length, FILLS = move cursor, SKIP toggles step, RESET resets.
3. **Game of Life:** FILLS=#bars, SKIP=next gen, RESET=new pattern, MST RESET=next gen (evolves pattern).
4. **Golomb Rulers:** FILLS=choose ruler, outputs marks at unique intervals, SKIP advances, RESET resets.
5. **Probabilistic:** FILLS=probability%. Probability "used up" sequentially across channels.
6. **Footwork:** STEPS=trigger length, FILLS=main controls (see screen), experimental, resets/skip/gate switches inactive.
7. **Pong:** Ball bounces per wall triggers channels 1–4. Pad size, ball speed, left/right and reset controls.

**Preset Management:**  
Up to 16 patterns (presets) per mode (Euclidean, Gate Seq). Use Preset Knob and Skip Step 3/4 as up/down; Menu button to confirm actions.

---

## **CONFIGURATION MENU**

Long-press the Menu button for config options. Key assignments include:
- Trigger time (2–32 ms)
- Gate time (fractions of step)
- Assign what the Swing/Assign knob and CV control (can be SWING, PRESETS, STEPS, G/T, SKIP, RESET per channel)
- MIDI bridge config (needs expansion module)

**Swing:**  
- **Default:** Delays steps for groove.  
  - 1st 1/4 = swing on every 3 clocks
  - 2nd = 4, 3rd = 6, 4th = 8
- **Assignable:** Knob or 0–5V CV

---

## **JACKS — DETAILED REFERENCE**

| JACK              | DIRECTION | SUMMARY                              | VOLTAGE RANGE       | NOTES                            |
|-------------------|-----------|--------------------------------------|---------------------|----------------------------------|
| Gate Out (x4)     | OUT       | Main gate/trigger output             | 0/5V                | CV/gate to envelopes, drums, etc |
| Inverted Gate Out | OUT       | Inverted logic of gate output        | 0/5V                | Triggers on "off" steps          |
| Fills/Param B CV  | IN        | Per-voice Fills/Param B CV           | 0-5V                | Scales knob when patch plugged   |
| Swing/Assign CV   | IN        | Global assignable CV (see config)    | 0-5V                | E.g. swing, steps, skip, reset   |
| Play/Pause Trig   | IN        | Gate or trigger to start/stop        | 0-5V (min. 2V)      | Acts as button press             |
| Clock In          | IN        | External clock input                 | 0-5V (min. 2V)      | Needed for rhythms!              |
| Master Reset Trig | IN        | Gate/trigger resets all patterns     | 0-5V (min. 2V)      | Both jacks & button              |

---

## **TIPS**

- Knob values only "take over" after crossing the saved value when switching modes (“pick-up”).
- Manual swing is global, per-trigger/gate (delay every Nth clock depending on knob range).
- All CV inputs: 0-5V recommended, 0V = min, 5V = max.
- Save/load per-mode; configurations are remembered at power up/down.
- In algorithms where STEPS/FILLS are inactive, CV/knobs do nothing.

---

## **LINKS**
- [Official ADDAC402 Manual PDF](http://addacsystem.com/sites/default/files/files/ADDAC402_USER_GUIDE.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
```