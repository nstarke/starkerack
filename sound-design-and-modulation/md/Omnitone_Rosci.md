# Omnitone — Rosci

- [Manual PDF](../../manuals/Rosci-Manual.pdf)

---

[**Download the Rosci User Manual (PDF)**](attachment://Rosci_User_Manual.pdf)

---

# Creative Modulation Ideas for Rosci (Eurorack)

Drawing from the Rosci Rev 3 manual, here are focused techniques and modulation patch ideas for three styles: distorted percussive hits, aggressive basslines, and haunting pads.

---

## 1. Distorted Percussive Sounds

**Key Parameters:**  
- **Complexity**: Number of points in waveform  
- **Roundness**: Interpolation shaping  
- **Harmonics**: Adds upper partials  
- **Formants**: Compresses waveform for "vowel" sounds  
- **Detune**: Tuning spread (up to a fifth)  

**Techniques:**

- **Envelope Percussive CV**: Patch a fast-decay envelope (from a function generator or EG) into the Harmonics or Complexity CV. This will create sharp, changing timbres on the attack, producing punchy and unpredictable percussive transients.
    - Example: Output of Maths/ADSR to Harmonics CV Input.
- **Noise-Based Modulation**: Send a clocked sample & hold or noise source to Complexity or Roundness inputs. Abrupt voltage changes will glitch the waveform shape for digital "crunch."
- **Detuned Thwack**: Automate the Detune CV with a snappy envelope or even a random stepped CV, spreading pitch for aggressive, attack-heavy distortion.
- **Overvoltage Saturation**: Exceed ±10V briefly (with carefully attenuated CV or boosted signals) for parameter saturation/distortion, as the Rosci will saturate beyond range for further sonic roughness.

---

## 2. Crazy Dubstep/Drum & Bass Basslines

**Key Parameters:**  
- **Complexity & Harmonics** modulated by LFO, envelopes, or sequenced CV  
- **Formants** for vowel or "talking" bass movements  
- **Detune** for thick, growling sounds  

**Techniques:**

- **Rhythmic LFOs**: Patch synced LFOs (or synced random generators) into Formants and Harmonics to sweep through "vowel" territory. This is key for "talking bass" effects.
    - Pro tip: Use multiple LFOs at different rates simultaneously patched into various parameters (knobs + CV are summed).
- **V/Oct Bassline Sequencing**: Use a quantized sequencer (or pitch CV from a DAW/keyboard) into the V/Oct input for pitch riffs. Layer with fast envelopes modulating Complexity/Harmonics for movement.
- **FM/AM tricks**: Patch the output of one VCO or modulation oscillator into the Harmonics or Complexity CV—try audio-rate FM for harsh, metallic basses.
- **Extreme Detune**: CV the Detune with a slow triangle LFO to swing between fundamental and perfect fifth, creating unstable, massive bass.
- **Hard Sync Percussion**: Gate the Generate function (if possible via trigger input)—each note or step can re-trigger/re-randomize the wave shape for "reset" artifacts.

---

## 3. Haunting Atmospheric Pads

**Key Parameters:**  
- **Complexity** (low to medium for organic tones)  
- **Roundness** (smooth curves for evolving waveforms)  
- **Formants** (modulated for shifting spectral focus)  
- **Detune** (slight movement for chorusing)  

**Techniques:**

- **LFO Swarm**: Patch multiple ultra-slow LFOs (sub-1Hz to ~0.1Hz) into Complexity, Roundness, and Formants. This will slowly morph the waveform over time, resulting in eerie, living textures.
    - Use external offset/attenuators to keep modulation in musical range.
- **Gentle Detune**: Use slow random or triangle LFOs (or hand-played CV) to modulate Detune lightly for drifting polysynth vibes.
- **Envelope Morphing**: Use looping envelopes with long attack/decay controlling Roundness and Formants for evolving pads.
- **Multimode Output**: Mult the output and process one copy through reverb (for pad body) and another through FX/distortion (for ghostly tails).

---

## Additional Rosci Tips

- **Parameter CV Summing**: Remember, the module sums knob and CV input—fine-tune static settings with knobs, then add movement with CV.
- **Tuning Stability**: Tuning is accurate to ±3 cents over the 0–10V V/Oct range; you can confidently sequence at precise pitches for basslines and pads.

---

> Download the original manual for reference:
> [**Rosci User Manual (PDF)**](attachment://Rosci_User_Manual.pdf)

---
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
