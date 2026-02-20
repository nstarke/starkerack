# Doepfer — A-138B

- [Manual PDF](../../manuals/A138_man.pdf)

---

[Doepfer A-138 Mixer Manual (PDF)](https://doepfer.de/a100man/A138_Manual.pdf)

---

# Creative Sound Design with the Doepfer A-138 Mixer (Eurorack)

The **Doepfer A-138** (System A-100 Mixer) is a simple but versatile four-channel mixer module for both CV and audio, equipped with individual input attenuators and a master attenuator. Despite being a straightforward module, you can use its features in combination with other Eurorack modules to explore creative, modulated, and highly original sound design for percussive distortion, gnarly basslines, and eerie atmospheres.

Below, you'll find usage strategies tailored for:
- **Distorted Percussive Sounds**
- **Dubstep/Drum & Bass Basslines**
- **Haunting Atmospheric Pads**

---

## 1. **Distorted Percussive Sounds**

### Techniques
- **Feedback Loops**: Patch the output of the A-138 back into one of its own inputs via a distortion, wavefolder, or filter module. This can push percussive signals into wild overdrive.
- **Mixing CV & Audio**: Send short envelopes or triggers (used as CV) into one channel and audio percussive samples (or noise sources) into another. The envelopes can shape the amplitude, especially if you modulate the level controls with automation.
- **CV Offset Distortion**: Use the JP4 jumper to enable the offset function on Input 1 (preferably set to positive offset, 0…+5V). If nothing is patched to Input 1, the mixer will inject an offset voltage, which can bias or push signals into clipping/distortion when combined with hot audio levels.

**Patch Idea:**
- Input 1: Leave unpatched (offset active, jumper set to +5V)
- Input 2: Drum trigger or audio click
- Input 3: Colored noise
- Input 4: Output of a distortion or wavefolder (part of a feedback loop)
- Output: To VCA/Filter/Additional FX

*Drive the input and output gain controls high for extra grit.*

---

## 2. **Crazy Basslines (Dubstep/Drum & Bass)**

### Techniques
- **Layering CV Modulation**: Use the ‘a’ version (linear) and mix LFOs, envelopes, or step-sequencer CVs on three channels, then patch the combined modulation to a VCF, VCO FM, or a waveshaper.
- **Cross-Modulation**: Mix audio-rate modulated CV (e.g., another oscillator at audio rate) with pitch or filter envelope CVs.
- **Bass Layering with Distortion**: Send different waveforms (triangle, saw, square) from VCOs into the mixer, sum them, and then send the output to a waveshaper, distortion, or filter to achieve “growl.” Use the mixer attenuators to control how much harmonic or sub content goes to the next stage.

**Patch Idea:**
- Input 1: Sawtooth VCO
- Input 2: Square VCO, tuned to sub
- Input 3: Audio-rate LFO or modulated noise (for movement)
- Input 4: Envelope- or sequencer-driven FM or PWM source
- Output: To distortion/filter, then VCA

*Automate input and output levels using external CVs or by riding the mixer controls live for evolving, modulated bass.*

---

## 3. **Haunting Atmospheric Pads**

### Techniques
- **CV Blending for Parameter Modulation**: Use A-138a (linear) to sum slow LFOs, random voltages, and aftertouch for modulating filter cutoff or VCA amplitude. The summed, evolving CV creates lush movement.
- **Audio Texture Layering**: Patch several atmospheric sources—long reverb/delay returns, granular samples, and drone oscillators—into the mixer. Adjust levels for subtle spectral blending.
- **Dynamic Offsets/Fading**: The JP4 offset feature (Input 1 unpatched) can introduce slow-rising drifts or spatial bias in a feedback effect chain or as a pad’s volume modulator.
- **CV/FX Crossfading**: Pan between four layers of sound using the mixer’s attenuators for continuously morphing textures (send the output to stereo FX for depth).

**Patch Idea:**
- Input 1: Unpatched (offset enabled for DC drift or amplitude rise)
- Input 2: Slow LFO or random sample/hold
- Input 3: Granular ambient sample
- Input 4: Drone oscillator
- Output: To lush reverb/chorus, then stereo output

*Animate input attenuators for evolving “ghostly” dynamics in the soundscape.*

---

## **Additional Modulation Tips**
- **Voltage Control**: While not CV-controllable, you can use external VCAs before each input to dynamically modulate each channel.
- **Patch Feedback Loops**: Patch the mixer output to effect modules and back into an input for nonlinear, evolving, and sometimes chaotic results.
- **Use as CV Processor**: By creatively patching envelopes, LFOs, and DC offsets, the A-138 can blend complex modulation sources for more organic modulation of destination modules.

---

## **Further Exploration**

- [Doepfer A-138 Mixer Manual (PDF)](https://doepfer.de/a100man/A138_Manual.pdf)
- 🔗 [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)