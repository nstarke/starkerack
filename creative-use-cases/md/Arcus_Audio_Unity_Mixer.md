# Arcus Audio — Unity Mixer

- [Manual PDF](../../manuals/Unity Mixer - Arcus Audio.pdf)

---

[Unity Mixer Manual PDF](https://arcusaudio.com/product/unity_mixer/)

---

## Creative Uses for the Arcus Audio Unity Mixer in Eurorack Systems

The Unity Mixer from Arcus Audio is a compact (2hp) dual 3:1 unity gain summing mixer that can also serve as a single 6:1 mixer. With DC-coupled inputs (for audio or CV), bi-color LEDs for signal level and polarity, and minimal power draw, it’s a versatile utility.

### 1. Merging Multiple Modulation Sources

**How:** Patch several LFOs, envelopes, or random CV sources into the inputs, sum them, and send the mixed output to a filter cutoff, oscillator pitch, or effect parameter.

**Creative Tip:** Combining static (LFO), dynamic (envelope), and chaotic (Sample & Hold) modulation sources through the Unity Mixer results in unique, evolving modulations for more nuanced patches.

**Module Recommendations:**  
- Make Noise Maths (LFO/Envelope)
- Mutable Instruments Tides (LFO/Envelope)
- Doepfer A-148 (Sample & Hold)

---

### 2. Mixing Audio Signals Before a Waveshaper or Effects

**How:** Patch multiple VCO waveforms (for example, sine, triangle, and PWM square) into one section of the Unity Mixer. Sum them into a single chain—then process through a wavefolder, ring mod, or distortion.

**Creative Tip:** Unity gain summing allows you to blend waveforms without changing their amplitude. This can introduce interesting harmonic content when run into distortion, wavefolders, or resonators.

**Module Recommendations:**  
- Befaco Wavefolder
- Intellijel Bifold
- Mutable Instruments Rings (resonator)

---

### 3. Creating a Submix for FX Sends

**How:** Use the Unity Mixer to sum a few drum or percussion voices and send the output to a delay or reverb module’s input.

**Creative Tip:** This enables you to apply collective FX processing (like sidechained reverb, compressed delay) to grouped signals—fine-tune your submix before the effect.

**Module Recommendations:**  
- ALM S.B.G (for pedal interface)
- Erica Synths Pico DSP (FX)
- 2hp Verb (reverb)

---

### 4. Summing Envelope or Gate Triggers for Rhythmic Complexity

**How:** Send multiple gate or trigger sources (sequencers, clock dividers, manual buttons) into the mixer and use the summed output for percussive voices, envelopes, or as a logic function (mixing triggers as 'OR').

**Creative Tip:** Summed gates can create slight timing overlaps, great for polyrhythmic or humanized percussion.

**Module Recommendations:**  
- Mutable Instruments Grids (trigger sequencer)
- 4ms QCD (Clock Divider)
- Intellijel Steppy (trigger sequencer)

---

### 5. Layering CV for Stereo or Multichannel Patches

**How:** Use each half of the mixer for left and right channel signals, layering stereo modulations or audio sources before routing to stereo processing or panning modules.

**Creative Tip:** Contrasting modulations per channel can create immersive stereo movement or spatialization.

**Module Recommendations:**  
- Happy Nerding PanMix Jr (stereo panner)
- WMD Overseer (stereo filter)
- Make Noise Mimeophon (stereo delay)

---

### 6. Mixing Audio for Feedback Patching

**How:** Patch the output of a filter or delay back into itself via the Unity Mixer, blending in external signals or modulations to control feedback level and timbre.

**Creative Tip:** Controlled feedback with summed signals can yield unique, evolving drones, textures, or noise beds.

**Module Recommendations:**  
- Mutable Instruments Clouds (granular)
- Make Noise QPAS (filter)
- Tiptop Echoz (delay)

---

### 7. Utility Functions

- **CV Normalization:** Take several unipolar or bipolar modulation signals and use the bi-color LEDs to visualize overall polarity—helpful for finding phase-correct blends.
- **Unity Gain Mixing:** Mix multiple pitch CVs (multiple sequencers/arpeggiators) to drive a single VCO and create evolving melodic sequences (works best with precise sources so tuning isn’t affected).

---

For further ideas, you can pair the Unity Mixer with logic modules, complex envelopes, granular processors, or stereo imaging tools—the possibilities are wide open for creative utility!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)