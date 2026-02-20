# Intellijel — Metropolix

- [Manual PDF](../../manuals/metropolix_manual_v1.4_2022.04.04.pdf)

---

[Metropolix Manual (PDF)](https://intellijel.com/downloads/manuals/metropolix/Metropolix-1.4-Manual-EN.pdf)

# Intellijel Metropolix: Modulation Strategies for Sound Design

The Intellijel Metropolix is a powerful Eurorack sequencer that excels at dynamic, real-time modulation. Below, you'll find strategies for using its unique features to generate **distorted percussive sounds**, **aggressive basslines**, and **atmospheric pads**. Techniques focus on leveraging modulatable lanes, ratcheting, gate manipulation, and external CV inputs to push Metropolix beyond standard step-sequencing into complex, performance-oriented modulation domains.

---

## 1. Distorted Percussive Sounds

### Key Modulation Tools:
- **Ratchets & Probabilities:** Use *per-stage ratchets* to generate bursty trills and “machine gun” effects common in glitch and IDM. Further, modulate ratchet amount with a MOD Lane or AUX input to add continuously changing density.
- **Gate Length & Gate Types:** Vary between HOLD, MULTI, SINGLE, and REST for stuttering, off-beat, or muted percussive hits. Shorten gate length for sharp, clicky sounds or lengthen for saturated distortions in your external drum voice.
- **Gate Stretching (Track Menu):** Turn ON to allow gates to “bleed” across pulses—great for overdriven envelopes or VCAs downstream.
- **Skip & Random Playback:** Use Skip per stage for pseudo-random rhythmic variation; combine with ORDER modes like Brownian or Random.

#### Example Patch:
- Assign a MOD Lane to “Ratchet” for Track 1, and map a slow external LFO to glide ratchets between 1 and 8 for unpredictable percussive bursts.
- Use Aux X for “Gate Length” modulation, patched to a snappy envelope output from another module set to random triggers for evolving decay artifacts.
- Engage “Swing” (non-4/4) and shuffle ORDER options to add off-grid “looseness” typical of breakbeat and d’n’b grooves.

## 2. Crazy Basslines (Dubstep/Drum & Bass)

### Key Modulation Tools:
- **Pitch Pre/Post & Transpose:** Assign a CTRL knob or MOD Lane to “Pitch Post” or “Pitch Offset” for wild, hands-on pitch drops or 1V/oct glides familiar from dubstep “wub” basses.
- **Accum Modulation:** Use ACCUM per-stage for staged, in-scale pitch sweeps—the ‘cumulative transposition’ is like ratcheted glide through the scale (set “Trigger” to Pulse or Ratchet for granular movements).
- **Slide Amount & Acid Slides:** With Slide Type set to Acid, slides emulate classic 303 “rubbery” bass. Modulate Slide Amount via AUX or MOD for evolving glide strength.
- **Gate Probability:** Randomize which pulses fire; you'll get organic, off-balance bass riffs.

#### Example Patch:
- CTRL 1 → “Pitch Offset ±” for immediate bass drops or rises.
- MOD Lane 2 → “Slide Amount” for automation of glide effect; sequence ramping voltage to morph between no glide and extreme glide.
- AUX Y → “Ratchet” CV, patched from a random LFO or step sequencer, to alternate between single notes and bursty bass rolls.
- Use per-stage REST gates to create syncopation and negative space.

## 3. Haunting Atmospheric Pads

### Key Modulation Tools:
- **MOD Lanes to OUT for CV:** Glide slow, random MOD lanes to OUT A/B and into a quad VCA or filter for evolving timbral movement.
- **Pitch Pre Modulation:** Assign a MOD lane or AUX to “Pitch Pre” in subtle amounts for gentle, random melodic drift within the scale.
- **Scale (User) Modulation:** Build custom, moody user scales; use a MOD lane or AUX to sweep through different user scales in the same bank for pseudo-modal pad evolution.
- **Gate Probability & Length:** Set long gate times and probabilistic firing to sustain notes into eerie, unpredictable drones.
- **Slide Amount & Swing:** High Slide Amounts and heavy swing (75%+) on long stages create dreamy, portamento-rich movement.

#### Example Patch:
- MOD Lane 1 → OUT A, routed to the CV input of a filter, modulating cutoff in sync with the sequence for subtle waves of filter movement.
- MOD Lane 4 → “Scale (User)” for changing scales every few bars, gently warping the harmonic center.
- AUX Z → “Gate Length,” use an LFO for slow morphing between choked and lush, held notes.
- Use Probability per stage at 70–80% for the washing in and out of notes.

---

## Additional Tips

- **Randomizing Parameters:** Use ALT + AUX X/Y to instantly morph or remix sequences, especially for live or generative performance.
- **Loopy Mode:** "Latch" short loops for stuttering repeats—excellent for sampled sound textures or rapid staccato effects.
- **Copy/Paste Patterns:** Quickly duplicate and vary segments—try copying a "normal" bassline and randomizing the copy for climactic breakdowns.

---

With Metropolix's rich modulation potential—spanning pitch, gate, order, probability, and more—you can push your sound design deep into the experimental, the brutal, or the atmospheric. Always experiment with routing MOD lanes to internal and external destinations—this sequencer truly rewards creative patching and hands-on control.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)