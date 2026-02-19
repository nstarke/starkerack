# 2hp — Euclid

- [Manual PDF](../../manuals/2hp_Euclid.pdf)

---

[2hp Euclid Manual PDF](https://2hp.com/docs/euclid.pdf)

---

# Using the 2hp Euclid for Densely Rhythmic and Hyper Complex Percussion Sequences

The **2hp Euclid** is a compact Eurorack module designed to generate Euclidean rhythms, which are mathematically distributed rhythmic patterns prized for their natural feel and musical utility. Here’s how you can use it in the pursuit of dense, hyper-complex percussion and polyrhythmic sequences:

---

## Key Features for Complex Rhythms

- **Euclidean Pattern Generation:** Creates patterns by distributing a set number of active steps as evenly as possible within a pattern length (1–16).
- **CV Control Over Parameters:** Modulate the number of steps, pattern length, and offset for real-time rhythmic morphing.
- **Ultra Narrow (2HP):** Integrates easily into even the most crowded systems.

---

## Approaches for Hyper-Complex Rhythms

### 1. Polyrhythms & Complex Time Signatures

- **Varying Lengths:** Patch several Euclid modules (or mult its output for offset control, see below) to gates of different pattern lengths (`LENGTH` parameter) e.g., 5, 7, 12, 13, etc. and combine their outputs with other percussion triggers. The mathematical nature of Euclidean distribution makes cross patterns immediately polyrhythmic.
- **Asymmetric Stepping:** Non-traditional pattern lengths (e.g., 11 steps, 13 steps) create complex, non-4/4 grooves. Adjust with the `LENGTH` knob or voltage control.

### 2. Pattern Complexity

- **Dynamic Step Density:** Use the `STEPS` control to alter the number of active triggers per pattern. Modulate this with CV for evolving, organically thinning/thickening patterns—great for IDM, glitch, and experimental rhythms.
- **Pattern Morphing:** Patch slow LFOs or stepped random voltage sources into the `LENGTH CV` and `STEPS CV` inputs, continuously morphing the density and length, creating ever-changing sequences.

### 3. Percussive Uniqueness

- **Offset Control:** The `OFFSET` pot lets you phase shift your rhythm. When clocking multiple voices with multiples of the Euclid, slight offsets between channels are a classic trick for bubbling, syncopated percussion.
- **Layered Complexity:** Stack or interleave outputs with other trigger/pattern sources, using Euclid as the base clock or accent pattern for hybrid, intricately layered rhythms.

### 4. Integration with Percussive Voices/Effects

- **Trigger Any Percussion Source:** Use the Euclid's trigger output to fire drum modules, samplers, or synth voices. For punchy and “spicy” results, route to envelopes with fast attacks/decays driving VCAs or filters after noise/tone sources.
- **Accent Generation:** Mult the Euclid output, using one path direct to percussion and another to kick an accent CV, distortion, or rapid envelope, making sounds cut through and feel more ‘alive’.
- **Voice Uniqueness:** Always try modulating not just the rhythm but the source voice. Pair evolving Euclidean triggers with a drum voice whose tone (pitch, decay, filter cutoff) changes per hit.

---

## Advanced Patch Tips

- **Logic Combinations:** Use logic modules (AND, OR, XOR) to combine Euclid triggers with other clocks—generates even more intricate, hybrid rhythms for complex sequencing.
- **Clock Division/Multiplication:** Use clock processors after Euclid to stretch or compress the rhythmic output, adding yet another level of structural complexity.

---

Keep in mind, the **2hp Euclid** is not a sound source or effect processor itself, but a rhythm/trigger generator. Its voice or timbral uniqueness therefore comes from how you patch and process the voices being triggered downstream. To maximize complexity: **modulate parameters, layer outputs, and use creative clocking and voltage control!**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)