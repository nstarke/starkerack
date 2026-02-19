# Pittsburgh Modular — Gamesystem

- [Manual PDF](../../manuals/game_system_manual.pdf)

---

[Download the Game System Manual (PDF)](https://pittsburghmodular.com/uploads/Game_System_Manual.pdf)

---

# Creative Patch Ideas for Pittsburgh Modular Game System

The **Pittsburgh Modular Game System** is a wildly unique sequencing and control source for Eurorack—part arcade interface, part algorithmic mind-bender, and always full of surprises. Below you’ll find patching ideas and module pairings to spiral your rack into new musical zones, leveraging each “game” mode’s quirks.

---

## Multi-Mode Sequencer Synergies

### 1. **Meteor Shower – Random S&H CV & Transient Percussion**
- **Patch Output 1 (random CV) to a VCO 1V/Oct input.**
  - This random melodic line, triggered by spaceship/meteor collisions, produces organic melodies.
- **Output 2 and Output 3 (gates) to trigger percussive modules** like **Mutable Instruments Peaks**, **ALM Akemie's Taiko**, or any gate-able envelope generator.
- **Output 4 (clock)** into a clock divider/multiplier (**4ms Rotating Clock Divider**, **Doepfer A-160-2**) to sync external rhythm sections.

### 2. **Music Sequencer – Melodic CV & Polyphonic Potentials**
- **Parallel Outputs 1 & 2**: Send both melodic CV outs to separate VCOs (**Make Noise DPO** + **Intellijel Dixie II+**) for intervallic/tuned layering.
- **Gate outputs for voice articulation**: Patch Outputs 3 (main seq gate) to envelope or LPG; use Output 4 for master clock to sync **sequenced modulation sources** (e.g., **Xaoc Batumi** running stepped LFOs in sync).

### 3. **Drum Sequencer – Polyrhythmic Drum Kits**
- **4 Gate outputs direct to drum modules** (**Tiptop Audio 808/909 modules**, **Vermona DRM1**, **Noise Engineering Basimilus Iteritas Alter**).
- **Stack gate outputs** via a simple **logic OR audio combiner** (e.g., **Doepfer A-186-1**) for complex trigger patterns or accent tracks.
- **Use outputs as triggers for random or S&H modules**—send resulting CVs to effects or timbral modulation elsewhere.

### 4. **Time Traveller – Polymetric Clocking & Generative Logic**
- **Four divided, offset-gate outputs** to clock separate sequencers/logic modules (e.g., **Intellijel Metropolis**, **Make Noise Rene**, **ALM Pamela’s New Workout**).
- **Patch outputs to different modulation clock destinations (LFO resets, S&H clock-ins, delays, etc.)** for evolving, ever-shifting movement across the entire rack.
- **Use “roaming” mode for generative unpredictability**—perfect for ambient or experimental/polyrhythmic sets.

### 5. **Probability Machine – Generative Modulation**
- **Send random CVs (Outputs 1/2) to filter cutoff (VCF), waveshaper amount, VCA level, or delay time.**
- **Use gate outputs to trigger/sample-and-hold modules** for constantly shifting textures.
- **Patch to Mutable Instruments Marbles for additional probability/randomization, or to orchestrated sample slicers like the  **1010music Bitbox**.

### 6. **Euclidean Rhythms – West Coast Grooves & Sequence Morphs**
- **Sync Euclidean gates to classic drum modules** for non-standard rhythms.
- **Patch random CV output** into quantizers like **Intellijel uScale** or **Doepfer A-156**, then to melodic voices.
- **Output 3’s “anti-gate”** can automate muting crossfades or retriggering a granular sampler when the rhythm “rests”.
- **Combine Euclidean gates with logic/comparator modules** (e.g., **Mutable Instruments Branches**, **Doepfer A-166**) to produce shifting patterns on the fly.

---

## Bonus Tips & Module Recommendations

- **External Clocking:** Use **Pamela’s New Workout** or **ALM QCD** for CV-divided or swung clocks—send these into the Game System for clock source variety.
- **Joystick CV Inputs:** Patch stepped LFOs or sequencer CVs (from **Make Noise Pressure Points**/**Doepfer A-155**) into the joystick’s CV/gate inputs for generative parameter surfing.
- **Preset-selected Modes:** Automate “game” and “mode” switching with simple gate triggers from a switching/sequencer module (**WMD Sequential Switch Matrix**, **Doepfer A-150**) to create evolving sets.

---

## Use Cases by Genre

- **Generative Ambient:** Use Probability Machine and Time Traveller to randomly clock, modulate, and texturize evolving patches.
- **Techno/House:** Drum sequencer with Euclidean rhythms for driving percussive patterns; use Music Sequencer to control acid basslines.
- **Experimental/Noise:** Use Meteor Shower for unpredictably triggered gates/CV. Cross-patch clock and random outputs to sampling/glitch modules.
- **IDM/Electro:** Blend polyrhythms from Time Traveller and Euclidean gates for off-kilter, Autechre-like drum breaks.

---

> **Remember:** The Game System invites hands-on play as much as CV automation. Use “joystick as performance” by riding patterns live, while CV externalizes control for advanced algorithmic sets.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
