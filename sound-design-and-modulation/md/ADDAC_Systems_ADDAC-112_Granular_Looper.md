# ADDAC Systems — ADDAC-112 Granular Looper

- [Manual PDF](../../manuals/ADDAC112_Granular_E_0.pdf)

---

[ADDAC112 VC Looper & Granular Processor Manual (PDF)](https://media.addacsystem.com/manuals/ADDAC112_USERMANUAL.pdf)

---

# Creative Modulation with the ADDAC112 VC Looper & Granular Processor
The ADDAC112 is a powerful and flexible looper + granular processor module, offering extensive voltage control, internal modulation sources, and hands-on real-time tweakability. Below, I'll break down approaches for three sound design goals—distorted percussive sounds, wild basslines, and atmospheric pads—using unique features and modulations possible with this module.

## 1. Distorted Percussive Sounds

Key concepts: glitch, stutter, aggressive grain settings, loop slicing, CV-driven disruptions.

**Recommended Patch/Settings:**
- **Source**: Feed a transient-rich signal (drum hit, or snappy synth hit) into the stereo/mono input.
- **Record Short, Tight Loops**: Use [REC NEW] to capture ultra-short drum segments (milliseconds to <1s).
- **Granular Engine**:  
    - Set [GRAINS ACTIVE] to a moderate value (2–4); more grains can create fuzzier, glitchier textures.
    - Use a small [PLAY LENGTH] with high [LENGTH DEVIATION] to generate broken, stuttered grains.
    - Crank [GRAINS VOLUME] for more prominence.
    - [GRAIN LOOP DELAY]: Short but **modulated by CV**—use an LFO or envelope (even audio-rate for hard stutters).
    - [POSITION] + [POSITION DEVIATION]: Modulate with stepped random/S&H to create retriggers or shifting slices.
- **Distortion via Feedback**:
    - Increase [GRAINS FEEDBACK] to route processed grains back into the looper—raise until feedback saturates for digital distortion/bitcrush.
    - Use [BIT DEPTH] at 8-bit and lower [SAMPLE RATE] in options for aliasing and lo-fi noise.
- **Modulation Inputs**:
    - Envelope followers for pseudo-sidechain or to “punch” in grains on each hit.
    - Step-sequencers or rhythmic triggers to glitch the [FORWARD/REVERSE] input.
    - Modulate [GRAIN REPEAT] or [REPEAT X] with randomness for stuttering ratchets.

**Outcome:**  
Metallic, glitched, and totally mangled drum textures with sharp, digital distortion and rhythmically shifting grain streams. CV modulation drives the chaos for evolving, unpredictable percussive hits.

---

## 2. Wild Dubstep/Drum & Bass Basslines

Key concepts: aggressive pitch, looping, fast transients, hard-modded grain timing, and feedback for growl.

**Recommended Patch/Settings:**
- **Source**: Synth bass, bass guitar, or even a full mix loop as input.
- **Loop Generation**:
    - Sample a short, wobbly bassline riff.
    - Manipulate [LOOP PITCH] CV input with an envelope or sequencer for fast pitch sweeps/glides.
    - Switch [REC MODE] to OVERDUB with [OVERDUB DECAY] <100% for evolving layers.
- **Granular Engine**:
    - [GRAINS ACTIVE]: 1–4 for clarity or up to 16 for wildness.
    - [POSITION] + [POSITION DEVIATION]: Use high values to scan across the bass sample.
    - [GRAIN PITCH] heavily modulated by ENV/LFO for pitch wobbles and slides; try audio-rate mod for FM-like effects.
    - [GRAIN FEEDBACK] up for saturation/growl.
    - Low [ATTACK] / short [DECAY] for snappy, percussive grains; increase [ATTACK]/[DECAY] for longer bass.
- **Clocked Mode**: Quantize actions to a clock for stepped, rhythmic gating or “chopped” phrasing.
- **External Sequencer/Controller**: Use sequencer notes to modulate [GRAIN PITCH], [LOOP PITCH], [GRAINS ACTIVE], and [DIRECTION].
- **Stutter/Glitch**: Trigger [RETRIG./PAUSE] or play with [GRAIN REPEAT] via CV for rapid-fire repeats.

**Outcome:**  
Thick, dynamic, and gnarly basslines with modulated digital distortion, pitch glitches, and bass “wobbles” characteristic of aggressive electronic genres.

---

## 3. Haunting Atmospheric Pads

Key concepts: evolving grain clouds, long buffer, diffuse layering, spatial movement, smooth time-variance.

**Recommended Patch/Settings:**
- **Source**: Sustained vocals, field recording, drone, or chords.
- **Long Buffer**: Record a long (several seconds to minutes) loop to act as a granular bed.
- **Granular Engine**:
    - Raise [GRAINS ACTIVE] for dense layering (6-16 grains).
    - High [POSITION DEVIATION] and mid-high [LENGTH DEVIATION] so grains are offset and overlap smoothly.
    - [GRAIN LOOP DELAY]: Medium/long, modulated with random LFOs for asynchronous caress.
    - [PLAY LENGTH] long, with drifting [LENGTH DEVIATION] so some grains swell and others fade quickly.
    - [ATTACK]/[DECAY]: Medium to high for fade-in/fade out, removing artifacts and creating ethereal swells.
- **Panning**: Modulate [GRAIN PANNING] across the range with a random or slow LFO for immersive stereo motion.
- **Feedback**: Gentle [GRAINS FEEDBACK] for dreamy, evolving soundscapes, but avoid over-saturating unless you want swirling distortion.
- **Sample Rate & Bit Depth**: 16bit, 44.1k or 48k for cleaner pads; drop to 8bit/11k for lo-fi, ghostly atmospheres.
- **CV Modulation**: Slowly modulated random signals to [POSITION], [LENGTH], [GRAINS ACTIVE], and [PANNING] keep textures alive and morphing.

**Outcome:**  
Lush, shimmering, and ever-evolving pads; clouds of grains move ghostlike through stereo space and pitch, perfect for dark ambient or cinematic backgrounds.

---

## Modulation Ideas At-a-Glance

- **LFOs**: To any CV input for cyclical movement (pitch, grain size, position, direction, repeat).
- **Random/S&H**: For unpredictable slice/position, glitch, and panning.
- **Envelopes**: Dynamic accents, especially for tight percussives and expressive pads.
- **Sequencers**: Melodic pitch quantization, rhythmic loop changes, glitch repetition.
- **Audio-rate**: Use for wild, aliasing-rich AM/FM effects via CV inputs.
- **Manual**: Real-time hands-on tweaks + CV for live performance.

---

### Tips
- Use the [PRESET] system to quickly jump between drastically different modulation “scenes.”
- Save/Load banks for instant recall in live setups.
- Use external mults and stackcables to send one modulation source to multiple CV inputs for complex correlation.

---

For even more creative patching, see the [full manual (PDF)](https://media.addacsystem.com/manuals/ADDAC112_USERMANUAL.pdf).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)