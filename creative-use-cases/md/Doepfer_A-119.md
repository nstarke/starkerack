# Doepfer — A-119

- [Manual PDF](../../manuals/A119_man.pdf)

---

[Doepfer A-119 Ext. Input / Envelope Follower Manual PDF](https://doepfer.de/a100man/A119_anl_e.pdf)

---

# Creative Eurorack Patching with the Doepfer A-119

The **Doepfer A-119 External Input / Envelope Follower** is a powerful tool for interfacing the outside world with your Eurorack system. Not only does it amplify and condition external audio signals (e.g., microphones, guitars, line signals), but it can also generate envelope and gate signals from those sources. This transforms **any audio**—from found sounds to percussion, vocals to field recordings—into dynamic synth control signals. Below are techniques and patch ideas to creatively integrate the A-119 with other modules for inspiring results.

---

## 1. **Envelope-Followed Effects (Dynamic Modulation)**
- **Patch:** Take an external sound (e.g., drum machine, voice, acoustic instrument) into the A-119, and patch the **Envelope Out** to modulate the cutoff of a VCF (Filter), resonance, or wavefolder.
- **Module Recommendations:** Mutable Instruments Ripples (VCF), Intellijel Polaris, Make Noise QPAS, or Dreadbox Euphoria
- **Result:** The tonality of your synth changes in real-time following the energy and dynamics of your external audio.

---

## 2. **Sidechain Compression/Ducking**
- **Patch:** Envelope or gate out to control a VCA affecting a synth/drum layer. When the input audio (e.g., a vocal or drum) is present, the synth ducking occurs.
- **Modules Needed:** VCA (e.g., Doepfer A-130, Intellijel Quad VCA), optional A-175 (for inverting envelope), ADSR for shaping
- **Result:** Classic sidechain "pumping" or ducking, as in dance music. Great for clearing space or creative rhythmic interplay.

---

## 3. **External Audio as Sequencer Trigger/Clock Source**
- **Patch:** Use transients from drum machines or acoustic percussion to generate gates at the A-119's **Gate Out**. Use these to clock a sequencer, trigger envelopes, or advance a sample & hold.
- **Module Recommendations:** Mutable Instruments Grids (rhythmic sequencer), ALM Pamela’s NEW Workout (clock divider), Doepfer A-160 (clock divider), Turing Machine/Random Looping Sequencer
- **Result:** Rhythms from your external source drive your modular’s timing.

---

## 4. **Envelope-Controlled Synth "Vocoder-lite"**
- **Patch:** Run your voice into the A-119. Use the **Envelope Out** to control the volume (VCA), pitch (via VCO FM/AM), filter, or effects parameters (delay/reverb send) on a synth voice or noise source.
- **Modules Needed:** VCA, VCF, analog effects (delay, phaser, spring reverb), noise or basic VCO
- **Result:** External speech/voice gestures become synth modulations for expressive, voice-controlled sounds.

---

## 5. **Gated Ring Mod/VCA for Percussive Squelch**
- **Patch:** Run the amplified output from the A-119 to a ring modulator (A-114, Make Noise ModDemix, Frequency Central System X Ring). Use the **Gate Out** to open a VCA at the output.
- **Modules Needed:** Ring modulator, VCA, optional LFO for additional movement
- **Result:** Noisy, percussive, or voice-based source is ring modulated with another oscillator, gated cleanly to eliminate bleed when the signal is at rest.

---

## 6. **Slew-Limited Envelope for Smooth Control**
- **Patch:** Take Envelope Out, run into a slew limiter (like A-170 or Mutable Instruments Stages in slew mode) to smooth abrupt transients; use this to modulate pitch, filter, or effect parameters.
- **Result:** Instead of harsh, spiky modulation, you get smooth, musical shape-following LFOs, perfect for timbral morphing or spatial effects.

---

## 7. **Audio-Driven Random/Chaos Modulation**
- **Patch:** Feed Envelope or Gate Out into a sample & hold, random voltage generator, or logic module such as Mutable Instruments Kinks, Doepfer A-149-1, or a noise module.
- **Result:** The unpredictable contours of your real-world audio sculpt randomized or semi-random events in your modular patch.

---

## 8. **Live Instrument Integration/Processing**
- **Patch:** Run a guitar, bass, voice, or acoustic instrument through the A-119 for live processing. Use the amp’d output for effects (delays, reverbs, loopers) and the envelope/gate for hands-free modulation (e.g., envelope controls reverb mix, gate triggers a sample playback).
- **Modules Needed:** Stereo effects module (e.g., Make Noise Mimeophon, Tiptop Z5000), sampler/looper (e.g., 4ms Stereo Triggered Sampler)
- **Result:** Modular becomes an interactive, expressive effects processor and controller for live instruments.

---

## 9. **Interactive Performance/Installation Control**
- **Patch:** Feed in environmental or ambient sounds from contact mics, field recorders, or piezos. Use envelope/gate to control lighting, visuals, or generative CV via modules like LZX Industries (for visuals/video synthesis).
- **Result:** Sound-reactive performances, installations that are controlled by the surrounding real-world soundscape.

---

## Tips, Tricks, and Further Exploration

- **Threshold Setting:** Experiment with Gate threshold for sensitive, dynamic triggers or robust, percussive gates.
- **Stereo Processing:** Though A-119 is mono, use two for stereo external audio (e.g., two mics, or left/right channels).
- **Feedback/Resampling:** Route modular outputs back to A-119 for self-patched feedback envelopes/gates that interact with your own system’s loops.

---

## Honorable Mentions: Other Modules to Pair With
- **Envelope Generators:** Maths, Make Noise Function, Intellijel Quadrax, for additional shaping/morphing.
- **Logic Modules:** Mutable Kinks, Doepfer A-166 (logic), for complex behaviors.
- **Slew/Glide:** Doepfer A-170, Mutable Stages, for smoothing envelope outputs.
- **Random:** A-149-1, Noise Engineering modules for further CV possibilities.

---

> [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---