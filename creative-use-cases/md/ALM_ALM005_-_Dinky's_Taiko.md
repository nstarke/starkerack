# ALM — ALM005 - Dinky's Taiko

- [Manual PDF](../../manuals/alm005-manual.pdf)

---

[ALM-005 ‘Dinky’s Taiko’ Manual PDF](https://busycircuits.com/alm002-alm005-dinkys-taiko/Dinkys-Taiko-Manual.pdf)

---

# Creative Uses for ALM-005 ‘Dinky’s Taiko’ in a Eurorack System

The **ALM-005 ‘Dinky’s Taiko’** is a flexible 12-bit digital drum voice with voltage control, accent/choke dynamics, analog EQ, and a rich sound palate. Here’s how you can creatively patch and combine it with other modules for unique and experimental results:

---

## 1. **Sequenced Drum Synthesis**
Pair *Dinky’s Taiko* with a trigger sequencer (e.g., **ALM Pamela’s PRO Workout**, **Intellijel Steppy**, or **Winter Modular Eloquencer**). Use programmable gates/triggers to drive both the regular and accent, choke inputs for groovy, textured percussion lines.

- **Pro Tip:** Patch a separate “fill” pattern to the Choke input for evolving breaks or stutter effects.

## 2. **Evolving Drum Timbres With Modulation**
Leverage the rich CV inputs (Start/End Freq, Spectrum, Wave, etc) from sources such as:

- **Random Generators/LFOs (e.g., Mutable Instruments Tides/Marbles, Make Noise Maths):**  
  Use slow LFOs or stepped random to morph timbre over time for generative, less-repetitive drum parts.
- **CV Recorders/Sequencers (e.g., Make Noise Pressure Points, Intellijel Tetrapad):**  
  Manually draw in or sequence parameter automation for dynamically shifting drum sounds.

## 3. **Drum FM and Cross Modulation**
Patch an external audio-rate oscillator’s output (e.g., **Noise Engineering Basimilus Iteritas**, or any analog VCO) into Dinky’s CV inputs. Rapidly modulating the Spectrum, Start Freq, or Release can lead to metallic or pseudo-FM drum textures.

- **Try:** Using envelopes or transient generators (ALM Pip Slope, Make Noise Function) to modulate these CVs for snappy FM drum hits.

## 4. **Multi-Voice Percussion Kit**
Layer multiple *Dinky’s Taiko* modules, or combine with other drum voices (e.g., **Hexinverter Mutant Drums**, **Tiptop Audio 808 Modules**) as a drum rack. Share clock/division patterns, but send different CV modulation to each for maximal variation.

## 5. **Experimental Tactile Drum Performances**
Patch the Choke and Accent to manual gate buttons, touchpads (Intellijel Tetrapad), or expressive controllers (e.g., **Makenoise Pressure Points**), allowing live muting/choking and accent addition—great for performance-oriented setups.

## 6. **Rhythmic Processing and Distortion**
Run Dinky’s output through analog distortion (**XAOC Devices Soviet**, **Erica Pico Drive**), wavefolders, or lo-fi samplers. Exploit the “hot” output (+/-10v) to push downstream modules into nonlinear ranges for grit and chaos.

## 7. **Open-Ended Sampling and Looping**
Sample percussive material straight from Dinky’s Taiko into a Eurorack sampler (e.g., **1010 Bitbox**, **Electrosmith Daisy Daisy Patch Submodule**, **Rossum Assimil8or**), chop/resequence for elaborate percussive textures.

## 8. **Creative Audio Rate Modulation**
Feed *audio* (not CV) into the CV controls for digital “abuse”—audio rate modulation at Spectrum or Wave can create clangorous, glitchy percussion sounds not ordinarily possible.

---

### *Module Type Recommendations for Pairing:*
- Gate & Trigger Sequencers
- Random/S&H Generators
- CV Sequencers/Recorders
- Function Generators/Envelopes
- Audio Rate Oscillators
- Distortion/Wavefolding FX
- Samplers/Loopers
- Physical Interface/Touch Controllers

---

For further experimentation and processing ideas, check out the [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor).