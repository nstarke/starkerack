# 2hp — Rout

- [Manual PDF](../../manuals/Rout_Manual.pdf)

---

[2hp Rout Official Manual PDF](https://2hp.com/docs/Rout%20Manual.pdf)

---

# Using the 2hp Rout Module for Full-Length Song Structure in Eurorack

Creating compelling, structured full-length songs in a modular environment can be challenging. While the 2hp Rout is a small, simple module, its voltage-controlled routing capabilities offer powerful methods for expanding single patterns into evolving song forms. Here are several creative strategies for deploying the Rout module in your rack, based on the attached manual, to achieve dynamic, evolving compositions.

---

## **Key Features Recap**

- **Voltage Controlled Gate Switch:** One input routed to any of 4 outputs.
- **Selectable via Knob or CV (0–5V):** Manual or automated selection.
- **Split or Variate Patterns:** Route gates to different destinations per song section.
- **Ultra-compact (2HP):** Fits in almost any system.

---

## **Song Structure & Variation Techniques**

### 1. **Pattern Switching for Song Sections**

**Idea:** Use the Rout’s ability to route a single rhythm (e.g., main gate clock, sequencer trigger, or pattern from a drum machine) to 4 different destinations, each corresponding to a different section or variation in your track.

**How-To:**
- **OUT 1:** Sends trigger pattern to a kick for verse.
- **OUT 2:** Sends to a snare for chorus.
- **OUT 3:** Routes to an effect or fill generator for breakdowns.
- **OUT 4:** Routes to all percussion for a climax.
- **Automate SEL (Selection) by CV:** Use a slow modulation source, scene-change sequencer, or manually switch with the knob.

> **Result:** Seamlessly morph between different song parts—no computer required.

---

### 2. **Create Performance-Friendly Fills and Breaks**

**Idea:** Use Rout as a manual or sequenced "live switch" to add fills, breakdowns, or sudden drops to your performance.

**How-To:**
- Route a gate/trigger clock from your master clock or drum sequencer to the Rout input.
- Send Rout outputs to:
  - **OUT 1:** Main drum pattern
  - **OUT 2:** Fill generator
  - **OUT 3:** Muted or alternate pattern
  - **OUT 4:** FX (e.g., manual stutter, glitch, or reverb burst)
- Use a CV source (manual fader, footswitch, performance controller, or even another sequencer track) to select song transitions, breaks, or “solo” moments live.

> **Result:** Human, performance-ready song sections, hands-on or automated.

---

### 3. **Dynamic Voice Allocation for Melodies or Basslines**

**Idea:** Route a single melodic trigger sequence to several voices for evolving, varied phrasing.

**How-To:**
- **OUT 1:** Main voice (lead synth)
- **OUT 2:** Doubled VCO (octave above/below)
- **OUT 3:** Bass synth
- **OUT 4:** Percussive element or FX voice
- Use SEL CV to sequence or randomly select which output is active per phrase, bar, or section.

> **Result:** One pattern can “move” between parts, creating evolving arrangements out of repetition.

---

### 4. **Automate Mutes and Drops**

**Idea:** Rout can act as a muting matrix. Automate SEL to "mute" various drums, synths, or effects for dynamic arrangements (a trick commonly used in DAWs but hard to achieve in modular).

**How-To:**
- Connect the desired pattern to Rout input.
- Let outputs go to various drum modules, envelopes, or effect triggers.
- Create a mute track on your sequencer to automate Rout’s SEL CV, dropping out whole parts instantly.

> **Result:** Instant mutes/breaks for tension, release, and transitions, without removing cables.

---

### 5. **Song Arrangement “Scenes” Control**

**Idea:** Use Rout to swap entire scenes at the press of a button or via a programmed control voltage.

**How-To:**
- Use an external CV sequencer or preset manager to step Rout’s SEL across your four outputs.
- Reroute all triggers to pre-patched voice or section "scenes" in your system.
  
> **Result:** Modular "scenes" or "song sections," like a groovebox or performance sampler.

---

## **Suggested Companion Modules**

- **Sequential Switch** (for more than four scenes)
- **CV Sequencer or Automation Source** (like Make Noise Pressure Points, Mutable Instruments Marbles, etc.)
- **Clock Divider/Multiplier** (for rhythmic variation)
- **Logic Modules** (combine signals for advanced patterns)
- **Envelope Generators or Slew Limiters** (for animated SEL CV dosage)
- **Drum Modules, Snares, FX—dynamic routing targets!**

---

## **Conclusion**

**2hp Rout** is deceptively simple but can be the modular “brains” of a song structure, enabling live switching, fills, breaks, scene changes, and real arrangement dynamics—entirely hands-on or fully automated.

**Experiment** with Rout, and you’ll find crafting a *full-length, engaging song* in your Eurorack is not only possible but deeply creative and performable, all without a screen.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)