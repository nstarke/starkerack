# Intellijel — Micro VCF

- [Manual PDF](../../manuals/uvcf_manual_2021.08.15.pdf)

---

[Download the Intellijel µVCF Manual (PDF)](https://intellijel.com/downloads/manuals/uVCF/uVCF_Manual_2021.pdf)

---

# Creative Eurorack Patching Ideas with the Intellijel µVCF

The **Intellijel µVCF** is a compact, versatile state variable filter that excels not just as a filter, but also as a unique sound source and modulation processor. Here are some creative patching and integration ideas to explore fresh sonic ground in your modular setup.

---

## 1. **Self-Oscillating Sine VCO**

- **Setup:** Remove the input signal, turn Q to maximum. The µVCF will self-oscillate and generate a stable sine wave.
- **Expand:** Use FM1 as a 1V/Oct pitch CV input (fully clockwise on the attenuator). You can now sequence melodies using any sequencer, quantizer, or analog keyboard.
- **Recommended Modules:** 
    - [Intellijel Metropolix](https://intellijel.com/shop/eurorack/metropolix/) for sequenced melodies
    - **Generic:** Any sequencer or quantizer

---

## 2. **Multi-Output Filtering for Parallel Processing**

- **Setup:** Pass the same sound source (e.g., complex oscillator, chord, drum loop) to the µVCF input. Send the LPF, HPF, and BPF outputs to different FX chains, VCAs, or mixes.
- **Creative Twist:** Crossfade or pan the different outputs for morphing filter textures, or use a switch module (like the WMD Sequential Switch) for rhythmically swapping filter flavors.
- **Recommended Modules:** 
    - [Intellijel Planar2](https://intellijel.com/shop/eurorack/planar2/) for manual/CV crossfading
    - [WMD Sequential Switch Matrix](https://wmdevices.com/) for rhythmically cycling outputs
    - **Generic:** Stereo/multichannel mixers

---

## 3. **Filter FM: Additive or Complex Modulation**

- **Setup:** Patch LFOs, envelopes, or even audio-rate oscillators into FM1 and FM2. 
- **Bipolar Fun:** Use the bipolar attenuator (FM2 knob) to invert modulation polarity on the fly.
- **Audio-Rate FM:** Try running a second oscillator (tuned to harmonic or inharmonic intervals) into FM2 for classic filter FM “zing” or metallic sounds.
- **Recommended Modules:** 
    - [Make Noise Maths](https://makenoisemusic.com/modules/maths) (complex envelopes/LFO)
    - **Generic:** Any VCO, LFO, or envelope generator

---

## 4. **Dynamic Timbre Animation with Envelopes & LFOs**

- **Setup:** Envelope to FM1; LFO to FM2. Set FM1 for tracking, use FM2 for slow movement or vibrato.
- **Hack:** Try patching gate signals or clocks into FM2, and experiment with the attenuator for rhythmic cutoff “stepping.”
- **Recommended Modules:** 
    - [Intellijel Quadra](https://intellijel.com/shop/eurorack/quadra/) (multi-envelope)
    - [ALM Busy Circuits Pam’s New Workout](https://busycircuits.com/alm017/) for clocked modulation

---

## 5. **Spectral “Split” via Parallel Filtering**

- **Setup:** Use a signal splitter (or mult) to send audio both pre- and post-filter.
- **Mix:** Wet/dry mix or parallel compression/EQ can be achieved with a mixer—process the filtered and dry sounds separately for punchy, custom results.
- **Recommended Modules:** 
    - [Intellijel Mixup](https://intellijel.com/shop/eurorack/mixup/) (compact audio mixer)
    - **Generic:** Buffered multiple

---

## 6. **Noise Shaping for Percussion and Texture**

- **Setup:** Patch white or pink noise into the µVCF. Sweep FREQ and Q for sweeps and wind noises, resonant snare/hi-hat shaping, or unusual percussive textures.
- **Tip:** Gate or envelope the input attenuator for percussion and rhythmic gating.
- **Recommended Modules:** 
    - [Mutable Instruments Peaks](https://mutable-instruments.net/peaks/) (envelopes, LFOs)
    - [Doepfer A-118](https://www.doepfer.de/A118.htm) (noise source)

---

## 7. **Voltage-Controlled Stereo Animation**

- **Setup:** Use two µVCF modules in parallel on the same source, modulate their cutoffs with different LFOs/EGs, and pan their outputs hard left/right for dramatic stereo movement.
- **Recommended Modules:**
    - **Second µVCF module**
    - [Happy Nerding PanMix Jr](https://happynerding.com/) (stereo mixer)

---

## 8. **Wavefolder/Distortion Pre- or Post-Filtering**

- **Setup:** Patch a wavefolder, distortion, or waveshaper before or after the filter to carve out exciting harmonics and tame or enhance them with resonance and cutoff.
- **Recommended Modules:** 
    - [Intellijel Bifold](https://intellijel.com/shop/eurorack/bifold/)
    - [Tiptop Audio Fold Processor](https://tiptopaudio.com/fold/)

---

## 9. **Triggerable Sound Effects (Karplus-Strong Style Plucks)**

- **Setup:** Patch noise or a short impulse to the input, set Q high but below full resonance, and ping (or envelope) the frequency for plucked string or percussive tones.
- **Recommended Modules:**
    - [Mutable Instruments Marbles](https://mutable-instruments.net/modules/marbles/) (random trigger source)
    - [Intellijel Quadrax](https://intellijel.com/shop/eurorack/quadrax/) (fast envelopes)

---

## 10. **CV-Controllable Feedback Loop**

- **Setup:** Patch one of the filter outputs (e.g., LPF) back into the input via a VCA, and modulate the feedback amount for evolving resonant effects.
- **Warning:** Adjust feedback carefully to avoid runaway self-oscillation.
- **Recommended Modules:**
    - [Intellijel VCA 1U/2U](https://intellijel.com/shop/eurorack/vca/)
    - **Generic:** Any linear VCA

---

## Bonus Tip: Use ModularGrid!  
Use [ModularGrid](https://modulargrid.net/) to virtually arrange your modules and plan power/hp usage for your system as you explore new patching possibilities.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
