# Make Noise — MultiMod

- [Manual PDF](../../manuals/multimod-manual.pdf)

---

[**MultiMod Manual PDF**](https://makenoisemusic.com/manuals/multimod-manual.pdf)

---

# MultiMod for Hyper-Complex Rhythmic Percussion—Eurorack Strategies

## Overview

The Make Noise MultiMod is a DSP-based mult, not a sound-generating voice or audio effect itself, but a modulation processor. Its power lies in generating multiple, time-modified, and phase-shifted control signals based on a single input (or internal LFO) for simultaneously animating multiple parameters, modules, or voices. The MultiMod is exceptionally well-suited to creating dense, polymetric and polyrhythmic modulation patterns, ideal for intricate percussion sequencing and advanced modular patching.

Below is a focused guide for using MultiMod in the pursuit of hyper-rhythmic, complex percussive outcomes:

---

## Core Techniques

### 1. Turning Single Clocks into Many Rhythms

- **Patch a master clock or pulse (e.g., from Pamela’s New Workout, Tempi, etc.) into the Signal In.**
- Use the **Spread** control to create divisions/multiplications of that clock across outputs.
  - At 12:00, all outputs align; turning Spread CW/CCW “bends” channels to faster/slower divisions/multiplications—even into irrational clocking regimes, not just musical integer divisions.
- **Result:** Instant polyrhythms or non-standard ratchets to trigger percussion voices, LPGs, or drum modules.

### 2. Generate and Manipulate Multilayer LFOs

- With nothing patched to Signal In, MultiMod’s internal LFO acts as a polymorphic master modulator. Use **Shape** to select classic or random waves.
- Modulate Time, Spread, and Phase with CV sequencers or random sources to warp those LFO shapes for punches, twists, and morphing modulations.
- Gate the **Hold** input to freeze (“buffer repeat”) phrasing, or reset sync with external triggers for repeatable, glitchy hits.

### 3. Phase-lock Polyrhythms

- Use **Phase** to shift outputs for complex step-offsets; with percussion, this offsets trigger/gate timing for flam, swing, or stagger effects.
- As Phase is increased from fully CCW to CW, outputs are distributed from identical (in-phase) to fully offset (channels 1 & 8 at 180° out).
- Periodically hit **Reset** (manual or CV/gate) to re-align all channels, making for pulsed grouping, bursts, or cyclical realignment—a key for punchy fills.

### 4. Polyrhythmic Sequencing with TEMPO and Reset

- Patch an external clock to **TEMPO In** to make all rhythmic relationships grid-locked but allow divisions/multiplications that cross metric boundaries.
- Use **different permutations of Time, Spread, Phase** (with or without CV modulation) for each session or section in your set.

### 5. Hyper-Complex Patterns: Shape Strategies

- Select non-linear or random shapes in Shape mode (Stepped Random—orange, Smoothed Random—yellow) for stochastic, west-coast-style percussion timing. Each output channel “walks” its own clocked random sequence, great for non-repeating rhythms.
- With **Square (Pink) shape** use MultiMod as a master clock generator. Outputs give multiples/divisions set by Spread, ideal for layers of pulses ticking in and out of phase.

---

## Patch Ideas for Densely Rhythmic Percussion

### A. Multichannel Trigger Generator

- **SIMPLE:** Patch MultiMod outs to percussive modules’ trigger/strike inputs. Set Spread off-center, Phase to taste, and modulate Time with a slow envelope for tempo automations.
- **COMPLEX:** Flick through Shapes during performance to morph the rhythm engine.

### B. Modulation of Percussive Parameters

- Take outs to modulate decay, pitch, filter, or wavefold amount on synth voices or drums. Each channel gives you a time-skewed version of the base input or LFO.

### C. Chain Reaction (Shift Register Patch)

- Send a modulated CV sequence (melodic or rhythmic) into Signal In. With Spread at noon, increase Phase for staggered outputs; patch outs to drum tunings, LPG amplitudes, or sequencer CV inputs for tightly related “echoes” or call-and-response.

### D. Burst Fills and Controlled Chaos

- Patch a regular or irregular burst generator (or a hand-triggered button) to Reset. The MultiMod outputs “snap back” into phase, accenting fills or imposing structure on a swirling cloud of rhythms.
- Engage Hold to freeze and loop a particularly complex rhythmic phrase, unleashing it again at will by releasing Hold.

---

## Percussive Effects (Punch, Grit, Uniqueness)

Since MultiMod isn’t a voice or audio effect, but a control voltage processor, you enhance percussiveness by:

- Rapidly modulating parameters of your actual drum synths/modules.
- Using random or heavily phase-shifted outputs for “off-the-grid” triggerings.
- For punch: Phase offset outputs to create micro-timing variation, pseudo-flams, handclap clusters, etc.
- For grit: Send noise or audio-rate pulses into Signal In and use shaped, phase/scattered outs to create randomized, glitchy modulation of percussive parameters.
- For uniqueness: Hyper-modulate Spread, Phase, and Shape with external sources (random, sequencers, envelopes) continually through the performance.

---

## Power Tips

- **All outputs are attuned to your input signal’s changes at different times; automating or jamming with the input signal leads to cascading pattern development across all outs.**
- Use Shape’s random modes with non-LFO input (random gates, envelope followers, etc.) for weighted randomizations of your entire percussion kit.
- Create coupling between percussion “voices” by cross-patching MultiMod outputs to each others’ mod and trig ins.

---

For even more inspiration, check the manual’s [Patch Corner](https://makenoisemusic.com/manuals/multimod-manual.pdf) and **Appendix: LED Cheat Sheet** for real-time feedback on what your MultiMod outputs are doing.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)