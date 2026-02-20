# 2hp — Blur

- [Manual PDF](../../manuals/2hp_Blur.pdf)

---

[2hp Blur Manual PDF](https://www.twohp.com/assets/files/BlurManual.pdf)

---

# Creative Modulation Techniques with 2hp Blur

The **2hp Blur** is a spectral processor designed for dynamic timbral manipulation and atmospheric sound design. By leveraging its primary controls—**Time**, **Vibe**, and **Mix**, as well as their respective CV inputs—you can take your patches from subtle shimmer to outlandish sound mangling. Here’s how to exploit this module to design **distorted percussive sounds**, **aggressive basslines**, and **haunting pads**, specifically in genres like **dubstep**, **drum & bass**, and cinematic/ambient music.

---

## 1. Distorted Percussive Sounds

**Patch Ideas:**
- **Input**: Use a snare, kick, rimshot, or high-frequency percussion sample (or the output from a sharp synth voice such as 2hp Pluck).
- **TIME**: Set the **Time** control towards the left for minimal spectral stretching. Use a fast, random or envelope-synced CV to modulate this for glitchy, grainy hits.
    - **CV Tip:** Patch an envelope or stepped random CV (like from Make Noise Wogglebug or ALM Pamela’s New Workout) into **Time CV**. Fast attack/decay envelopes will create a snappy, grain-processed feel, while random will introduce chaotic variation.
- **VIBE**: Sweep the **Vibe** knob from clean (left) to smeared (right) to taste. For percussive distortion, modulating **Vibe** with velocity or accent CV from your sequencer can exaggerate timbral shifts.
    - **CV Tip:** Patch the accent or a pitch envelope into the **Vibe CV** input for each hit.
- **MIX**: Blend the dry/wet using **Mix** or automate with CV for WHIPCRACK-effect smears coming in after the transient.

**Bonus:** Route the output through a distortion or wavefolder post-Blur for further saturation and edge.

---

## 2. Crazy Dubstep/Drum & Bass Basslines

**Patch Ideas:**
- **Input**: Feed Blur a bass synth voice—preferably a harmonically rich wavetable, saw, or pulse wave—then sequence ground-shaking patterns.
- **TIME**: Use LFOs synced to your groove (fast, rhythmic rates) into **Time CV**. With Time fully right, Blur stretches your signal x16 for monstrous, gliding bass movement. Modulate from center to right for time-melted, re-pitched growls.
    - **CV Tip:** Use a stepped/random or envelope-following LFO to dynamically shift the bass between normal and time-stretched.
- **VIBE**: CV in with crazy envelopes or random S&H to alter the harmonic spread, making your bassline morph between tight and smeared. Try fast, audio-rate modulation for digital crunch and spectral tearing.
- **MIX**: Rapidly automate the Mix for stuttered transitions between clean and processed bass—perfect for rhythmic gating effects.

**Pro-stack:** After Blur, send into a wavefolder, filter, or even a granular reverb for extra movement before hitting your VCA.

---

## 3. Haunting Atmospheric Pads

**Patch Ideas:**
- **Input**: Supply Blur with a lush polyphonic pad, chord, or stacked oscillator voices (like Swarm).
- **TIME**: Set **Time** past 12 o'clock for heavy time-stretching; modulate slowly with an LFO or the output of a complex envelope (e.g., aftertouch, random voltage, or even audio from another oscillator for slow “dream-state” wow).
- **VIBE**: Use the knob or modulate gently with a slow triangle/sine LFO for evolving harmonic diffusion; drift from recognizable chords into shimmering, spectral clouds.
- **MIX**: Keep mostly wet, but with subtle automated dry return to anchor the pad occasionally. Slow, random modulations impart organic movement.

**Luxury pads:** Pair Blur with stereo reverb (e.g., 2hp Verb) post-processing for immense spatial depth. Try running two Blurs in parallel (audio in, then stereo out to reverb) for dimensional pads.

---

## Modulation Sources to Try

- **Sequencer Mod Tracks:** Assign velocity or modulation lanes to Blur’s CVs for phrase-by-phrase expression.
- **LFOs (including audio-rate):** Exploit both slow, smooth LFOs for evolving atmospheres and audio-rate signals for digital artifacts.
- **Random Generators and S&H:** Patch for unpredictable, organic variation.
- **Envelopes (standard and non-traditional):** Envelope-followers from your drums or synths add dynamic, transient-responsive changes.

## Example Chain

**Distorted Snare:**

`2hp Pluck (perc mode) → Blur → Drive/Distortion → Reverb`

- **Modulate:** Time CV with snare envelope; Vibe CV with accent or random; Mix with a fast square LFO

**Dubstep Bassline:**

`Complex Oscillator → Blur → Filter → VCA`

- **Modulate:** Time CV with S&H or LFO synced to 16ths; Vibe CV with synced envelope; Mix with gate pattern.

**Haunting Pad:**

`2hp Swarm → Blur → 2hp Verb`

- **Modulate:** Time and Vibe with slow LFOs; gentle Mix modulation; aftertouch into Vibe CV for expressive morphs.

---

Explore more in their [official manual PDF](https://www.twohp.com/assets/files/BlurManual.pdf).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)