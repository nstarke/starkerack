# Nervous Squirrel — Conway's Game

- [Manual PDF](../../manuals/Nervous Squirrel - Conway's Game.pdf)

---

[**View the manual (PDF)**](attachment:Conways_Game.pdf)

---

# Creative Uses for **Nervous Squirrel – Conway’s Game**

The **Conway’s Game** Eurorack module is a unique hybrid: a cellular automaton visualized on an 8x8 matrix, generating up to 64 simultaneous trigger/gate outputs or functioning as a MIDI-to-trigger converter. The evolving chaos of **Conway’s Game of Life** makes it ripe for generative, probabilistic, and deeply organic compositions when paired with the right modules.

Below are creative setups and combinations—with both generic types and specific module recommendations—for unleashing its full potential in your rack.

---

## 1. **Generative Drumming and Percussion Mayhem**

**How:**  
Patch different groups of the 64 outputs to multiple drum modules (or channels of a multi-voice drum synth, e.g., **TipTop Audio MISO, Mutable Instruments Peaks, or Erica Synths Drum Series**). Each drum gets its own unpredictable trigger pattern, always evolving.

**Enhancements:**
- **Switches / Sequential Switches** (e.g., Doepfer A-151, Mutable Instruments Branches): Cycle patterns or combine outputs dynamically.
- **Logic Modules** (Intellijel Plog, Doepfer A-166): Merge or alter trigger streams for even less predictability.
- **CV-able Drum Modules:** Fire **Modular Grid sequencer triggers** with generative gates for polyrhythms.

---

## 2. **Generative Melodic Sequencing**

**How:**  
Send triggers to quantizer/gated sample & hold modules (e.g., **Mutable Instruments Marbles**, **Doepfer A-148**, or **ALM Busy Circuits Pamela’s Pro Workout**) which control CV lines to oscillators or voices.

**Layering Ideas:**
- Use one cluster of outputs for pitch triggers, another for envelope firing, others for rhythm or accents.
- **Envelope Generators** (Make Noise Maths, Intellijel Quadra) react to different cells for complex, layered phrases.
- Map MIDI to control which set of outputs are active, switching live between pre-structured and emergent patterns.

---

## 3. **Organic & Evolving Modulation**

**How:**  
Route triggers to **LFO Reset** jacks, **random generators** (e.g., **Mutable Instruments Tides or Peaks**), or **clock dividers/multiplier modules** (4ms QCD, Doepfer A-160/A-161).

**Outcomes:**
- Create rhythmic clocks that are almost-but-not-quite regular.
- Modulate delay, reverb, filters, or waveshaping parameters with erratic but structured On/Off gates.
- Use long “GATE” mode triggers in Life mode for advanced modulation, not just percussive shots.

---

## 4. **Trigger Audio Effects and Sample Players**

**How:**  
Patch gates/triggers to sample or loopers’ start/stop/reset functions (e.g., **4ms Stereo Triggered Sampler, Make Noise Morphagene, Erica Synths Sample Drum**).

**Creative Effect:**
- Live re-slicing, randomized sample retriggering, or polyphonic sample manipulation, with Life-state drama mapped to your playback.

---

## 5. **MIDI Integration: Algorithmic Control/Sequencing**

**How:**  
- Use DAW or MIDI controller to send note triggers (C2–E7, notes 36–100) mapping to the 8x8 grid. Each note = a cell/gate output.
- Live improvise which outputs fire, using MIDI keyboard or sequencer.

**Combo Ideas:**
- MIDI clock or gate into CLOCK IN to sync Life’s cycle to your set/BPM.
- Use the internal clock for standalone generative operation, then override with a DAW clock for live performance control.

---

## 6. **Feedback & Self-Patching**

**How:**  
- Feed a subset of outputs back into the module’s own RESET or CLOCK IN jack with buffered multiples, logic, or sequential switches.
- Patch outputs to other modules, then sum their outputs back in to modulate the Conway’s Game clock: self-evolving, entirely unpredictable structures.

---

## 7. **Visual & Performative Applications**

**How:**  
- Use Conway’s Game as a visual cue for live performance—mapping the 8x8 matrix to stage lighting, video synths (LZX Industries), or laser triggers.
- Create audio/visual sync with modular video gear, for evolving installations or experimental A/V sets.

---

## Quick Patch Matrix (Output → Target Module):

| Conway Grid Output | Recommended Target Module                  | Result                     |
|--------------------|-------------------------------------------|----------------------------|
| Row 1              | Kick / Drum Trigger Input                 | Algorithmic percussion     |
| Row 2              | Envelope Generator Gate                   | Dynamic modulation         |
| Row 3–4            | Quantizer S&H Trigger                     | Melodic steps              |
| Rows 5–6           | Logic Gate Combiner / Divider             | Clock/chaos source         |
| Rows 7–8           | LFO Reset / Delay Freeze / FX Mod         | FX with generative chaos   |

---

### **Recommended Module Pairings (by category)**

- **Logic/Random:** Mutable Marbles, Intellijel Plog, Doepfer A-166, WMD Probabilty Jector
- **Drum/Voice:** Erica Synths Drum Series, Mutable Peaks, TipTop 808/909, Noise Engineering Basimilus Iteritas Alter
- **CV Treatment:** ALM Pamela’s Pro Workout, 4ms QPLFO, Maths, WMD/SSF Modbox
- **MIDI Utilities:** Expert Sleepers FH-2, Doepfer A-190-4
- **Visual/AV:** LZX Industries video modules

---

### **Experimental Edge**

- Try audio-rate clocks to push the automaton into unpredictable glitchy states.
- Patch different rows to audio and CV at the same time, for cross-rhythms.
- Use minimalist Life states for minimal techno patterns; amplify density for IDM or breakcore chaos.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)