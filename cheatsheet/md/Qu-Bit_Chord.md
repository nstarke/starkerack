# Qu-Bit — Chord

- [Manual PDF](../../manuals/QB_Chord.pdf)

---

**[Chord v2 Manual PDF](https://qubitelectronix.com/manuals/Chord-V2-Manual.pdf)**

# Chord v2 Eurorack Module – Quick Cheat Sheet

A fast guide with references for all controls, inputs, and outputs, including essential tips and voltage ranges.

---

## Overview

- **Polyphonic oscillator:** 4 voices, various chord qualities, inversions, custom/user chords & wavetables.
- **Modes:** Chord (diatonic), Free Poly (independent), and Unison Poly.
- **Waveform sources:** 8 internal banks + user wavetable via SD card.
- **Voltage control:** All parameters via knob & -5V to +5V CV (unless noted).

---

## Front Panel Reference

| # | Label      | Type   | Description                                         | Voltage Range / Notes                |
|---|------------|--------|-----------------------------------------------------|--------------------------------------|
| 1 | frequency  | Knob   | Root note pitch (Coarse: 7 octaves / Fine: +/- P4)  | -                                    |
| 2 | bank       | Knob   | Select waveform bank                                | -5V to +5V CV                        |
| 3 | waveform   | Knob   | Select/blend waveform within bank                   | -5V to +5V CV                        |
| 4 | linear fm  | In + At.| FM input + attenuator                              | -                                    |
| 5 | voicing    | Knob   | Chord inversion/octave spacing                      | -5V to +5V CV                        |
| 6 | quality    | Knob   | Chord type (Maj, min, 7th, dim, sus etc)            | -5V to +5V CV                        |
| 7 | mode       | Btn+LED| Chord/Free Poly/Unison Poly/Melody (blue/green/teal)| (see Modes below)                    |
| 8 | harm       | Btn+LED| Auto-harm/Quantize major/minor/chromatic/off        | (blue/green/teal/off)                |
| 9 | triad      | Btn+LED| Mix out 7th omit/included                           | LED blue = 7th omitted               |
|10 | v/oct      | In     | 1V/oct input (root pitch)                           | 0V–5V                                |
|11 | lead       | In     | 1V/oct or independent voice (Mode-dependent)        | 0V–5V                                |
|12 | root       | Out    | Chord root audio out                                | Audio                                |
|13 | third      | Out    | Chord third audio out                               | Audio                                |
|14 | fifth      | Out    | Chord fifth audio out                               | Audio                                |
|15 | seventh    | Out    | Chord seventh audio out                             | Audio                                |
|16 | mix        | Out    | Summed audio (all, or omits 7th via triad button)   | Audio                                |

---

### Modes (Mode Button & LED)

- **Chord** *(LED off)*: Serial control, classic chord behavior.
- **Melody (LED blue):** 'lead' input controls an independent 7th melody.
- **Free Poly (LED green):** Each voice is fully independent, separate pitch input per voice.
- **Unison Poly (LED teal):** All oscillators tune together but have separate 1V/oct inputs for each voice.

---

### Auto-Harm/Quantize (Harm Button & LED)

- **Off:** No quantization.
- **Blue:** Major scale quantize.
- **Green:** Minor scale quantize.
- **Teal:** Chromatic quantize (Poly modes only).

---

### Creating & Saving User Chords

- **Access:** Hold *Harm* for 3s → Quality knob selects user chord.
- **Edit:** Hold *Harm*, press *Mode* (in user chord mode) → Adjust chord with knobs; Mode btn to save.
- **SD Chord File:** CHORD_#=x,y,z (semitone intervals for 3rd, 5th, 7th).

---

### User Wavetables

- **Load:** Hold *Mode* for 3s → switches factory/custom banks (SD card needed).
- **Format:** 32kB mono .wav (created in WaveEdit: 256 samples, 64 waves).

---

### Calibration

- Enter calibration: Hold Triad for 3s, follow LED/jack prompts (+1V/+3V for 1V/oct calibration steps).

---

## Reference Tables

### Voicings Table Highlights

- **17 Voicing positions** (various closed/dropped/raised/spread intervals, see appendix for all).

### Chord Qualities

- **Major 7:** 3rd: +4st, 5th: +7st, 7th: +11st
- **Minor 7:** 3rd: +3st, 5th: +7st, 7th: +10st
- **Dominant 7:** 3rd: +4st, 5th: +7st, 7th: +10st
- **Half Dim, Dim, Sus, Aug, etc...** (see manual)

---

## Typical Patches

- **Chord drone:** Just audio out from Mix—or all outputs multed!
- **Sequenced chords:** Use V/Oct input from sequencer/external controller.
- **Independent voices:** Use Free Poly mode and separate 1V/Oct inputs for each.
- **Melody over chord:** Melody mode, use Lead cv input for top voice.

---

### Tips

- All CV inputs: **Bipolar, -5V to +5V, summed with knob**
- Digital wave morphing: Smooth blending, CV or knob sweep.
- SD card slot: For custom chords, wavetables, and configuration.

---

**[Full Manual PDF Link](https://qubitelectronix.com/manuals/Chord-V2-Manual.pdf)**  
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)