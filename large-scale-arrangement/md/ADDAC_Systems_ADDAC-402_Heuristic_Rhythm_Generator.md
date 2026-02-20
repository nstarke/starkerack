# ADDAC Systems — ADDAC-402 Heuristic Rhythm Generator

- [Manual PDF](../../manuals/ADDAC402_UsersGuide_A_0_web_6500.pdf)

---

[ADDAC402 4-Voice Heuristic Rhythm Generator Manual PDF](http://media.addacsystem.com/ADDAC402_USERS_GUIDE.pdf)

---

## Using the ADDAC402 to Create Full-Length Eurorack Songs

### Introduction

The [ADDAC402 4-Voice Heuristic Rhythm Generator](http://addacsystem.com/) is an exceptionally flexible rhythm and trigger/gate source for Eurorack systems. Its core strength is in generating complex, evolving, and varied rhythmic patterns across four independent channels, using multiple algorithms (“heuristics”). While it easily creates intriguing beats, the real power comes from using its features—along with other modules—to move beyond loops and make dynamic, full-length compositions.

Below, you'll find strategies and patch ideas pairing the ADDAC402 with typical Eurorack modules to break out of the “4-bar loop” rut and structure actual songs.

---

## Strategies for Song Arrangement with the ADDAC402

### 1. **Preset Morphing and Scene Changes**

- **How:** The ADDAC402 allows up to 16 presets per some modes (Euclidean, Gate Seq). Changing presets can instantly reconfigure the rhythm for all four voices.
- **Arrangement Use:** Treat presets like "scenes" or "sections" of a song (intro, verse, chorus, bridge).
- **Patch Idea:** Trigger preset changes via CV/gates coming from another sequencer, manual button presses, or a preset CV "manager" module (e.g., macro controllers, Ornaments & Crime, etc.).

### 2. **Algorithm Mode-Switching for Variety**

- **How:** The ADDAC402 has 7 modes (Euclidean, Gate Seq, Game of Life, Golomb, Probabilistic, Footwork, Pong), each with unique logic.
- **Arrangement Use:** Switch between modes mid-performance to warp the rhythmic character across sections, for breakdowns or dramatic shifts.
- **Patch Idea:** Sequence the mode-select CV input (with, say, a sequential switch or voltage block) or switch it manually at section changes.

### 3. **Dynamic Parameter Modulation**

- **How:** All four voices have independent CV inputs for key parameters (“Fills”, occasionally “Steps”).
- **Arrangement Use:** Animate patterns over time via LFOs, envelopes, random voltage (Wogglebug, Marbles, etc.), or automation from DAW hybridizer modules like Expert Sleepers ES-8/9.
- **Patch Idea:** Fade in increasingly complex patterns for a build-up by modulating Fills/Steps with slow envelopes.

### 4. **Inverted Gate Outputs for Polyrhythms & Call-and-Response**

- **How:** Each output has an inverted version—triggers/gates when the main output is off.
- **Arrangement Use:** Use these for call/response effects, ghost notes, accenting alternate events, or to fill in gaps during breakdowns.
- **Patch Idea:** Patch inverted outputs to percussion, bass triggers, or effect switching for evolving interplay.

### 5. **CV-Controlled Skipping & Rotation (“Skip” Buttons) For Variations**

- **How:** Skip steps or rotate patterns via manual buttons, but also by assigning these to the Swing/Assign CV input.
- **Arrangement Use:** Sporadically rotate patterns or skip beats to introduce variation, fills, or breakdowns.
- **Patch Idea:** Use an LFO or sequencer row to automate pattern rotation or “skip” for glitchy fills or drop-outs.

### 6. **Leveraging Probabilistic, Game of Life, Footwork & Pong Modes**

- **How:** These modes generate unpredictability. In probabilistic and GOL modes, outcomes can be random or generative.
- **Arrangement Use:** Drop into these modes for breakdowns, transitions, or mid-song evolution (“live remix” moments).
- **Patch Idea:** Switch to Game of Life and trigger a new state at transition points for spontaneous rhythm changes.

### 7. **Swing/Assign Knob as a Macro Controller**

- **How:** The assignable Swing/Assign knob can control swing, or be reassigned to gate/trig, skip, reset, or even MIDI velocity (with expander).
- **Arrangement Use:** Perform macro gestures—adding swing, muting channels, triggering resets (for drops), or shifting pattern lengths (for fills).
- **Patch Idea:** Performative use in live jams—twist to swing on/off, or cue resets/skips in certain song sections.

---

## How to Integrate With Other Modules for Full Compositions

### **A. Melodic Sequencers and Quantizers**
- Route ADDAC402 gate/trig outputs into melodic sequencers as clocks or resets for changing up melodies with the rhythm pattern.
- Use triggers to advance chord sequencers (e.g., Intellijel Metropolis, Stillson Hammer, O_C).

### **B. Switches, Matrix Mixers, or Sequential Addressers**
- Use switch modules (Doepfer A-150, 4ms Rotating Clock Divider, etc.) to re-route rhythm outputs to different voices/effects during the track.

### **C. Logic and Randomization Modules**
- Patch multiple ADDAC402 outs to logic modules (Intellijel Plog, Mutable Kinks, etc.) to create composite patterns, fills, or conditional events.
- Use sample-and-hold or random modules to modulate ADDAC402 parameters dynamically.

### **D. Performance Controllers**
- Integrate with hands-on controller modules or MIDI-to-CV for real-time punches, mutes, or changes (Make Noise Pressure Points, Intellijel Tetrapad).

### **E. Scene Automation with Hybrid DAW**
- Use MIDI Bridge mode (with expander) or clock/reset inputs to sync ADDAC402 pattern changes to a DAW or external sequencer, automating song sections.

### **F. Combined with Effects and VCAs**
- Route gates to open/close VCAs or activate effects chains (delays, distortion, reverb) on certain hits or song sections.

---

## Example Patch Recipe for Full Song

1. **Basic Beat**: Start in Euclidean mode with simple fills.
2. **Verse Variation**: Use preset recall or rotate patterns forward on each 8 bars for evolving rhythms.
3. **Build-Up**: Increase 'Fills' parameter with slow CV, gradually thickening the rhythm.
4. **Chorus**: Change to Gate Sequencer mode, recall a denser preset, open additional channels.
5. **Bridge/Breakdown**: Switch to Game of Life or Probabilistic mode for controlled chaos.
6. **Finale**: Assign Swing/Assign knob to reset, and manually trigger resets for energetic “drops.”
7. **Extras**: Use inverted outputs to add ghost percussion throughout the song.

---

## Conclusion

The ADDAC402’s combination of preset management, algorithm variety, assignable macro control, generative modes, and extensive CV/gate connectivity makes it a powerful "song brain" for modular music. Leverage its features in combination, pair with other sequencing/melodic/logic modules, and use manual and automated control of parameters to ensure your modular pieces move dynamically from section to section—keeping listeners engaged from start to finish!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)