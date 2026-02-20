# Instruo — Tona

- [Manual PDF](../../manuals/Tona-Manual-A5.pdf)

---

[Instruō Tòna Oscillator User Manual PDF](https://www.instruomodular.com/wp-content/uploads/2021/03/tonau_manual_v1.0.pdf)

---

# Modulation Tips for the Instruō Tòna Oscillator

The Instruō Tòna is a powerful analog oscillator with a built-in wavefolder, making it ideal for a wide range of sound design applications in Eurorack, from extreme and distorted percussion to throbbing bass and eerie pads. Here’s how you can modulate the tòna to get those sounds:  

---

## 1. Distorted Percussive Sounds

### Key Features to Exploit  
- **Wavefold Output** & **Wavefold Fader**
- **Wavefold CV Input + Attenuator**
- **Linear FM Input + Attenuator**
- **Oscillator Sync (Hard Sync Input)**

### Techniques
- **Wavefolding “Strikes”**:  
  - Patch an envelope (snappy AD or AR) or even a drum trigger as a CV source to the Wavefold CV Input. Set the Wavefold Fader near the minimum (left) and the CV Attenuator to taste. The wavefolder will then “strike” the sine, creating clangy, metallic, or ‘torn’ percussive transients like FM percussion or Buchla bongo tones.
- **FM Drum Modulation**:  
  - Patch a fast envelope, LFO, or noise burst to the Linear FM Input, and carefully increase the FM Attenuator. This will create sharp, non-harmonic overtones—ideal for synthetic hats, toms, or snares.   
- **Hard Sync for Snap and Bite**:  
  - Use a gate, trigger, or audio-rate oscillator to the Sync Input. This will force tòna to “retrigger,” imparting aggressive attack transients.  
- **Stacked Distortion**:  
  - Mix the raw output (e.g., Triangle) with the Folded output for layered, biting sounds, especially after a VCA or distortion module.

---

## 2. Crazy Basslines (Dubstep, DnB, Neuro, etc.)

### Key Features
- **Wavefolded Sine for Aggro Timbres**
- **Audio-Rate FM**
- **Sync for Vocal/Cutting Effects**

### Techniques
- **Gnarly Wobble Bass**:  
  - Patch the Sine output of another VCO (the Modulator) into tòna’s Linear FM Input. Set tòna as the Carrier. Dial the FM Attenuator for the right amount of aggression.  
  - For “talking” bass, modulate the FM amount or even modulate the Modulator’s own pitch, then run tòna’s output through a bandpass filter or formant filter.
- **Bass “Growl” with Wavefolding**:  
  - Use the Wavefold output. Patch an envelope or LFO to the Wavefold CV Input, rhythmically modulating fold amount for “talkbox”/“vowel” or growling effects.  
- **Sync’d Bass Crunch**:  
  - Sync tòna to a lower-pitched modulator oscillator for “hard sync” sweep bass sounds; then modulate tòna’s pitch or the modulator’s pitch for vocal/jumping bass timbres.
- **Patch Example**:  
  - Sine from second VCO to tòna Linear FM input, set FM Attenuator to medium. Wavefold amount modulated by a fast, rhythmic LFO synced to your beats. Output Folded waveform to filter or direct to VCA.

---

## 3. Haunting Atmospheric Pad Sounds

### Key Features
- **Wavefolder for evolving timbres**
- **Fine VCO tuning for slow phasing**
- **Slow LFO or Envelope to Wavefold CV**
- **Gentle Linear FM**

### Techniques
- **Slow Animated Timbres**:  
  - Use slow triangle or sine LFOs into the Wavefold CV Input. Set fold to a subtle amount via the fader and modulate gently for spectral morphing, “breathing” pads.
- **Atmospheric FM**:  
  - Very slow modulation of tòna’s Linear FM via a wandering LFO or another VCO pitched below audio rate adds drifting overtones—very cinematic or textural.
- **Stacked Outputs for Richness**:  
  - Mix Sine, Triangle, and Folded outputs. Detune slightly using the Fine tuning (maybe even use two tòna modules for lush stereo spread).  
- **Envelope Modulation**:  
  - Use ADSR envelopes to modulate fold or FM depth for evolving, expressive pads.

---

## Additional Ideas

- **Feedback for Textures**: Try feeding one of tòna’s outputs (such as Folded or Triangle) back into its own Linear FM Input with attenuation for self-modulated chaos.
- **Rhythmic CV**: Use clocked LFOs/sequencers for rhythmic FM or folding patterns.
- **Multi-Output Layering**: Use all outputs at once into a mixer for richer, sometimes chaotic results.

---

**Full Manual:**  
[Instruō Tòna Oscillator User Manual PDF](https://www.instruomodular.com/wp-content/uploads/2021/03/tonau_manual_v1.0.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)