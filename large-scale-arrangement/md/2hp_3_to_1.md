# 2hp — 3 to 1

- [Manual PDF](../../manuals/3_To_1_Manual.pdf)

---

[Download the official 2hp 3:1 Manual (PDF)](https://2hp.com/docs/3to1_manual.pdf)

---

# Using the 2hp 3:1 to Build Full Songs in Eurorack

The **2hp 3:1** is a compact yet powerful voltage-controlled gate switch and summer. Its ability to route, combine, and algorithmically select gates/clocks makes it an excellent tool for transforming looped ideas into dynamic, evolving full-length tracks. Here’s how you can leverage its features for full song creation in a modular setup:

---

## Core Functionalities Recap

- **Voltage-controlled selection** of one input (out of three) to a single output
- **Gate summing** (merge multiple active gates to create polyrhythms or composite triggers)
- **CV controllable** switching for automating transitions
- **Gate to trigger conversion** in summing mode for regularized, precisely-timed events

---

## Techniques for Arranging Full Tracks

### 1. Scene Switching and Section Changes

**Use Case:** Automate introduction, breakdowns, drops, etc.

**How:**  
Patch three different rhythms (kick, snare, or clock patterns) into the three inputs. Use a sequencer, LFO, or an automation lane (SEL CV) to dynamically select between these inputs at different points in your track. By automating the SEL, the 3:1 will route only the desired rhythmic element, muting or unmuting sections.

**Module Interactions:**  
- **Sequencers (e.g. Pam’s New Workout, Hermod):** Generate CV to select scenes.
- **Clock Dividers/Logic Modules:** Change which gate is fed into each input for more complex transitions.

---

### 2. Polyrhythm Generation for Song Development

**Use Case:** Build complexity over time (e.g. intro = simple, mid-section = polyrhythms)

**How:**  
Set 3:1 to SUM mode. Input three different rhythmic sources—perhaps one is a master clock, one a divided clock, and one a Euclidean trigger. The output sums concurrent inputs, creating new, evolving trigger streams (polyrhythms) that can fire off envelopes, percussion, or melodic events only later in the track.

**Module Interactions:**  
- **Euclidean Rhythms/Grids:** Patch varied rhythms into inputs.
- **Gate/Trigger-Driven effects:** Output goes to percussive modules or modulation triggers.

---

### 3. Arranging Drum Patterns and Song Sections

**Use Case:** Switch drum/perc patterns for verse/chorus structure.

**How:**  
Feed different drum gate patterns (or clocked LFOs for movement/modulation) into inputs. Use SEL knob and/or SEL CV to “flip” between verses, choruses, fills, and drops live or via automation.

**Module Interactions:**  
- **Drum Modules (e.g., Mutable Peaks, Erica Pico Drums):** Receive pattern changes.
- **CV Recorders:** Capture and automate movement for playback.

---

### 4. Live Performance Transitions

**Use Case:** Perform sections or sudden parameter changes hands-on or automated.

**How:**  
Using the SEL knob or an external controller (joystick/CV keyboard), manually transition between input sources for expressive, performative control over structure and energy.

**Module Interactions:**  
- **Manual CV Generators (e.g., FSR, touch plates):** Control selection in real-time.
- **Switching FX sends or modulation sources for different song movements.**

---

### 5. Thematic or Tonal Variation

**Use Case:** Change melodic/harmonic patterns without repatching.

**How:**  
Send different quantized gate/trigger sequences that transpose, modulate, or open up new musical material at the output, routed to pitch sequencers or harmonic triggers.

**Module Interactions:**  
- **Quantizers/Sequential Switches:** Use output to advance or change pitch values.
- **Arpeggiators:** Change the clocking pattern for new phrases.

---

## Patch Example for Song Structuring

1. **IN 1:** Kick pattern (straight 4/4)  
2. **IN 2:** Fill pattern or alternate rhythm  
3. **IN 3:** Hi-hat pattern or breakdown clock  
4. **OUT:** Send to a drum module(s) or mix of voices  
5. **SEL CV:** Automated by your sequencer/automation lane to change song sections

This setup enables:

- **Intro:** Manual selection of IN 1 (just kick)
- **Buildup:** Gradually blend to IN 2 with a ramped CV
- **Chorus/Drop:** SUM mode, engage multiple patterns for high energy
- **Breakdown:** Flip back to IN 3 for sparse rhythm

---

## General Tips

- Automate **SEL CV** for precision, or control it by hand for performance jams.
- Use external logic or clock modules upstream to sculpt more complex arrangement triggers.
- Feed **polyrhythmic outputs** into not just percussion but also to clock S&H, change effects parameters, or drive melody sequencers for total song evolution.

---

> The **2hp 3:1** is far more than just a switch—it’s a powerful arrangement and performance tool in a compact case, enabling morphing, evolving, and controlled transitions that turn patterns into complete, narrative-driven modular songs.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
