# Tiptop Audio — MISO

- [Manual PDF](../../manuals/Tiptop_Audio_miso.pdf)

---

[**Tiptop Audio MISO Manual (PDF)**](http://tiptopaudio.com/manuals/MISOManual.pdf)

---

# Creative Modulation With Tiptop Audio MISO  
_A Guide for Experimental Eurorack Sound Design_

The Tiptop Audio **MISO** module is a Swiss army knife for control voltage (CV) and audio signal processing. Because it allows you to **Mix, Invert, Scale, Offset** (hence, MISO) and crossfade signals, it’s perfectly suited for pushing the boundaries of modular synthesis—especially in the domain of **distorted percussive sounds, aggressive basslines, and atmospheric pads**.

## Core Functions Recap
- **Scale/Invert:** Control gain and invert signals for phase/flavor changes.
- **Offset:** Add/subtract DC voltage for moving signals into the right range or to generate modulation manually.
- **Mix:** Merge multiple CVs or audios for layered, complex modulations.
- **Crossfade:** CV-controllable morphing between two mixes (top and bottom sections).

---

## 1. Distorted Percussive Sounds

**Strategy:** Use MISO to combine & distort envelopes, gates, and audio sources, making "clipped" or highly animated shapes.

**Patch Examples:**
- **Voltage Folding Drum Edge:**  
  1. Patch two envelopes or an envelope + gate (e.g., two channels from a Maths, or two function generators) to IN 1 and IN 2 of the top MISO.
  2. Crank the Scale/Invert knobs so signals are mixed at high gain or inverted for aggressive transients.
  3. Add positive or negative Offset to ensure signals are always above or below zero—this creates asymmetric "clicks" or crisp edges.
  4. **Mix** out (1+2) to a VCA or send it directly to a drum voice’s CV input.
- **Saturated Noise Snare:**  
  1. Send white noise to channel A, envelope to channel B.
  2. Use Scale/Invert on A for harshness; offset B for snappy decay.
  3. Output A+B mix to a distortion or wavefolder for extra grit.

**Pro Tip:** Maxing the Scale and using offset to clip the summed voltage can result in “hard” percussive artifacts, especially when mixed with audio.

---

## 2. Crazy Basslines: Dubstep/Drum and Bass  

**Strategy:** Layer and cross-modulate LFOs, envelopes, and audio to shape wild, evolving bass CV or audio signals.

**Patch Examples:**
- **Dual LFO Shaping:**  
  1. Patch a slow LFO to IN 1, audio-rate LFO to IN 2.
  2. Scale both to taste, and invert one of them for phase cancellation/folding.
  3. Mix OUT (1+2) to a filter cutoff or oscillator FM input of your bass voice.
- **Bass Growl Crossfade (Wub-Wub):**  
  1. Use top MISO (1+2) for LFO/envelope shaping, bottom (A+B) for pitch/rhythm CVs.
  2. Patch crossfade CV input with a sharp envelope or sequencer.
  3. Dial the crossfader knob or modulate for animated, morphing filter sweeps or “talking bass” effects.

**Pro Tip:** Cranking Scale while adding an inverted Offset introduces classic dubstep “honk” and DnB “wobble” by flipping LFO shapes on the fly.

---

## 3. Haunting Atmospheric Pads

**Strategy:** Blend multiple slow-moving modulation sources, gentle offsets, and subtle inversion to create drifting, eerie textures.

**Patch Examples:**
- **Complex LFO Sum for Pad Sweep:**  
  1. Connect two “out of phase” LFOs to IN 1 and IN 2.
  2. Fine-tune Scale/Invert for slow evolving movement.
  3. Add slight Offset for a wandering center.
  4. Output to multiple destinations (filter, VCA, reverb dry/wet).
- **Crossfade Quad Movement:**  
  1. Fill all four inputs (IN 1, IN 2, A IN, B IN) with different slow LFOs or envelope followers.
  2. Use the crossfader, manually or with a random CV source, to interpolate between complex modulations.
  3. Route to pad filters, VCA amplitude, or even effects sends for mesmerizing pad morphs.

**Pro Tip:** The mix and crossfade outputs are perfect for feeding into reverbs or delays, baking in spectral or dynamic movement.

---

## Advanced Tips
- Chain the MISO outputs back into its own inputs (feedback) for nonlinear, chaotic control voltage patterns—great for glitch percussion.
- Use the Offset knobs with no input to generate pure DC—combine with external random or stepped CV for more unpredictable modulation.
- Modulate the **crossfader input** with audio-rate signals for ringmod-like AM effects or crazy filter sweeps.

---

## Resources

- [**Tiptop Audio MISO Manual (PDF)**](http://tiptopaudio.com/manuals/MISOManual.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

Feel free to ask for specific patch diagrams or further ideas!