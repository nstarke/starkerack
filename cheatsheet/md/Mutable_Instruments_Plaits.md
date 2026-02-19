# Mutable Instruments — Plaits

- [Manual PDF](../../manuals/Mutable Instruments - Plaits.pdf)

---

Certainly! Here’s a concise cheat sheet for the Mutable Instruments Plaits Eurorack module, ideal for quick reference and performance.  
**Note: This is based on the content above, not an official PDF. [Official Mutable Plaits manual PDF link](https://mutable-instruments.net/modules/plaits/manual/)**

---

# Mutable Instruments Plaits Cheat Sheet

### Power
- **-12V / +12V power supply**  
- 2x5 pin connector (make sure red stripe matches “Red stripe” mark)  
- **Current draw:** +12V: 50mA, -12V: 5mA

---

## Front Panel Controls

| Label | Control         | Description                                                                            |
|-------|----------------|----------------------------------------------------------------------------------------|
| A     | Model Buttons & LEDs | Select Synthesis Model (2 banks × 8 models; LEDs show selection)                |
| B     | FREQUENCY      | Coarse tuning (default: 8 oct, adjustable to 14 semitones via settings)               |
| C     | HARMONICS      | Model-dependent timbre (details vary)                                                 |
| D     | TIMBRE         | Model-dependent texture/detail control                                                |
| E     | MORPH          | Model-dependent adjustment (often morph/pulse width)                                  |
| F     | Attenuverters  | For TIMBRE, FM, MORPH CVs—set modulation depth; when unpatched, controls from env     |

---

## I/O Jacks Reference

| Jack          | Type        | Description & Range                                      |
|---------------|-------------|----------------------------------------------------------|
| MODEL CV      | Input       | Selects model. 0V to +5V (LEDs show current/CV)          |
| HARM, TIMBRE, MORPH, FREQ CV | Input  | Model parameter modulation, typically -5V to +5V, expect CV scaling varies by model    |
| TRIG          | Input       | Gate/trigger (> 1.5V = trigger) – excites, envelopes, etc|
| LEVEL         | Input       | VCA/LPG/Accent (audio-rate OK); ~0V (closed) to +5V (open)|
| V/OCT         | Input       | Pitch CV, -3V to +7V for C0–C8 (1V/octave standard)       |
| OUT           | Output      | Main audio output (10Vpp max typical, bipolar audio)      |
| AUX           | Output      | Variant/sidekick/byproduct audio (10Vpp max typical)      |

---

## Fast Usage Guide

1. **Patch Power & Audio**: Connect power as instructed. Patch OUT (and AUX if desired) to mixer/VCA.
2. **Model Selection**:  
   - Use upper/lower (A) buttons to select model/bank. LEDs will indicate which.  
   - Patch MODEL CV for voltage control (0–+5V). When triggered, only changes at next TRIG.
3. **Tuning**:  
   - Set FREQUENCY (B). For fine range (14 semitones), hold 2nd button (A) and turn HARMONICS.
4. **Sound Shaping**:  
   - HARMONICS / TIMBRE / MORPH knobs: Adjusted per model (see summary below).
   - Modulate parameters via their CV ins, depth set by attenuverters (F).
5. **Pitch CV**:  
   - Patch 1V/oct source to V/OCT.
6. **Percussive/LPG**:  
   - TRIG fires an internal decay envelope/excites models, unless LEVEL is patched (then, LEVEL acts as VCA/Accent).

---

## Settings (Hold Button A Combos)

- **Adjust LPG/Envelope**: Hold 1st button (A), turn TIMBRE (VCFA↔VCA response) or MORPH (LPG ring time/envelope decay).  
- **FREQ Knob Range**: Hold 2nd button (A), turn HARMONICS. 8 settings: C0±7st, ..., all LEDs = C0–C8 (8 octaves).
- **Any knob used for these settings is not 'live' on main function until matched with physical position.**

---

## Synthesis Models: Parameter Summary

| Model                      | HARMONICS           | TIMBRE            | MORPH                  | AUX                                  |
|----------------------------|---------------------|-------------------|------------------------|--------------------------------------|
| Virtual Analog             | Detuning            | Pulse shape       | Saw notch width        | Hardsync sum waveform                |
| Wavefolder                 | Waveshaper curve    | Fold amount       | Asymmetry              | Alt wavefolder shape (Warps style)   |
| FM Synthesis (2op)         | Ratio               | Mod. index        | Feedback/Chaos         | Suboscillator                        |
| Formants                   | F1/FM2 ratio        | Formant freq      | Formant width/shape    | Filtered waveform type (filter morph)|
| Additive                   | Spectral bumps      | Bump position     | Bump width/shape       | Hammond drawbars partials            |
| Wavetable                  | Bank (A-D)          | Row (brightness)  | Column (varied)        | 5-bit lo-fi output                   |
| Chords                     | Chord type          | Inversion/transp. | Waveform select        | Root note of chord                   |
| Speech                     | Vowel/Word crossfade| Species           | Phoneme/Word segment   | Pure vocal fold signal               |
| Granular Cloud (Swarm)     | Pitch randomization | Grain density     | Grain overlap/duration | Sine grain variant                   |
| Filtered Noise             | LP↔BP↔HP morph      | Clock freq        | Filter resonance       | Dual BP filter, separation = HARM    |
| Dust Noise                 | Freq randomization  | Density           | Allpass↔BP morph       | Raw dust noise                       |
| Inharmonic String/Resonator| Material/inhar.     | Brightness/density| Decay time             | Exciter only (mini-Rings)            |
| Kick Drum (Analog)         | Attack/OD           | Brightness        | Decay                  | FM triangle drum synth               |
| Snare Drum                 | Harm↔Noise balance  | Drum mode balance | Decay                  | FM + noise-based snare               |
| Hi-Hat (Analog)            | Metal↔Noise         | HPF cutoff        | Decay                  | Ring-mod metal + clean VCA           |

---

## Calibration & Firmware

- **Calibration**: Hold both buttons; see detailed steps above.
- **Update/Firmware**: Listen to firmware audio file at MODEL CV in, freq knob at noon.

---

## Troubleshooting Highlights

- **Settings lost?** Change model after tweaking to save.
- **Unexpected clicks?** Check Frequency knob range.
- **Trigger not working?** Recalibrate.
- **2 LEDs lit (1 blinking)?** MODEL CV is not at 0V (unpatched or power fault).

---

## Voltage Ranges

| Input         | Range/Trigger                                           |
|---------------|--------------------------------------------------------|
| MODEL CV      | 0–5V (mod selects from full model set)                 |
| HARM, TIMBRE, MORPH, FREQ CV | -5V to +5V typical, CV scaling varies   |
| TRIG          | >1.5V for trigger                                      |
| LEVEL         | 0–5V (acts as VCA; percussive accent if TRIG patched)  |
| V/OCT         | -3V to +7V (C0–C8, 1V/octave)                          |

Outputs are typical audio modular levels, ±5V (10Vpp), unipolar in models with percussive envelopes, per model.

---

## Reference Links

- [Official Plaits Manual PDF](https://mutable-instruments.net/modules/plaits/manual/)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
