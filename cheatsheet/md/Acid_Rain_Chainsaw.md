# Acid Rain — Chainsaw

- [Manual PDF](../../manuals/Chainsaw_Manual_1.1.pdf)

---

[**Chainsaw Stereo Super-Oscillator Manual (PDF)**](https://www.acidraintechnology.com/chainsaw)

---

# Acid Rain Technology Chainsaw (Eurorack Cheat Sheet)

## Description
**Chainsaw** is a 3-voice, 7-oscillator-per-voice digital oscillator focused on "super-saw" and "super-square" sounds, providing wide stereo imaging and extensive polyphonic possibilities.

---

## FRONT PANEL OVERVIEW

| Ref. | Control/Input/Output | Function | Voltage Range |
|------|----------------------|----------|---------------|
| 1    | Encoder (push/turn)  | Root pitch (semitones) / Fine tune (cents) / Reset to C1 | N/A           |
| 2    | note LED             | Indicates root pitch mode | N/A           |
| 3    | alt LED              | Indicates fine tune mode | N/A           |
| 4    | Detune knob          | Detunes 7 waves per voice | N/A           |
| 5    | Wave morph knob      | Morphs saw→square for all waves | N/A  |
| 6    | CV in: Detune        | CV control of detune      | -5V to +5V    |
| 7    | CV in: Wave Morph    | CV control of wave morph  | -5V to +5V    |
| 8    | CV in: 1V/Oct Voice 1| 1V/Oct pitch for Voice 1  | 0V (C0)–10V+  |
| 9    | CV in: Linear FM     | Linear FM for all voices  | -5V to +5V (waves up to 2kHz) |
| 10   | CV in: 1V/Oct Voice 2| 1V/Oct pitch for Voice 2  | 0V (C0)–10V+  |
| 11   | Audio Out: L (Mono)  | Left output or mono out   | N/A           |
| 12   | CV in: 1V/Oct Voice 3| 1V/Oct pitch for Voice 3  | 0V (C0)–10V+  |
| 13   | Audio Out: R         | Right output (for stereo) | N/A           |

---

## QUICK-START CHEAT SHEET

### Basic Use
1. **Patch outputs:** Use OUT L (11) for mono, or OUT L (11) + OUT R (13) for full stereo super-saw/super-square sound.
2. **Pitch control:** Use encoder (1) to set the root note (1 semitone/step while "note" (2) LED is ON).
    - **Push encoder** to toggle to fine tune (1 cent/step, "alt" (3) LED ON).
    - **Long press (2 sec)** to reset to C1 (32.7 Hz).
3. **Pitch Inputs:** Patch 1V/Oct CV to Voice 1 (8), 2 (10), and/or 3 (12) for up to 3-voice polyphony (individual pitch per voice).
4. **Detune:** Adjust Detune knob (4) to spread the stacked waves for each voice. Use Detune CV (6) for voltage control (additive, -5V to +5V).
5. **Morph:** Adjust Morph knob (5) to sweep all oscillators from pure super-saw (ccw) to super-square (cw). Use Morph CV (7) for voltage control (additive, -5V to +5V).
6. **FM:** Patch linear frequency modulation CV to FM input (9), responds predictably up to 2kHz (use bipolar -5V to +5V LFOs, envelopes, etc. for FM).

---

## INPUTS SUMMARY

- **V/O 1 (8):** 1V/Oct pitch control, activates Voice 1; precision-tracked.
- **V/O 2 (10):** 1V/Oct pitch control, activates Voice 2.
- **V/O 3 (12):** 1V/Oct pitch control, activates Voice 3.
- **Detune CV (6):** Controls wave detune, -5V to +5V range.
- **Morph CV (7):** Controls waveshape morph, -5V to +5V range.
- **FM (9):** Linear frequency modulation, -5V to +5V (suitable up to 2kHz).

## OUTPUTS SUMMARY

- **OUT L (11):** Left/Mono audio output (all 21 voices spread spatially).
- **OUT R (13):** Right stereo output for spatial effect (use with OUT L for full stereo image).

---

## POWER REQUIREMENTS

- **+12V:** 110mA
- **-12V:** 10mA
- **Ribbon Orientation:** Red stripe = -12V
- **Width/Depth:** 4 HP / 35mm
- **Reverse Power Protection:** Yes

---

## REMINDERS

- Use with +12V/-12V regulated Eurorack power supply (2x5 ribbon, red stripe = -12V).
- Outputs are line-level modular audio signals.
- Manual morph and detune controls can be automated with CV (modulation sources: LFOs, envelopes, sequencers, etc.).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)