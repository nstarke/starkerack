# Sound Machines — Modulor 114

- [Manual PDF](../../manuals/MODULOR114-MANUAL-SEP16-V01.pdf)

---

[Download the MODULÖR114 Manual (PDF)](https://www.sound-machines.it/product/modulor114/MODULOR114%20OWNERS%20MANUAL%201.0.pdf)

---

# Creative Sound Design with the MODULÖR114 Eurorack Synth

The MODULÖR114 from soundmachines is a highly integrated eurorack-compatible analog modular synthesizer, packed with classic and unconventional modules—perfect for both bread-and-butter and experimental sound design. Let’s dive into modulation techniques for creating **distorted percussive hits**, **aggressive basslines**, and **haunting atmospheric pads**.

## 1. Distorted Percussive Sounds

**Key Modules:**  
- VCO1 (with noise sources)
- VCF (self-resonant)
- VCA (soft saturation)
- ENV (ADSR)
- S&H (Sample & Hold)
- FX (digital effects)

### Patch Concept:
- **Noise/Impulse Percussion:**  
  - Patch WHITE or PINK noise from VCO1 to the VCF input.
  - Envelope the noise with ENV → VCA.
  - Use the S&H output, triggered by an LFO or CLKDIV, to modulate the VCF cutoff for random percussive timbres.
  - Crank up RES (resonance) on the VCF—allow it to self-oscillate for metallic highs or sharp kicks.
  - Add DRIVE: Turn up INITIAL on the VCA for soft saturation or patch the output back into itself via mixers or attenuators for dirty, clipped sounds.
  - Finish the chain with FX (try using reverb for space or short delay for slap-back rhythms).

**Bonus:** Patch a LOGIC GATE output (e.g. XOR of multiple clocks or LFOs) to trigger ENV for unpredictable, “broken robot” rhythm patterns.

---

## 2. Crazy, Moving Basslines (e.g. Dubstep, Drum & Bass)

**Key Modules:**  
- VCO1/2 (for stacked/detuned oscillators)
- MIX1 (oscilator blend)
- VCF (aggressive filter movement)
- ENV (snappy or slow attack)
- LFO2, SLEW, RIBBON, DIGITAL
- FX (Chorus/Delay for movement)

### Patch Concept:
- **Meaty, Modulated Bass:**  
  - Use VCO1 SAW and SUB, and layer with VCO2 SAW/TRI. Detune VCO2 slightly (use FINE/TUNE).
  - Mix oscillators in MIX1, send to VCF.
  - Use ENV for sharp filter sweeps on VCF cutoff (classic “talking” wobble).
  - Modulate VCF cutoff with LFO2 or VC-LFO from VCO2. Patch SLEW between LFO and VCF for ever-evolving modulation (portamento-like sweeps).
  - Try inserting S&H in the modulation path for stepped/“glitched” filter motion. Or, use the QUANTIZER to lock random voltages into musical (but mental) pitch sequences.
  - For classic dubstep “wobble”: patch clocked LFOs or divide/multiply clocks with CLKDIV; patch these to VCF cutoff or VCA, or even drive FX parameters for time-synced stutters.
  - For extreme distortion, drive the VCA hard and/or feed back VCF output into the input via MIX modules.

**Tip:** The MIDI→CV section allows modwheel/CC to spit out CV; assign this to VCF or FX for hands-on, live modulation.

---

## 3. Haunting Atmospheric Pads

**Key Modules:**  
- VCO2 as VCLFO; VCO1 TRI for smooth base tones
- RIBBON for manual CV sweeps
- MIX2/3 for layering and blending pitch/CV sources
- VCF in Bandpass mode (for ethereal qualities)
- LFO2 for subtle, slow modulation
- FX (reverb/chorus for lushness)

### Patch Concept:
- **Dreamscapes & Movement:**  
  - Tune VCO1/2 for close intervals, layer with SUB for added depth.
  - Use ENVELOPE (long attack & release, LONG switch on) to smooth amplitude changes at the VCA.
  - Modulate VCF cutoff with ultra-slow LFOs (from VCO2 in LFO mode, or LFO2), and add a bit of SLEW for gentle, laggy motion.
  - Modulate the FX parameters (CV in to FX) with random voltages from S&H for evolving spaces.
  - Use the RIBBON to “play” pitch and filter sweeps manually for organic, ghostly sounds.
  - Patch an attenuated WHITE or PINK noise layer for texture.
  - For subtle pitching, use the QUANTIZER with a low-rate LFO or S&H, then mix this with your oscillator pitch CVs.

**Extra:** Use FX tap-tempo to sync slow delays to external divisions, creating dense, rhythmic pad trails or “clouds.”

---

## Modulation Patch Tricks (Advanced)

- **Dual Modulation:** Use MIX3 to combine LFO and ENV signals before sending to VCF for complex, evolving filter animation.
- **Triggered Mayhem:** Use LOGIC GATES to combine clock, LFO, and S&H outputs for “intelligent” bursts of modulation—patch to VCA CV for tremolos or to FX parameter for space “jumps.”
- **Ring Mod Emulation:** Patch two out-of-phase oscillators (square/saw) into XOR input for ring-mod-like metallic textures.

---

For further patch diagrams, the manual includes illustrated examples on pp. 26–29.

---

> [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---

**Have fun patching! With so many CV destinations, internal digital/logic blocks, and hands-on modulation options, the MODULÖR114 is a true playground for sound explorers.**