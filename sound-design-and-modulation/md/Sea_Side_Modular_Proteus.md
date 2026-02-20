# Sea Side Modular — Proteus

- [Manual PDF](../../manuals/ProteusManual.pdf)

---

[Proteus Eurorack Manual PDF](https://seaside.digital/proteusmanual.pdf)

---

# Modulating the Seaside Modular Proteus for Unique Eurorack Sounds

The Seaside Modular **Proteus** module is a generative sequencer/voltage processor that excels at blurring the boundaries between repetition and change. Below, I’ll explain how to use its modulation capabilities—via internal settings, CV, and patching—to sculpt **distorted percussive sounds**, **aggressive basslines**, and **atmospheric/ambient textures**. For each, I’ll recommend external patching, detailed Proteus parameters to focus on, and CV ideas.

## 1. **Distorted Percussive Sounds**

### **Patch Tips**

- **Trigger Proteus at Audio Rate**  
  Run a rapid trigger/clock (audio rate or near-audio rate) into the GATE IN. This will create fast, “pitched” clicks for use as noise/percussion.
- **Short Envelopes**  
  Use the GATE OUT to trigger a short envelope or directly hit a VCA for a clicking, percussive transient.

### **Proteus Settings**

- **SLEEP Knob:**  
  Set to 0 (no sleep), for rapid-fire sequence repetition.
- **GATE LENGTH (Settings Mode):**  
  Turn fully CCW for ultra-short trigger pulses = sharp transients.  
- **DENSITY:**  
  Keep near full CW for maximal step density—more notes, more hits per bar.
- **MUTATE:**  
  Moderate position for subtle note changes, adding surprising percussive movement.
- **COMPLEXITY:**  
  Low for simple rhythms, or higher for less predictable patterns.
- **PATTERN BANK:**  
  Save a few rhythmic patterns, and cycle between them to inject sudden “variation drops”.
- **CV Modulation:**  
  Patch random CV or sequenced voltage into the DENSITY, MUTATE, or SLEEP to create “broken” rhythms and glitches.

### **External Treatment**

- **Distortion/Folding:**  
  Take the Proteus pitch output and use it as an audio oscillator through distortion, wavefolders, or bitcrushers for harsh percussive clicks.
- **Ring Mod Adjustment:**  
  Use the pitch output as an FM or AM modulator for another sound.

---

## 2. **Dubstep/Drum and Bass Basslines**

### **Patch Tips**

- **Melody Generation for Bass**
  Set sequence LENGTH to 2–8, for repetitive, catchy bass phrases.
- **Scale:**
  Use a minor (or custom) scale for dark harmonics (e.g., Natural Minor, Harmonic Minor, or even a custom scale with repeated root/fifths).
- **OCTAVE:**  
  Keep the OCTAVE knob CCW for low “bass” output, but modulate with CV for jumps.
- **COMPLEXITY:**  
  Start at noon. If you want variations between whompy LFO-wobble and gnarly steps, set somewhere between noon and full CW.
- **DENSITY:**  
  Run at 75-100% for a pounding, rapid-fire bassline. Lower for “stutter” effect.
- **TRANSPOSE Input (with Quantize OFF):**  
  Route an LFO, stepped random, or envelope into the TRANSPOSE jack, creating bass “wobbles” or glides.
- **MUTATE:**  
  Low to moderate for micro-evolutions in bass riffs without going off the rails.

### **External Treatment**

- **Filter Modulation:**  
  Patch GATE OUT to trigger envelopes for cutoff resonance or even wild filter FM.
- **Distortion/Saturation**  
  Take Proteus pitch output through a waveshaper or tube-style module for driven, monster basslines.
- **Side-Chain:**  
  Use the SLEEP knob or GATE patterns to carve out rhythmic holes for kick/snare interplay.

---

## 3. **Haunting Atmospheric Pads**

### **Patch Tips**

- **SLEEP Knob:**  
  Medium–high values (leave gaps between sequences)—for haunting repetition with space to breathe.
- **DENSITY:**  
  Down at 30–60% for notes that unsystematically drop away, creating ghostly, fragmentary harmonies.
- **OCTAVE & MUTATE:**  
  Slightly above CCW and infrequently modulated = sudden spectral transpositions or evolving harmonics.
- **COMPLEXITY:**  
  Fully CW for evolving, ambiguous melodic material; or noon for something more harmonic.
- **PATTERN BANK Cycling:**  
  Store three slowly evolving patterns and CLOCK the NEXT input slowly for “movements” in the pad.
- **SLEW (Settings):**
  Engage Slew Mode. Adjust SLEW LENGTH/NOTES so only some steps glide for overlapping, smeared transitions (teal lights).

### **CV Modulation**

- **PATience:**  
  Patch a slow LFO or random voltage to the PATIENCE input for sequences to gently decay and “rematerialize”, adding long-form ambience.
- **Density/Complexity:**  
  Modulate via smoothed random/chaotic LFOs so the pattern breathes, sometimes busy, sometimes minimal.
- **Transpose:**  
  Slowly moving CV into TRANSPOSE, with quantization ON, for evolving modal atmospheres.

### **External Patch Ideas**

- **Reverb/Delay:**  
  Send pitch output to a heavily wet shimmer or modulated delay/reverb for ethereal soundscapes.
- **Polyphony Trick:**  
  Mult Proteus pitch and gate to several oscillators/different voices for pseudo-polyphonic pads.

---

# Workflow Summary

- Use all CV inputs for extra dynamism; try external sequencers, random sources, or even audio-rate signals for wild behaviors.
- Save your favorite “state” to the pattern bank and experiment with cycling them mid-performance.
- Explore custom scales (microtonal, just intonation, or “broken” scales) for genuinely alien sounds via the online config tool.
- Slew and gate settings allow you to morph the standard step sequencing into more legato, expressive, or chopped textures.

---

Explore more:  
Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)