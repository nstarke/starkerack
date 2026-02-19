# Tiptop Audio — MODFX FSU

- [Manual PDF](../../manuals/Tiptop_Audio_fx_manual_MODFX_FSU.pdf)

---

[**Official Manual PDF (Tiptop Audio ModFx & FSU):**](https://tiptopaudio.com/manuals/ModFX_FSU_Manual.pdf)

---

# Tiptop Audio ModFx & FSU — Cheat Sheet

ModFx and FSU are 8hp digital multi-effects modules for Eurorack. Each module features **3 major effect banks**, each with 8 programs, for deep but immediate modulation, filtering, chorus, distortion, glitching, and looper-style sound design.

---

## Panel & Controls Reference

### JACKS

| Jack           | Description                          | Type               | Voltage Range        |
|:--------------:|:-----------------------------------:|:------------------:|:--------------------:|
| **L IN**       | Left Audio Input                     | Audio Mono         | ±5V expected         |
| **R IN**       | Right Audio Input                    | Audio Mono         | ±5V expected         |
| **L (MONO) OUT**| Left / Mono Audio Output           | Audio Mono         | ±5V typical output   |
| **R OUT**      | Right Audio Output                   | Audio Mono         | ±5V typical output   |
| **CV 1**       | CV to first parameter (see below)    | CV Input           | 0–5V (unipolar), ±5V safe |
| **CV 2**       | CV to second parameter               | CV Input           | 0–5V (unipolar), ±5V safe |
| **CV 3**       | CV to third parameter                | CV Input           | 0–5V (unipolar), ±5V safe |
| **FIDELITY CV**| (Shared) Analog clocking (low-level control over DSP rate) | CV Input | 0–5V |

---

### MAIN CONTROLS

#### [BOTH MODULES — ModFX + FSU]

| Knob/Button         | Function                                                      | Voltage Control   |
|---------------------|--------------------------------------------------------------|-------------------|
| **Rate**            | Speed of LFO, modulation rate, playback speed, etc           | CV1               |
| **Filter/Fdback**   | Filter cutoff, feedback amount, tuning, or other function     | CV2               |
| **Depth**           | Depth of modulation, feedback, chorus range, etc             | CV3               |
| **Fidelity**        | DSP clock / LoFi effect / affects buffer length & character   | CV (label-specific)|
| **Mix**             | Dry/Wet balance (manual only)                                | –                 |
| **Bank Buttons (3)**| Select program banks (illuminated, labeled by mode)          | –                 |
| **Program Select**  | Push buttons to select one of 8 programs per bank            | –                 |

#### [FSU ONLY]

| Control (FSU)       | Function                                                      | Voltage Control   |
|---------------------|--------------------------------------------------------------|-------------------|
| **Gain**            | Output level (Distort bank), Record level (SOS bank)         | Replaces "Rate" in some modes |
| **Drive**           | Distortion/Input gain in Distort bank                        | (sometimes replaces "Depth")  |

#### [MODFX ONLY]

- **No unique extra controls** – all labeled as above according to effect.

---

## BANKS AND EFFECTS

### MODFX

- **Chorus**: 8 types (classic, ensemble, stereo, vibrato, random)
- **Flanger/Karplus**: stereo flange, tape/zero, Karplus-Strong, chord resonator, Haas panning
- **Filter/Phaser**: 12-stage phaser, bandpass LFO, tape/drive, tremolo pan, formant ping-pong, vowel/ahh

### FSU

- **Distort**: tape saturation, bit crusher, clipper, rectifier, ring mod, freq shift (mono/dual)
- **Glitch/Warp**: random pitch, glitch chorus, varispeed, granular, grains w/ feedback
- **Sound on Sound (Looper/Granular)**: dual head, dual pitch, chorus scrub, varispeed, panning, buffered degrade, frozen plate

**Each bank has 8 programs; see manual for full parameter assignment per effect.**

---

## VOLTAGE/CV INPUTS (per function)

| Parameter        | Typical CV Range | Effect (all banks/settings)                         |
|------------------|------------------|-----------------------------------------------------|
| Rate/Gain        | 0–5V unipolar    | LFO speed, playback speed, effect rate, gain input/output |
| Filter/Fdback    | 0–5V unipolar    | Filter cutoff, feedback amount, Q, feedback level   |
| Depth/Drive      | 0–5V unipolar    | Amount of modulation, distortion, detune, pitch     |
| Fidelity         | 0–5V unipolar    | Lowers clock for lo-fi, longer buffers on loopers   |

*CV inputs typically expect 0–5V; -5V to +5V is tolerated but may invert or fold control ranges at extremes.*

---

### BUTTONS (MODFX/FSU)

- **Bank Buttons**: Choose current effects bank ([Chorus/Flanger/Filter] or [Distort/Glitch/SOS]).  
- **Program/Select**: Illuminated selectors, change active program.
- **SOS Shift/Hold**: Hold to clear or reload SoS buffer (FSU only).

---

## USING THE MODULE

1. **Power Up and Patch Audio**:  
   - Patch L/R IN to your audio source and OUT to mixer/speakers.
2. **Bank & Program Select**:  
   - Use illuminated buttons to pick an effect bank, then select desired program.
3. **Adjust Main Controls**:  
   - Rate, Filter/Fb, Depth, Mix (and Fidelity) shape the effect (see per-effect mapping, many are intuitive).
4. **Patch CV for Modulation**:  
   - Send LFO, Envelope, Sequencer, etc. to any CV input to animate parameters in real time. 0–5V recommended.
5. **Experiment with Fidelity CV**:  
   - Lower audio fidelity for lo-fi, pitch, and buffer time changes.
6. **Set Mix**:  
   - For most Distort, Looper, Glitch programs, set to 100% wet. For Choruses/Flangers, try 50/50 or 100% wet.
7. **Monitor LEDs/Buttons**:  
   - Bank selection will be color/LED-indicated.

---

## QUICK TIPS

- **FSU Looper (SoS) buffer can clear**: Change preset for reset, or hold SoS button to clear in place.
- **Karplus/Flanger likes short, percussive inputs.**
- **Vowel and formant programs want harmonically rich sources (saw, square, etc).**
- **Fidelity knob or CV can radically transform the feel of most effects.**

---

### [Official Manual PDF](https://tiptopaudio.com/manuals/ModFX_FSU_Manual.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
