# Klavis — Grainity VCF

- [Manual PDF](../../manuals/Klavis_-_Grainity_User_Manual.pdf)

---

[**Klavis Grainity User Manual (PDF)**](https://www.klavis.com/into-the-drift/Grainity_UserManual_RevA.pdf)

---

# Using the Klavis Grainity Granular VCF for Full-Length Eurorack Songs

Creating a one-bar beat or catchy melody is easy—but evolving that into a full-length song is a classic challenge in Eurorack. The **Klavis Grainity Granular VCF** offers a toolbox for transforming and evolving sound in ways that go far beyond basic filtering. Here’s how you can use this module, in combination with other modules, to help structure and perform dynamic, evolving full-length pieces.

---

## Granular VCF as an Evolving Voice

**The Key Functionality**:
- Grainity has two parallel analog filters: a standard multimode VCF (M.VCF) and a "granular" VCF (G.VCF) that re-assembles filter settings in musical or random patterns.
- Unique parameters (structure, division, phase/track) enable harmonic, subharmonic, and rhythmic processing.
- A dedicated Mix section enables *morphing* between classic and wildly colored filter outputs.

### **1. Dynamic Song Sections with Granular Structures and CV Automation**

**Eurorack Application**:
- Use *different Structures* (granular loop patterns) as pseudo-“presets” for song sections: verse, chorus, breakdown, etc.
- Sequence or manually morph the Structure and Division via CV (from a sequencer, manual fader, or random LFO).
- This changes the harmonic content, filter behavior, and rhythmic feel, instantly transforming the timbre of a bassline, chord pad, or even a drum loop.

**Tip**: Map *Structure* CVs to song sections in a sequencer (e.g., Hermod, Metropolis, or via voltage presets in a CV matrix).

### **2. Live Performance Mixing Using the Mix Output**

**Technique**:
- The Mix knob and Mix CV input let you smoothly blend between the pure multimode filter and the granular path.
- Use this to create builds, drops, and transitions: e.g. fade in the granular effect for a wild chorus, then back to clean for a verse.

**Automate**: Patch a slow envelope, fader, or LFO to the Mix CV input for hands-free morphing.

### **3. Rhythmic & Harmonic Transformation via Detect Input**

**Eurorack Creativity**:
- Patch a **Clock, Trigger, Sequencer, or alternate VCO** into Detect. This lets you step the granular engine in sync with any rhythmic or melodic element (not just the audio input's zero crossings).
- For song breakdowns, use a gate pattern or Euclidean rhythm to create stepped, glitchy, or gated transitions, syncopated with your main clock.

**Advanced**: Change Detect source per section for radically different “grooves” within one voice.

### **4. Animated Filter Modulation for Movement Over Time**

- Use slow LFOs, envelopes, or sample-and-hold CVs on **Φ/Frq, Structure, and Mix**.
- For a sense of narrative or growth, automate resonance (Q), cutoff, and structure over long time spans.
- “Unison” and “Phasing” effects (via phase CV) add evolving stereo or mono textures—useful for intros, outros, and ambient breakdowns.

### **5. Evolving Polyphony and Layers**

**Techniques**:
- Use chords, stacked VCOs, or mix multiple sources as input, with one VCO's simpler wave on Detect for anchored, yet evolving filter patterns.
- The Grainity responds interactively to complex input: you can create refrains, bridges, and unique sonic “motifs” by feeding in different polyphonic or noise sources per song section.

### **6. Process Full Mixes or Drums for Song-Level “Events”**

- Run drum loops, percussion, or even a full stem or mix bus through Grainity.
- Use the Structure, Division, and Detect tricks above to create *filter sweeps*, *break-downs*, *build-ups*, or spectral “scene changes” reminiscent of DJ-style transitions.
- Automated level (via VCA) plus evolving Grainity settings: classic build/break structure without “preset recall”.

---

## **Classic Song Structure Routines**

Below are some **practical routings** using Grainity for structuring songs:

### **A. “Verse/Chorus” Mode Switching via CV Presets**
- Multitrack the Structure, Division, Phase/Track, Mix, and filter type CVs with a sequencer, switching them for each song section.
- For verses, use subtle grains and low division. For choruses, engage more radical structures, higher division, and more granular content.

### **B. Evolving Intros and Ambient Transitions**
- Start with strong M.VCF signal (“clean” mix).
- Slowly crossfade to more granular, harmonically rich textures via Mix knob or CV.
- Animate phase and structure for a slow “emergence” effect.
- Reverse at the end of the song for gentle fade-outs.

### **C. Breakdown/Drop via Random Structure Mode**
- Engage the random Structure family ([r] structures) for unpredictable “chaos” during a breakdown.
- Sync division to the tempo for rhythmic coherence.
- Return to “groovier” structure on the drop.

### **D. Layered Effects Rack**
- Parallel the Grainity outputs: route M.VCF and G.VCF through further FX (delays, stereoization, compressor) as two distinct voices.
- Crossfade or switch between them in your “arrangement”.

---

## **Module Pairing Suggestions**

- **Sequencers**: To automate structure, phase, Mix, Division and even input switching (e.g., Make Noise René, Five12 Vector).
- **CV Recorders/Presets**: For quick changes at defined song parts (e.g., Malekko Voltage Block, Expert Sleepers FH-2).
- **Random/LFOs**: For ever-changing ambient patches (e.g., Mutable Instruments Tides/Marbles).
- **VCA Mixers**: To fade/morph between filtered signals in performance (Intellijel Quad VCA).
- **Stereo Modules**: To exploit stereo trickery with M.VCF and G.VCF as left/right for “widener” effects.

---

## **Summary Table: Song Structuring with Grainity**

| Song Section   | Structure Tip                   | Detect Tip          | Mix Tip                       |
|----------------|---------------------------------|---------------------|-------------------------------|
| Intro/Ambient  | Long structures, lower division | Slow LFO or manual  | Granular path, modulate phase |
| Verse          | Subtle structure, low division  | Tied to main melody | Clean (M.VCF)                 |
| Chorus         | Wild structure, higher division | Clock or gate seq   | Crossfade to G.VCF            |
| Breakdown      | Random structure, high division | External triggers   | Heavy granular, lots of FM    |
| Bridge         | Modulated phase, subtle changes | Change Detect VCO   | Morph between paths           |
| Outro/Fade     | Fade division to minimum, mix to M.VCF | Fade Detect | Slow fade out Mix             |

---

By liberally automating and performing with the **Structure**, **Division**, **Detect**, **Mix**, and filter parameters, you can turn a simple loop into a living, evolving full-length song, all “in the rack.”

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)