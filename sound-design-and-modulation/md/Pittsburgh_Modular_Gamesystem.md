# Pittsburgh Modular — Gamesystem

- [Manual PDF](../../manuals/game_system_manual.pdf)

---

[View the Pittsburgh Modular Game System Manual PDF](https://pittsburghmodular.com/storage/Game-System-Manual-web.pdf)

---

# Modulation & Creative Patching with the Pittsburgh Modular **Game System**

The Pittsburgh Modular Game System is an innovative and deep multi-sequencer module for eurorack, featuring six "game modes" that excel at both traditional and experimental sequencing. With its **joystick, buttons**, and **fully voltage-controllable interface**, the Game System stands out for external modulation. The following are some patching and modulation ideas targeting **distorted percussion**, **aggressive basslines**, and **atmospheric pads**.

---

## 1. General Patch Ideas for Modulation

### Voltage Control Possibilities
Every Game/CV control (LEFT, RIGHT, UP, DOWN, BUTTON, MODE, RESET, CLOCK) can be triggered or modulated via CV/gate input. This makes it perfect for **CV/Gate automation**, LFOs, random sources, or triggers to push the sequencer in unexpected directions.

### Joystick/Step Modulation
- Use a chaotic LFO or stepped random (e.g., *Wogglebug*, *Pam’s New Workout*, *Turing Machine*) patched to the UP/DOWN/LEFT/RIGHT CV inputs to automatically navigate the Game System’s matrix/steps.
- Envelope generators or rhythmic gates can "press" BUTTON or MODE, toggling modes or filling in steps—great for *live algorithmic changes*.

---

## 2. **Distorted Percussive Sounds**

**Best "Game": DRUM SEQUENCER (GAME 3)**

- **Patch Tips:**
  - Patch the Drum Sequencer gates (Outputs 1-4) to a variety of percussion voices (classic drum modules, analog noise sources, or even envelopes keying VCAs).
  - Mult or stack the *same* gate output to trigger several modules for layered percussion.
  - Send your percussion voices through wavefolders, saturation, or distortion modules for aggressive, industrial tones.
  - Modulate the **joystick/cursor position** via *random* or *clocked stepped* CV to create erratic, glitchy fills—like random drum rolls or unexpected accent patterns.
  - Use MODE input (CV) to automate flipping green/red sequencers for dynamic, evolving rhythm structures.

**Supercharged Patches:**
- **Patch a CV sequencer or stepped random voltage into UP/DOWN or LEFT/RIGHT to make the Drum Sequencer continuously select different steps (auto-drum fill generator!).**
- Mult a *noisy* gate output to both a drum voice and a distortion/wavefolder’s CV input for interactive overdrive.
- Run a clock divider into RESET or MODE for shifting groove accents and live muting.

---

## 3. **Crazy Dubstep/Drum & Bass Basslines**

**Best "Games": MUSIC SEQUENCER (GAME 2), PROBABILITY MACHINE (GAME 5), EUCLIDEAN RHYTHMS (GAME 6)**

- **Patch Tips:**
  - Music Sequencer: Sequence 32 steps of 1V/oct bass (with slew on the output, if desired, for slides/portamento). Outputs are quantized for precise tuning. Patch through LPG with envelope for punch.
  - For movement, automate joystick left/right (step select) and up/down (pitch) with a slow or chaotic CV—basslines evolve in real-time!
  - Hold Joystick Button for "last step" resets to create *odd-length sequences* and polyrhythms, perfect for D&B.
  - Use Probability Machine: Patch gate outputs to bass voice envelopes. CV outs can FM or modulate bass harmonics for unexpected timbral variety.
  - In Euclidean mode: Automate sequence length/beats via LFOs or random CV for shifting, skittering syncopated bass.

**Supercharged Patches:**
- Sync the Game System clock to your master clock for tight grooves, then modulate the clock division via CV for drop/build effects.
- Clock-sync CV LFO into the BUTTON input and random source into RIGHT/LEFT for evolving steps.
- Use the Probability Machine’s paired CV/gates for bass voice cutoff and amplitude—randomized snarling movement.
- Patch a gate out to flip a waveshaper or distortion's mode in sync with bass pattern hits.

---

## 4. **Haunting Atmospheric Pads**

**Best "Games": MUSIC SEQUENCER, EUCLIDEAN RHYTHMS, TIME TRAVELLER**

- **Patch Tips:**
  - Use CV outs for slow-moving pitch or filter number sequences on dual/four-voice oscillators with long envelope releases.
  - Use external LFO or random source into UP/DOWN and LEFT/RIGHT for generative cursor motion—notes or chord changes all drift unpredictably.
  - In Time Traveller mode, send random or slow periodic voltages into joystick CVs for shifting polyrhythmic clocks that gate VCAs, filters, or reverb processors.
  - Euclidean mode: Program lush, polyphonic sustained chords or pulses, modulate beat count for evolving textures.
  - Use RESET or MODE button CV for sudden, ghostly pattern morphs.
  - Run CV and gate outs through delay and reverb for deep space.

**Supercharged Patches:**
- Mult the same CV output across several detuned oscillators for thickening.
- Use the Game System’s random CV sources (like Meteor Shower or Probability Machine) as slow modulator signals for *ambient washes*.
- Slowly randomize clock speed or division via CV for warbling effect.

---

## 5. Combining CV Inputs for Maximum Modulation

- Chain your control sources: Set up a sequential switch or logic module feeding random, LFO, and envelope signals to the Game System’s control inputs. This gives *real-time or automated variation* across all game modes.
- Stack clock divisions, clock multipliers, and logic signals to the CLOCK input for complex, non-repetitive rhythmic foundations.

**Example Patch Chain for Chaotic Bass-Drum Combo:**
- Use Probability Machine in *crazy* mode for main bassline pitch sequence (CV out), clocked at double-time.
- Drum Sequencer triggers main drums—MODULATE its cursor via a triggered random CV, driven in sync with Probability Machine gates for reactive percussion.
- Patch gate outs to trigger distortions and amplitude/fold parameters for *bass growls*.

---

## Further Reading and Resources

- [Game System Manual PDF (official)](https://pittsburghmodular.com/storage/Game-System-Manual-web.pdf)
- [Pittsburgh Modular Game System Official Page](https://pittsburghmodular.com/game-system)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)