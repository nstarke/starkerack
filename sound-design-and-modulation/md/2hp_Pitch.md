# 2hp — Pitch

- [Manual PDF](../../manuals/2hp_Pitch.pdf)

---

[**2hp Pitch Manual PDF**](https://www.twohp.com/_files/ugd/ebc3fb_ae5372ca563f47e7951bc2a0d87be263.pdf)

---

# Creative Modulation Tips for 2hp Pitch  
_**For Distorted Percussion, Aggressive Basslines, and Haunting Pads**_

The 2hp Pitch is a compact, time-domain pitch shifter with voltage-controllable wow & flutter, designed for highly musical or deeply experimental results. Let’s break down ways to patch and modulate this module into the realms you described.

---

## Key Modulation Points

- **W&F CV Input** – Modulates the wow and flutter effect; adds pitch warble similar to tape or vinyl irregularities.
- **Mix CV Input** – Controls the blend between dry (original) and wet (processed/pitch-shifted) signals.
- **1V/OCT Input** – Accepts pitch voltages for melodic or atonal pitch shifting, tracks an extra octave over the front knob.
- **Pitch Knobs** – Manual pitch shifting up to ±2 octaves.

All are voltage-controllable, so CV, LFOs, gates, envelopes, or sequencers can be used for dynamic manipulation.

---

## 1. Distorted Percussive Sounds

**Patch Idea**
1. Patch a short percussive audio source (kick, snare, plucky synth, noise burst) into **Audio Input**.
2. Send trigger or gate envelopes into the **1V/OCT** to modulate pitch shift with each hit, creating “pitched percussion” or glitchy artifacts.
3. Use the **W&F CV Input** with a fast, random stepped CV (like a sample and hold or fast random LFO) to cause unpredictable pitch flutter, mimicking tape or digital artifacting.
4. Set **Mix** to 100% wet for fully processed sound, or modulate **Mix** with an LFO/envelope to create motion—e.g., punch a hit then fade to dry.

**Experimental Tip:**  
Turn W&F fully CW for maximum instability, then send sharp CV bursts to W&F CV to add “tape break” drama to your percussive hits.

---

## 2. Crazy Dubstep/Drum & Bass Basslines

**Patch Idea**
1. Feed a rich oscillator or FM bass patch into **Audio Input**.
2. Sequence the **1V/OCT** with a pitch CV line running at 1/16th or 1/32nd notes for stepped, “talking” bass modulation.
3. Modulate **W&F** with a synced LFO or a tempo-synced stepped random, creating rhythmic vibrato or “robot malfunction” wobbles.
4. Use an envelope or LFO to sweep the **Mix**, so the bassline moves from “normal” to warped during drops or fills.
5. Push **Pitch Knob** away from center while modulating with **1V/OCT** for subharmonic or overtone madness.

**Experimental Tip:**  
Try audio-rate modulation into **W&F CV Input** for digital aliasing and gnarly artifacts—great for aggressive, distorted bass textures.

---

## 3. Haunting Atmospheric Pad Sounds

**Patch Idea**
1. Patch a slow-evolving pad or drone as **Audio Input**.
2. Use a slow triangle or sine LFO into **1V/OCT** to create gentle, gradual detuning or chorusing.
3. Patch a very slow, slewed random CV or fluctuating stepped source (like Wogglebug, Turing Machine, or noise & slew) into **W&F CV Input** for lush, unpredictable tape warble, giving the sound a ghostly, old-record vibe.
4. Keep **Mix** ~70% wet to retain some solidity but with an ethereal tail.
5. Slightly offset the **Pitch Knob** for ever-present otherworldliness.

**Experimental Tip:**  
If you have a second LFO, modulate **Mix** slowly and asynchronously with the above, gently fading the haunting effect in and out for evolving, cinematic richness.

---

## Bonus: Combination Effects

**Freeze + Pitch:**  
Pair the 2hp Pitch with a granular or freeze module for ultimate lo-fi unpredictability. Send modulated, pitch-shifted sounds into a buffer/freeze effect, then further pitch shift for haunted digital echoes or dystopian fragments.

**Layering:**  
Split your source: send the dry and pitch-shifted outputs into two channels of your mixer. Treat each channel separately (independent FX, panning, further processing) for wide, stereo-warped soundscapes.

---

## Technical Patching Reminders

- CV ranges are ±5V. Ensure your modulation sources match this for maximum effect.
- Keep power consumption modest: +12V: 78mA, -12V: 9mA—easily fits most small skiffs.
- Monitor headroom: pitch shifting can sometimes introduce level changes or phase artifacts.

---

For more info, download the [official PDF manual](https://www.twohp.com/_files/ugd/ebc3fb_ae5372ca563f47e7951bc2a0d87be263.pdf).  
Module and patching diagrams, troubleshooting, and further inspiration await!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)