# Doepfer — A-119

- [Manual PDF](../../manuals/A119_man.pdf)

---

[**Doepfer A-119 Ext. Input / Envelope Follower Manual (PDF)**](https://doepfer.de/a100man/a119_anl_e.pdf)

---

## Creative Modulation Techniques for Doepfer A-119  
*Focusing on Distorted Percussion, Dubstep/Drum & Bass Basslines, and Haunting Pads*

The Doepfer A-119 External Input/Envelope Follower lets you bring external audio (guitar, mic, drum machine, etc.) into your Eurorack and convert amplitude changes into CV and Gate signals. By creatively patching these outputs, you can generate dynamic, expressive modular sounds.

Below are techniques to achieve specific types of timbres, leveraging the A-119 as a critical modulation/control hub.

---

### 1. **Distorted Percussive Sounds**

**Key methods:**
- Bring in external drums or percussion through the A-119’s Asym (line) or Symm (instrument/mic) input.
- Use the preamp’s Gain control to overdrive the signal intentionally—watch the Overload LED for indicator (clip harshly for aggressive distortion!).
- The rectified, amplified, and envelope-followed signal is now available for modulation.

**Patch Ideas:**
- **Audio out > Wavefolder or Distortion Module:** Use §/$ Audio Out and send to additional distortion or wavefolding for layers of timbral grit.
- **Envelope out % > CV on filter/vca/wavefolder:** Patch Envelope Out to modulate your VCA/VCF cutoff, synchronized dynamically to volume of external hit/transient.
- **Gate out & > Envelope trigger:** Connect Gate Out to trigger an envelope, which can then modulate pitch or filter—try extremely fast attack/decay for snappy, glitchy percussion.
- **Feedback/Resample:** Route processed percussion back into A-119 for recursive, evolving distortion.

**Bonus:** Use an external drum machine or real-world percussive sounds as source. Overdrive the preamp for industrial or ‘broken PA’ character.

---

### 2. **Dubstep/Drum & Bass Bassline Madness**

**Key methods:**
- Use an external signal (e.g. bass guitar, synth, vocal growl) as modulator, or as the core of your bass patch.
- Exploit the A-119’s envelope to impart rhythmic, wobbling movement.

**Patch Ideas:**
- **Envelope Out % > Filter Cutoff/Resonance on a VCF:** Classic ‘wobble’—apply bass amplitude envelope to modulate a lowpass/bandpass filter’s cutoff.
- **Envelope or Gate Out > Waveshaper CV:** Animate a waveshaper or distortion module’s parameters with Envelope Out for vowel-like, FM, or talking bass effects.
- **Gate Out & > Sync or Retrig Oscillator/LFO:** Make oscillator/LFO restart in sync with external grooves—great for tight, rhythmic bass modulations.
- **Aggressive preamp abuse:** Crank Gain for gnarly harmonics on the external signal; send through further saturation/bitcrushing downstream.

**Pro tip:** Combine with fast-speed modulation and resonance for "growling" bass. For advanced mayhem, use the A-119 to process sidechain signals, making bass duck or ‘pump’ in time with your beats.

---

### 3. **Haunting Atmospheric Pad Sounds**

**Key methods:**
- Feed in evolving ambient recordings, field samples, or drones.
- Use the envelope follower to animate multiple downstream parameters for organic, living textures.

**Patch Ideas:**
- **Audio Out §/$ > VCF/Phaser/Resonator:** Process field recordings or drone sounds through filtering with slow modulations.
- **Envelope Out % > Slow filter sweep/VCA amplitude:** Create subtle movements—envelope tracks evolving swells in the pad, shaping cutoff/resonance.
- **Gate Out & > Random/S&H trigger, Polyphonic voice cycling:** Use Gate Out to randomly trigger events, new notes, or micro-loop granulation.
- **Patch Envelope Out to modulation matrix:** Animate reverb send level, wavefolder CV, or delay feedback based on the incoming pad’s volume.

**Ambient tip:** Combine Envelope Out with a slew limiter (as advised in the manual) for smooth, ghostly CV movements. Layer multiple external sources for lush, evolving atmospheres.

---

### **Bonus Experimental Tips**

- Use both inputs with different sources to blend signals (1:25 ratio), then modulate the Gain for crossfading or signal-morphing effects.
- Abuse the comparator and threshold for unpredictable rhythmic gates.
- Tap Envelope and Gate to sequencer resets, clock dividers, or logic modules for chaos-based rhythmic generation.

---

By creatively routing the A-119’s amplified audio, envelope, and gate signals throughout your system, you can unlock experimental dynamics that respond to the real-world nuance of your inputs. Treat it as both a distortion/preamp and a multi-function CV generator for maximum modular weirdness.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)