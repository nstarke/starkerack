# ADDAC Systems — ADDAC-506 SignalFlow

- [Manual PDF](../../manuals/ADDAC506_SignalFlow.pdf)

---

[ADDAC506 VC Stochastic Function Generator & Expansion Manual (PDF)](https://media.addacsystem.com/files/manuals/ADDAC506_MANUAL.pdf)

---

## Generating Hyper Complex Percussion and Rhythms with the ADDAC506

The **ADDAC506 VC Stochastic Function Generator & Expansion** is a powerhouse for crafting densely rhythmic and hyper complex percussion sequences in your Eurorack setup. Here’s how you can exploit its features to make polyrhythmic, multi-timbral, and idiosyncratic percussion:

---

### **1. Use All Four Channels Independently for Polyrhythms**

- **Four Independent Envelopes**: Each channel acts as a function generator/envelope that can be triggered or slewed by independent sources.
- **Unsynced Cycles**: Trigger channels using unrelated or clock-divided gate/triggers, causing each envelope to loop at different rates. This immediately creates polyrhythms and cross-rhythms.
- **External Randomization (Expansion)**: Use the Expansion’s RANDOM TRIGGER inputs to re-randomize envelope times mid-cycle for bursts, fills, and unexpected time changes.

---

### **2. Embrace Complexity with Stochastic Rise/Fall Times**

- **Variable RISE/FALL Minimum & Maximum**: Set each channel’s RISE and FALL min/max to different, musically meaningful ranges (e.g., one short, one long, one medium, etc.).
- **Randomization per Trigger**: Each new trigger/loop chooses a new envelope time within set limits, resulting in constantly shifting, non-repeating patterns. Modulate min & max with CV for evolving polyrhythmic envelopes.
- **Lock Feature**: Lock certain channels to “freeze” a rhythm, then unlock and modify others for very intentional variability in patterns.

---

### **3. Exploit Loop/One-Shot and Gate/Trigger/Slew Behavior**

- **Loop Mode**: Use some channels as looping envelopes and others as one-shots to overlay static time signatures with freeform or stochastic elements.
- **Slew Mode**: Slew can turn stepped voltage sequences (like LFOs or random CVs) into percussive envelope shapes, following CV inputs in a unique, organic way. Great for anti-clock “ratcheting” percussive effects or unexpected swells.

---

### **4. Gate & EOR/EOF Outputs for Complicated Triggers**

- **Gate Outs**: Use the GATE OUT during the “rise” segment to define gate length; patch these to drum modules, VCAs, or hit/reset/clock inputs of other sequencers or digital modules for off-grid triggers.
- **EOR/EOF**: Use these outputs for meta-patterns – patch them to other envelope triggers, clocks, or sequential switches to create generation-on-generation polyrhythms.

---

### **5. Modulate Everything for “Living” Percussion**

- **CV Control Over Everything**: Feed LFOs, stepped modulations, random CV, or even audio-rate signals to RISE/FALL min or max, amplitude, offset, and curve parameters. Your envelopes become meta-instruments, responding dynamically in highly nuanced ways.
- **Curve Control (LIN/LOG)**: Morph between linear and logarithmic curves for each envelope to get snappier, more articulate “attack” phases or slow, booming decays—turning basic envelopes into a rich palette of percussion energies.

---

### **6. Summed & Averaged Mix Outs for Layering**

- **SUM/AVERAGE Outputs**: Use the sum or average of all 4 envelopes mixed together as a multi-layered modulation source—excellent for modulating filters, FX sends, or even as the master VCA envelope for a drum mix bus.

---

### **7. Unique Percussive Voice Design**

If using the outputs as voices:
- **Ping “Analog” Percussion Circuits**: Patch envelope outs directly to resonant filters, LPGs, or dedicated analog drum circuits for wildly unique percussive pings and thwacks.
- **Punch & Character**: Modulate amplitude and offset for each percussive hit. Pair with non-linear curves for snap. Try extreme settings to get glitchy, hyperactive digital artifacts.

---

### **Patch Examples**

#### **Meta-Polyrhythm Patch**
- ENVELOPE 1: Set to fast loop, RISE/FALL random range narrow (5–50 ms), into hat module trigger input
- ENVELOPE 2: Medium loop, wide random range, into snare trigger
- ENVELOPE 3: Triggered from an external rhythm generator, used as a complex modulation source for a drum synth’s pitch or filter
- ENVELOPE 4: One-shot mode with stochastic Rise, to play on “off-beat” kicks or FM percussion
- Use SUM/AVG out to modulate a send effect amount for all drums or drive a resonant LPG for pseudo stereo panning.

---

### **Final Tips**
- Always experiment with cross-patching random outputs, EOR/EOF, and random triggers.
- Morph CV and amplitude throughout a performance for evolving, living rhythms.
- The stochastic re-triggering means no two bars will ever be identical—harness this for unpredictable, intricate sequences.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
