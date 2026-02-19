# Toadstool Tech — Ectocore

- [Manual PDF](../../manuals/ectocore_quickstart.pdf)

---

[Download the Ectocore Manual PDF (image source)](https://cdn.discordapp.com/attachments/1041147095957966899/1248495278915553330/ectocore_quickstart.png)

---

# **Ectocore Cheat Sheet**

A reference and performance guide for the **Ectocore** eurorack sample FX sequencer by Toadstool Tech x infinitedigits.

---

## **Jacks: Input & Output Summary**

| Jack         | Type      | Voltage Range       | Function                                   |
| ------------ | --------- | ------------------ | ------------------------------------------ |
| **Output L** | Audio Out | Typical eurorack   | Main left audio output                     |
| **Output R** | Audio Out | Typical eurorack   | Main right audio output                    |
| **CV Inputs**| CV In     | 0V–5V †            | Modulates various parameters (see below)   |
| **Output**   | Trigger   | 0-5V (standard)    | Trig output (configurable trigger events)  |
| **Clk Out**  | Clock     | 0-5V (standard)    | Clock output                               |
| **Clk In**   | Clock In  | 0-5V (standard)    | External clock input                       |

† (unless otherwise specified)

---

## **Front Panel Controls**

### **Knobs**

| Control   | Function                                                                                      |
|-----------|----------------------------------------------------------------------------------------------|
| **Break** | Controls FX density. Up = more frequent FX, scoped to current Grimoire selection.            |
| **Grimoire** | Selects active FX group: each glyph determines which subset of the 16 FX can be active.     |
| **Sample** | Selects currently playing sample within the current bank. LED ring indicates selection.       |
| **Bank**   | Selects active sample bank (16 available). Hold **Bank + Sample** for quick bank select.      |
| **Amen**   | Controls random slice-looping (Turing machine-style). Left = sequential, right = max random. 1–16 steps; LED ring shows step count. Full right: new loop pattern per cycle w/ FX fill.  Reroll pattern by turning fully right then back.|
| **Amen Attenurandomizer** | Left = random chaos; right = predictable (closer to playhead). When CV is patched, attenuates/randomizes incoming CV signal. |

---

### **Buttons**

| Button                    | Function                                                                           |
|---------------------------|------------------------------------------------------------------------------------|
| **Tap Tempo**             | Set internal clock tempo (double-tap). When clocking externally, acts as reset. Also used as a shift function with other controls.          |
| **Clock Mult/Div**        | Tap to multiply (faster); hold to divide (slower) the clock.                        |

#### **Advanced / Combo Functions**
- **Tap + Break:** [Special function, not detailed in this image]
- **Tap + Amen:** [Special function, not detailed in this image]
- **Tap + Sample:** [Special function, not detailed in this image]

---

## **Other Features**

- **Trig Output Modes**: Cycle trigger behaviors via the Trigger Mode (details not described here — refer to full manual).
- **FX Types**: 16 total; grouped by Grimoire knob positions/glyphs. 
- **Sample Banks**: 16, each with multiple samples addressable via Sample knob.
- **LED Ring**: Displays sample selection and, for Amen, step count.

---

## **Typical Patch Example**

1. Patch **Audio Output L/R** to mixer/interface.
2. Send clock to **Clk In** _(0-5V Eurorack clock)_ or tap tempo.
3. Use **Grimoire** to choose FX group, **Break** to set FX density.
4. Select bank/sample; dial in **Amen**/**Amen Attenurandomizer** for looping effects and randomization.
5. Utilize **CV inputs** to modulate parameters for hands-off or sequenced variation.

---

## **Quick Reference Table**

| Function      | Where                            | Notes                                                        |
|---------------|----------------------------------|--------------------------------------------------------------|
| Audio Out     | Output L/R                       | Left/Right channel out                                       |
| CV Mod        | CV Inputs                        | See Amen Attenurandomizer for dynamic randomization          |
| Trig Out      | Output                           | Assignable via Trigger Mode                                  |
| Clock Out     | Clk Out                          | Pulse per beat/event                                         |
| Clock In      | Clk In                           | Accepts 0–5V clock, tap for manual tempo/reset               |
| FX Density    | Break knob                       | More = busier FX                                             |
| FX Group      | Grimoire knob                    | Glyph determines which FX subset is active                   |
| Sample #      | Sample knob + LED ring           | Instant selection                                            |
| Bank #        | Bank knob, hold w/Sample         | 16 total                                                     |
| Slices/Loops  | Amen knob                        | Turing loop control, LED ring = 1–16 steps                   |
| Randomness    | Amen Attenurandomizer + CV       | Chaotic left, tamer right, also attenuates CV input          |
| Clock Multi/Div| Clock Mult/Div button           | Tap for multiply, hold for divide                            |
| Combo Fn.     | Tap + (Break/Amen/Sample)        | See manual for “super cool” extras                           |

---

> For deeper dives (including CV routings, external sample management, and bonus functions) **consult the full PDF manual**.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
