# Blue Lantern Modules — Voks Analog Filter

- [Manual PDF](../../manuals/BLM Voks Analog Filter.pdf)

---

[BLM Voks Analog Filter Manual (PDF)](https://www.bluelanternstore.com/store/p133/BLM_Voks_Analog_Filter.html#/)

---

# Creative Patch Ideas for the BLM Voks Analog Filter

The **BLM Voks Analog Filter** is a versatile, Polivoks-inspired analog filter with unique “Unstable Brite Mode” and a diode limiter option. It offers both 12dB lowpass and 6dB bandpass outputs, with convenient input and CV configurations. Below are creative ways to integrate it into your Eurorack system!

## 1. **Classic Acid Basslines**
- **Modules Needed**: Analog oscillator (e.g., Mutable Instruments Braids, Dreadbox Hysteria), envelope generator (e.g., Maths or Intellijel Quadra), sequencer.
- **Patch**: 
  1. Send a saw or square wave from your oscillator into the attenuated input.
  2. Envelope generator output to the CV input for snappy filter modulations.
  3. Use the 12dB lowpass out for the classic squelchy acid character, especially engaging “Unstable Brite Mode” for extra drive and gnarl.
  4. Optionally insert a distortion or wavefolder post-filter for added aggression.

## 2. **Fuzzy Dual-Band Filtering**
- **Modules Needed**: Stereo mixer, two VCAs.
- **Patch**: 
  1. Patch the same sound source to the Voks filter.
  2. Take both LPF and BPF outs to separate VCAs.
  3. Use an LFO or envelope to crossfade between LPF and BPF outs, then sum them in a stereo mixer for timbral movement.
  4. This can turn simple drones into swirling, evolving textures.

## 3. **FM Filter Freakouts**
- **Modules Needed**: LFO, random voltage source, audio-rate oscillator.
- **Patch**: 
  1. Patch random voltage or audio-rate oscillator to the bipolar FM input for wild, unpredictable modulations.
  2. Try clocking an LFO at audio rates for intense FM effects, altering harmonics and resonance character significantly.

## 4. **Waveshaping Percussion**
- **Modules Needed**: Drum module or external drum machine, envelope generator.
- **Patch**: 
  1. Feed percussive sounds through the Voks filter with the diode limiter enabled.
  2. Envelope-follower modules can extract CV from the drum signal to modulate cutoff, causing filter to “react” to drum energy.
  3. Output to distortion, wavefolder, or granular module for added grit.

## 5. **Unstable Resonant Feedback**
- **Modules Needed**: Mixer with attenuator, delay module, VCA.
- **Patch**: 
  1. Mult the BPF or LPF output back into the filter’s input via an attenuated mixer.
  2. Control feedback amount with a VCA, and use CV to modulate the VCA for feedback sweeps.
  3. Run in Unstable Mode for unpredictable resonant feedback bursts—great for building industrial/noise textures.

## 6. **Dynamic Filter Panning**
- **Modules Needed**: Dual filter (optional), quad VCA or stereo mixer, modulation source (LFO, sequencer).
- **Patch**: 
  1. Use both outputs (LPF & BPF) as stereo channels.
  2. Modulate L/R balance with an LFO or sequencer for real-time stereo movement.
  3. Add a phaser or chorus after for lush, animated stereo filtering.

## 7. **Vocal Formant FX**
- **Modules Needed**: Fixed filter bank, additional bandpass filter, envelope follower.
- **Patch**: 
  1. Stack the Voks’ bandpass output with other bandpass filters to form multi-peak “formant” structures.
  2. Modulate cutoff points for vowel-like motion.
  3. Process vocals through for Cyborg/Demonic vocoder-like sounds.

---

### Recommended Module Types and Specifics

- **Oscillators**: Mutable Instruments Plaits/Braids, Doepfer A-110, Erica Synths Pico VCO
- **Envelope/LFO Sources**: Maths, Make Noise Function, Intellijel Quadrax, XAOC Batumi
- **Random/Chaos Modulation**: Wogglebug, SSF Ultra-Random Analog, Joranalogue Orbit 3
- **Mixers/VCA**: Intellijel Quad VCA, Mutable Instruments Veils, Befaco STMix
- **Additional FX**: Disting mk4 (for flexible effects), Happy Nerding FX Aid

---

**Generated With Eurorack Processor**  
[https://github.com/nstarke/eurorack-processor](https://github.com/nstarke/eurorack-processor)