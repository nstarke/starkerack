# Erica Synths — Sample Drum

- [Manual PDF](../../manuals/FINAL_sample_drum_instrukcija_A4.pdf)

---

[Erica Synths Sample Drum Manual PDF](https://www.ericasynths.lv/media/Sample-Drum_1_07_manual.pdf)

---

# Creative Modulation with Erica Synths Sample Drum  
_**Distorted Percussion, Crazy Basslines, and Haunting Pads**_

The Erica Synths Sample Drum is incredibly powerful for sound design when you leverage its advanced modulation capabilities. Below are focused patching and modulation ideas—perfect for distorted one-shots, wild movement in basslines, and deep evolving ambiences.

---

## 1. **Distorted Percussive Sounds**

### **1.1. Bitcrush & Drive FX Modulation**
- **How:** Load your drum one-shots (kicks, snares, hats) and assign CV inputs (CV1-CV3) to different FX parameters, such as BITCRUSH and DRIVE. Patch in stepped or random LFOs, envelopes, or sequenced voltages to modulate the BITCRUSH depth or the DRIVE amount.
- **Pro tip:** Use a fast envelope to modulate DRIVE or BITCRUSH only during the attack portion of the sound for a “smack” that decays to clarity.

### **1.2. Envelope Shaping**
- Go into the **AMPLITUDE** menu and assign the CV to envelope parameters (Attack, Decay SHAPE). Send in rapid envelopes from another module or mult the Sample Drum’s own output to create self-modulating parameters.
- **Distorted stutters:** Modulate the loop point or end point aggressively with stepped random or audio-rate CV.

### **1.3. Sliced Glitch Percussion**
- Use **sample slicing** (manual or zero-crossing) on drum loops or hits, then assign a fast random or S&H CV to SLICES:INDEX. Result: every trigger fires off a different micro-slice—superb for broken, IDM/glitch percussion.
- Combine this with modulated BITCRUSH or FOLD for even more chaos.

---

## 2. **Crazy, Evolving Basslines**

### **2.1. 1V/Oct for Bassline Sequencing**
- Load a bass sample and use the 1V/Oct mode for pitch tracking. Use a sequencer or step random generator for wild, inharmonic melodies.
- Assign a CV to the TUNE parameter for additional pitch wobbles and slides.

### **2.2. FX Parameter Wobble**
- **Setup:** Assign LFOs or random CV to FX:PARAM1 (filter cutoff if using LPF/HPF, or BITCRUSH/FOLD amount).
- **Dubstep growl:** Mult an envelope or LFO so it controls both level and bitcrush/fold for highly animated, dirty bass timbres.

### **2.3. Loop Point or Start/End Wavetable**
- Modulate the sample START/END or LOOP points with an external LFO or the output of a sequencer. This can “scan” through a bass sample or wavetable for dynamic digital harmonic motion.

---

## 3. **Haunting Atmospheric Pads**

### **3.1. Long Samples + Slicing**
- Load long, atmospheric field recordings or synth swells.
- Use auto or manual slicing and assign SLICE:STEP to random or slow LFO. Trigger slices at slow or irregular intervals for an eerie, evolving collage effect.

### **3.2. FX Creative Layering**
- Assign CV inputs to REVERB, HPF/LPF cutoff, and parameter mix. Patch smooth, slow, or attenuated LFOs.
- Modulate REVERB depth, filter cutoff/fold, blend dry/wet in real time for movement.

### **3.3. Envelope & Level Movement**
- AMPLITUDE menu: assign a slow LFO to envelope parameters (Attack/Decay/Shape) and LEVEL.
- Result: “ghostly” fade-ins, unexpected swells, vanishing echoes. Set envelope RANGE to RELATIVE so the envelopes stretch to the slice—further enhancing movement.

---

## **General Modulating Tips**

- **CV Mapping:** Each channel has three freely assignable CV inputs—use for nearly any parameter, from slice selection to FX types.
- **Performance Mode:** Assign the six encoders to your favorite mod destinations; use in tandem with external modulation for hands-on tweaks plus LFO/envelope morphing.
- **Randomness:** For experimental results, send random stepped CV (e.g., from a Turing Machine or Wogglebug) to sample start/end points, FX type, and slice.

### **Signal Flow Example for Complex, Distorted Bass**
1. Load a bass hit sample, set to forward loop mode.
2. Assign CV1 to TUNE (1V/Oct from sequencer).
3. Assign CV2 to FX:BITCRUSH.
4. Assign CV3 to End point or Loop point.
5. Send a synchronized LFO (with subharmonic divisions from your main clock) to both CV2 and CV3.
6. Bass hit's pitch, timbre, and loop position “wobble” in sync with the groove for a mutant, ever-changing line.

---

# Links

- [Erica Synths Sample Drum Manual PDF](https://www.ericasynths.lv/media/Sample-Drum_1_07_manual.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)