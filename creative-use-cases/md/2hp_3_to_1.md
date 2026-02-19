# 2hp — 3 to 1

- [Manual PDF](../../manuals/3_To_1_Manual.pdf)

---

[**Download the 2hp 3:1 Manual (PDF)**](https://2hp.com/docs/2hp-3-1-manual.pdf)

---

# Creative Patch Ideas with the 2hp 3:1 Gate Switch

The **2hp 3:1** is a compact, voltage-controllable gate/trigger switch and summer. It can function as both a **selective switch** (routing one of three gates to a destination) and a **gate summer** (outputting triggers for all active channels). Below are some ideas for creative use in your Eurorack system.

---

## 1. Dynamic Sequencer Variation

**Concept:** Use 3:1 to select between multiple gate/trigger sources, creating evolving rhythmic patterns.

**How-To:**
- **Connect three different gate sources** (e.g., from a sequencer like **Intellijel Metropolix**, **Make Noise Tempi**, or **Pamela’s New Workout**) to the inputs of 3:1.
- Use the **SEL CV** with an LFO, random voltage, or stepped voltage (e.g., from **Mutable Instruments Marbles** or **ALM Busy Circuits Pamela’s New Workout**) to automate which input is currently active.
- Send the output to an envelope generator or percussion module for shifting rhythmic variations.

---

## 2. Fast Drum Fill Generator

**Concept:** Automatically layer and rearrange multiple drum triggers for fills or rolls.

**How-To:**
- Patch kick, snare, and hat triggers into the three inputs.
- Use the **SUM mode** (MODE switch right) to create complex layered patterns—when multiple inputs are "selected," short triggers will be output for each pulse.
- Sequence the **SEL CV** input to periodically "open up" the switch for all drums at once, then return to selecting just one or two for fills/breakdowns.

---

## 3. Polyrhythm Maker

**Concept:** Fuse multiple clock sources at different time divisions for unique polyrhythms.

**How-To:**
- Send gates from multiple clock dividers (like **4ms Rotating Clock Divider** or **Doepfer A-160**) to the 3:1.
- Use the SUM mode; each input adds a trigger to the output.
- Send the result to a sequencer clock input, randomizer, or trigger an entire drum voice, generating evolving, non-repetitive patterns.

---

## 4. Performance Gate Routing

**Concept:** Live-swapping controller inputs for expressive performance.

**How-To:**
- Patch gates/triggers from something like **Make Noise Pressure Points**, a midi-to-gate converter, or manual gate buttons to 3:1.
- Use the SEL knob by hand during a performance to instantly reroute which input controls a target (like a VCA, effect trigger, or sample player).
- Automate changes for surprise drops or shifts during the set.

---

## 5. Gate-Controlled Effect Switching

**Concept:** Toggle between modulation sources or "punch in" effects at precise times.

**How-To:**
- Gate/trigger outputs from different modulation sequencers or function generators (e.g., **Maths**, **Zadar**, **Batumi**) to 3:1 inputs.
- Output goes to an effect module’s gate or trigger input (e.g., a burst generator, delay tap, or reverb freeze).
- Use SEL CV to let a sequencer or random source pick which modulation gets through.

---

## 6. Randomized Pattern Generator

**Concept:** Use random sources to automate selection for organic, never-repeating rhythms.

**How-To:**
- Patch outputs from games of chance/random modules (**Mutable Instruments Turing Machine**, **Wogglebug**) to SEL CV.
- Each time a random gate is sent, a different trigger sequence or cross-rhythm is produced.

---

## 7. Expand Envelope/Function Generator Complexity

**Concept:** Sequence access to multiple envelope shapes for a single destination.

**How-To:**
- Patch different function generator end-of-cycle/gate outputs (or use varied length trigger sources) into 3:1 inputs.
- The output can sequence different envelope shapes to a single VCA or filter, providing unique modulation movement tailored by how you control the SEL position.

---

## Useful Module Recommendations

- **Random CV/LFO:** Mutable Instruments Marbles, ALM Pamela’s New Workout, Make Noise Maths
- **Clock Divider/Drum Trigger:** 4ms QCD, Doepfer A-160/161, TipTop Trigger Riot
- **Envelope/Function Generators:** Intellijel Quadra, Make Noise Function, Zadar
- **CV Step/Sequencing:** Malekko Voltage Block, Intellijel Metropolix, Doepfer A-155
- **Gate/Trigger Controllers:** Erica Synths Pico Trigger, Mutable Instruments Peaks

---

## Tips for Advanced Patching

- Use **stackable cables or mults** to share gate sources and create interlocked rhythms.
- Try using **audio-rate signals** in SUM mode for unusual, glitchy effects—be sure to protect sensitive modules!
- Experiment with clocking SEL CV for highly repeatable pattern switches, or with slow/random voltages for more generative compositions.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)