# Tubbutec — 6m0d6

- [Manual PDF](../../manuals/6m0d6-User-Manual-1.0.pdf)

---

Certainly! Here’s a concise **cheat sheet** for the **LPZW & Tubbutec 6m0d6 Eurorack Drum Module** based on the manual you provided. This guide covers essential usage, controls, inputs/outputs, and voltage ranges.

---
## [6m0d6 User Manual (Official PDF)](https://tubbutec.de/files/6m0d6_Manual.pdf)

# 6m0d6 Quick Reference Cheat Sheet

### Overview
- 7 Analog Drum Voices: Bass Drum, Snare Drum, Low Tom, High Tom, Cymbal, Open Hihat, Closed Hihat
- Enhanced parameter set for each drum (beyond classic TR-606)
- **CV + MIDI control, Dynamic triggers**
- Individual outs and mix out

---
## **Inputs and Outputs**

### Instrument Triggers
- **7 x Trigger Inputs** (BD, SD, LT, HT, CY, OH, CH)  
  - **Voltage:** 1V to 15V  
  - Trigger > 1V = fire drum
  - Individual instrument can be patched or normalized from LINK/MIDI

### Accent Section
- **Accent Amount (AC.AMT)**  
  - **CV input:** 0V to 5V (acts as gain/attenuator for instrument when accent ON)
- **Accent Gate**  
  - **Gate input:** On/Off (normalised to ON, can be set to OFF via config)
- **Accent Amount Knob**  
  - Manual accent/gain control if jack unpatched

### Decay CV Inputs
- **SN.Dec, CY.Dec, HH.Dec**  
  - CV decay control for Snare, Cymbal, and Hihats  
  - **Bipolar:** -5V to +5V

### Noise / Metal Modulation
- **Noise Tune CV**: (controls lofi/bit-crush character or noise tuning)
- **Metal Tune CV**: (1V/oct compatible, plays metal layer chromatically)
- **Metal Spread CV**: +/-5V (detune spread between the 6 oscillators)

### LINK Input
- **Tubbutec 6equencer** connectivity for direct triggering & accenting via back panel LINK

### MIDI IN
- **TRS MIDI A & B** (autodetect)
- Drum triggers on Channel 10 (see mapping table)
- Accent: Velocity 127 or note 34/A#1 held
- Velocity < 64: shorter pulse (lower volume), more dynamic
- Can play "metal" voice as 6-voice synth via Channel 1

### Outputs
- **7 x Individual Outs**: (BD, SD, LT, HT, CY, OH, CH)
  - Patch cable here removes drum from Mix Out
- **1 x Mix Out**: summed signal of all drums not patched individually

---

## **Front Panel Controls**

### Global / Shared
- **Accent Amount Pot**
- **Accent Gate Jack**
- **Accent CV Jack**
- **Mixer Out**
- **CY.Pulse Button**: Toggles cymbal pulse shaping / enters config menu (hold 3+ sec)

### Instrument Parameters *(per drum, varies by voice)*
- **Tune** (BD, SD, LT, HT, CY)
- **Tone/Body** (BD, CY)
- **Decay** (BD, SD, LT, HT, CY, OH, CH)
- **Click** (BD)
- **Snappy** (SD)
- **Noise Source** *(Switch: Noise, Metal, XOR)* (SD, CY, HH)
- **Metal Tune, Metal Spread** (CY, HH)
- **Pulse Shape Select (CY/Pulse Button)** - disables pulse shaping for CY to allow "drone/string" sounds

### Hihat & Cymbal Specials
- **Swap**: Inverts Open/Closed hihat order
- **OH.Decay, CH.Decay**
- **CY.Pulse**: enables/disables trigger length gating

### Tom Specials
- **HT Tune, LT Tune**
- **Sub Tom**: drops LT by 1 octave (toggle)
- **Noise Amt**: alters reverb (noise-based)

---

## **Config Menu**
- Enter: Hold `CY.Pulse` button 3 seconds
- Accent Gate Normalization: Use `M.Tune knob` (left=OFF, right=ON)
- Exit: Press `CY.Pulse` again (config saved)

---

## **MIDI Trigger Reference**

| Drum           | MIDI Note | Voice |
|----------------|-----------|-------|
| Bass Drum      | 35 (B0)   | BD    |
| Snare          | 38 (D1)   | SD    |
| Low Tom        | 45 (A1)   | LT    |
| High Tom       | 50 (D2)   | HT    |
| Cymbal         | 49 (C#2)  | CY    |
| Open Hihat     | 46 (A#1)  | OH    |
| Closed Hihat   | 42 (F#1)  | CH    |
- **Accent:** Note 34 (A#1) or velocity 127

*Metal Synthesis: MIDI Channel 1, play up to 6-note chords on CY/HH/SD metal source*

---

## **Voltage Ranges Recap**
- All CV & modulation inputs: -5V to +5V (survives up to +/-12V)
- Trigger/Accent Inputs: 1V to 15V
- Accent Amount: 0V–5V
- Metal Tune: 1V/oct compatible

---

## **Quick Tips**
- CV all "tune/decay/spread" parameters for evolving, expressive rhythms
- Plug individual outputs to isolate sounds; unplug for MIX OUT
- MIDI for deep, velocity-sensitive control; external CC for parameter automation
- Use Metal and XOR noise sources for highly experimental timbres
- Hold CY.Pulse for config, adjust M.Tune knob for Accent Gate norm
- Play chords on MIDI Ch.1 for metallic 6-voice pseudo-synth sounds

---

**Full Manual & More:**  
[Read the official PDF manual (tubbutec.de)](https://tubbutec.de/files/6m0d6_Manual.pdf)

---
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
