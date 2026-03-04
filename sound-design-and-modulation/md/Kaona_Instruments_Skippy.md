# Kaona Instruments — Skippy

- [Manual PDF](../../manuals/Skippy_2-2_ENG.pdf)

---

[**Download the SKIPPY Manual PDF**](https://www.kaona.fr/assets/files/how-to-tame-skippy-en.pdf)

---

# Creative Modulation Strategies for Kaona Skippy

As a eurorack synth musician aiming to extract the wildest, most expressive sounds from your Skippy sequencer, here are some creative ways to use its features for **distorted percussive sounds**, **crazy basslines**, and **haunting pads/atmospheres**.

---

## 1. Distorted Percussive Sounds

### **Strategies:**
- **Random Gate Triggering (Proba & Chaos):**
  - Use SKIPPY’s **PROBA** (probability) function to randomly omit steps, adding unpredictability to percussive rhythms.
  - Dial in **CHAOS** to inject random timing between triggers—pair this with drum modules or noise sources for glitchy, erratic percussion.
- **Non-Metric/Logarithmic Timings (Gauss):**
  - Use **GAUSS** to distribute steps unevenly (high positive/negative values) for broken, stuttering rhythms. Feed these gates to distortion/wavefolder modules or even trigger retrigger envelopes for hard-hitting, evolving drum hits.
- **Gate Length Modulation (GATES):**
  - Experiment with very short and very long gate settings. Overlapping or micro-gated percussion can be perfect for distortion when passed through wave shapers or VCAs with nonlinear responses.
- **Irregular Tempos (WAY & Swing):**
  - Set **WAY** to “Ping Pong” for unpredictable bouncing rhythms.
  - Add **Swing** for syncopated, shuffled percussion—a staple in broken beat, DnB, and glitch genres.

---

## 2. Crazy Basslines (Dubstep / Drum & Bass)

### **Strategies:**
- **Euclidean & Polyrhythmic Patterns (EUCLID & POLYR):**
  - Use **EUCLID** to generate complex rhythmic gates—patch these to VCO sync, VCA, or filter cutoff for squelchy, syncopated basslines.
  - **POLYR** mode combines two tempi (e.g., 4/3, 5/4)—great for ever-shifting, non-repetitive bass sequences.
- **Probability Skips (PROBA):**
  - Set medium-to-high **PROBA** for skipping notes—makes basslines less predictable.
- **Step Modulation (SPIN & Tiles):**
  - Use **SPIN** to rotate step patterns on the fly, shifting the groove in interesting ways.
  - **TILES** can programmatically alternate silent and triggered steps, letting you create intentional gaps, tension, and rolling bass movement.
- **CV/Gate Processing Downstream:**
  - Use SKIPPY gates as envelopes or audio triggers for aggressive wave shaping, filter FM, or even direct oscillator re-triggering (hard sync).

**Patch Idea:**  
- Send SKIPPY gates to a LPG or VCA keyed to a detuned sine/saw. Modulate EG/ADSR parameters for varied punch; add a suboctave generator or audio-rate FM for dubstep growls and DnB reese textures.

---

## 3. Haunting Pads & Atmospheres

### **Strategies:**
- **Long Euclidean Sequences and Gaussian Timing:**
  - Use long, slowly evolving Euclidean patterns for ghostly, shifting pad gates.  
  - High **GAUSS** values stretch time unevenly—some notes will hang for seconds or more, perfect for slow-motion atmospheres.
- **Begin/End Arc Modulation:**
  - Use **BEGIN/END** to activate only a specific “arc” of the sequence—great for cyclically morphing drones or evolving textures.
- **Pause, Ping Pong, and Manual Resets (WAY):**
  - Freeze time with the **WAY** stop function, change parameters, and restart for sudden atmospheric shifts.
  - Ping Pong movement with slow steps helps build shimmering, tense pads.
- **Multiple Tracks, Multiple Destinations:**
  - Use all four color-coded tracks to control different timbral layers—trigger sample players, open VCA’s, modulate filters, control reverb skews, or crossfade between multiple sound sources.

**Patch Idea:**  
- Use slow **GAUSS**-distributed gates on one track to sweep through granular or sample-based textures; another track controls filter or reverb CV; a third intermittently triggers a noise generator or ring modular pad for spectral interest.

---

## Other Tips
- **External Clocking:** Use interesting, non-even clock sources (LFOs, other sequencers, clock dividers/multipliers) for generative, evolving patterns—especially powerful with SKIPPY’s MATRIX/POLY clock modes.
- **Save Happy Accidents:** SKIPPY has save/recall; grab your best results for live performance.

---

**References:**
- [Kaona Skippy Official Manual (PDF)](https://www.kaona.fr/assets/files/how-to-tame-skippy-en.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)