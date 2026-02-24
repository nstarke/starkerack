# Hexinverter — Orbitals

- [Manual PDF](../../manuals/hexinverter-orbitals.pdf)

---

[Hexinverter Orbitals User Manual PDF](https://hexinverter.net/public/OFFICIAL_OrbitalsUserManual.pdf)

---

# Creative Ways to Use the Hexinverter Orbitals Step Sequencer

The **Hexinverter Orbitals** is a powerful dual (or single 16-step) voltage-controlled step sequencer with a unique set of features such as dual operation, bipolar outputs, voltage-addressed modes, transposition, and extensive clock/reset/gate control. Here are some ideas to get the most out of it, especially when patched in creative ways with other Eurorack modules:

---

## 1. **Complex Melodic Sequencing**
- **Module types:** Quantizer (e.g., Intellijel Scales), Analog Oscillator (e.g., Make Noise STO), Envelope Generator, VCA.
- **Patch Idea:** Use Orbitals as the main pitch CV source, sending its CV output through a quantizer to keep melodies in key. Use the gate output to trigger an envelope generator, which then controls a VCA for your oscillator.
- **Creative Twist:** Use the transpose input (plug a keyboard or pressure sensor) for live transpositions, instantly reshaping patterns for performance.

---

## 2. **Evolving Patterns with Random and Voltage-Addressed Modes**
- **Module types:** S&H/Noise (e.g., Mutable Instruments Kinks), LFOs, Other sequencers.
- **Patch Idea:** Set one Orbitals sequencer to RANDOM or CV-addressed mode. Use an LFO or S&H to "scan" across the steps, creating non-linear, chaotic melodies or modulations.
- **Creative Twist:** Cross-patch the CV output back into another sequencer (or even the Orbitals’ own step-address input) for recursive, generative patches.

---

## 3. **Dual Polyrhythmic Sequences**
- **Module types:** Clock Divider/Multiplier (e.g., 4ms QCD), Drum modules (e.g., Tiptop Audio), Logic modules (e.g., Doepfer A-166).
- **Patch Idea:** Use the two sequencers independently, both clocked at different rates or divisions for polyrhythmic patterns controlling drums, bass, or percussive CV lines.
- **Creative Twist:** Combine the outputs through logic modules (AND, OR) to create even more complex triggers/gates.

---

## 4. **Voltage-Controlled Step Addressing for Live Performance**
- **Module types:** Touch Controller (e.g., Make Noise Pressure Points), Joysticks (e.g., Intellijel Planar), Envelope Followers.
- **Patch Idea:** Feed external CV (from touch controllers, joysticks, or audio-followed envelopes) into the CV-addressed step input. This allows hands-on control of sequence position, great for adding expressiveness or live manipulation.
- **Creative Twist:** Use audio-rate signals to the CV-address input for audio-rate "sequencing," producing wild, complex modulations.

---

## 5. **Automated Parameter Changes**
- **Module types:** Clockable Effects (e.g., Mutable Instruments Clouds), Filter (e.g., Mannequins Three Sisters), Dual LPG, Mod Matrix.
- **Patch Idea:** Use one sequencer row to control musical pitch and the other to modulate a filter cutoff, effect parameter, or VCA level, turning your rhythms and melodies into evolving, self-animating soundscapes.
- **Creative Twist:** Patch the gate outputs to re-trigger envelopes for layered or dynamic effects.

---

## 6. **Drum Sequence Variation with Bipolar CV**
- **Module types:** Drum modules with CV control (e.g., Basimilus Iteritas Alter), CV-controlled Switch (e.g., Erica Synths Sequential Switch).
- **Patch Idea:** Use bipolar output mode to sweep drum parameters both positively and negatively, or to scan a switch selecting different drum sounds or processing chains per step.

---

## 7. **Chain Sequencers for Longer Patterns**
- **Module types:** Logic/Sequential Switch, Multiple Orbitals units or other sequencers.
- **Patch Idea:** Use the Slave B>A function to chain Orbitals with another sequencer. Expand beyond 16 steps or have coordinated multi-voice sequences.

---

Each of these suggestions combines the unique **Orbitals** sequencing engine with common or creative Eurorack utilities, providing endless possibilities for musical exploration.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)