# 2hp — Arp

- [Manual PDF](../../manuals/2hp_Arp_Manual_2023.pdf)

---

[2hp Arp Manual (PDF)](https://2hp.com/wp-content/uploads/2022/02/Arp_Manual.pdf)

---

# Using the 2hp Arp for Full-Length Eurorack Songs

**The 2hp Arp** is a compact, gate-driven arpeggiator that unlocks complex melodic possibilities within a minimal HP footprint. It generates musically useful arpeggios based on user-selected chords, playback mode, and root note, and it can be advanced or reset via external triggers. While arpeggiators are often used as “set and forget” modules for quick melodic interest, the 2hp Arp’s flexibility can make it a vital tool for songcraft and live performance, especially when composed within the broader eurorack ecosystem.

Below, I’ll break down strategies for turning this module into a centerpiece for *full-length songs*, offering composition techniques, patching ideas, and integrations with other modules.

---

## 1. **Scene and Section Transitions**
### **Arp Mode and Chord Automation**
Most songs comprise multiple sections (verse, chorus, bridge, etc.). With the 2hp Arp:
- **Automate the Chord & Mode** using CV from a sequencer or automation source (e.g., Pam’s New Workout, Voltage Block, or Ornament & Crime).
- **Set up scene changes** by altering Arp modes (ascending, descending, pendulum, random) between sections for contrast.
- **Fade or switch chords** for new moods and harmonies—possible even with basic CV automation.

#### **Patch Example:**
- *Sequencer 1* sends triggers/gates to the *Trig Input* to advance the arpeggio in time with your song.
- *Sequencer 2* (or LFO/Envelope) modulates the *Chord CV Input* to select different chords at key song moments.
- Use a clock divider/multiplier (e.g. 4MS Rotating Clock Divider) to change Arp timing for transitions and fills.

---

## 2. **Dynamic Melodic Content**
### **Programmatic Variation**
- Use the *Mode* input (CV or manual) to switch between predictable (ascending/descending) and more improvisational (random/pendulum) modes.
- Introduce *Root CV* automation for key changes or melodic “jumps”—transposing the entire arpeggio by musical intervals for choruses or breakdowns.

#### **Patch Example:**
- Route an LFO to gradually sweep the *Root Knob* CV during a breakdown, giving a sense of modulation without much manual intervention.
- Use manual switches or performance controllers (e.g. FSR, ADDAC Manual Gates, Intellijel Tetrapad) to “play” chords and arpeggio modes live.

---

## 3. **Rhythm and Arrangement**
### **Gate-Driven Choreography**
- The module advances with *external gate/trig signals*—use opportunity for “rhythmic gating” where different sections of your song fire more complex or sparser arpeggio patterns.
- Use clocked logic modules (e.g., Mutable Instruments Branches, Doepfer A-150 series) to generate varied gating rhythms for arpeggio advancement and resetting.

#### **Patch Example:**
- During a verse, fire regular 16th-note triggers to *Trig* for steady arps.
- In a chorus, combine clock and gate signals to create syncopated, lively arpeggiator movement.
- Tie *Reset Input* to the downbeat or a fill to ensure the arpeggio re-aligns to your song’s rhythmic cycle.

---

## 4. **Modular Song Dynamics: Layering and Substitution**
### **Integrated Song Structures**
- Pair 2hp Arp with quantizers, sample & holds, and sequential switches for generative parts that can be muted, swapped, or transitioned for longer songs.
- Route its V/Oct output to different sound sources on various song sections (e.g., bass voice in verse, lead in chorus) using switches.

#### **Patch Example:**
- Use a sequential switch (e.g. Doepfer A-151) to send Arp’s V/Oct output to different oscillators or synthesizer voices, creating timbral change across song sections.
- Layer the arpeggiated melody on top of a static pad or chord progression for harmonic richness.

---

## 5. **Performance and Live Song Progression**
- Use manual controls live for on-the-fly chord and mode changes.
- Exploit the *output’s 0V-5V range* to interface cleanly with most 1V/oct synth voices.
- Use the module’s compact size as a “performance lead” center without sacrificing precious rack space.

---

## 6. **Additional Songcraft Tools to Pair**
- **Sequencers (e.g., Metropolis, Eloquencer):** Control trigger inputs, chord/mode CV.
- **Logic/Random Modules:** Vary trigger sources for non-repetitive arps.
- **Quantizer (e.g., Tiptop Quantizer):** Add more scales/modes for melodic variation.
- **Switches/Matrix Mixers:** Route melodies to different voices for evolving arrangements.
- **Effects (Delays, Reverbs, Phasers):** Expand arpeggio parts for breakdowns or ambient sections.

---

**Workflow Example:**

1. **Intro:** Sparse triggers, slow clock to Arp, random mode for ambient shimmer.
2. **Verse:** Up the gate rate, use ascending arp, major chord, automate root CV for melodic progression.
3. **Chorus:** Fast, pendulum or 2-octave mode; chord and root CV inputs sequenced for a lift in energy.
4. **Bridge:** Reset input fires at specific measures to bring the arp back "home," adding a sense of return.
5. **Outro:** Diminish gate activity, slow automation, return to random/blinking chord for a dissolve.

---

### **Conclusion**

The 2hp Arp, when integrated with appropriate Eurorack companions, becomes more than a background tool—it enables structured melodies, harmonic progression, live improvisation, and dynamic arrangements. By sequencing its chords, roots, and modes, and creatively advancing or resetting its arpeggio, you can build evolving pieces that avoid the pitfalls of static modular jams. Treat it as another instrument in your ensemble, capable of both lead and supportive roles throughout your song.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)