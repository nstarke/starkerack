# Pittsburgh Modular — Gamesystem

- [Manual PDF](../../manuals/game_system_manual.pdf)

---

[Download the Pittsburgh Modular Game System Manual (PDF)](https://pittsburghmodular.com/assets/game_system_manual.pdf)

---

# Using Pittsburgh Modular Game System for Full-Length Eurorack Songs

The Game System is a powerful Swiss Army knife of sequencing and rhythm generation, offering multiple distinct modes to control pitch, rhythm, gates, and voltage in unpredictable or tightly structured ways. One common challenge in modular music is getting from a looping "groove" (beat, melody, bass) to an evolving, narrative full-length song. Below are strategies to use Game System for song creation, with practical integration tips for other eurorack modules.

---

## Core Strategies for Full Song Composition

### 1. **Song Sections and Scene Chaining**

- **Multiple Sequencers:** Each "game" provides a radically different approach. You can use each one for a different song section (e.g., Meteor Shower for intros/outros, Music or Euclidean for verses/choruses). 
- **Manual or CV Section Changes:** Use the CV/Gate MODE input or an external switch/sequencer (like Mutable Instruments Frames, Sequential Switches, or S&H modules) to swap modes in real time, structuring your song.
- **Settings Recall:** Use the joystick/button for hands-on "live" structural changes, or automate via external triggers.

### 2. **Dynamic Rhythms and Evolving Patterns**

- **Euclidean Rhythms:** Slowly modulate the number of beats or sequence length over time with LFOs, random voltages, or envelopes. This creates ever-evolving rhythms perfect for builds, breakdowns, or shifting grooves.
- **Probability Machine:** Route CV from LFOs, random sources, or performance gestures into the joystick controls to transition from sparse to dense rhythms, easily morphing between minimal and maximal activity—great for tension and release.

### 3. **Melodic and Harmonic Evolution**

- **Music Sequencer as Melodic Brain:** Use 32 steps and random direction for non-repeating patterns. Change direction, length, or individual voltages on-the-fly (via CV and external triggers) for melodic development.
- **Meteor Shower for Generative Melodies:** Its random CV output on collision can drive lead/bass lines. Sequence the maximum meteor count (with button/CV) to control density/evolution.
- **Transpose and Modulate:** Use external quantizers or precision adders to create key changes or melodic shifts per section.

### 4. **Polyrhythms, Cross-Rhythms and Clocking**

- **Time Traveller as Song Clock Brain:** Use its four independent clocked outputs for different rhythmic layers. Adjust divisors and offsets throughout the song. Activate "roaming" outputs for more chaos during climatic moments.
- **Drum Sequencer for Sectional Changes:** Switch between patterns (and last steps) to mutate rhythm sections as the song progresses.

### 5. **Live Performance and Resampling**

- **Joystick as Expressive Control:** Assign gestures or button presses to key song transitions—filters open, sequences reset, or patterns invert. External gate/CV from foot pedals, gesture sensors, or other performance modules expands possibilities.
- **External Processing and Resampling:** Record Game System sequences into loopers/samplers during performance, then re-sequence or mangle them for breakdowns, drops or new sections.

### 6. **Song Structure with External Module Integration**

- **Switching Games in Set Order:** Use a sequential switch or voltage-addressed router (such as Doepfer A-150, Intellijel Planar, or WMD Sequential Switch Matrix) to step through "games" or banked presets live.
- **Master Clock Control:** Sync Game System clock with external master clock (Pamela's New Workout, Tempi, etc.) for tight integration with all modular elements.
- **State Automation:** Save voltage-based "scenes" in matrix mixers or sequencer memories, then trigger them with gates/scenes throughout your song for macro-level shifts.

---

## Example Song Structure Using Game System

- **Intro:** Start with Meteor Shower, few meteors, sparse explosions gating a reverb-heavy pad, random CV droning a VCO.
- **Verse:** Switch to Music Sequencer, 12-step pattern, moderate tempo, gates trigger VCA/EGs for regular melodic phrases and simple drums.
- **Chorus:** Engage Drum Sequencer, invert/increase last step for energy, add Euclidean for polyrhythmic gating of percussion.
- **Breakdown:** Move to Probability Machine, high complexity, evolving chaos, random voltages controlling effects, minimal melodic content.
- **Build:** Euclidean gradually grows steps/beats, more density, filter sweeps via external automation, Time Traveller re-syncs clock pulses for staggered returns.
- **Climax/Outro:** Return to Meteor Shower or chaotic Time Traveller/Probability state for maximum density, then dial it down or reset for ending.

---

## Key Tips

- **Voltage Automate Everything:** The Game System comes alive when joystick and buttons are controlled by CV/gates. Sequence these changes just as you would note or drum triggers.
- **Stack Modes:** Use different games for melody, rhythm, modulation, and clocking in parallel, leveraging the four outputs creatively with mults or logic modules.
- **Continuously Morph Patterns:** Evolve both macro (sectional) and micro (step, density, complexity) elements for true song progression.
- **External Sequencers/Logic Expand Narrative:** Complement Game System with external sequencers, manual gates, Sample & Hold, or logic modules for scene programming and unpredictable variation.

---

### Further Reading
- [Pittsburgh Modular Game System Manual (PDF)](https://pittsburghmodular.com/assets/game_system_manual.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---