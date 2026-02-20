# Noise Engineering — Numeric Repetitor

- [Manual PDF](../../manuals/NR_manual.pdf)

---

[**Noise Engineering Numeric Repetitor Manual (PDF)**](https://manuals.noiseengineering.us/NR/NoiseEngineering-Manual-NumericRepetitor.pdf)

---

# Creative Modulation with the Numeric Repetitor: Distorted Percussion, Dubstep Bass, and Haunting Pads

The **Noise Engineering Numeric Repetitor** is a powerful rhythmic gate generator based on prime rhythm patterns and binary multiplication. The real magic in the module comes from modulating CV inputs (PRIME and FACTORS) and clever patching. Let's dive into some advanced modulation strategies tailored to create:

- Distorted rhythmic percussion
- Complex, evolving basslines (dubstep/DNB)
- Haunting, atmospheric pads

---

## Key Modulation Inputs

- **PRIME (knob & CV):** Selects base rhythm pattern
- **FACTOR 1-3 (knob, CV):** Modifies the product/variation of the main rhythm (multiplicative, offset, and bit-masked variations)
- **BEAT input:** Clock source (dictates pattern rate)
- **MEASURE input:** Resets pattern to start (can use for rhythmic resets/glitch effects)

---

## Techniques & Patch Ideas

### 1. Distorted Percussive Rhythms

**Goal:** Glitchy, evolving, or even aggressive rhythms for metallic hats, broken claps, or industrial drums

**Patching & Modulation Tips:**

- **CLOCK:** Patch an audio-rate clock (very fast LFO or even audio oscillator) for hyper-fast triggering or clock it at normal rates for groove. Drive the BEAT input hard for ratcheting or machine-gun rolls.
- **GATES ➔ Distortion/Eurorack Effects:** Route Numeric Repetitor outputs (PRIME/PRODUCTS) to drum envelopes/VCA combos controlling analog drum modules, or straight into audio-rate distortions (bitcrushers, wavefolders, etc.) for harsh artifacts.
- **CV MODULATION:** Assign random voltages, slow LFOs, or a stepped CV sequencer (like from Turing Machine/Random Source) to one or more FACTOR CVs. Extreme, sudden changes can create unpredictable gating patterns—useful for glitch or IDM percussion.
- **RESET/TRIG HACK:** Use the MEASURE input with random, audio-rate, or odd-patterned gate sources (like a burst generator or random divider). This can add stun-gun resets and pattern choking.

---

### 2. Complex, Evolving Basslines (Dubstep/DNB Style)

**Goal:** Syncopated, off-beat, or morphing bass patterns, kill-switch wobbles, and binary gate sequencing

**Patching & Modulation Tips:**

- **BASS OSC GATING:** Gate bass oscillator VCAs or filter cutoff with PRODUCT outs. You get tight, snapped-on bass notes—especially powerful through a saturated lowpass.
- **MULTI-PRODUCT:** Mix multiple PRODUCT outputs through a logic OR or analog mixer, and send the merged signal to the bass module to create hybrid gate curves.
- **PRIME PATTERN CV:** Modulate the PRIME input with a synced sequencer, envelope, or randomly-stepped CV to jump through pattern banks as the bass phrase unfolds. Example: a slow LFO upwards sweep gives rising rhythmic complexity.
- **FACTOR MOD & GLIDE:** Use CV glide sources or S&H with slew (think "wobble" control) into a FACTOR input to change the feel and movement of the underlying rhythm.
- **BASS AUDIO MOD:** Ring modulate your bass waveform with a fast squarewave that matches the rhythm of a Numeric Repetitor PRODUCT output for digital choppiness.

---

### 3. Haunting Atmospheric Pads

**Goal:** Ethereal, shifting textures and gating patterns to modulate pads, granular clouds, or harmonic drones

**Patching & Modulation Tips:**

- **PAD GATING:** Patch Numeric Repetitor CHANNEL outputs to open/close the VCA or LPG on a long-attack/release pad voice; try PRODUCT 2/3 for less regular, more "living" patterns.
- **HARMONY LAYERING:** Send PRODUCT gates to trigger different envelopes or VCAs on several voices (sine, triangle, granular) for dispersed and polyrhythmic pad events.
- **SLOW MODULATION:** Modulate FACTOR and PRIME with very slow LFOs or envelope followers from another voice in the patch—field recordings, voice samples, or environmental sounds (through an envelope follower) work well.
- **BANK SWITCH:** Use the SET switch live or via manual intervention at key moments for immediate, dramatic shifts in rhythm texture.
- **REVERB/DELAY POST:** After gating, send audio through big reverbs, shimmer delays, or spectral processors for a truly haunted, evolving soundscape.

---

## Combining Approaches

- **Hybrid Madness:** Use MULTs to send the same clock to NR and other modulators (envelopes, sequencers) for intricate cross-rhythms.
- **CV Recipes:** Try a CV mixer to blend multiple LFOs/steps for PRIME or FACTOR modulation—this yields incredibly morphing rhythms.
- **Feedback:** Route one PRODUCT gate to a trigger sequencer that, in turn, modulates the NR's own FACTOR input—a self-influencing pattern!

---

## General Tips

- Experiment with **audio-rate CV modulation** for digital chaos (especially on FACTOR CVs) for completely new textures.
- Use slow random walks or quantized S&H to keep patterns organic but non-repeating.
- The **MEASURE** input is powerful for re-timing and adding live “pattern cut” effects—don't overlook it!

---

**[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**
