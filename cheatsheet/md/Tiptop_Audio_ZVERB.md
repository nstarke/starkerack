# Tiptop Audio — ZVERB

- [Manual PDF](../../manuals/Tiptop_Audio_fx_manual.pdf)

---

[Tiptop Audio Z5000, ZVERB, ECHOZ User Manual PDF](https://tiptopaudio.com/manuals/Z5000.pdf)

---

# Tiptop Audio ECHOZ / ZVERB / Z5000 - CHEAT SHEET

## OVERVIEW
- **ECHOZ**: Stereo multi-FX module focused on delay echoes and tape/digital/flange/chorus effects.
- **ZVERB**: Features 24 reverb-based and combined effects, grouped into 70s/80s/90s banks.
- **Z5000**: General multi-effects—reverbs, delays, pitch/modulation, harmonizers.

---

## PANEL CONTROLS (ALL MODULES)

### BUTTONS
- **Left / Middle / Right Buttons:**  
  - Hold to load bank (3 banks of 8 programs = 24 FX).
  - Single press (in selected bank): Scroll through 8 effects.
  - Press inactive bank button to show current preset (in Default mode).

### KNOBS
- **TIME**  
  - Adjusts delay/reverb time, or LFO speed per program.
- **FILTER**  
  - Band/low/highpass filter cutoff, formant/vowel selection, or patch-specific function.
- **FEEDBACK / MOD**  
  - Controls delay feedback, depth/rate of modulation, or program-defined effect.
- **FIDELITY**  
  - Varies internal analog clock — affects DSP sample rate, introducing pitch shifting/lo-fi artifacts.
- **IN / MIX**  
  - Sets level or dry/wet mix.

### TOGGLE SWITCH (Z5000/ECHOZ/ZVERB)
- **Time / Fidelity CV Select:**  
  - Center CV jack routes to either Time **or** Fidelity (sample clock) control.

---

## JACKS

### INPUTS
- **IN** (1x 3.5mm mono, normalized to stereo):  
  - Audio input

- **CV INPUTS** (3x 3.5mm)
  - **Feedback/Mod (Left):** 0–5V (controls Feedback/Mod knob parameter)
  - **Time/Fidelity (Center):** 0–5V or ±2.5V (depending on toggle position; controls Time or Fidelity knob parameter)
  - **Filter (Right):** 0–5V (controls Filter knob parameter)
  - *NOTE:* DSP CVs are internally slewed (for smooth modulation); Fidelity CV is fully analog, allows fast/audio-rate modulation.

### OUTPUTS
- **L / R** (2x 3.5mm):  
  - Stereo audio output

---

## STATUS INDICATORS
- **Clipping Light:**  
  - Monitors input/output clipping (reduce IN or Feedback to eliminate clipping).
- **Bank/Program LEDs:**  
  - Indicates FX/bank selection (see module-specific chart).

---

## QUICK START
1. **Set Fidelity to max (full CW).**
2. **Connect audio to IN and both L/R outputs.**
3. **Set IN, MIX, TIME, FILTER, FEEDBACK/MOD to center.**
4. **Hold a bank button to select desired FX bank.**
5. **Press bank button to scroll through 8 FX programs within bank.**
6. **Fine-tune with knobs, CV, and switch.**

---

## VOLTAGE RANGES & SIGNAL LEVELS
- **CV Inputs:** 0–5V (Fidelity CV up to ±2.5V)
- **Audio Input:** Max 12V p-p before clipping
- **Audio Output:** Max 10V p-p before clipping
- **Output Level:** Line or Eurorack—adjusted automatically by IN knob (exponential response)
---

## DISPLAY MODES  
- **Default:** Display program LED code when changing programs; remembers last program in each bank.
- **Minimal:** LED only shows program #8 as red, banks always reset to program 1 on change.  
  - **To switch modes:**  
    - Hold **Center** button on power-up = Minimal  
    - Hold **Right** button on power-up = Default  
  - Mode is saved in memory.

---

## PROGRAM BANKS/FX SUMMARY  
(See manual pages 13, 24, 36 for full color-coded effect charts!)

#### Z5000:  
- **Reverbs**: Hall, Plate, 80's Verb, Gate, Room, Void, Delay>Hall, Shimmer.
- **Delays**: Mono/Ping Pong Digital/Tape, Tape Multi-head, Band Delays, Tape Chorus, Warp Pong.
- **Pitch/Mod**: Stereo Chorus/Flanger, Vintage/Ahhhnsemble, Formant Delay, Microshift, Interval, Detuned Taps.

#### ECHOZ:  
- **Tape Echo**: Mono, Ping Pong, 3-Head Mixed/Switch, Chorus, Diffuse, Wobbly, Warp Pong.
- **Digital Delay**: Mono, Ping Pong, BBD, Formant, Tapped, Bandpass, Diffuse, Multi-tap.
- **Pitch**: Mono Pitch, Interval, Chord, Interval FB, Microshift, Shimmer Taps, Pitch Band, Detuned Taps.

#### ZVERB:  
- **70s**: Hall, Plate, Bright Plate, Tape>Plate, Earliest Verb, Space Station, Exhibit A, Epic Mod Hall.
- **80s**: BarrVerb, Ambience, Gated, Delay>Hall, Shimmer up/down/adj, Blooming, Pitch>Plate.
- **90s**: Room, Void, Downward Spiral, Random Hall, Pong Verb, ChordHall, Pitch>Chorus, Formant Verb.

---

## POWER SPECIFICATIONS
- **Width:** 8HP  
- **Depth:** 40mm  
- **Power:**
  - +12V 130mA (black), 100mA (white)
  - –12V 20mA

---

## TIPS
- **Fidelity CV acts on entire DSP rate/structure—expect global pitch/time/texture changes.**
- **DSP can crash from extreme negative CV on Fidelity—cycle presets to recover.**
- **No external clock sync for delay times.**
- **Last-used program recalled on power-up (Default mode); always program 1 (Minimal mode).**

---

[Manual PDF](https://tiptopaudio.com/manuals/Z5000.pdf)  
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)