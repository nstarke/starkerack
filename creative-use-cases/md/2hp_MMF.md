# 2hp — MMF

- [Manual PDF](../../manuals/2hp_MMF.pdf)

---

[Download the MMF Manual (PDF)](sandbox:/mnt/data/MMF_manual.pdf)  
*(Replace this with the actual public link if available, as "sandbox" links are not accessible outside of this Chat environment)*

---

# Creative Patching Ideas for the MMF 2HP Multimode Filter

The **MMF** is a versatile 2HP analog multi-mode filter offering simultaneous low-pass (LP), high-pass (HP), and band-pass (BP) outputs with voltage control over the cutoff frequency and resonance. Here’s how you can stretch its sonic capabilities in your Eurorack system:

## 1. **Triple-Output Parallel Processing**

- **Try This:** Split a complex audio source (e.g., a multi-oscillator drone or drum loop) into all three outputs (LP, HP, BP).
- **Process Together:** Send each output to different destinations for processing:  
  - LP → Reverb (e.g., Erica Synths Pico DSP)  
  - BP → Delay (e.g., Make Noise Mimeophon)  
  - HP → Wavefolder or Distortion (e.g., Tiptop Audio Fold Processor or Intellijel uFold)
- **Combine Back:** Mix these individually processed outputs for a rich, multi-layered effect.

## 2. **Dynamic Spectral Animation Using CV**

- **Cutoff Modulation:** Patch an LFO (e.g., Doepfer A-145, or Maths ch1/4 if available) into the **FREQ** CV input for slow morphing or fast squelchy sweeps.
- **Envelope Animation:** Use an envelope generator (e.g., Make Noise Function, Intellijel Quadra) to CV the cutoff or resonance, shaping filter movement with your note events.
- **Sequencer Pings:** Use rhythmic gates/triggers from a sequencer (e.g., Pamela’s New Workout) into a sample-and-hold or stepped random CV, then patch into **FREQ** for unpredictable filter motion.

## 3. **Self-Oscillation & Resonant Percussion**

- **Ping It:** With high RESO settings, “ping” the filter by sending short envelopes or triggers to the audio input.
- **Result:** You get a resonant, sine-like burst—great for modular percussion, bell tones, or tuned drums. The frequency becomes “pitch”.

## 4. **External CV Feedback**

- **Audio Feedback:** Try patching the BP output back into the audio input, possibly through an attenuator or VCA for feedback control. You'll get wild, unstable textures and self-oscillating chaos.
- **CV Feedback:** Patch a spare BP or HP output into another module’s CV processing chain—attenuverter, VCA, or sample/hold—and return as a CV to the MMF’s FREQ or RESO input for evolving, self-modifying sounds.

## 5. **Formant & Vowel Synthesis**

- **Formant Filtering:** With three filter outputs, take three sound sources into a mixer, each processed with different filter types/positions. Modulate cutoffs individually to morph between synthetic vowel sounds.
- **Voice-Like FX:** Modulate cutoff frequencies with slightly offset LFOs for shimmering, voice-like textures.

## 6. **Creative Sidechaining & Frequency Keying**

- **Envelope Follower:** Feed a drum or vocal loop into an Envelope Follower module (e.g., Mutable Instruments Ears, or Doepfer A-119). Use the follower’s CV output to modulate the MMF’s cutoff or resonance, causing the filter to “duck” or “sweep” in response to another signal.

## 7. **Waveshaping/Distortion Pre-Filter**

- **Waveshape First:** Pass your oscillator through a wavefolder (e.g., Befaco Chopping Kinky), then into the MMF. Sweep the filter frequency to emphasize or tame specific harmonics of the distorted sound.

## 8. **Stereo Spectral Splitter**

- **Clever Patch:** Use LP for the left channel, HP for the right, or swap for extra weirdness. Pan both outputs for wide, spectral stereo effects!

---

### Recommended Companion Modules
- **Utility Modules:** VCAs (for feedback, level control), Attenuverters, Mixers, Envelope Generators, LFOs
- **Effect Processors:** Reverb, Delay, Distortion/Wavefolder/Waveshaper
- **Random/S&H:** For chaotic CV animation
- **Audio Splitter/Mult:** To rout one signal into multiple filter types

---

## More Info

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)