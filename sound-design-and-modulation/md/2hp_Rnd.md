# 2hp — Rnd

- [Manual PDF](../../manuals/2hp_Rnd.pdf)

---

[**PDF Manual for 2hp Rnd**](https://2hp.com/wp-content/uploads/2hp-rnd.pdf)

---

# Creative Patching with 2hp Rnd for Distortion, Basslines, and Atmospheres

The **2hp Rnd** module is a compact, versatile random voltage and gate generator. Let's explore patching ideas for your modular system to create **distorted percussion**, **crazy modulated basslines**, and **haunting atmospheric pads**.

---

## Overview of 2hp Rnd Modulation Potential

- **Smooth Output (Random S&H/LFO):**
  - Variable, continuously changing random voltage (rate set by RATE knob).
  - Attenuator available for output scaling (0-10V range).

- **Quant Output (Stepped Random):**
  - Generates a new random value on each clock pulse (sync to internal or external clock).
  - Attenuator for output scaling.
  
- **Gate Output:**
  - Produces either steady clock (internal) or random gates (external).

---

## 1. Distorted Percussive Sounds

**Approach:** Modulate distortion/waveshaper, VCAs, and drum voice CV inputs for unpredictable, glitchy timbres.

### Patching Tips

- **Random Envelope Decay:**
  - Patch ***Quant Output*** to a drum VCA's decay or release CV for wildly changing tail lengths and transients.
- **Random Distortion/Drive:**
  - Send ***Smooth Output*** to control a distortion module’s drive/amount CV, creating unpredictable, evolving saturation over your drum hits.
- **Random Gates for Percussive Rhythm:**
  - Set Rnd to **external clock** mode and patch ***Gate Output*** to trigger drum modules or envelopes for non-repetitive, syncopated patterns.
- **Granular Glitch:**
  - Use ***Smooth Output*** to modulate sample position or bit reduction on a granular or lo-fi sampler.

**Pro Tip:** Adjust the RATE knob to taste—the faster, the more frantic and harsh the modulation.

---

## 2. Crazy Dubstep/Drum & Bass Basslines

**Approach:** Channel the classic "talking"/moving bass sound by modulating filters, wavetable positions, and amplitude.

### Patching Tips

- **Filter Modulation:**
  - Patch ***Smooth Output*** to a low-pass or band-pass filter’s cutoff frequency. The non-repetitive motion creates constantly evolving bass timbre.
  - Use ***Quant Output*** (stepped) for sudden, dramatic filter jumps—especially with sync to your beat clock.
- **Amplitude & Timbre Chaos:**
  - Use Gate Output in **random** mode to fire VCAs/envelopes on bass notes, adding broken-glitch rhythm (think: neuro, halftime).
- **Waveshaper/Wavetable Scanning:**
  - Feed ***Smooth Output*** into the wavetable position or wavefolder CV input for constantly morphing bass sounds.
- **Subtle Randomization:**
  - Use the output attenuators to scale modulation amount, keeping the chaos in control or letting it go wild.

---

## 3. Haunting Atmospheric Pad Sounds

**Approach:** Slow, unpredictable motion creates evolving textures and eerie soundscapes.

### Patching Tips

- **Evolving Filter/Pan/Reverb:**
  - Patch ***Smooth Output*** to the cutoff/resonance of a filter applied to a pad sound, or to the wet/dry CV of a reverb.
  - Send the same output to a stereo panner, slowly drifting the sound across channels.
- **Clocked Random for S&H Pads:**
  - Sync ***Quant Output*** to a slow LFO or external clock, driving slow-changing but stepped textures (modulate wavetable, filter, or harmony CV).
- **Random Layer Movement:**
  - Use two channels (Smooth & Quant), one for filter movement, another for amplitude or FX parameters.
- **Atmospheric Swells:**
  - Use the internal clock and RATE knob to set the pace of movement—slower for more ominous atmospheres.

**Pro Tip:** Try stacking several random modulations on different voice layers for lush, morphing backdrops.

---

## General Modulation Strategies

- **External Clocking:** Sync Rnd’s randomization to your sequencer for “in time” modulations.
- **Voltage Scaling:** Use attenuators on Rnd to precisely dial in subtle or extreme random movement.
- **Cross-Modulation:** Feed one random output into a CV-controlled crossfader or mixer, blending/modulating between several modulation targets.

---

### More Resources  
- [2hp Rnd Official Manual (PDF)](https://2hp.com/wp-content/uploads/2hp-rnd.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)