# Mutable Instruments — Branches

- [Manual PDF](../../manuals/branches_quickstart.pdf)

---

[Manual PDF - Mutable Instruments Branches](https://mutable-instruments.net/modules/branches/manual.pdf)

---

## Creative Ways to Use Mutable Instruments Branches in Your Eurorack System

Mutable Instruments Branches is a Dual Bernoulli Gate, making it a probabilistic voltage-controlled switch—essential for generative, stochastic, and evolving patches. Below are creative ways to utilize Branches in your rack, both with specific and generic module recommendations:

---

### 1. Generative Rhythms
**Branches** can turn a single trigger source into two probabilistically distributed trigger streams.

- **Example Patch:** Feed a clock or trigger source (e.g., **ALM Pamela’s New Workout**, **4ms QCD**, or any basic clock module) into the IN of Branches. Route outputs A and B to two different drum modules (e.g., **Tiptop Audio ONE**, **Mutable Instruments Peaks**, or any drum voice).
- **Result:** With the probability knob/CV, vary which drum gets the trigger, creating shifting, evolving rhythms without complex sequencing.

---

### 2. Probability-Based Sequencing
- **Patch idea:** Route a step gate from a sequencer (e.g., **Intellijel Metropolix** or **Make Noise René**) into Branches.
- Send Output A to a melodic voice, and Output B to a different sequence or transposition circuit (**Doepfer A-156 Quantizer** or similar).
- **Result:** Some notes/steps will randomly change path, creating variations and happy accidents in your sequences.

---

### 3. Probabilistic Modulation Routing
- Route LFOs or envelopes (e.g., from **Mutable Instruments Tides**, **Doepfer A-140**, or **Joranalogue Contour 1**) into VCAs.
- Use clocked triggers divided and randomized by Branches to open the VCAs, thus sending modulations to different destinations probabilistically (e.g., filter cutoff or oscillator FM).
- **Result:** Dynamic and evolving modulations where destinations or timing change per patch cycle.

---

### 4. Drum Fill and Accent Control
- Insert Branches between your drum sequencer/triggers and the drum voices that you want to accent or fill occasionally.
- Use the probability knob to control how often a fill or accent actually fires.
- **Modules to combine:** **DFAM**, **Accent input on Tiptop drum modules**, or **Bastl Tea Kick**.

---

### 5. Generative SFX and Ambient Events
- Sample & Hold random CV (e.g., from **Mutable Instruments Marbles**, or **Noise Engineering Mimetic Digitalis**) can control the probability CV input.
- Route triggers from Branches to activate reverb throws, granular effects (such as **Mutable Instruments Clouds**), or event-style samples.
- **Result:** Occasional, unexpected sonic events that animate ambient or generative patches.

---

### 6. Toggle and Latch Modes for Alternating Patterns
- In Toggle mode, used with a hi-hat or percussion voice, create “always alternate” patterns from one trigger stream—great for open/closed hat alternation.
- In Latch mode, one output stays high until the next event, ideal for holding gates for event-driven effects or switching duties, like muting/unmuting voices (**Doepfer A-150 Switch** or **Intellijel Mutamix**).

---

### 7. Controlled Randomization with External CV
- Use random voltage sources, stepped random, or sequencer gates to control Branches’ probability CV input for deterministic or pattern-based switching.
- **Modules to combine:** **Mutable Instruments Marbles**, **ALM Pamela's New Workout (Random Outputs)**, **WMD Probabilistic Skipper**.

---

### 8. Performance Utility
- Use manual mode switching (toggle/latch) as a live performance tool, instantly re-structuring which voice gets triggered, or bringing in fills/effects with a long button press.
- Pair with an **Intellijel Tetrapad** for manual trigger or latch CV control.

---

## Tips
- **Branching Audio:** Branches is designed for triggers/gates, but you can experiment with logic-level audio for creative gating/chopping effects. Just be sure to protect your audio path if levels exceed safe thresholds.
- **Preset Storage:** Toggle/latch modes are retained on power cycle, ideal for gig or studio setups with repeatable probabilistic processes.

---

Let your patches evolve and surprise you by introducing chance! Mutable Instruments Branches is a powerful tool in generative, experimental, and performance Eurorack systems.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)