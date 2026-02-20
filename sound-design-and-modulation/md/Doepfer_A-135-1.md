# Doepfer — A-135-1

- [Manual PDF](../../manuals/A135_man.pdf)

---

[Doepfer A-135 VC-Mixer Manual (PDF)](https://doepfer.de/a100man/A135_tech_e.pdf)

---

## Creative Modulation Techniques for the Doepfer A-135 VC-Mixer

The **Doepfer A-135 VC-Mixer** is a voltage-controlled four-channel audio mixer module, making it a flexible tool for complex patches, dynamic mixing, and CV or audio-modulated movement. Below are some patching techniques and modulation approaches to create a variety of modern electronic sound types, including distorted percussive effects, aggressive basslines, and ethereal pads.

---

### Understanding Modulation Points

Each of the four channels features:

- **Audio In** (with level attenuator)
- **Gain** (offset/amplification)
- **CV In** (with attenuator for voltage or audio-rate modulation)

The summed output goes to the main Audio Out. Each channel's VCA responds to linear CV control (0V = off, +5V ≈ full open), with the effective CV being the sum of the Gain setting and external CV input.

---

## 1. Distorted Percussive Sounds

**Patch Example: Glitchy Hats/Claps**

- **Audio Inputs:** Patch different short, noisy, or metallic sources (samples, white noise, cymbals) into channels 1–4.
- **CV Modulation:** Use very fast-decay envelopes or even trigger pulses from modules like A-140, A-142, or function generators as CV inputs on one or more channels.
- **Gain Settings:** Set Gain just above zero so you get output only when a CV pulse comes through.
- **Overdrive/Distortion:**  
  - Crank the **Audio In** and **Output** level going into a wavefolder or external distortion effect after the A-135.
  - Alternatively, set Audio In attenuators high *and* push Gain, sometimes overdriving the summed output internally for clipped, crunchy artifacts.
- **Rhythmic Movement:** Modulate each channel's CV In with rapid, rhythmic triggers or random bursts (try A-118/A-148 random modules).
- **Layering:** Use each channel for a different sound element in your drum patch, stacking and cross-fading for hybrid percussive timbres.

---

## 2. Crazy Basslines (Dubstep/Drum and Bass)

**Patch Example: Wobble/Resonant Bass**

- **Audio Source:** Patch a rich oscillator bass voice (saw, pulse, or FM source) into Audio In 1. Try additional layers or harmonics to the other channels.
- **Movement:** Feed CV Ins with different LFOs (A-145, A-146, A-147), each set at different rates or synced to your clock for wobble effects on each layer.
- **Morphing Bass:**  
  - Use the A-144 Morph Controller to drive the A-135's four CV Ins from a single macro controller. Sweeping the A-144 morphs between channels for hybrid bass sounds.
  - Try crossfading between sub layers, distorted top ends, or modulated harmonics.
- **FM/Audio-Rate Mods:** Route an audio-rate source (from another VCO or even feedback from output) into a channel's CV In for amplitude modulation, resulting in gritty, aperiodic textures and metallic “robotic” bass timbres.
- **Distortion:** After mixing, run the A-135’s out into a wavefolder or distortion module.
- **Dynamic Resampling:** Use an envelope follower on an external drum sound (A-119) to modulate the amplitude of your bassline via CV In for rhythmic “sidechain” effects.

---

## 3. Haunting Atmospheric Pads

**Patch Example: Morphing Ambient Texture**

- **Audio Sources:** Input four different evolving sources — chords, drones, granular textures, field recordings — into Audio Ins 1–4.
- **Morphing Control:**  
  - Use ultra-slow, phase-shifted LFOs or the A-144 Morph Controller to crossfade between pad layers with the CV In attenuators.
  - Use the Gain control to set base levels just below audibility, so layers gently emerge as modulation peaks.
- **Envelopes:** Complex envelopes or random voltage sources can create evolving, ghostly volume movements per layer.
- **Atmospheric FX:**  
  - Try patching heavily delayed/reverbed signals back into other channels (feedback).  
  - Experiment with modulating CV Ins using an external audio signal for subtle AM/ringmod shimmer.
- **CV Modulation:** Use aftertouch, modulation wheel, or other MIDI-to-CV sources for expressive, hands-on crossfading during performance.

---

### Additional Tips

- **Use negative CVs:** Set Gain above zero, and use bipolar CVs (from LFOs or random sources). When CV goes negative, it cancels the base level, so you get negative amplitude “ducking” effects.
- **Mix audio-rate and slow modulation:** Patch audio signals into CV In for tremolo/ringmod effects, or combine slow envelope/LFO and fast audio-rate sources for layered dynamics.

---

## References

- [Doepfer A-135 VC-Mixer Manual (PDF)](https://doepfer.de/a100man/A135_tech_e.pdf)
- [Doepfer A-135 Product Page](https://doepfer.de/a135.htm)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)