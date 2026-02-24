# Hexinverter — Orbitals

- [Manual PDF](../../manuals/hexinverter-orbitals.pdf)

---

[Download the Orbitals User Manual PDF](https://hexinverter.net/public/assets/documentation/orbitals/Orbitals_User_Manual_v104.pdf)

---

# Creating Full Length Songs With the Hexinverter Orbitals Step Sequencer

The Orbitals is a feature-rich dual (or single 16-step) voltage-controlled step sequencer for Eurorack, capable of providing the evolving structure required for full-length compositions. Moving from simple loops to "songs" requires strategies to introduce variation, progression, and dynamic changes over time.

Below are detailed techniques, patch ideas, and workflow suggestions combining Orbitals with other modules to build extended, evolving tracks.

---

## 1. **Song Structure Through Sequence Length and Modes**

**Orbitals Key Features:**  
- Dual 8-step or single 16-step operation  
- Individual sequence lengths per side  
- Multiple step modes: forward, reverse, pendulum, random, CV, and clocked CV  
- Manual or CV-addressed step selection  
- Transpose CV input

**Song Application:**  
- **Verse/Chorus Alternation:** Use the dual sequencer mode (2x8) for A/B song sections. Each sequencer can control a different synth voice, or you can switch between them for melodic vs. bass/lead duties.
- **Progressive Variation:** Modulate the LENGTH knob with stepped or random voltages (from a sample & hold or another sequencer) to shift between patterns of different lengths over time.
- **Mode Modulation:** CV-control the MODE knob (via external switches, sequential switch, or manual tweaks) to transition from straightforward to random or pendulum patterns—perfect for breakdowns, fills, or transitions.

---

## 2. **Performance and Live Song Morphing**

- **RUN Inputs and Reset:** Use external gate/logic modules, footswitches, or a MIDI-to-CV interface to start/stop sequences or reset for synchronized drops and section changes.
- **Manual Performance:** The RUN, MODE, or LENGTH controls can be tweaked in real-time during a set, letting you reconfigure the sequence’s behavior for dynamic song sections.

---

## 3. **Inter-Module Integration for Arrangement Control**

- **Slave B>A and External Clocks:**  
  - Sync Orbitals with external or master clocks (Pam’s New Workout, MIDI clock, etc.) to ensure your arrangement follows song tempo.
  - Enable SLAVE B>A for tight alignment between melodic and rhythmic elements.

- **Sequence Transposition:**  
  - Plug a keyboard or sequencer into TRANSPOSE A to change the musical key live—great for choruses, bridges, or modulations.

---

## 4. **Evolving Textures and Long-Form Development**

- **Utilize Bipolar Output:**  
  - Bipolar CV (centered around 0V) lets you scan back and forth across filter frequencies, pan, crossfade between effects, or smoothly animate parameters that benefit from negative-to-positive voltage swings.
- **Voltage Controlled Step Addressing:**  
  - Use an LFO, random source, or complex modulator patched into the RST/CV input in CV or CLK mode. This enables the sequencer to "jump" around steps, introducing generative phrasing and long-evolving patterns perfect for ambient, IDM, or experimental tracks.

---

## 5. **Melodic, Bass & Rhythmic Layering**

- **Polyrhythms with Independent Clocks:**  
  - Drive each sequencer with different clock sources, clock dividers, or clock manipulators to layer asynchronous grooves. This can create unpredictable but musical variations throughout a track.

- **Multiple Voices:**  
  - Use sequencing A for melody and B for bass, or route A to oscillator pitch and B to filter cutoff, effect send, or other modulation destinations for evolving timbres and complexity.

---

## 6. **Automation and Song Progression**

- **External Modulation:**  
  - Modulate the RATE, GATE, MODE, or LENGTH using CV from automation lanes (via CV recorders), other sequencers, or random/chaotic sources to create macro changes, such as slower rates in breakdowns, increased gate length for drone sections, or switching to random/ping-pong mode for fills and bridges.

- **Preset Changes and “Scenes”:**  
  - Use a sequential switch (e.g., Doepfer A-151, WMD Sequential Switch Matrix) to change which stages or outputs from Orbitals go to which sound destinations, simulating “song scenes” or traditional verse/chorus/bridge structures.

---

## 7. **Patch Example: Performance Song Structure**

**Modules Used:**  
- Orbitals Step Sequencer  
- MIDI-CV interface (for keyboard transpose and/or clock)  
- Logic module (for sequencing RUN/RESET or clock divisions)  
- Two Synth Voices (e.g., VCO, filter, envelope, VCA)  
- Mixer & FX

**Patch Flow:**  
1. Sequencer A to voice 1 (melody), Sequencer B to voice 2 (bass line).
2. External clock drives both sequencers, with a clock divider/comparator switching B between RUN/STOP to alternate verse/chorus.
3. Use a keyboard to transpose melody (plugged into TRANS A).
4. Send LFO or random CV to MODE/LENGTH inputs for scene changes.
5. Patch GATE outputs to trigger rhythmic elements or lip-sync drums for variation.
6. Use an external switch or CV mixer to change which output (A/B) hits your main effects for live breakdowns or transitions.

---

## 8. **Additional Tips**

- **Manually or with CV, change GATE length for expressive phrasing.**
- **Combine with trigger/gate sequencers for drums, or use Orbitals’ random/pendulum modes for fill creation.**
- **Automate RESETs at key points for synced drops or transitions.**

---

By carefully patching, combining features, and integrating Orbitals with other Eurorack utilities and voice modules, you can move far beyond simple loops into true song structure—building evolving, expressive, and dynamic full-length tracks within your modular synthesizer.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
