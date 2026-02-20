# 2hp — Bell

- [Manual PDF](../../manuals/2hp_Bell.pdf)

---

[**2hp Bell Manual PDF**](https://2hp.com/docs/bell.pdf)

---

# Creative Modulation Techniques for 2hp Bell

The **2hp Bell** is a polyphonic melodic percussion generator, making it a flexible voice for a wide range of sounds beyond traditional bell tones. Based on modal synthesis, Bell is capable of everything from clean tuned percussion to gnarly, distorted chaos and lush, otherworldly textures—when modulated creatively in a Eurorack system.

Below are strategies for using external modulation and creative patching to achieve three specific sonic goals: **distorted percussive sounds, intense basslines, and atmospheric pads**.

---

## 1. Distorted Percussive Sounds (Industrial, Glitch, Experimental)

To move Bell into aggressive, distorted territory:
- **Model Selection**: Use the *Hard Marimba*, *Wine Glass*, *Redwood Plate*, or *Tibetan Bowl* models for less traditional, more tonally complex starting points.
- **Damp Control**: Modulate the *DAMP* CV with a fast random or stepped voltage source (e.g., Sample & Hold or fast LFO). Extreme values create snappy, clipped decays and metallic resonance.
- **Pitch Modulation**: Mult a fast envelope, sequencer, or synced LFO into the *PITCH* input while a note is ringing—this exploits the “live pitch control” for the most recent trigger, adding pitch bends, rolls, or vibrato every hit.
- **Trigger Madness**: Use probabilistic, shuffled, or logic-combined trigger sources to create bursts, rolls, or ratcheting effects into the *TRIG* input.
- **Audio Rate Modulation**: Run a loud, fast audio oscillator (square/saw) into the *MODEL* or *DAMP* CVs for brutal, unpredictable timbre distortion.
- **External Distortion/Folding**: Run the output of Bell into a wavefolder, saturator, or in-feedback with ring mod/fuzz to emphasize nonlinearity and aggressiveness.

### Example Patch
- *MODEL* knob at 3-4 (Wine Glass or Redwood Plate)
- Random stepped CV into *DAMP* (-5V to 5V)
- Envelope to *PITCH* (modulate decay for pitch sweep)
- Trigger rolls (clock divider/multiplier)
- Post Bell: wavefolder + distortion

---

## 2. Crazy Basslines (Dubstep, Drum & Bass, Neuro)

You can use Bell for bass by exploiting:
- **V/Oct Tracking**: Sequence notes via the *1V/OCT* input, using a pitch CV/gate sequencer or pattern generator. Stay low (below C3).
- **Pitch Voltage**: Add an LFO, function generator, or envelope to *PITCH* for wobbles, slides, and growls—try slow triangle/sine for “dubstep wub” style.
- **Model Mutation**: Sweep *MODEL* with a CV LFO for moving harmonic content—use bipolar modulation for full model spread.
- **Damping for Impact**: Use the *DAMP* control in conjunction with triggers/gates to adjust note length dynamically (short for plucky, long for sustained growl).
- **Resonator Feedback**: Feed Bell’s output into a bandpass/lowpass filter and resonance circuit, then mult that signal back into Bell's *MODEL* or *DAMP* (if you're using a mixer/attenuator for safety)—for physical modeling "feedback squelch."
- **Layering**: Layer Bell with a sub-oscillator below, to reinforce sub-bass presence.

### Example Patch
- Bassline sequencer to *V/OCT* and *TRIG*
- Sine LFO (~0.5-2Hz) to *PITCH* (*intense* for full FM wobble)
- Mild random/slow LFO to *MODEL* (adds timbral variation per note)
- DAMP modulated for snappy or drawn-out plucks
- Output to saturation/drive, then aggressive filter (VCA envelope after filter)

---

## 3. Haunting Pads & Atmospheric Sounds

For lush, eerie, or evolving soundscapes:
- **Polyphonic Texture**: Use multiple *TRIGs* in relatively quick succession to layer voices (Bell can do 6-voice polyphony). Use random, Euclidean, or manually-timed triggers.
- **Slow Damping**: Set *DAMP* high, or modulate slowly with an LFO/envelope for evolving reverb-like decays.
- **MODEL Scanning**: Use a slow, bipolar LFO, or a pressure/joystick controller to sweep through different *MODEL* positions for changing harmonic profiles.
- **Pitch Glides/Vibrato**: Route a slow, gentle LFO or random smooth voltage to *PITCH* for chorus-like drift or whale-song undulation.
- **Harmonic Layering**: Mult Bell output through different reverb, shimmer, or granular effects and blend; stereoize with subtle detune on *PITCH* live fiddling.
- **Atmospheric Effects**: Patch drone triggers at regular, slow intervals, and use a looping envelope for ongoing mild pitch modulation.

### Example Patch
- MODEL: Slow LFO modulation (full sweep, ~1 cycle/30 sec)
- TRIG: Multi-gated/randomized for overlapping polyphony
- DAMP: Set high, modulate with slow LFO for motion
- PITCH: Small vibrato (sine LFO), or sample & hold for subtle pitch clouds
- Output: Long reverb, stereo widener, shimmer

---

## General CV/Modulation Tips

- All modulation inputs (*MODEL* and *DAMP*) accept -5V to +5V: scale your sources for full-range movement.
- *1V/OCT* accepts -1V to +6V: you can create subharmonic and very high-pitched effects by pushing CVs outside standard keyboard/pitch input ranges.
- Live wiggle *PITCH* after triggering for on-the-fly vibrato, bends, or crazy macro gestures (use attenuators for smoother action).
- Combining traditional melodic sequences with frequent parameter modulation can yield sounds unachievable with acoustic bell-like sources.

---

Have fun ringing Bell far beyond its classical roots!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)