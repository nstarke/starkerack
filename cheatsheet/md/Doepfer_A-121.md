# Doepfer — A-121

- [Manual PDF](../../manuals/A121_man.pdf)

---

[Doepfer A-121 VCF2 System A-100 Manual PDF](http://www.doepfer.de/a100man/a121_man.pdf)

---

# Doepfer A-121 VCF2 (System A-100) Cheat Sheet

**Type:** Analog Voltage Controlled Multimode Filter  
**Slope:** -12 dB/octave  
**Modes:** Simultaneous LP, BP, HP, NOTCH outputs

---

## PANEL OVERVIEW

### CONTROLS / KNOBS

| Label        | Function                                                      |
| ------------ | ------------------------------------------------------------ |
| **Audio Level** | Attenuator for input audio signal. Reduce if output distorts.      |
| **Freq.**        | Manual cut-off frequency control.                             |
| **FCV 2**        | Attenuates CV input to cut-off frequency at FCV 2 jack.         |
| **Res.**         | Manual resonance (Q/emphasis) control (self-oscillation when near max).|
| **QCV 2**        | Attenuates CV input to resonance at QCV 2 jack.                |

---

### INPUTS & OUTPUTS

| Jack Label | Type        | Function                                                                                   | CV Range         |
| ---------- | ----------- | ----------------------------------------------------------------------------------------- | ---------------- |
| **Audio In (!)**  | Audio In    | Main audio input. Patch VCO/Noise/Mixer here.                                        | Audio (-5V/+5V typical) |
| **FCV 1 (")**     | CV In       | Cut-off frequency CV input. 1V/oct scaling. Patch keyboard CV, LFO, ADSR, etc.      | 0-10V            |
| **FCV 2 (§)**     | CV In       | Second cut-off frequency CV input via attenuator 3.                                 | 0-10V            |
| **QCV 1 ($)**     | CV In       | Resonance (Q) CV input. 1V/oct scaling. Patch LFO/Envelope etc.                     | 0-10V            |
| **QCV 2 (%)**     | CV In       | Second resonance CV input via attenuator 5.                                         | 0-10V            |
| **Low (&)**       | Audio Out   | Low-pass output (frequencies below cutoff pass).                                   | Audio            |
| **Band (/)**      | Audio Out   | Band-pass output (only a narrow band around cutoff passes).                         | Audio            |
| **High (()**      | Audio Out   | High-pass output (frequencies above cutoff pass).                                   | Audio            |
| **Notch ())**     | Audio Out   | Notch (band-reject) output (all but a narrow band passes).                          | Audio            |

---

## QUICK REFERENCE

- **Cut-off Frequency (Freq.)** shifts filter point for all modes.  
  - CV inputs (FCV 1, FCV 2) can be summed; FCV 2 is attenuated with knob 3.  
  - FCV 1 is calibrated 1V/oct for filter tracking or as a sine oscillator.

- **Resonance (Res.)** accentuates frequencies at the cutoff point; high resonance leads to self-oscillation (sine wave output).  
  - Resonance CV via QCV 1 (full-scale) and QCV 2 (attenuated by knob 5).

- **Output Jacks**: All filter ’modes‘ (LP, BP, HP, Notch) are available simultaneously.

---

## PATCH IDEAS

- **LFO to FCV 1:** Auto-wah/flanging effects.
- **Envelope to FCV inputs:** Classic subtractive synth sweeps.
- **Use as Sine Oscillator:** Max-out resonance; 1V/oct CV to FCV 1.
- **Quadraphonic/Spatial Processing:** Route each mode output to different speakers for spatial spectrum manipulation.

---

## VOLTAGE CONTROL SUMMARY

| Parameter         | Manual Control | CV Control (input jacks)                  | Range                |
|-------------------| --------------|-------------------------------------------|----------------------|
| Cutoff Frequency  | Freq.         | FCV 1 (1V/oct), FCV 2 (w/ attenuator 3)   | 0–10V (typ), audio-rate possible |
| Resonance         | Res.          | QCV 1 (1V/oct), QCV 2 (w/ attenuator 5)   | 0–10V (typ), up to self-osc.    |

---

## TIPS

- If output is distorted, reduce Audio Level.
- Max resonance + high cutoff = sine oscillator mode (frequency may drop slightly at extreme settings; a characteristic of CEM3320 chip).
- All outputs are active at all times: patch for creative mixes.
- Patch **slew limiter** to VCO pitch CV for portamento (vocal patches).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)