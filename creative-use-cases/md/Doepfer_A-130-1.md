# Doepfer — A-130-1

- [Manual PDF](../../manuals/A1301_man.pdf)

---

[**Doepfer System A-100 VCA A-130 / A-131 Manual (PDF)**](https://www.doepfer.de/a100man/A130_131_anl.pdf)

---

# Creative Patch Ideas for Doepfer A-130 (Linear VCA) & A-131 (Exponential VCA)

The A-130 and A-131 are extremely versatile VCAs at the heart of any modular system, going far beyond simple volume control. Their dual audio inputs, dual CV inputs with attenuators, and linear/exponential responses make them valuable tools in both audio and control voltage processing. Here are creative ways to get more from these modules:

---

## 1. Sidechain Compression (Ducking Effect)

- **Modules needed:** Envelope Follower, LFO or Gate/Trigger Module, Noise Source, Audio Mixer
- **Patch Idea:**
  - Patch your main audio signal (e.g., bassline or pad) into Audio In 1.
  - Use an envelope follower module (such as Doepfer A-119) to convert an incoming kick drum or rhythmic audio to a CV.
  - Send this CV to CV In 1 (or CV In 2 for attenuation) of the VCA.
  - Fine-tune the gain and CV attenuation so that each time the kick hits, the bass (or other signal) is reduced in level — i.e., "ducked."
  - Try swapping the exponential (A-131) and linear (A-130) response based on the musical result.
- **Result:** Classic "pumping" effect as heard in electronic dance music.

---

## 2. Automated Crossfading / Panning

- **Modules needed:** Two sound sources, one LFO (or random/slew generator like Maths)
- **Patch Idea:**
  - Patch Audio Source A to Audio In 1, Source B to Audio In 2.
  - Use a slow LFO (triangle or sine wave) into CV In 2.
  - Set the VCA so only one input passes when CV is low and the other when CV is high.
  - You can use linear for equal-power crossfading, or experiment with exponential for more dramatic transitions.
- **Alternative:** Use two VCAs, one for each channel, and use complementary (inverse) CVs for stereo panning.

---

## 3. Amplitude Modulation & Ring Modulation

- **Modules needed:** Audio rate oscillator (VCO), LFO, additional VCA if available
- **Patch Idea:**
  - Audio signal (VCO A) into Audio In 1 or 2.
  - Modulator signal (VCO B or LFO) into CV In 1 (or CV In 2 if you want to shape depth with the attenuator).
  - Set VCA gain above zero for classic amplitude modulation, or to zero for more ring-mod-like results.
- **Pro Tip:** Patch an LFO into the gain CV for tremolo; use an audio-rate VCO for ring modulation/complex overtones.

---

## 4. Dynamic Waveshaping with Control Voltages

- **Modules needed:** Audio source, random source (e.g., Wogglebug, Sample & Hold), sequencer
- **Patch Idea:**
  - Feed a steady audio waveform (saw/square) into Audio In 1.
  - Use random voltages or sequenced voltages into the CV inputs to morph the loudness in a stepped fashion.
  - Combine different CV sources for evolving textures (e.g., slow LFO + stepped random + manual control).
- **Result:** Rhythmic stuttering, gating, and generative dynamics.

---

## 5. Envelope-VCA Chaining for Custom Attack/Release Curves

- **Modules needed:** Two envelopes (ADSR), two VCAs (A-130 and/or A-131)
- **Patch Idea:**
  - Use one envelope to control gain of VCA 1, another for VCA 2 (in series).
  - CV-link the envelopes (A output into next envelope's gate) to create multi-segment, complex level shapes.
- **Result:** Custom multi-stage dynamics (soft attack, punchy middle, slow fade).

---

## 6. Voltage-Controlled Feedback Circuits

- **Modules needed:** Mixer, delay or reverb, VCA, external or in-system processor
- **Patch Idea:**
  - Send audio out from a delay/reverb, pass it through the VCA, and return to the effect’s input.
  - Use LFO, envelope, or random CV to modulate the VCA—this lets you dynamically sculpt the depth and intensity of feedback.
- **Result:** Animate space and time effects while avoiding runaway self-oscillation.

---

## 7. VCA as Voltage-Controlled Attenuator (for Modulation Control)

- **Modules needed:** LFO or modulation source, destination module with CV input (e.g., filter cutoff, oscillator FM)
- **Patch Idea:**
  - Pass your modulation source through A-130/A-131 before sending it to the modulation destination.
  - Modulate the VCA’s gain/CV for dynamic depth scaling—e.g., envelope controls LFO depth to VCF cutoff.

---

## Module Recommendations for Pairing
- **Random/Chaos CV:** MakeNoise Wogglebug, Doepfer A-149-1
- **Function/Envelope:** MakeNoise Maths, Intellijel Quadra, Doepfer A-140
- **MIDI-to-CV:** Expert Sleepers Disting, Doepfer A-190 series
- **Utility Mixers/Multiples:** Mutable Instruments Shades, Doepfer A-138
- **Logic/Gates:** Doepfer A-166 Dual Logic
- **Audio Rate Modulation:** Any analog VCO, or digital oscillator

---

## Bonus Tip: Experimental Audio-Rate "CV" Processing
- Try sending audio signals to the CV inputs (not just LFO or envelopes). This can result in audio-rate amplitude modulation and strange sideband spectra, especially intriguing on the exponential VCA.

---

**Remember:** VCAs are the magic dust of modular systems. Use them not just for audio loudness, but for dynamically sculpting any voltage—think of them as voltage-controlled "shapes" for everything!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)