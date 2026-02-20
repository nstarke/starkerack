# Shakmat — Time Wizard

- [Manual PDF](../../manuals/TW-User_Manual.pdf)

---

[**Shakmat Time Wizard Manual PDF**](https://shakmat.com/manuals/Shakmat_Time_Wizard_Manual.pdf)

---

## Using the Shakmat Time Wizard to Structure Full Length Songs in Eurorack

The Shakmat Time Wizard is far more than just a clock divider—it’s a powerful “song structure” tool for your eurorack system. When working in modular, building song-like progression and structure can be difficult due to the typical lack of “arranger” tools. The Time Wizard helps break free from repetitive loops by giving you complex, controllable timing and clocking possibilities.

Below, I’ll outline how you can use the Time Wizard—especially when combined with sequencers, switch modules, and modulation sources—to create tracks with true narrative and evolution.

---

### Key Features Useful for Song Structure

1. **Multiple Dividers:** 6 independent clock dividers, each with a selectable division factor.
2. **Multiple Routing Variations:** 4 switches provide 81 routing/logic variations.
3. **Clock/Reset Input Flexibility:** Can reset all dividers or act as a second clock for complex polyrhythms.
4. **Logic Functions:** Basic logic operations between clocks for layered triggers.
5. **Trigger/Gate Mode:** Jumpers for gates or triggers on outputs 5 & 6.

---

## Approaches to Song Structure

### A. **Section Switching (Verse/Chorus/Breaks) with Advanced Clocking**

- **Concept:** Use divided/multiplied clock outputs to drive different sequencers, generating different song sections.
- **Method:**  
  - Patch main clock to Time Wizard’s CLK IN.
  - Set A1 to a fast division (e.g., 4) for verse.  
  - Set B3 to a slower one (e.g., 16) for chorus.
  - Use a sequencer for each section, clocked by A1 & B3 respectively.
  - Route outputs to a switch module (e.g., Doepfer A-150) to choose which section is active.
  - Manually flip the switch or automate it via a voltage from a modulation source (envelope/LFO).

### B. **Song Length & Section Transitions with Gated Events**

- **Concept:** Use B6 divider’s reset or logic output to trigger transitions.
- **Method:**  
  - Set B6 to a division that matches your desired full-length phrase (e.g., 64 for 16-bar pattern).
  - Use the RESET B6 switch to automatically reset sequencers, start new melodies or patterns, or trigger global events (like scene changes).
  - Send B6 gate/trigger to a quantizer or sequential switch that advances song sections.

### C. **Subtle Progressions with Polyrhythms & Clock Multiplication**

- **Concept:** Employ the Multiply A and Clock B switches to phase patterns against each other, creating evolving textures and groove changes.
- **Method:**  
  - Use Multiply A to generate triplets or other non-standard divisions.
  - Assign one divider to a drum sequencer and another to a melodic sequencer.
  - Over minutes, these clocks will “drift” relative to one another, naturally evolving the pattern and keeping the listener engaged.

### D. **Automated Fills and Breaks**

- **Concept:** Use gate outputs (especially with the half-period gate jumper) to trigger extra sounds or modulation changes on phrase boundaries.
- **Method:**  
  - Set up a drum module to play a fill every time divider B5 or B6 outputs a trigger/gate (e.g., every 8 or 16 bars).
  - Use these gates to open up effects sends (reverb/delay modules), or crossfade in additional layers or timbral changes.

### E. **Dynamic Resetting and Chain-Sequencing**

- **Concept:** Use the module's robust reset capabilities to synchronize disparate modules or forcibly reshuffle running sequences, breaking cycling patterns and generating progression.
- **Method:**  
  - Use the RESET/IN B input as a manual or automated reset point for multiple sequencers or clock-modulated parameters.
  - Chaining Time Wizard with other dividers (or something like Pamela’s New Workout) builds more complex but controlled probability-based evolutions.

---

## Practical Patch Example

1. **Main Clock Source:** Pamela’s New Workout or simple clock (e.g., 120 BPM)
2. **Time Wizard:**
    - Feed clock to `CLK IN`.
    - Configure dividers:  
        - A1 = 4 (trigger step sequencer for verse)  
        - A2 = 8 (for melody pattern)  
        - B3 = 16 (trigger chorus section or drum fill)
    - Use A2 or B3 to reset or phase-shift a melodic sequencer for evolving melodies.
    - Send B6 out to a sequential switch for smooth song section progression.

---

## Creative Combinations

- **Logic & Probability:** Patch logic-enabled outputs to trigger randomizers, quantizers, or switches for generative passages.
- **Preset Save/Recall:** Combine with modules able to recall patterns (e.g., Mutable Instruments Marbles or Expert Sleepers Disting) for easy song re-composition.
- **Hands-On Performance:** Manually switch routing with the Time Wizard’s switches while performing, re-routing clocks mid-song for dynamic changes.

---

### Why the Time Wizard Excels at Song Creation

- **Break the Loop Cycle:** Make each pass through the pattern unique with resets, multiplications, and manual intervention.
- **Automate Structure:** Use divider logic and outputs to automate when phrases, fills, or changes occur.
- **Embrace Polyrhythm:** Weird/complex ratios help music breathe and avoid “machine gun” repetition.
- **Flexible Integration:** Pairs with any clocked sequencer, switch, or logic module.

---

**For the full feature list, routing diagrams, and technical details, consult the original [Shakmat Time Wizard Manual (PDF)](https://shakmat.com/manuals/Shakmat_Time_Wizard_Manual.pdf).**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)