# 2hp — MMF

- [Manual PDF](../../manuals/2hp_MMF.pdf)

---

[Read the MMF Manual PDF](https://2hpmodules.com/docs/mmf.pdf)

---

# Creative Modulation with the 2hp MMF Eurorack Module

The 2hp MMF is a compact, voltage-controlled multimode analog filter, offering Low Pass (LP), High Pass (HP), and Band Pass (BP) outputs simultaneously. With CV control over frequency (cutoff) and resonance, it’s capable of everything from smooth sweeps to aggressive, resonant squelches.

Below are patching and modulation ideas for **distorted percussive hits**, **crazy basslines**, and **haunting atmospheric pads**:

---

## 1. Distorted Percussive Sounds

**Goal:** Sharp, snappy, and even distorted filter-driven percussion or “clap/snare” hits.

**Tips & Patches:**
- **Audio Input:** Use a noise source, short burst of audio, or a drum sample into the **Input** jack.
- **Cutoff Envelope:** Patch a fast envelope generator (AD or AR) to the **FREQ CV**. Keep the envelope sharp/non-sustained for snap; set base freq knob low for clickiness.
- **Resonance Exciter:** Turn up **Reso** knob for ringing, metallic sounds. Patch a second envelope or even a gate to **RESO CV** for animated resonance, creating more dynamic hits.
- **Distortion:** Overdrive the input or output with external modules, or increase the input gain before the MMF to push its analog circuit into gentle saturation.
- **Multimode Magic:** Mix **LP** and **BP** outputs for complex timbres, or swap to **HP** for more pronounced clicks.

---

## 2. Basslines for Dubstep or Drum & Bass

**Goal:** Wobbling, squelchy, aggressive or talking bass.

**Tips & Patches:**
- **Rich Input:** Use a saw or square wave from an oscillator into **Input**.
- **Wobble LFO:** Send an LFO (triangle, sine, or even stepped random) to **FREQ CV** for cutoff wobbles. Sync the LFO to your clock for tempo-synced movement.
- **Envelope Punch:** Layer in an envelope (perhaps via a CV mixer) to **FREQ CV** for movement at note-on. Start with cutoff low; let envelope “open” the filter, then LFO modulates.
- **Resonance Squelch:** Increase **Reso**. Patch a slow-moving LFO or an envelope to **RESO CV** for evolving “talking” vowel-like bass effects.
- **Parallel Filtering:** Send **LP** output for sub, **BP** or **HP** for higher harmonics. Mix externally for huge, layered basses.
- **Tonal Overdrive:** Overdrive the input signal, or use a waveshaper before MMF for contemporary DnB/Dubstep aggression.

---

## 3. Haunting Atmospheric Pad Sounds

**Goal:** Evolving, spectral, chilly pads with movement and space.

**Tips & Patches:**
- **Layered Input:** Several oscillators with detuning, or a wavetable drone, into **Input**.
- **Slow Modulation:** Use a very slow LFO or sample & hold (random) to **FREQ CV** for drifting filter movement. Set **FREQ** knob to taste.
- **Resonance Texture:** Engage moderate **Reso**; gently modulate with a slow triangle LFO or envelope follower for shimmer or spectral “breathing.”
- **Triple Output:** Patch **LP** to one channel, **BP** to another, **HP** to a third – send each to reverb or delay with different settings, then blend for a “spectral” pad with rich stereo field.
- **CV Layering:** Sum multiple CVs (envelope for fade in, LFO for slow cycling, random for wander) to the **FREQ CV** for organic, non-repeating motion.
- **Subtle Squelch:** Occasionally nudge **RESO CV** high with random bursts for eerie filter self-oscillation “ghosts.”

---

## Advanced Bonus Patch

- **Audio-Rate FM:** Try sending an audio oscillator (tuned below or above your main pitch) to **FREQ CV** for filter FM – rendering clangorous, metallic, or granulated sounds unlike static filters.
- **Pseudo-Karplus:** Short excitation or noise burst into **Input**, trigger high **Reso**, and tune **FREQ** for pitch – MMF can produce plucky string-like tones or zaps.

---

**General Tips:**
- **Voltage Ranges**: FREQ CV (-8V to +8V), RESO CV (-5V to +5V). Use attenuation/inversion as needed.
- **Stacking**: Multi CV signals (LFO+Envelope) with a CV mixer can create more complex motion.
- **Mix Outputs**: Use external mixers for creative blends of LP/BP/HP, dynamically change routing during performance.

---

For more advanced creative patching ideas and utilities, explore:  
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)