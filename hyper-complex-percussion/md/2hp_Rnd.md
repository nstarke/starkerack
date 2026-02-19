# 2hp — Rnd

- [Manual PDF](../../manuals/2hp_Rnd.pdf)

---

[**2hp Rnd Manual (PDF)**](https://2hp.com/wp-content/uploads/2018/03/rnd_manual.pdf)

---

# Using the 2hp Rnd for Hyper-Complex Percussion & Rhythms in Eurorack

The **2hp Rnd** is a powerful random gate and random voltage source that becomes a playground for experimental rhythmic and percussive synthesis. For the creation of dense polyrhythms, complex meters, and intricate percussive patterns, this compact module can be leveraged in several creative ways:

---

## Clocking, Gates, and Rhythms

### 1. **Randomized Gate Patterns (Polyrhythmic and Complex Sequences)**
- **External Clock Mode:**  
  Send a non-standard (e.g., quintuplet, 7/8) clock into the **CLOCK IN** jack.  
  - **Rate Knob** shapes the density and probability of the random gates.
  - **Gate Output** will generate unpredictable triggers at non-binary subdivisions, perfect for hyper-kinetic or polyrhythmic percussion tracks.

- **Patch Example:**  
  - Use a rhythmic step sequencer or clock divider to provide several mismatched clocks to multiple Rnd units.  
  - Output random gates to varied percussion voices (hi-hats, metallic pings, clicky samples) for organically evolving, interlocking patterns.

### 2. **Internal Clock for Steady Rhythms with Unpredictable Modulation**
- **Internal Clock Mode:**  
  Use the **Rate Knob** to set a base tempo, outputting a standard clock to a trigger sequencer or drum voice.
  - Stack multiple Rnd modules for layered, phase-shifted clocks and polyrhythms.

- **Randomization Layer:**  
  Send the random gates to percussion accents, fills, or ratchets—combining steady beats with sudden bursts of chaos that are always time-synced.

---

## Modulating Percussion: Unique, Punchy Sounds

### 3. **Generate Unique Modulations with Smooth & Quant Outputs**
- **Smooth Output:**  
  - Sends a constantly morphing random CV (0V-10V).  
  - Use **Smooth Attenuator** to fit modulation depth.  
  - Patch to VCA, VCF, or percussion voice FM input for dynamic, wildly animated timbres or envelope shapes.

- **Quant Output:**  
  - Each clock pulse emits a stepped random voltage for sample-and-hold effects.  
  - Clock this at an odd division for shifting, jerky dynamics in percussive voices (panning, pitch, filter cutoff).

- **Example:**  
  - Smooth CV to the decay time of a drum envelope—get lively, swerving tails.
  - Quant CV to oscillator pitch or drum sample selector for generative, unpredictable patterns.

---

## Advanced Patching Ideas for Hyper-Complex Percussion

| Goal                      | Patch Suggestion                                                                                   |
|---------------------------|---------------------------------------------------------------------------------------------------|
| **Unusual time signatures**| Run the Rnd’s Gate Output to a clocked logic module or rhythmic addressable switch                |
| **Densely layered rhythms**| Chain multiple Rnd modules, each with different clock sources and modulate each other's Rate Knob|
| **Chaotic event accenting**| Use the random gate output to punch in effects (reverb bursts, distortion) on percussion hits     |
| **Meta-polyrhythm creation**| Use Slew (Smooth Out) as a clock modulator, warping the perceived tempo of other rhythmic modules|

---

## Sound Design Tips

- **Punch and Snap:**  
  Patch the stepped (Quant) output to both pitch and VCA envelopes for percussive voices.  
  Apply sharp, high-pass filtered Smooth CV for snappy transient modulations.
- **Organic Variation:**  
  Use attenuators to finely scale randomness—keep patterns musical, not purely chaotic.
- **Flavor Multiple Voices:**  
  Mult or sequential switch Rnd’s outputs to apply its unique movement across your drum architecture.

---

> *The 2hp Rnd is not a voice or effect by itself, but as a control/modulation generator can transform even basic drum modules into wildly animated, complex, and rhythmically rich percussive sources.*

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)