# ADDAC Systems — ADDAC-402 Heuristic Rhythm Generator

- [Manual PDF](../../manuals/ADDAC402_UsersGuide_A_0_web_6500.pdf)

---

[ADDAC402 Heuristic Rhythm Generator User’s Guide (PDF)](http://addacsystem.com/sites/default/files/files/ADDAC402-Manual-V01.pdf)

---

## Creative Patch Ideas for the ADDAC402 Heuristic Rhythm Generator

The ADDAC402 is an extremely versatile rhythm generator, packed with diverse algorithms (Euclidean, Game of Life, Pong, Probabilistic, etc.) and features that make it a powerful hub for generative and algorithmic rhythmic sequencing. Here are some creative ways you can leverage its unique capabilities in a Eurorack setup by pairing it with other modules:

### 1. Rhythmic Modulation of Sound Sources

#### *A. Complex Drum Programming*
- **Patch the ADDAC402’s gate outputs** directly to the trigger inputs of drum modules like **Hexinverter Mutant Drums, ALM Busy Circuits Akemie’s Taiko, or Mutable Instruments Peaks** (in drum mode).
- Use the different modes (e.g., Euclidean for polyrhythms, Pong for unpredictability) to generate complementary or contrasting drum rhythms.
- **Variation:** Send inverted gate outs to additional percussion for “ghost hits” or accents.

#### *B. Synth Voice Triggers*
- Use the outputs to fire envelope generators (e.g., **Intellijel Quadra, Maths, or Make Noise Function**) that control:
    - VCA for percussive synth voices.
    - Filter pings or LPG (Low Pass Gate) modules for organic percussive sounds.

---

### 2. Manipulating Melodic Sequencing

#### *A. Clocking Melodic Sequencers*
- Use the OR-ed (combined) output of multiple ADDAC402 gates or just a single out as a master clock for a melody sequencer (e.g., **Make Noise René, Malekko Voltage Block, or Tiptop Z8000**).
- **Result:** Melodic sequences only step when a particular rhythm pattern is active, creating polymetric melodic movement.

#### *B. Modulating Quantizers or Switches*
- Patch rhythm outputs to the **gate input of a sequential switch (e.g., Doepfer A-151 or Erica Synths Sequential Switch)**, which selects different melodies or CV paths according to your rhythm pattern.
- Use the triggers to fire sample-and-hold modules to create pseudo-random arpeggios tied to the ADDAC402’s evolving rhythms.

---

### 3. Algorithmic Interactions & Complexity

#### *A. Rhythmic Modulation of Effects*
- Use ADDAC402 outputs to rhythmically activate send/return paths or freeze functions on effect modules (e.g., **Make Noise Mimeophon, Mutable Instruments Clouds, or Strymon Magneto**).
- Create live/remixed drum breaks or morphing ambient textures by rhythmically gating effect trails.

#### *B. Cross-Modulation via CV Control*
- Patch CV outs (e.g., Euclidean “fills” input CV) from a random or stepped CV source (like **Mutable Instruments Marbles, Turing Machine, or S&H modules**) to different ADDAC402 inputs, morphing rhythm parameters dynamically.

---

### 4. Generative/Heuristic Compositions

#### *A. Generating Breakbeats & Glitches (Footwork & Probabilistic Modes)*
- In **Footwork mode**, modulate STEPS with an LFO (e.g., Batumi, Zadar) for chaotic, ever-morphing breakbeats.
- **Probabilistic mode**: Use a slow random CV to modulate probability percentage, making different channels more or less likely to trigger—great for “organic” patterns.

#### *B. Evolving Polyrhythms & Polymeters*
- Run several ADDAC402 channels into a quad envelope (e.g., **Intellijel Quadra, Quadrax**) and use each envelope to control different sound-shaping parameters on multiple voices.
- Sync ADDAC402 to external clock sources like Pamela’s New Workout, Tempi, or MIDI clock for integration with DAW or other gear.

---

### 5. Generating Dynamic Modulation Sources

#### *A. Triggering Other Sequencers or Utilities*
- Use the different outputs to:
    - Cycle through presets on other modules or sequencers.
    - Trigger randomizations or “reset” events on modules like Ornament & Crime, or WMD Sequential Switch Matrix.

#### *B. Swing-based Groove Modulation*
- Exploit the **assignable Swing/Assign CV** to rhythmically rotate patterns or parameters elsewhere in your rack. For instance:
    - Patch a rhythmic LFO or Sample & Hold into the Swing/Assign CV input, letting external modulation create subtle groove shifts or pattern rotations.

---

### 6. MIDI Integration

*(With the ADDAC402B Expander)*
- **Sync with DAW/External Gear:** Use the MIDI Bridge mode for clock or transport integration.
- **Hybrid Setups:** Have ADDAC402 rhythms drive Eurorack drums while MIDI sequences from Ableton Live or hardware sequencers (like Elektron Digitakt) play pitched parts.

---

### Recommended Generic Module Pairings

- **Envelope Generators:** Maths, Quadrax, Function, Zadar
- **Drum Modules:** Hexinverter Mutant Drums, ALM Akemie’s Taiko, Tiptop One
- **Melodic Sequencers:** Rene, Voltage Block, Z8000, O&C in Sequencer Mode
- **Random/Modulation Sources:** Marbles, Turing Machine, Noise Tools, Batumi
- **Switches/Logic/Multiples:** Doepfer A-151, Mutable Branches, WMD SSM, Intellijel Mutamix
- **CV Utilities:** Attenuverters, Sample & Hold, Slews, VCAs
- **Effect Processors:** Clouds, Mimeophon, Magneto, Happy Nerding FX Aid

---

> Experiment with pairing ADDAC402’s generative rhythms with various modules and utility blocks—often the most original results come from cross-patching gates, triggers, and CV-controllable parameters in unexpected ways!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)