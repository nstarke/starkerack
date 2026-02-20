# Abstract Data — ADE-33 Event Boss

- [Manual PDF](../../manuals/ADE33_Manual_v1_0.pdf)

---

[**Abstract Data ADE-33 Event Boss User Guide (PDF)**](https://www.abstractdata.biz/files/Event_Boss_v1.0.1.pdf)

---

# Using the ADE-33 Event Boss to Create Full-Length Eurorack Songs

## Introduction

The Abstract Data **ADE-33 Event Boss** is a sophisticated rhythm and pattern creation/manipulation module for Eurorack modular synthesizers. Its 6 Global Modes and 36 total algorithmic variations make it a powerful tool for moving beyond simple patterns toward dynamic, evolving, and structured full-length compositions.

This guide analyzes the Event Boss in the context of modular songcraft. It provides practical workflows and patching strategies—especially for those who struggle to move from tasty loops to real, evolving songs.

---

## Core Functions in the Songwriting Context

### Traditional Weakness: Going Beyond the Loop

Eurorack's strengths often breed its central challenge: amazing, groovy loops that seem to resist evolving into full songs. The key to "songification" is **macro-level control** over:

- Patterns: Variability, fills, and breakages
- Transitions: Introductions, breakdowns, buildups, drops, etc.
- Arrangement: Evolving energy, structure, and form

The ADE-33 can underpin all of the above.

---

## Using the ADE-33 as a Song Structure Machine

### 1. **Build the Foundation: Clock/Pattern Manipulation**

- **Primary Beat Source:** Feed a steady clock or simple trigger pattern (from Pamela’s New Workout, Tempi, etc.) into GATE A1 or A2.
- **Pattern Evolution:** Use Variables (Global Mode 1) to create evolving rhythmic variations or Probability (Global Mode 3) for chance-based fills.
- **Arrangement Macro-control:** Modulate local mode or CV with longer envelopes, manual knobs, sequencers, or automation sources (e.g., voltage block, rotating clock divider).

### 2. **Introduce Song Sections: Dynamic Pattern Shifts**

- **Section Changes:** Use external CV (from a sequencer, MIDI-to-CV module, or manual controller) into IN: MODE SELECT or GATE B/CV to **change modes, patterns, and logic** at predetermined song sections.
- **Example:** At “chorus,” switch from basic clock division to complex probability patterns. For a “breakdown,” dial in logic operations to create sparser or syncopated structures.

### 3. **Create Fills and Breaks: Probability & Multiples**

- **Percent Chance Fills:** Use Probability Mode so certain triggers (i.e., snare drum hits) only happen on a random or CV-determined likelihood.
- **Ratchet or Multiply for Moments of Energy:** During a fill, introduce the Multiples mode with clock multiplication for double-time or burst effects.
- **Evolve Over Time:** Slowly fade a CV that gradually increases gate probability or clock division/multiplication for long, subtle energy builds.

### 4. **Control/Automate Structure: External CV & Sequencers**

- **Song “Chapters”:** Use a slow CV sequence (possibly with a sequencer not used for pitch) to step through Local or Global modes, driving the “chapters” of your song.
- **Footswitches/Manual Buttons:** Patch external triggers or manual gate sources to input(s) to step through arrangement sections on the fly.

### 5. **Arrange Melodies & Basslines: Synchronized Pattern Manipulation**

- **Sync Melodic Change:** Use the **rhythmically processed output** from Event Boss to control sample & holds, quantizers, or melodic sequencer resets, ensuring that bass/melody pattern changes are tightly matched to drum/rhythm changes.
- **Polyrhythms & Cross-Rhythms:** Using logic and multiple gate inputs, create evolving melodic and percussion relations—great for experimental sections or breakdowns.

### 6. **Create Dynamic Intros, Outros, and Transitions**

- **Start with Simplicity:** Begin with the most basic mode—one clock, no CV, pure repetitive pattern.
- **Morph:** Slowly bring in CV modulation, then step through Local/Global modes for gradual, dramatic changes.
- **Silence/Break:** Use Logic or Gates modes to program blank/quiet bars or abrupt stops using Boolean conditions.

---

## **Practical Patch Example: Macro Song Structure**

1. **Set Up Master Clock** — Clock divider/multiplier as master clock into ADE-33 GATE A1.
2. **Kick Pattern** — Output Event Boss to the trigger input of a drum module’s kick. Start in Variables Mode for basic kick pulse.
3. **Fills & Variations** — Every 16 bars, use a CV/gate to change ADE-33 mode to bring in burst, probability, or multiplied rhythms for end-of-section fills.
4. **Section Changes** — Use a sequencer or manual controller to switch ADE-33 Global Modes (e.g., to Logic for breakdown, to Phase for swing/groove in chorus).
5. **Melodic Resets** — Output to a sample & hold module clock input; change the Event Boss rhythm for a fresh melody every section.
6. **Automation** — Use longer envelopes or tracked LFOs to sweep CVs for gradual, evolving variances over the course of the track.

---

## **Combining with Other Modules**

- **Sequencers** (e.g., Metropolis, Hermod): Sequence mode/CV changes for song parts.
- **Voltage Block, Planar2, etc.:** Manual performance/automation of arrangement controls.
- **Logic Modules** (e.g., Mutable Kinks): Further combine Event Boss outputs for complex, reactive arrangements.
- **Samplers/Loopers**: Use ADE-33 outputs to control playback start/stop/loop points.
- **Envelopes, LFOs**: Provide slow modulation to create structure over minutes.

---

## **Inspiration: Macro-level Modular Arrangements**

The real trick is not just making your patches sound good for 16 bars—but manipulating CV and mode inputs on the ADE-33 to orchestrate changes, transitions, surprise moments, breakdowns, and dynamic builds throughout the track.

You’ll be using **pattern mutation, probabilistic triggers, phase and logic hacks, and tightly timed mode switches as your “arranger” and “conductor,” just as you might use the scene or pattern buttons in a DAW.**

---

## **Quick Tips**

- Use **long LFOs, CV recorders, or automation sequencers** as the source for ADE-33’s mode/CV inputs for evolving songs without hands-on intervention.
- Combine multiple ADE-33 outputs for layered sections (e.g., one running kicks, one snare/fill FX).
- **Patch ADE-33 clock outputs into non-percussion modules** (melodic resets, FX triggers) for total song cohesion.

---

### [ADE-33 Event Boss Official Manual PDF](https://www.abstractdata.biz/files/Event_Boss_v1.0.1.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
