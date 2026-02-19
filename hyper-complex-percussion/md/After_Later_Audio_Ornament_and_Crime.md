# After Later Audio — Ornament and Crime

- [Manual PDF](../../manuals/ornament and crime.pdf)

---

[**Download Ornament & Crime v1.3 User Manual (PDF)**](https://ornament-and-cri.me/user-manual-v1_3/)

---

# Ornament & Crime for Hyper-Complex, Densely Rhythmic Percussion

Ornament & Crime (O_C) is exceptionally suited for creative rhythmic architectures: advanced polyrhythms, odd time signatures, Euclidean sequencing, and self-mutating patterns. While not a "voice" or "effect" module in the traditional sense, O_C becomes a powerful rhythmic engine/triggers brain or a “musical modulation” generator, ideal for sophisticated percussion sequencing. Here’s how to exploit it for densely rhythmic and hyper-complex percussion:

---

## Strategy: Use O_C as a Rhythmic Brain for Percussion

Rather than producing sounds directly, O_C spits out precisely controlled and wildly evolving CV/gate streams. Route these outputs to drum voices, percussion modules, sample players, or any CV/gate sources to drive rich rhythmic interplay. Chain, cross-patch, or layer with other sequencers for utter rhythmic mayhem or structure.

---

## Best O_C Apps for Advanced Rhythms

### **1. Piqued (Quad Voltage-Controlled Envelope/Trigger Generator w/ Euclidean/Polyrhythms)**
- **Euclidean Trigger Filters:** Turn each channel into a polyrhythmic/Euclidean trigger and envelope generator.
- **Pattern Length, Fill, and Rotation:** Per-channel control of how often an envelope fires within a set length—perfect for complex polyrhythms (e.g. 5 in 8, 3 in 7, etc.).
- **Variable Envelope Shapes**: Make your drum triggers not just gates but custom-shaped envelopes (very punchy, or slow ramps for “fuzzy” percussion).
- **Looping/Burst Mode**: Use the envelope looping/ratcheting for fast rolls, bursts, retriggering hi-hats, or glitchy hats.
- **CV Control**: Sequence or modulate envelope parameters for constant evolution/“mutation”.

**Patch Ideas:**
- *Euclidean Triggers*: Channel A = Kicks (5 in 8), B = Snares (3 in 8), C = Claps (7 in 13), D = Perc Hits (2 in 9).
- *Envelope Loops*: Self-retrigger envelopes for rapid burst percussion.
- *Randomize*: Modulate Euclidean parameters or envelope durations with LFO/CV for shifting grooves.
- *Chained Envelopes*: Use end-of-cycle (EOC) as triggers for other envelopes (drum fills that trigger new hits).

---

### **2. Dialectic Ping Pong (Bouncing Ball Envelopes for Chaotic Percussion)**
- *Simulates physics of bouncing balls*—inherently non-grid, evolving rhythmic trigger/gate sequences.
- *Control initial amplitude, gravity, “bounce loss”, retrigger count—ideal for swinging, accelerating, decelerating percussion patterns.*
- Great for flams, fills, fills, rolls, and “organic” ever-mutating percussive movement.

**Patch Idea:** Use several channels with different gravities and loss to trigger “drunken” percussion.

---

### **3. Sequins (Dual 4x16-Step Sequencer with Pattern Chaining, Direction, Probability, Randomness)**
- *Chain patterns together for extremely long/complex sequences.*
- *Any channel can be clocked by a different clock for ratio-based polyrhythms (e.g., one at 9 triggers, the other at 8).*
- *Direction: random, pendulum, Brownian motion: introduces variation and anti-repetitive rhythms.*
- *CV addressing: CV controls step position for non-linear drum triggering (e.g. live modulation of sequence steps).*

---

### **4. Piqued + Sequins Hybrid**
- Use Sequins CV outputs to modulate envelope length, fill amount, or step count on Piqued, turning your percussion lines into evolving, self-mutating polyrhythmic monsters.

---

### **5. Meta-Q (Quantizer with Scale/Mask/Step Sequencing)**
- Use dual quantizers to mangle drum pitch, or—by feeding stepped modulation from an LFO or random source—send irregular clocking/gates to percussion modules.

---

### **6. Harrington 1200 / Automatonnetz (Chord & Transformation Triggering)**
- *Euclidean trigger masks per transformation (PLR/NSH)*: Not limited to melody—use to gate percussive elements with logic or sequential “rhythmic chord changes”.
- *Programmable transformation order/priority gives shifting accents and “hiccuping” patterns.*

---

### **7. Viznutcracker, sweet! (ByteBeat)**
- *Bytebeats can be clocked by external or Euclidean triggers—use them as CV for drum parameter “glitch FX” or (with slew/quantize) as unpredictable stepped mod signals.*
- *Audio-rate bytebeats patched into a VCA/Filter, triggered by rhythmic envelopes, become abrasive percussion blocks.*

---

## Making Percussion Unique, Punchy, and Percussive

1. **Dynamic Envelope Shaping:** In Piqued, modulate attack/release/shape per striking event for every hit to be slightly different—keeps percussion from sounding static.
2. **Fast Envelope Modulation for "Punch":** Short snappy attack, variable decay and amplitude (modulate with sequencers/LFO for “living” drums).
3. **Self-modulation:** Patch O_C outputs to your drum modules, and route their envelope (or amplitude) CV out back into O_C’s CV inputs for auto-evolving rhythms.
4. **Cross-Channel Triggering/Chaining**: Chain EOC to trigger other envelopes for layered percussion, micro-fills, or ghost notes.
5. **Ratchets and Burst Envelopes:** Use Piqued’s max loops + retrig envelopes for ratchets/trills—great for hats, snare rolls, or machine-gun fills.
6. **Envelope Shapes:** Use “wiggle” and “dipper” shapes for more organic percussive envelopes, or Gate shape for hard-edged triggers.

---

## Patch Tips for Complex Polyrhythms

- **Multiple Clocks:** Feed separate, non-multiplicative clocks to each O_C channel.
- **Euclidean Mode Everywhere:** Dissimilar pattern lengths & fills per channel = layers of poly-metre, always shifting.
- **External Modulation:** Modulate Euclidean fills/offsets with slow LFOs, stepped CVs, or even other O_C channels for algorithmic, never-repeating patterns.
- **Brownian/Rnd Directions:** Let patterns “walk” or “jump” randomly for controlled chaos.
- **Envelope/Gate Logic:** Sum, XOR, or logic-combine envelope outs for even denser triggers.
- **Chain O_C with Sequential Switch or Matrix:** Route these rhythms dynamically to different voices, drums, or FX for "live remixing".

---

## Exploiting Output Uniqueness

- **Drum Voice Pitch/Bend/Fx:** Use O_C’s evolving envelopes/CVs to modulate pitch, filter, decay, overdrive, or wavetable position in drum and percussion voices.
- **Bytebeat Glitches:** Use Viznutcracker’s audio outs for digital “clap” or “noise” components, filter heavily, and mix with regular drums for one-of-a-kind hits.

---

## Practical Application Example

**Patch: Polyrhythmic Euclidean Drum Machine**
1. Set Piqued Channel A: Euclidean (5 fills, 7 steps, offset 0)—to trigger Kick.
2. Channel B: (13, 16, 3)—Snare.
3. Channel C: (7, 9, 2)—Clap/Conga.
4. Channel D: (3, 5, 0)—Hi-Hat, with looping AD envelope.
5. Modulate fill and offset with slow LFOs or random CV.
6. Use Sequins to modulate Piqued’s envelope length/randomness per hit.
7. Crosspatch EOC from one envelope as retrigger to another for microfills.
8. Send Bytebeat or Lorenz attractor out to modulate filter/decay/pitch for accent and random FX.

---

## Further Reading

- [Ornament & Crime v1.3 User Manual (Web)](https://ornament-and-cri.me/user-manual-v1_3/)
- [O_C Scales and Custom Scales](https://ornament-and-cri.me/custom-scales/)
- [Mutable Instruments Grids/Peaks for Euclidean Inspiration](https://mutable-instruments.net/modules/grids/)

---

**Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)**