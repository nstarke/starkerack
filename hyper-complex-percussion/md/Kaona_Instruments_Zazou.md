# Kaona Instruments — Zazou

- [Manual PDF](../../manuals/Zazou_manual_ENG_V1-0.pdf)

---

[**Zazou Manual PDF**](https://www.kaona.fr/_files/ugd/7f371b_965c1827e6f74eaa80eb467ed5e2c282.pdf)

---

# Using Zazou for Densely Rhythmic, Complex Percussion and Polyrhythms

Zazou is a powerful generative melodic sequencer, but with creativity, it can absolutely drive rhythmically dense, hyper-complex polyrhythmic percussive setups in a Eurorack environment. Here’s how to use it for such explorations, especially when pairing it with drum/percussion voices and modules that respond musically to melodic triggers.

## 1. **Zazou is Not a Drum Voice—it’s a Note/Trigger Generator**
- **Key Point:** Zazou *does not* output sound; it outputs four channels of chromatic notes via MIDI, CV/Gate, and velocity.
- **How to Use:** Route Zazou's four gate outputs (and optionally pitch/velocity CV outs) into drum synth modules, samplers, or percussive synth voices. Many Eurorack percussion modules (like Basimilus Iteritas Alter, Plonk, etc.) react creatively to pitch and velocity modulation!

---

## 2. **Building Dense, Polyrhythmic Structures**

### **A. Use Gate Inputs Per Track for Independent Polyrhythms**
- **Each Zazou Track (Red/Yellow/Green/Blue) is triggered by its own gate input** (e.g., from your modular sequencer, clock divider/multiplier, or rhythm generator like Kaona's Skippy).
- **Set up gate patterns for each track that are different lengths or divisions:** For example, run:
  - Track 1 @ 4/4 pulse
  - Track 2 @ triplet rhythm
  - Track 3 @ 5-step euclidean rhythm
  - Track 4 @ 7-step loop
  
  This instantly generates polyrhythmic interaction as Zazou is only triggered when each track’s gate input is high.

### **B. Manipulate Sequence Length, Steps, and "Alternate" Functions**
- In the **Sequences** screen (Long press encoder 2), experiment with:
  - **STEPS CHANGE:** Use different values per track (e.g., 3, 4, 5, 7 steps). Uneven lengths guarantee phase-shifting and evolving composite rhythms.
  - **REPEAT CHORD:** Stretches or abridges the number of fires before changing to next chord/step; use per track.
  - **ALTERNATE M/m & RND ALTERNATE:** Generates harmonic/rhythmic variety as sequence steps may flip mode.

### **C. Apply Advanced Algorithms for Unpredictable Patterns**
- **ARPEGGIO**, **CANTOR**, **Sierpinski**, **WalkingBass**—these can all create repeating or self-similar note patterns.
- **Use “Random” algorithm** for unpredictable step lengths and note repetitions.
- **Serial** (chromatic/12-tone row) for maximum complexity and dense note patterns (good for triggering percussion where pitch-value is not semantically musical, but variety is key!).

---

## 3. **Gate Lengths, Velocity, and Modulation for Percussion**
- **Gate Length:** Set note duration as “Gate” (matches your input gate’s length for tight, percussive effects) or experiment with polyrhythmic note durations per track.
- **Velocity CV:** Route to CV input of percussive modules for dynamic accents, expressiveness, and variation.
- **Pitch CV (1V/oct):** Some drum modules change timbre/model with pitch; randomize or algorithmically wiggle this parameter via Zazou for unique hits.

---

## 4. **Live Manipulation & Real-Time Improvisation**
- **Mute/Unmute in Live Mode:** Use track buttons to remove or bring in streams instantly.
- **Change/Reset/Step by CV or Button:** Manual or CV control for on-the-fly pattern resyncing or “one-shot” percussive fills.
- **Algorithm and Ornament On-the-fly Adjustment:** Select and adjust arpeggio, recursion, or fractal parameters for evolving complexity without stopping the music.

---

## 5. **Complex Time Signatures**
- **Zazou doesn’t provide “meter” but does allow sequences, steps, and gates of arbitrary length/input—so YOU decide the pulse and composite signature.**
- **Feed Zazou’s tracks odd-length Euclidean patterns, clock multipliers/dividers, or even external polyrhythmic triggers** (pam’s new workout, Batumi, Tempi, etc).

---

## 6. **Tips for Unique, Punchy, Percussive Results**
- **Patch one or more tracks to melodic percussion (Plonk, Rings, BIA, etc.) and let Zazou pitch/gate control give complex tuned percussion.**
- **Route velocity to modulate amplitude, filter, or decay for variety.**
- **Ornament/Trill/Repeat ornaments**: Use these to inject machine-gun fills, ratchets, flam effects, or jazzy rolls.
- **Arpeggio “Strum” and “Random” types**: These can emulate burst/vault/hit clusters.
- **Use CV-sequenced changes to jump between algorithms/sequences for "pattern morphing."**

---

## 7. **Modular Eco-system Pairings**
- **Skippy or any rhythm generator** for dense, Euclidean, or generative gate patterns as input.
- **Switches/mutes for abrupt pattern changes or generative gating.**
- **Clocked effects (delay, reverb) downstream for even more rhythmic complexity.**

---

## 8. **Saving and Recalling Hyper-Complex Setups**
- **Use the SD card file system to save and recall complex setups fast** (great for performing or A/B comparisons).

---

## 9. **Bonus Patch Idea**
- Use Zazou’s pitch CV as the “model select” on a percussive module (via quantizer/attenuator), so each fire switches drum sound or effect, driven by generative algorithms.
- Use four tracks with different polyrhythms each on a single 4-voice drum synth, for swirling, evolving, dense rhythm beds.

---

## Quick Reference: Key Zazou Manual Pages

- **Gate/Track Inputs:** p.3 / Quick Start
- **Algorithms/Ornaments:** pp. 7–15
- **Sequences/Step Settings:** p.16
- **CV/Gate Output Routing:** p.3, 8, 20

---

[**Zazou Manual PDF**](https://www.kaona.fr/_files/ugd/7f371b_965c1827e6f74eaa80eb467ed5e2c282.pdf)  
[**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)