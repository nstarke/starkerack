# ADDAC Systems — ADDAC-207 Quantizer

- [Manual PDF](../../manuals/ADDAC_207_Quantizer_REV05.pdf)

---

[ADDAC207 INTUITIVE QUANTIZER User's Guide (PDF)](https://www.addacsystem.com/Manuals/ADDAC207_MANUAL.pdf)

---

# ADDAC207 Intuitive Quantizer – Creative Modulation Tips

The ADDAC207 Intuitive Quantizer is a highly flexible quad quantizer with user-definable scales, microtonal options, assignable CV functions, independent voice fine-tuning, chord generation, scale transposition, and more. Understanding its functions opens a great deal of sonic territory for modular musicians wanting to create **distorted percussion**, **crazy dubstep/drum'n'bass basses**, and **haunting atmospheric pads**. Below are patching and modulation ideas targeted at these sound design goals.

---

## 1. Distorted Percussive Sounds

**Strategy:** Use sharp, fast random or rhythmic voltage bursts to rapidly jump between quantized notes/scales with tight gate lengths and unusual scales/intervals.

### Patch Tips & Techniques

- **Short Gate Modulation:**  
  Set very short gate lengths in the GATE L. menu (Button 6 → Button 1–3: 10–40ms) for punchy, clicky outputs.
- **Rhythmic/Random Triggers:**  
  Patch clock dividers, random gates, or burst generators into the GATE IN jacks for on-the-fly rhythmic quantization changes.
- **Microtonal Scales:**  
  Enter the FINE TUNE menu (Button 10 → Buttons 11/12 to alter 1v/oct response) and reduce it to get 24 or even 48 notes per octave—making alien, metallic percussion.
- **Scale/Note Mutation:**  
  Permanently modulate scale selection on the fly by using the CV ASSIGN input to change presets, scale transpose (Button 12, 11), or quantization type (Button 5).  
  Try stepping through scales every trigger to create machine-gun style melodic drum patterns.
- **Chord Percussion:**  
  Set output intervals in NOTE 2, 3, 4 menus for stacks of intervals. Use these with a fast envelope or VCA for dissonant, metallic percussion stabs.

**Example Chain:**
```
Clock/Random Gate Out → 207 GATE IN  
Random/CV Burst → 207 CV IN  
207 OUT → VCO pitch  
207 GATE OUT → VCA envelope  
Modulate Assign with LFO/S&H → change preset/scale/chord intervals on the fly
```

---

## 2. Crazy Dubstep/Drum & Bass Basslines

**Strategy:** Use rapidly shifting quantizer intervals, scale transpositions, and extreme glide for unpredictable, modulating bass riffs.

### Patch Tips & Techniques

- **Note/Interval Modulation:**  
  Assign CV to NOTE 2-4 or SCALE TRANSPOSE. Sequence or randomize which notes/offests are active for each trigger. This makes FM/AM-like pitch jumps and "wobbles."
- **Glitchy Quantization Modes:**  
  Change Quantizer Type (Above/Below/Ignore) dynamically via Assign CV (Button 5 assignment). This creates note stutters and sharp pitch artifacts as the quantizer input swings around.
- **Dirty Chords:**  
  Use chords with non-diatonic intervals (e.g., up 1, 3, 7 or microtonal steps) and modulate these intervals while clocking the quantizer fast for cascading, digital-sounding basses.
- **Extreme Octave Offsets:**  
  Patch LFOs/noise to the Assign CV input, mapped to Octave Offset (Button 9), causing bass notes to jump several octaves within a scale/arpeggio.
- **Scale Transpose Basslines:**  
  Use another sequencer or envelope to modulate the Scale Transpose input (Button 11), moving your whole bassline to different "keys" with every phrase for broken, gliding riffs.

**Example Chain:**
```
Step Sequencer → 207 CV IN  
Envelope/LFO → Assign 1V/Oct In (scale transpose)  
Noise/Random CV → Assign (Quantizer Type or Octave Offset)  
207 OUT → VCO (preferably with some wavefolding/distortion)  
207 GATE OUT → Snap Envelope for VCA
```

---

## 3. Haunting Atmospheric Pads

**Strategy:** Use the quantizer for drifting, generative melodies within haunting scales, microtonal textures, and subtle chord shifts.

### Patch Tips & Techniques

- **Just/Bohlen-Pierce Temperament:**  
  Enter the TUNING menu (Button 10) and select nonstandard scale temperament (Buttons 5–9, especially 7 or 8) for scales with unfamiliar interval relationships.
- **Slow, Random Modulation:**  
  Feed slow, smooth random voltages (e.g., Wogglebug, S&H + Lag, or generative fluctuation sources) to the CV INs and Assign CV for drifting pad movement.
- **Real-Time Scale Change:**  
  Use Assign to alternate between major/minor or even modulate between user-defined scales by changing presets live (Button 12 assignment).
- **Large Chord Voicings:**  
  Use Voices 2–4 set at distant intervals (e.g., 5th, 9th, 11th), all set to long Attack/Release envelopes.  
  Quantize multiple slow LFOs for multiple melodic pad layers.
- **Microtonal Washes:**  
  Fine-tune 1v/oct ratios for "out-of-tune" cluster chords: select extreme FINE TUNE values for each output, then slowly sweep inputs for amorphous, evolving atmospheres.

**Example Chain:**
```
Slow/Smoothed Random CV → 207 INs 1–4  
Slow LFO/Random → Assign (scale transpose, preset change, etc.)  
Set Tuning = Just or Bohlen-Pierce  
207 OUTs → VCOs → Reverb/Delay feedback chain  
207 GATE OUTs → Slow envelope/VCA
```

---

## Bonus Modulation Ideas

- **CV-Controlled Assign Routing:**  
  The Assign function allows for mapping an incoming CV to multiple parameters at once: chord intervals, quantization mode, gate length, octave offset, etc.  
  Experiment with multed LFOs, envelopes, or chaotic sources sent to Assign to create unpredictable, "living" modulation.
- **Gate Out Length for Texture:**  
  Use varying GATE L. settings on different voices for overlapping textures or staggered percussive pulses.
- **Nonvolatile Presets for Live Play:**  
  Quickly swap between user presets containing wildly different scales/intervals to morph moods/scenes.

---

For complete reference and more details, check the full [ADDAC207 Intuitive Quantizer User's Guide (PDF)](https://www.addacsystem.com/Manuals/ADDAC207_MANUAL.pdf).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
