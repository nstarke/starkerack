# 2hp — Grain

- [Manual PDF](../../manuals/2hp_Grain_Manual.pdf)

---

[2hp Grain Manual PDF](https://2hp.com/docs/grain.pdf)

---

# Using the 2hp Grain Module for Full Length Eurorack Songs

## Introduction

The **2hp Grain** is a powerful yet compact granular audio processor capable of transforming any sound source with real-time micro-slicing, pitch shifting, and wet/dry blending. Many modular musicians find themselves stuck with great patterns but struggle to arrange them into full-length, evolving tracks. Below are strategies and patch ideas to integrate Grain into extended song structures, ensuring dynamic progression and engaging compositions.

---

## Key Functions for Song Composition

### 1. **Granular Texture Shifts for Transitions**
- **Use Case:** Employ Grain to transform a loop, vocal, or ambient background during song transitions (intros, breakdowns, outros).
- **How:** Automate the **Mix CV** and **Density CV** from a sequencer or manually modulated LFO/envelope. During a breakdown, fade towards fully granular, increasing density for a swelling, cloudy effect. Return towards dry/clear for drops or verses.

### 2. **Granular Percussion for Variation**
- **Use Case:** Process drum loops or hits to generate glitched or stuttering fills.
- **How:** Patch percussion audio to **IN**, then modulate **Density** (for stutters) and **Freq** (for tuned hits or pitch jumps). Sequencers or random CV sources like Turing Machine can introduce rhythmic changes.

### 3. **Melodic Granular Sequences**
- **Use Case:** Sequence melodic grains for leads, risers, or arpeggios.
- **How:** Send sampled vocals, pads, or synths into **IN**. Use a pitch CV sequencer on **V/Oct** to play melodic lines with grains. Morph between dry and wet using the **Mix** knob or CV.

### 4. **Granular Pads and Bed Textures**
- **Use Case:** Support sections of your song with evolving backgrounds.
- **How:** Feed in a chord, field recording, or rhythmic loop; set **Density** for slow-moving grains, **Mix** for blend, **Freq** for lush pitch shifting. Modulate these parameters slowly over song sections.

### 5. **Live Performance and Improvisation**
- **Use Case:** Manipulate a part in real time for live jams or recording new sections.
- **How:** Use tactile controls (knobs) with external modulation (LFOs/Envelopes) routed to CV ins. Freeze or release grains, sweep pitch, or crossfade granular content for dynamic interaction.

---

## Practical Patch Examples

### **Patch 1: Dynamic Song Intros and Outros**
1. Route a synth or vocal line to **IN**.
2. Start with **Mix** fully left (dry), **Density** centered (no grain).
3. Gradually turn **Mix** right and increase **Density** to flood the mix with grains, introducing texture as an ambient intro.
4. At song start, fade **Mix** left to return to the clear signal.

### **Patch 2: Creating Song Progression**
1. Feed a rhythmic stem or sample into **IN**.
2. Use a stepped random voltage source or sequenced CV to modulate **Density** over 8-16 bar cycles.
3. Increase **Freq** to lift grains in pitch during pre-chorus/build-ups, extending the energy.

### **Patch 3: Granular Breakdowns**
1. During a song’s breakdown, automate the **Mix** knob/CV and **Density** to generate a cloud of the original riff or beat.
2. Slowly decrease **Density** and return **Mix** to dry as you rebuild into the next section.

---

## **Tips for Full Song Structure with Grain**

- **Scene Automation:** Use external sequencers, scenes, or trigger-based modulation to change Grain’s controls at specific song points.
- **Multi-Voice Layering:** Chain Grain with delays, reverbs, or effects send/return for spatial depth during extended breakdowns or ambient sections.
- **Evolving Modulation Sources:** Pair with modulation modules (e.g., LFOs, function generators) programmed to change over long cycles for evolving textures.
- **Granular Basslines:** Layer in a sub-oscillator or direct bass for a hybrid core, letting Grain manipulate melodic or harmonic elements for motion above a solid foundation.
- **Record, Rearrange, and Re-Process:** Use a looper module to capture Grain’s output, then slice and re-introduce it as new material later in the song.

---

By unlocking these approaches, the **2hp Grain** becomes a compositional tool for arrangements well beyond static loops, lending a dynamic, morphable texture to your modular songs.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)