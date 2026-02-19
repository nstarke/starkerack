# 2hp — EG

- [Manual PDF](../../manuals/EG_Manual-7ja4.pdf)

---

[**EG 2HP Envelope Generator Manual (PDF)**](https://2hp.com/docs/EG/2hp_eg_manual.pdf)

---

## Using the 2hp EG for Dense, Hyper-Complex Percussion

The 2hp EG is an ultra-compact, full-featured two-stage envelope generator. In your pursuit of hyper-complex, densely rhythmic percussion with polyrhythms, odd time signatures, and wild textures, this module can become a central utility—especially if you’re working within tight HP constraints or want multiple envelope generators in your system.

### Core Strengths for Complex Percussion

- **Ultra-Fast to Ultra-Slow Envelopes:** Ranges from punchy 3ms attacks/decays up to sprawling 11 minute swells per stage.
- **Linear/Exponential Curve Options:** Dial in snappy "percussive" or smooth "natural" contours on the fly.
- **Built-In CV Attenuator:** Modulate your envelope amplitude for dynamic grooves or evolving accent patterns.
- **Dedicated CV Over Attack/Decay:** Voltage control means you can sequence or modulate your rhythmic shapes for intricate patterns.
- **Tiny Form Factor:** Stuff more envelope action into your case for maximal layering.

---

### Strategies for Generating Complex, Rhythmic Percussion

#### 1. **Multiple EGs for Polyrhythms**
To exploit advanced rhythms, use several EGs—each trigged by a different clock division, pattern generator, or probabilistic gate. Sum their outputs to a VCA or combine them to modulate different drum/percussion voices, with each generator shaping a distinct percussive event at a distinct rhythmic subdivision.

**Example Patch:**
- EG1: Trigged by a 5-step clock; CV modulating decay with a random stepped generator for irregular swing.
- EG2: Trigged by a 7-step clock; CV modulating attack from a Euclidean pattern.
- Both envelopes go to separate VCAs/drum modules, or are mixed to create staggered, polyphonic percussion bursts.

#### 2. **Envelope Modulation for Evolving Grooves**
The CV inputs for attack and decay are critical for programmed complexity. Use LFOs, stepped random voltages, sequencers, or envelope followers to continually change the envelope shape.

- Random stepped CV to Decay: Each trig results in subtly (or drastically) different envelope lengths for organic percussion.
- Euclidean gate/patterns to Attack CV: Shifting how "punched" or "soft" each hit is for expressive grooves.

#### 3. **Linear vs Exponential**
Switch between linear and exponential responses for each rhythm or even automate the toggle with a “hand-on” approach during performance. Linear provides harder, more mechanical percussion; exponential gives you snappier, more natural drum contours.

#### 4. **Attenuation for Accent Patterns**
The AMP knob can be used to program accents: Manually or via CV, reduce amplitude on unaccented steps to create ghost notes, or amplify certain pulses to make accented hits pop.

#### 5. **Envelope as Audio Source**
For even more unique results: Use the envelope OUT as an audio-rate source for "clicks," “ticks,” or layered percussive noise, especially with fast decay settings. The module slams out fast voltage spikes that can be filtered or waveshaped for glitchy percussion.

---

### Pro Tips for Uniqueness, Punch, and Percussiveness

- Use very fast attack/decay times with exponential response for “transient designer” style punch.
- Stack several EGs for layered transients, each modulated separately to avoid robotic repetition.
- Route EG outs to filter CVs (especially ultra-snappy attacks) to create "snap" or "pluck" percussion, or to FM drum VCOs for clicky, metallic timbres.
- Combine envelopes of different lengths (polyrhythmic cycling) for non-repeating grooves.
- Change attack/decay times on the fly with sequencer lanes assigned to CV ins for morphing between percussive feels.

---

**More Details:**
For exact jack and knob placement, power ratings, and user controls, view the full manual [here](https://2hp.com/docs/EG/2hp_eg_manual.pdf).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)