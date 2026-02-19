# Schlappi Engineering — Three Body

- [Manual PDF](../../manuals/three_body_manual_01302023a.pdf)

---

[**Download Schlappi Engineering Three Body Manual (PDF)**](https://schlappiengineering.com/static/manuals/Three_Body_Manual.pdf)

---

# Creative Patching Ideas for the Schlappi Engineering Three Body

Three Body is a deep, stereo-capable digital oscillator with phase and frequency modulation, ideal for harmonic, metallic, and generative textures. Its normalized cross-modulation and ratio tracking open up a ton of both classic and experimental FM/PM synthesis. Here are some creative integrations with other modules to push it further:

---

## 1. **Dynamic Timbre Control with Envelopes/LFOs**
- **Idea:** Use modulation sources (envelope generators like Intellijel Quadrax, LFOs like Xaoc Batumi, or even random sources like Make Noise Wogglebug) to control the FM/PM indexes and RATIO CV.
    - **Why:** Introduce evolving movement; envelope-followed FM index will create “pluck” effects, slowly cycling LFOs will expose harmonic movement over time.
    - **Pro Tip:** Mult a single envelope/LFO through stackcables or a buffered mult to modulate both phase and frequency at different depths.

---

## 2. **Spectral Chaos via Cross-Modulation**
- **Idea:** Take a noisy or chaotic modulation source (Schlappi Angle Grinder, Make Noise Maths in cycle mode, or a dedicated chaotic CV generator like Nonlinear Circuits Sloths) and patch it into the PHASE or FM inputs.
    - **Why:** The extended through-zero and phase mod depths will let low-frequency chaos create complex, evolving spectra.
    - **Variation:** For feedback, patch a Three Body output back into its own CV inputs via a VCA, or through effects modules (see #6).

---

## 3. **Eurorack Sequencers and Quantizers for Harmonic Exploration**
- **Idea:** Use a precision quantizer like Mutable Instruments Shades, Ornament & Crime, or TipTop Audio Quantizer to send quantized voltages to the RATIO or V/Oct inputs. Drive with a sequencer (Winter Modular Eloquencer, Make Noise Rene, etc).
    - **Why:** This produces melodies that jump between frequency ratios for unusual, harmonic (or inharmonic) sequences.
    - **Pro Tip:** Random or non-pentatonic scales will emphasize the FM character and push into atonal territory.

---

## 4. **Stereo Expansion and Spatial Patching**
- **Idea:** Exploit Three Body’s stereo Sine/Cosine (or Saw/Cosaw) outs by running them through stereo effects or panners (Make Noise X-Pan, Intellijel Mixup, Happy Nerding FX Aid in stereo).
    - **Why:** The wide stereo effect derived from phase manipulation gives huge, immersive energy—great for ambient or experimental music.
    - **Plus:** Modulate the indexes with differing LFOs for constantly shifting spatial movement.

---

## 5. **External Sync and Clock Division**
- **Idea:** Use a master clock (Pamela’s New Workout, ALM Pamela's Pro Workout, or Tempi) into Three Body’s SYNC inputs to rhythmically lock the oscillators to external clocks for coordinated FM rhythms, clocked LFOs, or clock division.
    - **Why:** Sync to rhythms allows for tightly integrated melodic and percussive patterns; with PLL mode you could even patch in DAW clocks.
    - **Fun:** Mult clock outs to THREE BODY and drum modules for synchronized drum-bass tones.

---

## 6. **Processing Through Filters, Distortion, or Spectral Effects**
- **Idea:** Patch a highly phase- or FM-modulated Three Body output into:
    - Warm analog filters (Mutable Ripples, Doepfer SEM, Erica Synths Wasp)
    - Resonant/overdriven filters (Schippmann VCF-02, Serge VCFQ)
    - Spectral processors (4ms Spectral Multiband Resonator, NEM Ruina Versio)
    - Wavefolders (Intellijel Bifold, TipTop Fold Processor)
- **Why:** The added harmonics from PM/FM patching will yield evolving textures, especially when filtered. Wavefolders can “fold” already complex signals for unusual results.
- **Trick:** Use Three Body’s unmodulated or square output alongside the modulated ones for sub-oscillator bass reinforcement—sum with a mixer or VCA for lush bass.

---

## 7. **Experimental: Audio-Rate Modulation From Other Oscillators**
- **Idea:** Use another digital or analog VCO (Make Noise DPO, Instruo Cs-L, Endorphin.es Furthrrrr Generator) to modulate Three Body’s PHASE or FM inputs at audio-rates.
    - **Why:** FM/PM between dissimilar core oscillators produces both classically metallic (Yamaha DX/FM) and extreme, noisy digital textures.
    - **Tip:** Use a VCA between the external VCO and Three Body’s CV input for dynamic modulation control.

---

## 8. **Generative/Randomized Patching**
- **Idea:** Use random voltage sources (Mutable Marbles, Toppobrillo Sport Modulator, Doepfer A-149-1) into RATIO, FM/PM CV, and/or SYNC for generative aleatoric melodies and rhythmically shifting textures.
    - **Why:** Random modulation + the Three Body’s ratio tracking = endlessly surprising tones and structures.
    - **Try:** Clock random generators from Three Body’s SYNC outputs for tightly integrated generative results.

---

## 9. **Re-Patching Internal Normalization**
- **Idea:** Break normalization to explore new modulations:
    - Patch outer oscillator sine outs into unrelated CV destinations—or take LFOs from elsewhere and patch into OSC phase/frequency CVs.
    - Use stackcables or a matrix mixer (Doepfer A-138m, WMD SSM) to route signals from/to phase, index, and FM in creative blends.

---

## 10. **Oscilloscope and Visual Music**
- **Idea:** With phase-locked (PLL) external SYNC and square wave outs run through video interface modules (LZX Industries, Befaco VCMC), you can do audio-visual experiments like oscilloscope music, XY plotting, or video-rate modulation.

---

## BONUS: *Patch Example - Feedback Glitch Cloud*
- Take Center Cosine out > Delay/Looper (Endorphin.es Milky Way, Mimeophon)
- Delayed/looped output > PHASE 1 index in
- Outer oscillators in RATIO mode, sequence multipliers with random CV
- Use triangle out from Right OSC > FM index of Left OSC
- All outputs sum into a stereo mixer
    - Result: Slow-evolving, glitchy, metallic, almost granular stereo drones with wild, unpredictable motion

---

## Suggested Module Types for Deeper Integration

- **Complex oscillators & wavefolders**
- **Random/sample & hold sources**
- **Multi-channel sequencers/quantizers**
- **Envelope generators and ultra-slow LFOs**
- **Matrix mixers and manual crossfaders**
- **Stereo and multi-band effects**
- **Spectral processors and resonant EQs**
- **Syncable or tap-tempo LFOs**
- **CV-controlled VCAs**

---

> Want to experiment more? Grab the full [Three Body Manual PDF](https://schlappiengineering.com/static/manuals/Three_Body_Manual.pdf).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)