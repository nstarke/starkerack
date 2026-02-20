# Kaona Instruments — Stereo Weaver

- [Manual PDF](../../manuals/stereoweaver.pdf)

---

[Download the Stereoweaver Manual (PDF)](https://www.kaona.fr/uploads/1/3/2/1/132150736/kaona_stereoweaver_manual_en.pdf)

---

# Modulation Strategies for Kaona Stereoweaver  
*Eurorack Techniques for Percussion, Bass, and Haunting Pads*

---

## Introduction

The Stereoweaver module isn't just a “stereo widener.” Its clever use of depth, phase, micro-delays (Haas), animated panning, and simulated rotary effects allows for powerful sound shaping. Below are some modulation tips and patches specifically geared toward:

- Distorted percussive hits  
- Unhinged basslines for dubstep/DnB  
- Haunting pads  

All suggestions below assume you have access to external modulation sources (LFOs, Envelopes, Sequencers, etc.) and patch cables.

---

## 1. Distorted Percussive Sounds

**Goal:** Tight, aggressive stereo sound with distortion, percussive movement, and coloration.

- **Input Gain:** Push the input gain until the clip LED blinks (or stays on). This induces pleasing analog distortion.
- **Depth:** Set medium-high to increase the interaction of spatial effects, introducing phase/chorus artifacts.
- **Motion:** Assign a sharp, fast envelope (from your kick/snare envelope) to the Motion CV. Fast attack/release creates animated “surge” in stereo movement with every hit. Try the “Rotary” mode for rolling, shattered transients.
- **Haas:** Use a decayed envelope or synced stepped CV to modulate Haas. Snappy modulation gives a “slap-back” character, exaggerating percussive attack.
- **Phase:** Modulate with a slow random LFO or stepped CV to shift the character between hits, making each percussive note subtly different.
- **Width:** Keep this moderate, but use another envelope for occasional “ghost” widening at the end of percussive bursts.

*Pro Tip*: Envelope followers from the drum can modulate Haas or Phase so that harder hits widen and smear more, making complex transients.

---

## 2. Dubstep/Drum & Bass Basslines

**Goal:** Wide, animated, and at times chaotic bass, combining movement and timbral evolution.

- **Input Gain:** Push until just before heavy clipping, for grit. For “growls,” you can allow some saturation/distortion.
- **Depth:** Higher settings, for more enveloping, organic texture; sweep with a slow LFO for living stereo.
- **Motion:** Use an LFO synced to your sequencer to modulate Motion between slow and fast. “Rotary” mode creates swirling, Leslie-like movement that's excellent when processed with filtering/distortion after Stereoweaver.
- **Haas:** Automate with a squelchy, audio-rate LFO or sample & hold for jittery, erratic stereo effect. Sudden Haas changes “shake” the basslines out of the center.
- **Phase:** Assign a random or slow evolving LFO. Changing Phase will “tilt” the stereo image, making the bass weave left to right.
- **Width:** Automate with CV, possibly using accent triggers from your bass sequencer for sudden “side” expansion on particular notes, making lines jump out.

*Pro Tip*: Insert Stereoweaver before a distortion device—the stereo modulation interacts strongly with classic overdrive or wavefolder modules.

---

## 3. Haunting Atmospheric Pads

**Goal:** Lush, evolving, and sometimes eerie stereo fields for ambient/film textures.

- **Input Gain:** Clean or subtle warmth; avoid heavy clipping for maximum stereo clarity.
- **Depth:** High, sweeping with very slow LFOs for continuous morphing.
- **Motion:** Use a very slow, smooth LFO; in “Rotary” mode, the stereo field will swirl slowly, emulating a slowly spinning speaker.
- **Haas:** Modulate with a subtle, drifting LFO. Micro-fluctuations mean the pad never sits still; it feels alive.
- **Phase:** Very slow LFOs or random generators, or even manually sweeping on occasion for dramatic moments.
- **Width:** Maxed for total immersion, but automate reduction occasionally (with CV) for moments where the sound “focuses” to mono for musical tension.

*Pro Tip*: Send long, evolving modulation envelopes from complex LFOs or random voltage generators to every available CV input. Modulate Depth, Haas, Width, Phase, and Motion differently for endless subtle variations.

---

### Modulation Routing Cheat-Sheet

| CV Input   | Good Modulators                      | Characteristic Effect                        |
|------------|--------------------------------------|---------------------------------------------|
| Depth      | LFO, Envelope, Random                | Spacial “relief,” micro-chorus/phase        |
| Phase      | LFO, Sample & Hold                   | Stereo “tilt,” weirdness, coherence shifts  |
| Motion     | Envelope, LFO, Clocked Random        | Movement speed/animation, rotary swirl      |
| Haas       | Envelope, High-rate LFO, Random      | Slapback, presence, chaotic stereo jumps    |
| Width      | Accent CV, Very slow LFO             | Scene grows/shrinks, center “hollowing”     |

---

## Final Tips

- **Patch Multimodulation:** Use multiple simultaneous CVs for evolving, complex soundscapes; for example, LFOs to Depth/Width, envelopes to Motion/Haas.
- **Feedback Processing:** Stereoweaver is perfect before/during feedback loops or after reverbs for thick, swirling spaces.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)