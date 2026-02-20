# IO Labs — Flux Sequencer

- [Manual PDF](../../manuals/IO Labs - Flux Sequencer - 107 User Manual.pdf)

---

[**Download the FLUX Manual PDF**](https://iolabs.co.uk/flux/downloads/FLUX_USER_MANUAL_OPEN_BETA_V1.07.pdf)

---

# Using FLUX to Create Distorted Percussive Sounds, Crazy Basslines, and Haunting Pads

The FLUX module by IOLabs is an exceptionally deep and flexible sequencer/modulation source for Eurorack, based on Temporal Modulation Synthesis® and packed with advanced modulation, logic, and CV/gate possibilities. Here's how you can exploit its architecture for the type of sounds you want:

---

## General Modulation Approaches in FLUX

FLUX offers three primary modulation sources:
- **Macro Pots (Manual Potentiometers)**
- **CV Inputs (Four Assignable Jacks)**
- **Evolve LFOs (85 Internal Per-Parameter LFOs, Savable Per-Preset)**

You can mix and match these sources using the **modulation matrix** and three color-coded **mod buses** (Yellow, Grey, Purple), assignable **per-step**!

### Setting up Modulation

- **Quick Setup:** In the Main UI, select a parameter, then hit the `MOD` button to jump directly to its modulation nodes (Evolve, Macro, CV in sequence).
- You can modulate virtually any parameter per step and per channel: density, curve, value, phase, gate, humanize, mask, CV min/max, envelope, LFO params, quantization, etc.
- The Evolve LFO engine offers multiple waveforms—including various random, square, and triangle types, as well as bipolar (invertible) shapes for more expressive changes, plus a VCA-style dry/wet per LFO to control depth or automation.
- Macro Pot mapping and CV input mapping are via attenuverters for positive or negative modulation of each parameter.

---

## Distorted Percussive Sounds

### Parameter Tricks

- **Density (`DENS`) & Compression (`COMP`):** Push trigger density high and use negative compression/expansion to cause rapid fire/flammed triggers—increase distortion or overdrive in following drum modules.
- **Humanize (`HUMA`), Mask, Phase (`PHAS`):** Add randomness for organic "broken" distortion.
- **Gate Lengths (`GATE`):** Short/long gate times create clicky versus smeared/overdriven pulses.
- **CV Outputs:** Modulate VCA envelopes controlling drum VCAs, introduce random or envelope-controlled transients.
- **Auxiliary Outputs in Boolean Modes:** Use AND, OR, XOR logic to interleave or alternate triggers unpredictably.
- **Random LFO on Accent/CV Out:** Assign a random or triangle LFO to trigger amplitude tweaks, pitch modulation, or even FM input on external voices for noisy, gnarly percussion.

#### Patch ideas:

- Use a single-step pattern with high density (`DENS > 32`), long length (`LENG > 8`), then automate `VAL` with an LFO for moving between clustered and spread hits.
- Layer two percussion voices (e.g., kick/snare) and use different masks and phase offsets; modulate which AUX output is performing logic like AND/OR for trigger interplay.
- Send envelope CV out to a wavefolder or distortion module gated by a random or square LFO pattern for crushed, broken percussive textures.

---

## Crazy Basslines (Dubstep, DnB, Neuro)

### Parameter Tricks

- **TM Curve (`CURV`) and Value (`VAL`):** Skew bass notes or rhythmic triggers unpredictably for that chopped/jerky feel—modulate with triangle or sample-hold LFOs.
- **CV Modulaton:** Assign LFO, AR-envelope, or even random S+H voltages to filter cutoff or oscillator pitch of your bass voice. Use frequency-synced LFO modulation for classic dubstep LFO-wobble.
- **Quantization (QUAN):** For more chaotic basses, reduce quantization steps or leave only a few nodes active per octave for "broken" scales.
- **Macro Pots:** Use a macro to sweep filter cutoff, FM depth, or wavefold amount in real-time over evolving step sequences, then automate macro depth to create performance macros.
- **Burst Mode:** Use Burst mode with triggers controlled externally—they allow you to retrigger steps/basses for re-syncs or fills typical in DnB.

#### Patch ideas:

- Automate step CV out mode to `LFO`, sync it to step/trig, and send to a resonant LPF or VCF on your bass synth. Assign Evolve LFO (triangle or random) to `MAXV` and `MINV` for fluctuating LFO depth, mimicking modern growl bass modulations.
- Use step-specific quantization and mask with macro/CV assignment to "mute" or "ghost" notes, yielding syncopated, chopped grooves.
- Utilize auxiliary outputs set to chained logic modes to generate stuttery gate patterns for gating distortion or bitcrush on your bass voice.

---

## Haunting Atmospheric Pads

### Parameter Tricks

- **Long Envelope Mode (`ENV+`/`ENV-` on CV Out):** Program step CV outs as long AR envelopes modulated by Evolve LFOs with slow triangle/sine shapes for evolving textures.
- **CV Output Range (`MINV`, `MAXV`):** Automate the voltage range per step to create shifting timbres—perfect for morphing pads.
- **Phasing, Compression (`COMP`):** Use subtle negative compression and phase modulation to produce drifting, ambiguous attacks for each trigger—think smearing granular textures.
- **Humanize/Mask:** Add low-level humanize and complex mask steps for unpredictable ambience.
- **Quantization Nodes:** Turn on only certain intervals per step for modal, non-Western, or ambiguous harmonies.
- **LFO’s VCA Dry/Wet:** Fade in/out modulation depth per LFO over time with the per-parameter VCA control, creating swelling/ebbing textural movement.

#### Patch ideas:

- On a dedicated channel, sequence long 8+ step patterns with low density and widely spaced triggers. Set CV Out to AR envelope, modulate release/attack times with Evolve LFOs, and use the pad's CV to modulate reverb/delay on your effects to simulate distant, breathing atmospheres.
- Randomize quantization nodes and automate CV range per step so each new chord or drone step is harmonically ambiguous and morphing.
- Stack multiple CV outs routed to different oscillators’ timbral controls, each with different LFO/ENVELOPE settings, for evolving polyphonic pads.

---

### Advanced Tactics

- **Boolean Logic for Surprises:** Use AUX logic modes (&, ||, x||, etc.) for pseudo-generative triggers—ideal for both glitchy percussion and unpredictable pad textures.
- **Step-by-Step Wild Variation:** Use ALL mode to initialize patterns, then go off ALL and hand-edit irregularities—good for "almost repetitive" sequences that trick the ear.
- **Macro + Mod Matrix Automation:** Assign multiple parameters to a single Macro or CV input for one-knob (or envelope) deep transformations across the entire patch.

---

### Additional Resources

- [Full FLUX Manual PDF (Official)](https://iolabs.co.uk/flux/downloads/FLUX_USER_MANUAL_OPEN_BETA_V1.07.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
