# 2hp — Turing Machine

- [Manual PDF](../../manuals/TM_Manual.pdf)

---

[2hp TM Manual PDF](https://cdn2.shopify.com/s/files/1/1526/0915/files/2hp_TM_Manual.pdf)

---

# How to Use the 2hp TM for Full-Length Song Creation in a Eurorack System

The 2hp TM module is an extremely flexible probabilistic random sequence generator, inspired by the concept of the Turing machine. Its role is to provide evolving or locked random voltages, ideal for generative and variation-based sequences. However, building *full songs* in modular environments requires planning for progression, movement, and variation—not just great patterns in a loop.

Below are detailed strategies on using the TM with other modules to move beyond loops, building engaging full-length tracks.

---

## 1. Evolving Melodic and Harmonic Content

**TM as Melodic Source:**  
- **Quantizer:** Patch TM’s OUT to a quantizer to ensure output voltages create melodic lines in a desired scale. Use PROB to lock/unlock parts of the melody, letting themes evolve or repeat.
- **Song Structure:** As your track develops, automate PROB via CV (using sequencers or LFOS/envelopes) so some sections introduce more randomness (“verse-style”), and in others, the melody becomes repetitive (“chorus-style” or motif).

**Harmonic Movement:**  
- Use several TM modules, or a sample & hold fed by TM OUT, to drive harmonies, chord roots, or even drum pitch/sample selection.

---

## 2. Creating Verses, Choruses, and Bridges

### **Scene Changes via Probability or Steps**
- **Mutate/Revert:** Assign scenes (song sections) by having clocked signals shift PROB or STEPS, e.g. verse (random/prob high, long sequence), chorus (locked/prob low, shorter motif), bridge (medium-high randomness and step length).
- Use sequential switches or sequential function generators to automate these transitions over time.

### **Automated Song Structure**
- **Macro Sequencers:** Use an external sequencer to send distinct CVs to TM’s PROB and STEPS. At different points in your composition, force the TM to:
    - Generate new material (high randomness, longer sequences)
    - Lock to a repeating phrase (zero randomness)
    - Change the sequence length to tighten or stretch thematic content

---

## 3. Dynamic Variation for Bass, Drums, and FX

### **Basslines**
- Clock TM at a lower division to provide slowly evolving randomized bass movement, or lock PROB for repetitive riffs.
- Use amplitude control (AMP) to sculpt levels, or send OUT to a VCA for dynamic energy shifts per section.

### **Drums/FX**
- Use TM’s random voltages to trigger drum fills, switch drum kits, or modulate effect parameters, ramping up intensity for builds or breakdowns.

---

## 4. Controlling Movement and Build-Ups

### **Morphing and Transitions**
- Modulate TM’s PROB and AMP with LFOs, envelopes, or sequenced controls during breakdowns and drops, causing melodies or textures to destabilize, then “reset” at the drop by locking probability.

### **Automated Evolution**
- Use external logic, sequential switches, or control modules to systematically adjust TM parameters song-wide (e.g., every 16 bars change PROB, AMP, or STEPS).

---

## 5. Patching Examples

### **Basic Melodic Evolution**
```
TM OUT → Quantizer → VCO 1V/Oct
TM TRIG → Clock Divider
Quantizer OUT → VCA → MIXER
- CV modulate PROB with a slow LFO for organic movement.
```

### **Scene-Based Song Structure**
```
TM PROB CV ← Macro Sequencer Scene 1: high (random), Scene 2: low (repeat theme), Scene 3: medium (variation)
TM STEPS CV ← Macro Sequencer to shift sequence length to match song sections
```

### **FX Automation**
```
TM OUT → FX Module Wet/Dry CV
- In chorus, AMP is raised so effects open up, dropping in verse to tighten sound.
```

---

## 6. Tips for Full Songwriting Approaches

- **Combine TM with preset-sequencing modules** (like the Mutable Instruments Frames, or Sequential Switches) for “section recall.”
- **Use TM as a drummer or fill generator** by modulating percussive voices, arpeggiators, or ratcheting modules.
- **Layer several TM instances** for ensemble-like generative textures that can be faded/solo’d in your mix for arrangement control.

---

By blending probability, step length, and amplitude modulation—especially when CV-controlled from other modules or sequencers—you can animate the TM to create living arrangements suitable for full-length modular compositions.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
