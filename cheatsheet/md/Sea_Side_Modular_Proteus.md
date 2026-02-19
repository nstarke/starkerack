# Sea Side Modular — Proteus

- [Manual PDF](../../manuals/ProteusManual.pdf)

---

[Proteus Manual PDF](attachment://proteus_manual.pdf)

---

# Proteus Eurorack Cheat Sheet

## Quick Start

1. **Power On**: Connect power, shrouded header (-12V labeled), reverse polarity protected.
2. **Patch Setup**:  
   - **Clock input** → GATE IN  
   - **GATE OUT** → Envelope/voice  
   - **V/OCT OUT** → Oscillator pitch input
3. **Knob Suggestions** (for musical/generative patch):  
   - **SCALE**: Pick a scale  
   - **LENGTH**: 8 steps  
   - **DENSITY**: As desired  
   - **PATIENCE**: Noon  
   - **OCTAVE, MUTATE, SLEEP**: Fully CCW  
   - **COMPLEXITY**: Fully CW  
   - **LOCK TOGGLE**: Up (melody locked)  
   - **NEW button** = Generate new melody

---

### **Panel Controls**

#### **Knobs**
- **LENGTH**: Sequence steps (2–32). (CV: -5V to +5V)
- **DENSITY**: % of active notes (rests vs notes). (CV: -5V to +5V)
- **SLEEP**: Beats to rest before repeating sequence. (CV: -5V to +5V)
- **PATIENCE**: How quickly randomizes, CCW=impatient, CW=infinite. (CV: -5V to +5V)
- **OCTAVE**: Octave transposition probability. (CV: -5V to +5V)
- **MUTATE**: Probability of single note mutation. (CV: -5V to +5V)
- **COMPLEXITY**: Affects new melody complexity (CCW=simple, CW=complex). (CV: -5V to +5V)
- **SCALE**: Selects scale (not voltage controlled)

#### **Toggles / Switches**
- **LOCK TOGGLE** (Melody Lock):  
  - Up: Melody locked, no changes/transpose/mutate  
  - Down: Melody evolves according to settings
- **MODE SWITCH**:  
  - Down: Regular operation  
  - Up: Settings mode (silver labels apply)

#### **Buttons**
- **NEW (center)**: Generate new melody
- **Pattern Bank (1–4)**: Save/load/erase melodies
- **Option buttons** (Settings Mode):  
  1. Vary Gates with Rests  
  2. Add Slew to notes  
  3. Preserve Melody Parameters  
  4. Quantize Notes (for TRANSPOSE input)

---

### **CV/IO Reference**

#### **Inputs**
- **GATE IN**: Clock input (advances sequence)
- **NEW (jack)**: Trigger = generate new melody
- **NEXT**: Trigger = load next pattern bank slot
- **TRANSPOSE**: v/oct input; added to melody (typically 1V/oct expected, -5V to +5V range for full sum), quantization optional.
- **CV Inputs**: All knobs except SCALE have CV in (-5V to +5V, summed with knob value).

#### **Outputs**
- **V/OCT OUT**: Pitch CV output.  
  - Default range: 1.0V–4.0V (base C3=2.0V, customizable), unipolar.
- **GATE OUT**: Step gate output.

---

## Sequence Memory / Pattern Bank

- **4 Pattern slots**: Save (press unlit), Load (press lit), Clear (long press lit)
- **Autopersist**: Pattern saved to memory on clock stop, can change persistence in config
- **Cycle Patterns**: Send trigger to NEXT

---

## Tips/Notes

- **Knob Lock Behavior**: After mode switch or save/load, knobs “lock” until turned back to original value
- **Settings Mode**: Access alternate knob functions (Gate length, Slew, LED brightness, Rotate, etc.)
- **Custom Scales**: Up to 6 slots, set via `proteus_config.json` on USB drive ([customize here](https://seaside.digital/proteusconfig/))
- **Firmware Update**: Place `.bin` on USB, reboot; recalibrate (see manual) if prompted.
- **Calibration**: Required if pitch is off or transpose is inaccurate (see manual page 22).

---

### **Color Legend**
| Color   | Meaning                                       |
|---------|-----------------------------------------------|
| Off     | Step not played (rest)                        |
| Blue    | Active step                                   |
| Green   | First step of sequence                        |
| Orange  | Sleeping (rest cycle)                         |
| Yellow  | Octave transpose (first step)                 |
| Pink    | Step mutated                                  |
| Teal    | Slewed note                                   |
| Purple  | Locked parameters overlap (knob unlocking)    |

---

## *Useful Links*

- [Full Manual PDF](attachment://proteus_manual.pdf)
- [Proteus Configurator](https://seaside.digital/proteusconfig/)
- [Official Discord Support](https://discord.gg/pNR2ZPgWgq)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)