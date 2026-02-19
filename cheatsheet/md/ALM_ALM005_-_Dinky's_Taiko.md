# ALM — ALM005 - Dinky's Taiko

- [Manual PDF](../../manuals/alm005-manual.pdf)

---

[Official ALM-005 ‘Dinky’s Taiko’ Manual PDF](https://busycircuits.com/docs/alm005-manual.pdf)

---

# ALM-005 ‘Dinky’s Taiko’ Cheat Sheet

## Overview
- 12-bit digital drum voice module with full voltage control (except EQ).
- Digital noise + wavetable oscillator (24 waveforms) + analog tilt EQ.
- Trigger, Accent, and Choke for expressive play.
- All major parameters (except EQ) are voltage controllable.

---

## PANEL REFERENCE

### Input Jacks
| Jack       | Function                         | Voltage Range         |
|------------|----------------------------------|----------------------|
| Trigger    | Main trigger (fires hit)         | ~+3V rising edge min |
| Acc        | Accent trigger (emphasizes hit)  | Trigger gate         |
| Choke      | Choke trigger (cuts hit short)   | Trigger gate         |
| Spectrum CV| Digital noise spectrum control   | 0V to +5V            |
| Noise Rel CV| Noise release time              | 0V to +5V            |
| Start Freq CV| Oscillator start freq          | 0V to +5V            |
| End Freq CV | Oscillator end freq             | 0V to +5V            |
| Speed CV   | Oscillator slew time             | 0V to +5V            |
| Osc Rel CV | Oscillator release time          | 0V to +5V            |
| Wave CV    | Oscillator waveform select       | 0V to +5V            |
| Mix CV     | Noise/Osc crossfade              | 0V to +5V            |

### Output Jack
| Jack   | Function               | Voltage Range      |
|--------|------------------------|-------------------|
| Out    | Main audio output      | +/- 10V (can be hot) |

---

## KNOB & CONTROL SUMMARY

| Control       | Section     | Function                                                                                                 | CV | Notes                    |
|---------------|-------------|----------------------------------------------------------------------------------------------------------|----|--------------------------|
| Spectrum      | Noise       | Digital noise frequency                                                                                  | ✔  | 0-5V                     |
| Noise Release | Noise       | Release time for noise envelope                                                                          | ✔  | 0-5V                     |
| Start Freq    | Oscillator  | Sets starting frequency of oscillator (not 1V/oct)                                                       | ✔  | 0-5V                     |
| End Freq      | Oscillator  | Ending frequency before reset                                                                            | ✔  | 0-5V                     |
| Speed         | Oscillator  | Sweep speed from start to end frequency. Higher = metallic/FM sounds                                     | ✔  | 0-5V                     |
| Osc Release   | Oscillator  | Release time for oscillator envelope                                                                     | ✔  | 0-5V                     |
| Wave          | Oscillator  | Selects one of 24 waveforms                                                                              | ✔  | 0-5V                     |
| Mix           | Output      | Crossfade Noise ↔ Oscillator on output                                                                   | ✔  | 0-5V; Osc only ≈ +10V out|
| EQ (Tilt)     | Output      | Tilt-style EQ: CCW = high freq emphasis, CW = low freq emphasis                                          | ✗  | Only manual, affects out |

---

## USAGE TIPS

- **All CV inputs are summed with the corresponding knob position as an offset.**
- **All parameters (except EQ) are “snapshotted” at the instant the TRIGGER is received.**
- **Accent and Choke are live while the hit is playing.**  
- **Trigger:** +3V (min) rising edge (standard modular trigger) required.  
- **Pairs especially well with clock/divider modules for rhythmic triggers and modulation.**

### Voice Structure:
1. Trigger input fires a hit (“drum”).
2. Digital noise and wavetable oscillator run through analog tilt EQ and crossfader (Mix).
3. All core sound design comes from tuning and/or modulating the Spectrum, Release, Speed, Freq, and Wave controls (with or without modulation).
4. All audio is output through a “hot” audio out (LED level indicator provided).

---

## QUICK PATCH EXAMPLES

- **Basic Hit:**  
  Patch clock or sequencer trigger to TRIGGER in. Audio from OUT to mixer.

- **Snare or Perc:**  
  Use mostly NOISE, shorter release times, tilt EQ towards high.  

- **Metallic/Funky:**  
  Raise Speed and modulate with CV for ring/FMX hits. Try out various waveshapes.

- **Dynamic Patterns:**  
  Use divided triggers or shifted clocks for ACCENT and CHOKE to create varied sequences.

---

## POWER & SIZE

- Power: +/-12V, ~80mA
- 12HP wide, 32mm deep (skiff friendly)
- Reverse polarity protection

---

### [Official Manual PDF](https://busycircuits.com/docs/alm005-manual.pdf)  
### [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)