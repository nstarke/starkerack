# 2hp — Comb

- [Manual PDF](../../manuals/Comb_Manual.pdf)

---

[**Download the Comb Module Manual (PDF)**](sandbox:/mnt/data/Comb_2hp_Manual.pdf)

---

# Using the 2hp **Comb** Module for Full-Length Song Creation in Eurorack

Creating grooves, melodies, and bass lines in Eurorack is often straightforward—turning these jam moments into full-length, structured songs can be much more challenging. The **2hp Comb** module, with its IIR peaking comb filter architecture, offers unique and dynamic ways to provide song evolutions, transitions, and textural developments across an extended musical form. Below are detailed and practical strategies to harness this module—alone and with others—to make your tracks go from loop to song.

---

## Comb’s Strengths for Song Arrangement

- **Dynamic Timbre Control:** Adds harmonic richness or radical character shifts to virtually any audio source.
- **Voltage Control:** All key parameters (frequency, resonance, damp) are CV controllable—perfect for automation and modulation over a song timeline.
- **Feedback for Self Oscillation:** Can become a sound source itself, introducing new motifs or motifs-turned-atmospheres.
- **Damp Filter:** Moves between dark warmth and bright overtones on demand, useful for moment-to-moment contrast.

---

## Techniques for Turning Loops to Songs

### 1. **Intro/Outro Automation**
- Use subtle **comb filtering** on high hats or noise at the intro, gradually opening the damp or resonance CV for a slow reveal or build.
- For outros, do the reverse—turn up damp to slowly darken and dissolve textures.

### 2. **Transitional Sound Design**
- Automate FREQ and/or RES (with envelopes or LFOs synced to song phrasing) to dramatically morph a repeating phrase, cueing listeners to a new section (verse, chorus, break).
- Feed melodic or rhythmic content (bassline, sequencer) through Comb, automate parameters to sweep resonance or frequency during fills or transitions.

### 3. **Polished Drops and Builds**
- When a build-up is needed, increase resonance and brighten the damp to crescendo into a drop.
- Use fast CV modulations for comb frequency during fills/breaks for glitchy or shimmering effects.

### 4. **Thematic Variation/Development**
- Repeated motifs (melody, percussion) can be filtered with different Comb settings during each section, lending instant variety to a repeating line.
- Morph a clean lead into a string-like pad for bridges or breakdowns by increasing resonance and brightening damp.

### 5. **Layering and Texture**
- Mult out a signal (e.g., melody) to both dry and Comb-processed paths. Crossfade or switch between them for instant variation.
- Send white noise or field recordings through Comb for evolving pads behind other instruments.

### 6. **Self-Oscillation As Voice or Accent**
- Let Comb self-oscillate, and VCA/gate it rhythmically—either as a percussive element or a droning pitch—syncing its FREQ (comb’s cutoff frequency) to the song’s key or chords for harmonic interest.

### 7. **CV Automation and Performance**
- Use sequencers or function generators (like Make Noise Maths, Intellijel Quadrax) to modulate FREQ/RES/DAMP in time with your song structure.
- Record knob movements or use programmable CV sources to perform macro song-level shifts with Comb.

---

## Example Patch Ideas

- **Build a Pad Sweep:** Send a sustained VCO tone or noise through Comb, automate DAMP with an LFO/envelope, and bring in RES for a pad that rises in brightness/resonance toward a chorus.
- **Drum Processing:** Pass all percussion through Comb with slow modulation of FREQ & DAMP, blending clean and effected signals for evolving rhythm beds.
- **Bass Evolution:** Use low-resonance Comb filtering on a bassline, open up the resonance just for breakdowns or choruses.

---

## General Songflow Strategy with Comb

1. **Define Sections:** Assign distinct Comb settings to song parts (e.g., verse = subtle, chorus = bright and resonant).
2. **Introduce Automation:** Control changes over time via CV (sequencer, envelopes, LFOs, or manual wiggling).
3. **Create Movement:** Continuously vary Comb parameters on repeated motifs so they evolve—never remain static for long passages.
4. **Leverage Feedback:** Use self-oscillation or near-oscillation states as sonic signatures in intros, breakdowns, or transitions.

---

With its compact interface and deep modulation options, the **2hp Comb** gives you the power to move beyond static loops, organically sculpting and transforming the texture and shape of your songs in real time.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)