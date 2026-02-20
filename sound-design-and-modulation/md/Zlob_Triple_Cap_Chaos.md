# Zlob — Triple Cap Chaos

- [Manual PDF](../../manuals/Zlob Modular - Triple Cap Chaos.pdf)

---

[Triple Cap Chaos Manual PDF (Build Docs / BOM Info / Videos)](https://zlobmodular.com/product/triplecapchaos/)

---

# Modulation Tips for Zlob Modular Triple Cap Chaos  
## For Distorted Percussion, Crazy Basslines, and Atmospheric Pads

The **Zlob Modular Triple Cap Chaos** (C³ Chaos) is a 2hp Eurorack module that acts as a chaotic analog oscillator, audio mangler, and pseudo ring modulator. Its unique chaotic core allows for rich, unpredictable behaviors that are perfect for experimental textures, aggressive timbres, and evolving soundscapes.

Below are modulation strategies tailored for the sound design themes you mentioned, using information directly from the manual and feature set (CV, IN, emanate/width knobs, X and Y outs):

---

## GENERAL MODULATION STRATEGY

- **Two Main Controls**:  
  - *Emanate*: Coarse chaos control — more CCW = busier, noisier; CW = more stable, closer to steady oscillation.
  - *Width / CV Attenuator*: Fine chaos control or acts as an attenuator for *CV* input.

- **CV Input**:  
  - Breaking normalization (by patching something into CV) lets you externally modulate the chaos oscillator’s width and overall character.
  - Expects ±5V signals for best results.

- **AC-Coupled Audio IN**:  
  - Takes both audio and CV signals—patching audio here creates interactions from “ring mod”-like to harmonic/bit crushed, depending on input signal and output selection.

- **Outputs**:  
  - *X*: “Windy”, noisy, more sinusoidal.
  - *Y*: “Squarer”, harsher, more aggressive.

---

## 1. Distorted Percussive Sounds

- **Patch Tips**:
  - *Kick/Snare*: Send a sharp envelope or short trigger (from an envelope generator or sequencer running fast gates) to both the *CV* and/or *IN* jacks. Experiment with amplitude and pulse width for “punchiness.”  
  - Drive *Emanate* and *Width* nearly full CCW for more chaos/noise, then tweak Width for focus.
  - Audio-rate pulses or “thump” waveforms into *IN* will introduce bit-crushed transients and metallic artifacts.
  - Stack and EQ output with distortion/external VCA for more impact.

- **Modulation**:
  - Modulate *Emanate* with fast, falling envelopes for dynamic “hits.”
  - Send audio-rate LFOs or oscillator square waves into *CV* for digital/artifacted drum elements.
  - Switch between X and Y out for blended noisy/snarling or sharp attack percussion.

---

## 2. Crazy Dubstep/Drum & Bass Basslines

- **Patch Tips**:
  - Use an LFO or sequencer to step-modulate the *CV* input at audio or sub-audio rate for deep, variable “wobble” or FM-like effects.
  - Use “Y” output for aggressive, crunchy bases — try audio-rate modulation for vowel-like or robotic-tones.
  - For bit-crush/sync bass, send an audio oscillator or chopped audio samples into *IN*.
  - Sweep *Emanate* for rhythmic, tearing movement or metallic overtones.

- **Modulation**:
  - Route a bass-heavy oscillator or drone into *IN* for sideband/ring-mod distortion.
  - Patch a stepped random voltage or S&H LFO into *CV* for unpredictable rhythmic variations.
  - Modulate *Width* with a secondary envelope for punchier, start-stop “growl” effects.

---

## 3. Haunting Atmospheric Pads

- **Patch Tips**:
  - Feed slow LFOs, random, or sample-and-hold CVs into *CV* and/or *IN* to create undulating, unstable drone beds.
  - Use “X” output for more subdued, evolving noise layers; blend “Y” for sharper spectral edges.
  - Tune *Emanate* toward the middle for sustained, less-chaotic movement; nudge *Width* for gentle harmonic shifts.
  - Layer reverb, long delay, and phaser after the output for maximum spookiness.

- **Modulation**:
  - Slowly modulate *Emanate* via a looping envelope or slow LFO for spectral evolution.
  - Modulate *Width* with a very slow triangle or sine LFO, synced to a musical phrase length.
  - For extra depth, cross-modulate: send cyclic LFOs to *CV*, and modulate their speeds/phase with other controllers.

---

### ADVANCED PATCH IDEAS

- **Feedback Loops**:  
  Try routing X or Y out (attenuated) back into *IN* or *CV* for recursive chaos—watch levels!

- **Chaining Modules**:  
  Use Triple Cap as a wild audio source, then process post-filter/VCA for timbral control, or put it in parallel with other oscillators for hybrid textures.

---

## SIGNAL SUMMARY

| Input     | Use for           | Modulation Suggestions                   |
|-----------|-------------------|------------------------------------------|
| CV        | Chaos depth/focus | Audio/LFOs, Envelopes, S&H, mod slow/fast|
| IN        | External mangling | Audio-rate signals, percussion thumps, LFOs|
| Emanate   | Chaos spectrum    | Manual/swept envelopes for dynamics      |
| Width     | Finer spectrum    | Manual/LFO/envelope modulation           |

---

## CREDITS & RESOURCES

- [Manual, Build Docs, BOM, Videos](https://zlobmodular.com/product/triplecapchaos/)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---

**Tip:** This module rewards wild experimentation—push unexpected signals into the *IN* and *CV*, and remember to try both outputs for flavors from subtle to savage!