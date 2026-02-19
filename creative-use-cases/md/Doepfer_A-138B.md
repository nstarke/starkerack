# Doepfer — A-138B

- [Manual PDF](../../manuals/A138_man.pdf)

---

[Doepfer A-138 MIXER Manual PDF](https://www.doepfer.de/a100_man/A138_Manual.pdf)

---

# Creative Uses for Doepfer A-138 Mixer (System A-100)

The A-138 is a versatile 4-channel mixer, available with linear (A-138a, best for CVs) or logarithmic (A-138b, best for audio) response. Its ability to mix both audio and control voltages, plus its output attenuator and optional offset on input 1, makes it a powerful utility in any Eurorack system.

Below are creative ways to integrate it with other modules for exciting, musical, or experimental results:

---

## Audio Processing & Mangling

### 1. **Submix & VC-Morphing**
- **Use Case:** Combine several oscillators (e.g., Doepfer A-110, Mutable Instruments Plaits, or a Make Noise STO) for complex, evolving timbres.
- **How:** Patch multiple VCO outputs into the A-138 inputs. Morph between them live or with automation for layered or crossfaded textures before sending to a VCF or external effects.

### 2. **Waveshaping Pre/Post-mix**
- **Use Case:** Place the A-138 before or after a waveshaper (e.g., Intellijel Bifold, Doepfer A-137-1) to blend various harmonics, subharmonics, or waveforms for unique distortion or saturation effects.

### 3. **Mixing Audio with Noise/Modulation**
- **Use Case:** Blend your main synth voices with noise sources (A-118 Noise/Random) or filtered audio from other modules to add texture or grit to the master signal.

---

## Creative CV Mixing

### 4. **Animated Modulation Sources**
- **Use Case:** Use A-138a to blend LFOs (A-145), envelopes (A-140), random sources, and manual CV for constantly evolving modulation.
- **Recommended Modules:** A-145 (LFO), Maths (Make Noise), Quadrax (Intellijel).

### 5. **CV Summing & Offset Tricks**
- **How:** Utilize the offset generator feature (on inputs with nothing patched) to add or subtract DC offsets to your modulation — apply this to VCO FM attenuators or filter CV for wild modulations.

---

## Feedback Patching & Sound Design

### 6. **Mixer Feedback Loops**
- **Use Case:** Create feedback by patching the output of a filter, distortion, or delay back into one input of the A-138 along with the dry signal. Adjust levels for controllable feedback ranging from subtle harmonics to screaming chaos.
- **Recommended Pairings:** Erica Synths Fusion Delay, Doepfer A-124 Wasp Filter, Mutable Instruments Rings.

### 7. **Signal Inversion via Offset**
- **How:** Combine the offset jumper with negative polarity to invert a signal — useful for phase cancellation or anti-phase processing in stereo rigs.

---

## Utility & Performance Tricks

### 8. **Master Volume & Performance Fader**
- **Use Case:** Use the output attenuator as your final "volume" for a group of voices or modulation. Great for live sets to fade in/out submixes, sequences, or entire stems.

### 9. **Stereo/EQ Networking**
- **How:** Chain two A-138s for makeshift panning (left mixer = left channel, right = right) or to mix wet/dry signal paths for parallel processing (e.g., blend dry VCO with effected daughter signal).

---

## Experimental Patch Ideas

### 10. **Pseudo-Ring Modulation**
- Mix two audio-rate oscillators and a sub-audio source (like a slow LFO) in the A-138, then send the output to a VCA controlled by yet another modulator for clangorous, Autechre-style tones.

### 11. **MIDI or Trigger Bus Mixing**
- Use to combine different gate or trigger streams (from sequencers, logic modules, or random sources) to make complex rhythmic patterns for percussion or synced modulation.

---

### Hot Tip
The A-138 is unassuming but is the cornerstone of creative patching. Explore it as a dynamic "hub" — not just an end-of-chain utility!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)