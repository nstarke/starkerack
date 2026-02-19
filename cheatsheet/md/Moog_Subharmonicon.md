# Moog — Subharmonicon

- [Manual PDF](../../manuals/Subharmonicon_Manual.pdf)

---

[Moog Subharmonicon User Manual PDF](https://www.moogmusic.com/sites/default/files/2020-09/Subharmonicon-Manual-v1-Web.pdf)

# Moog Subharmonicon Eurorack Cheat Sheet

**Type:** Semi-modular analog polyrhythmic synthesizer (60HP Eurorack compatible)  
**Main Features:**  
- 2 VCOs (each with 2 subharmonics, 1-16 integer division undertones)  
- 4 Rhythm Generators (integer tempo divisions, create polyrhythms)  
- 2 x 4-step Analog Sequencers  
- Moog 4-pole Ladder Filter  
- Dual Envelope Generators (Attack/Decay, for VCF & VCA)  
- 32-point Patchbay (17 In, 15 Out)

---

## Quickstart
1. **Power:** +12V only, 360mA max (no -12V). See manual for safe installation.
2. **Audio Out:** 1/4" on the back, or `VCA OUT` on patchbay (Eurorack level, 10Vpp).
3. **Basic Flow:** Oscillators > Mixer > Filter > VCA > Audio Out.
4. **Rhythm Generators:** Divide master tempo by 1-16 (per generator), assign to sequencers for polyrhythms.
5. **Sequencers:** 4 steps per, pitch (and optionally integer division for subosc), assign to VCO, Sub 1, and/or Sub 2.
6. **Patchbay:** Use to break internal routing and integrate with external CV/midi/eurorack.

---

## Panel Controls

### Knobs
- **VCO FREQ (1 & 2):** Oscillator frequency, 4 octave range (Middle C to C6).
- **SUB FREQ (x4):** Division from 1-16 (clockwise = unison, counter = /16).
- **Waveform Select (toggle, x2):** Square / PWM + Sub Saw / Saw.
- **Mixer Levels:** VCO 1, SUB 1, SUB 2, VCO 2, SUB 1, SUB 2.
- **CUTOFF:** VCF Cutoff, 20Hz–20kHz.
- **RESONANCE:** Self-oscillate at max.
- **VOLUME:** Main output level.
- **VCF EG:** ATTACK (1ms–10s), DECAY (5ms–10s), AMT (bi-directional).
- **VCA EG:** ATTACK (1ms–10s), DECAY (5ms–10s).
- **TEMPO:** .333Hz–50Hz (20–3000 BPM).

### Buttons
- **SEQ n ASSIGN:** Assign step CV to VCO, Sub 1, and/or Sub 2.
- **Quantize:** 12-ET, 8-ET, 12-JI, 8-JI, OFF.
- **SEQ OCT:** ±1, ±2, ±5 step range.
- **PLAY:** Sequencers on/off.
- **RESET:** Resets sequencers/rhythm.
- **NEXT:** Advances step.
- **EG:** On/Off/Held (Hold to tune with EGs open).
- **TRIGGER:** Manual envelope retrigger.

### Rhythm Gen Section
- **RHYTHM (x4):** Integer clock divider [1–16].
- **SEQ 1 & SEQ 2 assign (x4):** Assign rhythm output to sequencers.

---

## Patchbay Reference

**Inputs** (Normal text):  
| Jack                | Function                          | Range        |
|---------------------|-----------------------------------|--------------|
| VCO 1 IN            | VCO 1 1V/Oct pitch CV             | -5V to +5V   |
| VCO 1 SUB IN        | CV choose Sub 1/2 divisor         | -5V to +5V   |
| VCO 1 PWM IN        | PWM Mod for VCO 1 & subs          | -5V to +5V   |
| VCA IN              | VCA CV (volume)                   | 0V to +8V    |
| VCO 2 IN            | VCO 2 1V/Oct pitch CV             | -5V to +5V   |
| VCO 2 SUB IN        | CV choose Sub 1/2 divisor         | -5V to +5V   |
| VCO 2 PWM IN        | PWM Mod for VCO 2 & subs          | -5V to +5V   |
| CUTOFF IN           | Filter cutoff modulation           | -5V to +5V   |
| PLAY IN             | Play/stop gate (rising/falling)    | 0V to +10V   |
| RESET IN            | Sequencer/rhythm reset/trig/hold   | 0V to +10V   |
| TRIGGER IN          | EG trig input                      | 0V to +10V   |
| RHYTHM 1–4 IN       | Integer value, Rhythm (centered)   | -5V to +5V   |
| MIDI IN             | Mini-jack, Type A                  | —            |
| CLOCK IN            | External clock override            | 0V to +10V   |

**Outputs** (Reverse text):  
| Jack                | Function                          | Range        |
|---------------------|-----------------------------------|--------------|
| VCA OUT             | Main Eurorack level audio out      | 10Vpp        |
| VCO 1 OUT           | VCO 1 audio/CV                    | 10Vpp        |
| VCO 1 SUB 1/2       | Sub oscillator outputs             | 10Vpp        |
| VCO 2 OUT           | VCO 2 audio/CV                    | 10Vpp        |
| VCO 2 SUB 1/2       | Sub oscillator outputs             | 10Vpp        |
| SEQ 1 OUT           | Seq 1 CV out (follows quantize)    | -5V to +5V   |
| SEQ 1 CLK OUT       | Seq 1 clock pulse                  | 0V to +5V    |
| SEQ 2 OUT           | Seq 2 CV out (follows quantize)    | -5V to +5V   |
| SEQ 2 CLK OUT       | Seq 2 clock pulse                  | 0V to +5V    |
| CLOCK OUT           | Master clock (all sources)         | 0V to +10V   |
| TRIGGER OUT         | EG trigger pulse                   | 0V to +5V    |
| VCA EG OUT          | VCA envelope CV                    | 0V to +8V    |
| VCF EG OUT          | VCF envelope CV                    | 0V to +8V    |

---

## Voltage Ranges

- **Pitch CV inputs (VCO 1/2 IN):** 1V/oct, -5V to +5V
- **PWM, Subharmonic, Rhythm inputs:** -5V to +5V
- **CUTOFF, VCA CV IN:** CUTOFF: -5V to +5V; VCA: 0V to +8V
- **Gate/Trigger/Reset:** 0V (low), +10V (high, trigger/gate)
- **Audio Outputs:** 10V peak-to-peak (Eurorack level)
- **Envelope Outputs (VCA/VCF EG):** 0V to +8V

---

## MIDI & Other Notes

- MIDI input via included Type A minijack adapter: clock, note, CC messages (see manual for full CC list).
- Supports just intonation and equal temperament quantization.
- All functions can be decoupled from quantization/seq octave settings for advanced patching.
- All internal routing can be overridden with patch cables.

---

## Links

- [Moog Subharmonicon Manual PDF](https://www.moogmusic.com/sites/default/files/2020-09/Subharmonicon-Manual-v1-Web.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)