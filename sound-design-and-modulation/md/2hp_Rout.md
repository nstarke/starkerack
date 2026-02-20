# 2hp — Rout

- [Manual PDF](../../manuals/Rout_Manual.pdf)

---

[Download the Rout Manual (PDF)](https://2hp.com/docs/Rout_Manual.pdf)

---

# Patch Tips: 2hp Rout Module for Advanced Sound Design

## Module Overview

**2hp Rout** is a voltage-controlled gate switch. It takes a single gate/trigger input and, based on manual selection or control voltage (CV), routes that input to one of four outputs. The module shines at pattern distribution, variation creation, and gate routing under automation.

You can modulate which output the gate is sent to by:
- Turning the **SEL** knob manually, or
- Applying a CV (0-5V) to the **SEL CV** input.

Outputs are only active when selected; each has an associated LED indicator.

---

## Creative Modulation Strategies

### 1. Distorted Percussive Sounds

**Goal:** Use Rout to trigger samples, envelopes, or percussive voices in unpredictable, digitally sharp/rhythmic ways.

#### Method:
- Use a fast, highly variable LFO, stepped random, or envelope as the **SEL CV** source.
- Input: Supply regular clock/gate or snappy percussive triggers.
- Route outputs to different drum synth voices or into the same voice with differing effect chains/distortion.

**Tip:** Because Rout only switches which output gets the gate, you can use it to rapidly alternate which drum or sample gets hit, especially effective if the sound chains have aggressive wavefolders, bitcrushers, or other distortion effects downstream.

#### Example Patch:
- Clock/gate from sequencer → INPUT
- Stepped random CV (e.g., Sample & Hold) → SEL CV
- OUT 1 → Analog kick channel (patch to distortion/saturation)
- OUT 2 → Heavy processed snare (bitcrusher/EQ)
- OUT 3 → Metallic noise (modulate filter, add reverb)
- OUT 4 → Open hi-hat or glitch voice
- Tweak SEL CV depth/range for unpredictable, evolving patterns.

---

### 2. Crazy Dubstep/Drum & Bass Basslines

**Goal:** Gate switch multiple bass voices or effects chains for movement and rhythmic complexity.

#### Method:
- Use a rhythmically synced envelope or complex LFO for the **SEL CV**.
- Input: Sequence or arpeggiated bass trigger pattern, or a steady gate.
- Outputs: Route to different bass synths or effects-inserts (formant filter, distortion box, ring mod, etc.).

**Tip:** Rout is especially powerful if you have several filter/distortion/wave-shaping chains in parallel and want to "flip" a single bass synth through those paths per step.

#### Example Patch:
- Sequencer gate (sync’d to main groove) → INPUT
- Audio-rate LFO or sequencer CV lane → SEL CV
- OUT 1 → Clean sub (lowpassed, un-fx’d)
- OUT 2 → FM/Resonator chain for growls
- OUT 3 → Tape stop/bit reduction
- OUT 4 → Highpass or phaser for laser FX
- Use Rout’s switching to chop between growls, subs, and movement in a bassline—perfect for DnB/dubstep switches.

---

### 3. Haunting Atmospheric Pads/Layers

**Goal:** Create evolving pads with dynamic triggers/envelopes sent to different mod sources or effect chains for a ghostly, morphing feel.

#### Method:
- Slowly evolving LFO (like a slow triangle or sample & hold) to **SEL CV**.
- Input: Occasional, irregular gates from a random rhythm source or even a field recording’s transient detector.
- Outputs: Route each to a different modulation destination—VCA triggers on different pad layers, reverb bloom triggers, spectral shift accents, etc.

**Tip:** Since Rout can move gates to any path, use it to randomly (or intentionally) enliven layers of a pad with different amplitude contours, effect “pops,” or filter sweeps, making the pad never exactly repeat.

#### Example Patch:
- Granular/atmospheric sample voice gate → INPUT
- Ultra-slow LFO (or manual modulation) → SEL CV
- OUT 1 → Triggers long ADSR on one pad oscillator
- OUT 2 → Sends +5V to freeze a shimmer reverb
- OUT 3 → Pings LPG for ghostly clicks/perc
- OUT 4 → Opens a VCA on a sub-bass texture
- Adjust SEL (w/ manual or CV automation) to determine haunting evolutions and unpredictable accents in the ambient wash.

---

## Extra Tips

- **Combine Rout with a clock divider/multiplier for more complex polyrhythms.**
- **Use stepped random or quantized noise for SEL CV for stochastic pattern generation.**
- **Route Rout outputs to trigger sequencer resets, modulation changes, or even clock resets for extreme structural variations.**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)