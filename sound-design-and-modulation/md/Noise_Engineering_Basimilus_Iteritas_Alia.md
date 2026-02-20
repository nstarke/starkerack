# Noise Engineering — Basimilus Iteritas Alia

- [Manual PDF](../../manuals/Basimilus Iteritas Alia Manual - Noise Engineering Documentation.pdf)

---

[Basimilus Iteritas Alia Manual PDF](https://manuals.noiseengineering.us/bia/)

---

# Creative Modulation Strategies for Basimilus Iteritas Alia  
_(with a focus on percussive distortion, wild basses, and atmospheric pads)_

The Noise Engineering Basimilus Iteritas Alia (BIA) is an immensely versatile digital drum and percussion voice that goes far beyond kicks and snares—it’s a wild sound design workstation in 10HP. Below are focused modulation and patching strategies for three creative applications:

---

## 1. Modulating Distorted Percussive Sounds

**Core Concepts:**
- BIA excels at aggressive, harmonically rich percussion via its *Fold*, *Morph*, and *Harm* parameters.
- Patch dynamic (envelope, LFO, or random) CV to these parameters for constantly evolving, gnarly distortion.

**Modulation Techniques:**
- **Distorted Kicks/Snares:**  
  - Use the *Metal* mode for a noisier, trashier backbone.
  - Patch a random stepped LFO or fast envelope to *Fold CV* for unpredictable digital wavefolding—crunchy, broken-glass tones.
  - Send a fast, decaying envelope to the *Morph CV* to sweep from sine/triangle at the attack to saw/square at the tail for evolving timbres.
  - Slightly modulate *Spread CV* with an LFO to detune the oscillators, introducing fluctuating inharmonic overtones.

- **Glitch Percussion:**  
  - Mult your trigger to *Trig* and *Decay CV* so that every hit is a different length; clocked random for even more variation.
  - Modulate *Harm CV* with either clocked or unclocked random voltages for each hit to have a unique harmonic structure.

*Bonus Tip:* Use the *Envelope Out* to modulate other effect parameters (distortion pedals, VCA levels, etc.) downstream for even nastier transients.

---

## 2. Crafting Dubstep/Drum & Bass Basslines

**Core Concepts:**
- BIA is secretly a monstrous FM-esque bass synth, not just a drum voice.
- Key modulation points: *Pitch*, *Fold*, *Morph*, and *Spread*.

**Modulation Techniques:**
- **Growling & Talking Basses (Think Skrillex):**  
  - Use *Liquid* or *Metal* mode for maximum aggression; *Liquid* introduces a pitch envelope for a snappy attack.
  - Send a stepped sequencer or expressive controller to *Pitch CV* for bassline melodies.
  - Multi-destination modulation: Use an envelope follower or sequencer to simultaneously modulate *Fold* and *Morph* to sweep from soft to hard, and from pure to harmonically brutal.
  - Wobble: LFO to *Spread CV* or *Morph CV* for “talky”, vowel-like movement.
  - Macro modulation: Use a CV mixer to sum LFO, envelope, or MIDI-CV sources for live, performable bass morphs.

- **FM Bass Growl:**  
  - Patch audio-rate signals (another VCO or noise source) into *Decay*, *Attack*, or *Spread* CV inputs for unexpected audio-rate modulation/distortion (be careful with levels!).

---

## 3. Haunting Atmospheric Pads

**Core Concepts:**
- While BIA’s envelope is percussive, careful patching and re-triggering + parameter modulation enables droning or paddy textures.
- Use low *Decay* and high *Attack* for slow ramps and long tails.

**Modulation Techniques:**
- **“Eternal Hit” Pads:**  
  - Use a slow clocked gate to regularly re-trigger *Trig*; set *Decay* and *Attack* high for amorphous, overlapping tones.
  - Mult an LFO (slow triangle or sine) to *Morph* and *Harm* CV to create ever-shifting harmonic color and texture.
  - Modulate *Spread* gently for subtle movement between harmonic and inharmonic spectra.
  - For spectral “smears”: Use *Skin* mode with lots of harmonics, long *Decay*, and subtle, slow *Spread* modulation.

- **Textural Atmospheres:**  
  - Patch *Envelope Out* to modulate a filter cutoff or reverb mix in your system, so each hit blooms and recedes.
  - Modulate *Pitch* with a very slow, shallow LFO for subtle microtonal shifts (“detuned melted tape” effect).

---

## General Tips for All Sound Types

- Patch audio back through the BIA’s own *Envelope Out* controlling an external VCA or waveshaper for dynamic and interactive effects.
- Try using BIA as part of a feedback loop (send its output to an external module and route some of that back to a modulation input) for unstable, living sounds.
- Don’t forget the *Firmware Swap*: Try other Alia platform firmwares for drastically different capabilities using the same hardware!

---

> For more details:  
> [Basimilus Iteritas Alia Manual PDF](https://manuals.noiseengineering.us/bia/)

---
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)