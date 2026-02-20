# Noise Engineering — Integra Funkitus

- [Manual PDF](../../manuals/Integra Funkitus - Noise Engineering Documentation.pdf)

---

[Integra Funkitus Manual PDF](https://manuals.noiseengineering.us/if/)

---

# How to Use Integra Funkitus to Create Full-Length Songs in Eurorack

## Overview

Many modular musicians struggle to transition from strong loops or beats into **full-length, evolving compositions**. The [Noise Engineering Integra Funkitus](https://manuals.noiseengineering.us/if/) offers robust tools for rhythmic variation, generative evolution, and macro-level song structuring, making it an excellent centerpiece for turning patterns into engaging, complete tracks.

Below, you'll find strategies for using Integra Funkitus to unlock song-level structure, combined with common Eurorack modules.

---

## What Does Integra Funkitus Do?

Integra Funkitus takes **up to four gate rhythms** (from sequencers or clocks), and—via different modes and probability/logic controls—outputs related, processed rhythms. This allows on-the-fly **variation, mutation, and combinatorial remixing** of your core rhythms.

### Main Modes:
- **Trigger Mode:** Knobs set the probability an input gate will pass through (variation per trigger).
- **Gate Mode:** Probability applied to both rising and falling edges (hold/sustain unpredictably).
- **Logic Mode:** Knobs sweep between which input channels are summed into which outputs. Full CCW = single channel, full CW = mute, middle = unique logic combinations.

---

## Strategies for Full-Length Songs

### **1. Macro-Structure via Probability and Muting**

- **Use External Modulation:** Patch slow LFOs, sequencers, or automation (via MIDI-to-CV, or complex envelope generators) into the `Rhythm Modification` CV inputs. This will make the rhythm modification knobs evolve over time—so that the density/complexity of your rhythm parts change for verses, choruses, breakdowns, etc.
    - *Example:* Fade up the probability on hi-hats or snare triggers over 16 bars, emulating drum fills, intensification, or breakdowns.

- **Automated Muting:** Logic mode allows for permanent or momentary channel mutes via knob or CV—ideal for dropping kicks, hats, or entire voices out for classic "breakdown sections" or "drops."

---

### **2. Generative Song Evolution**

- **Logic Mode for Dramatic Variations:** Move smoothly from simple triggers (one-to-one) to complex rhythm combinations (all-to-all) as a song progresses, so the groove morphs but remains related to the source patterns. 
    - *Example:* Start with just the original rhythm for the intro, blend in additional parts as the song reaches the chorus, drop to minimal for the bridge.
- **Burn Function:** Use Burn as a one-shot or occasional fill—trigger manually or with a performance controller at dramatic section changes (e.g., "fill into chorus takeover").

---

### **3. Intermodulation With Other Modules**

- **Source Material:** Feed Integra Funkitus from different sequencer rows (e.g., Numeric Repetitor, Zularic Repetitor, Pamela’s New Workout), LFOs, or even random gate sources (Wogglebug, Turing Machine, Temps Utile).

- **Target Voices:** Send modulated gate outputs to drum modules (TipTop, ALM, Erica Pico Drums), envelope triggers for melodic voices, or even modulation destinations (e.g., envelope for filter cutoff).

- **Song Section Switching:** Use a sequential switch (e.g., Doepfer A-151, Erica Sequential Switch) to reroute CV modulation or input sources, automating or performing macrostructural changes.

---

### **4. Manual or Sequenced Tweaks (Performance/DAW Control)**

- **Knob Performance:** Ride the modification knobs live during performance, or sequence them via CV from a DAW or hardware sequencer (e.g., Hermod, NerdSeq, Voltage Block), automating changes for each song section.
- **Random/Procedural Music:** Send stepped random CV (Turing Machine, Wogglebug, Marbles) to modification CV ins for ever-evolving, non-repetitive grooves that remain musically relevant to your core beats.

---

## Patch Example: Simple Song Structure with Integra Funkitus

1. **Inputs**: Four sequencer rows (kick, snare, hi-hat, percussion).
2. **IF Outputs**: To drum voices.
3. **CV Modulation**: Slow LFO (for fade-in/fade-out of percussive elements on certain song sections).
4. **Logic Mode**: Use for the bridge so rhythm parts combine uniquely (dense and unexpected).
5. **Burn Button**: Hit before chorus or drop for a temporary fill.

By crossfading probability and logic settings, and modulating outputs to mute/activate different parts, you create **progression, breakdowns, drops, and build-ups**—all the needed macro structures for full song forms.

---

## Conclusion

**Integra Funkitus** is not just a "variation generator"—with thoughtful patching, performance, and modulation, it becomes a **powerful tool for dynamic, evolving song structure** within your Eurorack system.

---

**Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)**

---