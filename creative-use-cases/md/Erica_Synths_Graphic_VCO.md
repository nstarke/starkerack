# Erica Synths — Graphic VCO

- [Manual PDF](../../manuals/graphic_vco_manual_web.pdf)

---

[Erica Synths Graphic VCO Manual (PDF)](https://www.ericasynths.lv/media/Graphic_VCO_Manual_1_05.pdf)

---

# Creative Uses for the Erica Synths Graphic VCO

The **Erica Synths Graphic VCO** is an exceptionally powerful and flexible digital oscillator, capable of bespoke wave design, deep wavetable and matrix morphing, and advanced FX processing. Below are some ideas on how to combine this module with other Eurorack modules to push its sonic boundaries.

---

## 1. **Waveform & Wavetable Animation with Sequencers and Modulators**

- **Use Case:** Animate complex wavetables or morphing parameters in real-time.
- **Recommended Modules:**
  - **Generic:** CV Sequencer (e.g., Make Noise René, Arturia Keystep Pro, or Doepfer A-155)
  - **LFO/Envelope Generator** (Mutable Instruments Stages, Xaoc Zadar, or Intellijel Quadra)
- **Technique:**  
  Patch sequenced or random CV to the Morph, X, or Y inputs of the Graphic VCO. This will scan through wavetables and morph between custom-designed waves, yielding ever-evolving timbres for melodic, harmonic, or percussive applications.

---

## 2. **Audio Rate Modulation: FM, RM, and Cross-Modulation**

- **Use Case:** Leverage digital precision of the Graphic VCO’s FM and Ringmod features with other VCOs.
- **Recommended Modules:**
  - Analog VCO (ALM MCO, Mutable Instruments Plaits, or Instruō Cš-L)
  - Random Source or Noise sources (WMD/SSF Ultra-Random Analog, Make Noise Wogglebug)
- **Technique:**
  - Use the **FX CV** or **FM input** to process audio from another oscillator. The unique user-defined waveforms of the Graphic VCO modulated at audio rates can subtly or radically reshape complex tones, metallic percussive sounds, or growling basses.

---

## 3. **Dynamic Signal Processing with Modulation FX**

- **Use Case:** Exploit built-in effects like wavefolding, bitcrush, or overdrive, modulated by complex CV.
- **Recommended Modules:**
  - Complex Envelope Generators/Function Generators (Maths, Joranalogue Contour 1)
  - Step/Random CV Generators (Malekko Voltage Block, Mutable Instruments Marbles)
- **Technique:**
  - Patch evolving or random CV into the FX Amount or FX Parameter CV inputs to drive animated distortion, folding, or lo-fi textures.

---

## 4. **Polyphonic and Multi-Layer Textures via Suboscillator and Layering**

- **Use Case:** Create pseudo-polyphonic or thick unison-style sounds.
- **Recommended Modules:**
  - Audio/cv Mixer (Intellijel Mixup, Mutable Instruments Veils)
  - Quad VCA (ALM Tangle Quartet, Intellijel Quad VCA)
  - Stereo Effects Processor (Tiptop Z-DSP, Happy Nerding FX Aid)
- **Technique:**
  - Utilize the **configurable suboscillator output** (harmonized, offset, or even a different waveform) and mix it with the main output, possibly applying external VCA or stereo processing.
  - Offset or detune the suboscillator for drifting, chorus-like sounds.

---

## 5. **Custom Percussive & Glitch Design**

- **Use Case:** Craft custom transient shapes, glitch hits, and digital percussion.
- **Recommended Modules:**
  - Trigger Sequencer (e.g., Mutable Instruments Grids, 4MS Rotating Clock Divider)
  - Fast Attack/Decay Envelope (ALM Pip Slope, Intellijel Dual ADSR)
- **Technique:**
  - Draw or morph abstract, clicky or noisy waveforms, trigger them in rapid succession, and process further with envelopes or VCAs for custom percussion.
  - Use the FX section's bitcrush and wave distortion for gritty, digital drum hits.

---

## 6. **Live Waveform Drawing for Interactive Performance**

- **Use Case:** Improvise and mutate waveforms and wavetables live.
- **Recommended Modules:**
  - Touch Controllers (Make Noise Pressure Points, Intellijel Tetrapad)
- **Technique:**
  - Assign CV from a pressure or touch controller to Morph or FX parameters, then interactively morph and manipulate the sound directly.

---

## 7. **Wavetable Scanning with Video/CV Sources**

- **Use Case:** Use external sources (including cameras or sensors) for wild wavetable navigation.
- **Recommended Modules:**
  - CV-to-Video or Light-to-CV interfaces (LZX Video Interface, Befaco CV Thing, E-RM Polygogo)
  - Light sensors/Audio-to-CV (e.g., Doepfer A-119)
- **Technique:**
  - Feed dynamic, non-musical CV into the X/Y matrix CV ins for organic, visually-controlled sound transitions.

---

## 8. **External Audio Processing via the Graphic VCO FX**

- **Use Case:** While not a traditional audio processor, some creative patching can treat the VCO as an FX generator/modulator.
- **Recommended Modules:**
  - External-in Interface (ALM S.B.G, Befaco InOut)
  - Envelope Follower (Doepfer A-119)
- **Technique:**
  - Send external audio to the FX CV or Morph inputs, using the external dynamics or audio shape to modulate and mutate the oscillator’s output.

---

## Tips for Integration & Personalization

- **Snapshots:** Combine the above with the snapshot system to instantly recall complex, prepared sound setups for composition or live performance.
- **Matrix Modulation:** Use two LFOs or sequencers to animate both X and Y axes in Matrix Mode for intricate, 2D morphing soundscapes.
- **Precision CV Scaling:** Use precision adders or utility modules (e.g., Mutable Instruments Shades, Tiptop MISO) to fine-tune, invert, or blend modulation sources for even more expressive control.

---

For further modular patch inspiration and signal processing utilities, check out:

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)