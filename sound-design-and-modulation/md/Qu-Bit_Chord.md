# Qu-Bit — Chord

- [Manual PDF](../../manuals/QB_Chord.pdf)

---

[Chord v2 Manual (PDF)](https://www.qubitelectronix.com/_files/ugd/cc030c_c1c2d1c3aa6246319eef319b6901f600.pdf)

---

# Creative Modulation with Chord v2  
_**For Percussive Distortion, Dub/Drum & Basslines, and Haunting Pads**_

The Qu-Bit Chord v2 is a surprisingly deep tool for polyphonic sonics. With its functionality, modulation possibilities, and flexible CV addressability, you can move beyond vanilla chords into aggressive, textural, and evolving sounds perfect for adventurous electronic music.

Below are focused modulation strategies and patch ideas for your specific musical interests, referencing how to best use each section of the module for your goals.

---

## **1. Distorted Percussive Sounds**

**Key Features to Use:**
- *Waveform Bank* (choose “Distorted” or “FM” banks)
- *Wave* knob/CV (sweeping/blending waveforms)
- *Linear FM input*
- *Voicing/Quality* for chord tension
- *Fast, clicky envelope or trigger CV on V/Oct or FM*

**Patching Tips:**

- **Distorted Tone Bed:**  
  - Set the Bank to *Distorted* or *FM* (Banks 3 or 4, see Factory Banks in manual).
  - Patch a short, snappy envelope or burst generator to *Linear FM* with amount at midday—this will add a bright hit/transient on each trigger.
  - Sweep/sequence the *Wave* parameter with either random stepped voltages or rhythmic LFOs for percussive timbre changes.
  - Use envelope or fast LFO on *Voicing* for moving chord shapes; try sending a random stepped LFO for glitchy “stuttered” inversions.
  - For more chaos, glitch, and foldover, pitch the Chord module very low or very high, especially using the *Coarse* and *Fine* tune. This can create aliasing and digital grit.

- **Extra Character:**
  - Patch individual outputs (root, third, etc.) to separate VCAs or effects for layered drum hits.
  - Experiment with *Mode* in Unison Poly Mode, then trigger rapid random voltages into each voice’s 1V/Oct input for pseudo-granular textures.

---

## **2. Aggressive/Crazy Basslines (Dubstep/Drum and Bass)**

**Key Features to Use:**
- Waveform Bank—especially “FM”, “Distorted”, or “Video Game.”
- Bank and Wave knobs/CV
- Linear FM for audio-rate modulation (patch another oscillator for “FM bass growl”)
- Voicing and Quality modulation for instant phase and harmonic shifting

**Patching Tips:**
- **Bass Growl:**
  - Set *Bank* to “FM” or “Distorted.”
  - Patch a bassline gate sequencer to the *V/Oct* input.
  - Use *Linear FM* for audio-rate modulation: patch in a separate analog VCO tuned low, adjust depth for classic dubstep/gritty FM growl.
  - Use a slow envelope/LFO on *Wave* for timbral motion within a note.
  - Modulate *Quality* (CV) with an LFO or sequencer for chord type morphs—this changes harmonic content dramatically.
  - Try *Mode = Free Poly*—now you can sequence/slide each voice independently (holy chaos basslines!).

- **Bonus Tips:**
  - Patch *Root* and *Fifth* outputs into a stereo pair for a wide, detuned bass presence.
  - Sequence the *Coarse* tuning by CV for octave jumps or “Reese bass” style slides.
  - Quantize to Minor (with *Harm* button) for more sinister, dark intervals.

---

## **3. Haunting Atmospheric Pads**

**Key Features to Use:**
- Blended/interpolated *Waveforms* in “Voice”, “Organ”, or custom user banks
- Voicing/Quality slow modulation (LFOs/Envelopes for harmonic motion)
- Multimode (Normal = Chords, Free Poly = evolving textures)
- User wavetables via SD card

**Patching Tips:**
- **Evolving Pad Motion:**
  - Select the *Voice* or *Organ* Bank (Banks 5 or 8).
  - Apply a very slow LFO or random/slew generator to *Wave* and *Voicing/Quality* for drifting timbres & chord qualities.
  - Use *Mode = Melody*; sequence the *Lead* input for pads with a moving top line, or *Unison Poly* for 4 subtly detuned voices.
  - *Harm* in Major or Minor helps lock atmospheric progressions to tonality.
  - Mix individual outputs and process with delay/reverb for wide, lush space.

- **Cloud-like/Cluster Textures:**
  - On SD card, define custom chords (*CHORD_4=0.2,0.4,0.6*) for microtonal or spectral clusters.
  - Slowly cycle through custom chords with the *Quality* knob in User Chord Mode.
  - Modulate *Voicing* for subtle spreads, nudging intervals apart dynamically.

- **Extra Atmospheric Tips:**
  - Feed pink/white noise to the *Linear FM* input for shimmer or granular-like character.
  - Patch gentle LFOs or randoms to all CV inputs for shimmering life.

---

## **Other Pro Tips:**
- **Bank and Wave CV Range**: -5V to +5V, so use attenuverters or offset mixers for sensitive control.
- **FM input**: Use both slow envelopes and audio rate for maximum range (think both “wow” and “screech!”).
- **Triad Control**: Remove the 7th in chords for simpler or more open pad voicings, useful when sending melodies to the 7th output.

---

For more in-depth configuration, custom wavetables, and chord design, see the [full manual (PDF)](https://www.qubitelectronix.com/_files/ugd/cc030c_c1c2d1c3aa6246319eef319b6901f600.pdf).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)