# IO Labs — Flux Sequencer

- [Manual PDF](../../manuals/IO Labs - Flux Sequencer - 107 User Manual.pdf)

---

[Flux Open Beta V1.07 User Manual PDF](https://iolabs.co.uk/downloads/Flux_Open_Beta_User_Manual_V1.07.pdf)

---

# Using Flux to Create Full-Length Songs in Eurorack Setups

Flux is an advanced rhythm and modulation sequencer designed to transcend the limitations of traditional step-grids by using **Temporal Modulation Synthesis®**. Its deep feature set makes it an ideal module not just for beat-making, but for structuring and performing entire songs within a Eurorack environment. Below, I’ll break down strategies for using Flux—alone and with other modules—to create compositions that evolve over several minutes, embracing structure, development, and dynamic changes.

---

## 1. Arrange with Per-Step, Per-Channel Variation

**How:**  
Flux allows nearly every rhythm and CV parameter to be set per-step and per-channel (4 channels, 16 steps each). This means every step can have unique trigger density, gate length, curve, CV envelope, mask, mod bus, and more.

**Use for Song Creation:**  
- **Sectional Arrangement:**  
  - Dedicate groups of steps to different song sections (e.g., steps 1-8 = intro/groove, 9-12 = breakdown, 13-16 = build/drop).
  - Use the `LOOP` parameter to tightly loop sections during performance, then progress to the next by changing the loop points or using modulation.
- **Parameter Morphing for Variety:**  
  - Gradually modulate trigger density or CV values over several steps (or with LFOs, see below) to create crescendo, breakdowns, or evolving sequences. Changing parameters per step lets you script these transitions.

## 2. Advanced Modulation for Macro-Level Changes

**How:**  
Flux features three modulation sources:
- **Macro Potentiometers** (manual)
- **Dedicated CV Inputs**
- **85 Internal Evolve LFOs**, saveable per preset

**Use for Song Creation:**  
- **Structural Evolution:**  
  - Assign a Macro Pot (or CV input from external sequencers/envelopes) to global parameters like BPM, density, or shuffle for manual “scene” changes.
  - Use slow, long-period internal LFOs (Evolve) to modulate parameters over several minutes—think of one Evolve LFO per channel as a “track macro” driving the song’s shape.
- **Automation via External Modules:**  
  - Patch envelopes or sequences from other modules into Flux CV inputs and assign them to parameters like COMP (compression/expansion of rhythm), LENG (step length), or CURV (curve of TM synthesis) to trigger song sections or changes in response to external events.
- **Multiple Modulation Buses:**  
  - Use different mod buses (Yellow, Grey, Purple) to activate certain modulation routings only in specific steps/sections. This lets you “cue” evolutions or breakdowns easily.

## 3. Preset Morphing and Live Section Switching

**How:**  
- Flux supports fast preset loading from microSD, with the ability to sync preset changes to 16th-note grid boundaries.
- As of V1.07, you can autoload the last loaded/saved preset at boot, and create several 'defaults' for quick access.

**Use for Song Creation:**  
- **Pattern Chaining:**  
  - Save “verse,” “chorus,” “fill,” “breakdown” patterns as separate presets. Load them in rhythmically perfect sync while performing.
- **Live Remixing:**  
  - Overwrite and reload active presets to constantly morph the sequence while keeping the groove.

## 4. Complex Rhythmic Variations, Fill-Ins, & Transitions

**How:**  
- Advanced rhythm shaping via mask, humanize (HUMA), phase shift (PHAS), probability (PROB), and AUX logic outputs.

**Use for Song Creation:**  
- **Fills/Breaks:**  
  - Program certain steps with extreme values (i.e., high density, maximal humanization, special mask patterns) to serve as “fills” or transitions.
  - Trigger mask changes, phase offsets, or probability drops via macro or CV to inject spontaneity.
- **Logic-Gated Transitions:**  
  - Use AUX outputs in boolean logic mode to gate external modules or effects, e.g., muting bass on the chorus, triggering FX sends, or launching alternate melodic sequences.

## 5. Integrated Melodic & Harmonic Progression

**How:**  
- Each channel has a per-step CV output, with quantization and selectable voltage range.
- CVs can deliver envelopes, LFOs, random values, or static voltages.

**Use for Song Creation:**  
- **Melodic Sequencing:**  
  - Sequence basslines, melodies, or modulation signals, quantized to scales or free-ranged, with per-step voltage changes.
- **Chord Progressions:**  
  - Assign channels to different voices (e.g., bass, pad, pluck, etc.). Use stepwise or modulated CV changes to create chord movement across song sections.

## 6. Syncing with External Clock and MIDI

**How:**  
- Flux supports MIDI in/out/clock, and advanced external clocking (EXT/EXTS), including DAW tight sync and trigger-based burst mode.

**Use for Song Creation:**  
- **DAW Integration:**  
  - Drive your whole rack from a DAW for precise arrangement and multitrack recording.
- **Responsive Song Form:**  
  - Use triggers or MIDI notes from external sources to switch song sections, trigger bursts, or cue events in real time.

## 7. Song Progression Example Workflow

1. **Establish your main groove (steps 1-8, Channel 1 & 2 for drums and bass).**
2. **Copy to later steps, vary density, CV, and shuffle for a bridge or drop.**
3. **Set up a Macro Pot to control overall groove density or swing.**
4. **Use Evolve LFOs on CV outputs to fade in melodic elements over time.**
5. **Assign different MOD buses to steps in the breakdown to turn modulation on/off at key moments.**
6. **Save sections as presets and use LOAD SYNC to jump between them in performance.**
7. **Use AUX logic outs to send clock, mutes, or trigger other sequencers/switches for transitions.**

---

## Integrating with Other Eurorack Modules

- **Drum modules:** Patch Flux rhythm outs to trigger inputs. Use humanize/mask/prob/chance for groove.
- **Synth voices:** Feed CV outs as pitch, envelope, or modulation signals for bass/melody/pad evolution.
- **Effect modules:** Use AUX logic outputs to trigger delays, reverbs, or switch matrixes for drops/fills.
- **External sequencers/modules:** Sync, modulate, or reset them with Flux outputs or use their CV to drive Flux parameter changes.
- **Samplers/Loopers:** Use Flux’s per-step rhythmic or CV data to evolve sampled textures or cue clips.

---

By planning out sections, automating transitions, and taking advantage of Flux’s deep per-step customization, you can move beyond “looping patterns” to programmed, live-playable song structure—just like a DAW but in full modular form.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)