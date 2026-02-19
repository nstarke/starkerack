# Noise Engineering — Numeric Repetitor

- [Manual PDF](../../manuals/NR_manual.pdf)

---

[Noise Engineering Numeric Repetitor Manual (PDF)](https://static.noiseengineering.us/static/manuals/Noise%20Engineering%20Numeric%20Repetitor%20Manual.pdf)

---

# Using the Numeric Repetitor for Hyper-Complex Polyrhythmic Percussion

The **Noise Engineering Numeric Repetitor** is a rhythm generator that excels at producing rich, evolving, and highly complex rhythmic material thanks to its unique approach using binary arithmetic. You're aiming for dense, interlocking rhythms and intricate time signatures — the Numeric Repetitor is an outstanding tool for this kind of work. Here’s how you can leverage it to create hypertight, punchy, and intricately layered percussion:

## 1. **Harness Core Polyrhythmic Structures**

- **Patch One Clock, Get Four Independent Gates:**  
  Start by patching a master clock into the BEAT input. Then, route each of the four outputs (PRIME + PRODUCT 1-3) to different percussion voices or envelope generators.
- **Select and Morph Patterns:**  
  Use the PRIME knob and/or CV input to sweep through 32 meticulously curated 16-step patterns, each designed for rhythmic interest. Sweeping or CV-sequencing the PRIME input allows immediate switching between core rhythmic building blocks (with no two being rotationally similar!).  
- **Accent Polyrhythms with Product Outputs:**  
  The PRODUCT outputs generate variations based on multiplying the PRIME pattern with “factors.” Each PRODUCT output can be offset and modulated independently (via knob or CV input), producing mathematically related but rhythmically unique sequences — the heart of polyrhythmic and polymetric work.

## 2. **Go Beyond 4/4: Complex Time Signatures**

- **Exploit the Measure Reset:**  
  Use the MEASURE input or manual reset to impose phrase lengths not evenly divisible by 4, 3, or the PRIME length. This creates looping cycles of varying length, laying the foundations for complex time signatures and evolving meters.
- **Product Multipliers for Meter Modulation:**  
  Employ the FACTOR knobs and their associated CVs to modulate the multiplication factors live — running Euclidian rhythms against prime-based binary patterns, resulting in a-typical feels and time signatures. Automate these with slow LFOs or step sequencers for morphing, emergent rhythms.

## 3. **Dense, Evolving Groove: Pattern Modulation Techniques**

- **Cross-Modulate with External CV:**  
  Use a divided or otherwise processed version of your master clock to modulate the FACTOR inputs. E.g., clock-divide by non-standard factors to push and pull rhythmic accents “off grid.”
- **Layering with Other Euclidean Modules:**  
  Output gates from Numeric Repetitor to percussion voices already running Euclidean or other algorithmic rhythms for polyrhythmic complexity.

## 4. **Punchy Percussive Sound Design Tips**

Even though Numeric Repetitor is a gate sequencer and not a voice or effect, how you patch it influences your punch and percussive articulation:
- **Trigger Fast, Snappy Envelopes:**  
  Use its gates to ping LPGs (Low Pass Gates) or tight envelopes — Numeric Repetitor is fast and accurate, great for complex, clicky percussion.
- **Accent Randomization:**  
  Patch the PRODUCT outputs to modulate not just “triggers,” but also CV-ins of percussion modules (e.g., pitch, decay, or distortion) for additional movement and dynamic surprise.
- **Dynamic Variation:**  
  Automate PRIME and FACTOR CVs using sequencers, S&H, or LFOs for evolving, morphing, but related percussion patterns.

## 5. **Advanced Tricks**

- **Binary Logic Patchwork:**  
  Use the different PRODUCT outputs into logic modules (AND, OR, XOR), and recombine with gates from other sequencers.
- **Self-Clock:**  
  Feed one of Numeric Repetitor’s outputs back into a related module as a clock multiplier/divider or reset — producing spiraling, semi-self-referential polyrhythms.

## 6. **Patch Example: Dense Layered Polyrhythms**

1. Patch a 16th-note clock to BEAT.
2. Send 4 Numeric Repetitor outputs to 4 percussion voices.
3. Modulate the PRIME CV with a stepped random, changing every 2 bars.
4. Modulate FACTOR 1 with a slow triangle LFO.
5. Send a reset signal every 5 or 7 beats to MEASURE input for phasing effects.

---

This approach allows you to move from tight, groove-heavy patterns into wild, unpredictable territory without losing the “punch” and sync demanded by dense, modern percussion. The organic yet algorithmic rhythm generation is well-suited to techno, IDM, modular hip-hop, and experimental beat-making.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)