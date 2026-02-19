# 2hp — Euclid

- [Manual PDF](../../manuals/2hp_Euclid.pdf)

---

[Euclid 2hp Manual PDF](https://2hp.com/docs/euclid.pdf)

---

# Euclid (2hp) Module Creative Patch Ideas

The **2hp Euclid** is a compact, CV-controllable Euclidean pattern generator that outputs rhythmically distributed triggers. Below are several creative patch ideas and combinations with other modules to maximize its potential in your eurorack system.

---

## 1. **Euclidean Drum Patterns**

- **Patch:**  
  Connect **Euclid's OUT** to a drum module's trigger input (e.g., Mutable Instruments Plaits, Noise Engineering Basimilus Iteritas Alter, or Erica Synths Pico Drum).
- **Variation:**  
  Use the **Length** and **Steps** CV inputs with sequencers or random generators (e.g., Pamela's Pro Workout, Make Noise Maths, ALM Pamela's New Workout, or a voltage randomizer like Mutable Instruments Marbles) to dynamically morph patterns.

---

## 2. **Polyrhythmic Layering**

- **Patch:**  
  Chain multiple **Euclid** modules (or combine with other Euclidean generators such as Euclidean Circles (vpme.de) or the Mutable Instruments Grids) with different pattern lengths.  
  Send outputs to different sound sources (e.g., kick, snare, high-hat) for instant polyrhythms that evolve as you modulate Length, Steps, and Offset.
- **Pro Tip:**  
  Use an **offset generator** (e.g., Doepfer A-183-2, Intellijel Quadratt) to manually adjust the Offset and create "shifting" grooves.

---

## 3. **Dynamic Rhythmic Modulation**

- **Patch:**  
  Use a spare LFO, envelope, or random CV source (e.g., Mutable Instruments Peaks, Make Noise Function) patched into the **Steps CV** or **Length CV**.  
  This morphs the density and length of rhythmic triggers in real time—ideal for evolving IDM or live techno.
- **Layer:**  
  Split the Euclid output with a mult. One output triggers drums, the other modulates a VCA or effects processor (e.g., Clouds), synchronizing filtering, effects, or amplitude changes with the rhythm.

---

## 4. **Synth Line Gating / Rhythmic Stabs**

- **Patch:**  
  Use **Euclid OUT** to trigger an envelope generator (e.g., Intellijel ADSR, Mutable Instruments Tides in trigger mode). Then use this envelope to modulate the amplitude or filter of a synth voice, creating percussive or chopped synth lines matching the Euclidean rhythm.

---

## 5. **Algorithmic Melodic Generation**

- **Patch:**  
  Send **Euclid OUT** to the clock/reset input of a sequencer (e.g., Make Noise René, Intellijel Metropolis, Arturia Keystep Pro) for irregular phrase advancement, yielding unique melodic patterns.
- **Variant:**  
  Combine with quantizers or logic modules (e.g., Doepfer A-166, Mutable Instruments Branches) to make generative or probability-based melodic structures.

---

## 6. **Gestural Control & Live Performance**

- **Setup:**  
  Map faders, joysticks, or touch controllers (e.g., Intellijel Tetrapad, Soundmachines LP1, Doepfer A-174-1) to the **Length**, **Steps**, or **Offset** CV.  
  This allows dramatic live manipulation of patterns—morph between minimal, dense, short, or offset rhythms on the fly.

---

## 7. **Advanced Clock Manipulation**

- **Patch:**  
  Use a clock divider/multiplier (e.g., 4ms RCD/SCM, Doepfer A-160/A-161) before the **Trig In** for shifting time bases. Create evolving nested patterns by combining with clock logic or combined clock sources.
- **Bonus:**  
  Run a synchronized reset pulse from your master clock/reset to **Reset In** for repeatable yet complex rhythmic structures—great for live performance or DAW sync.

---

## 8. **Triggering Effects in Sync**

- **Patch:**  
  Send **Euclid OUT** to trigger an audio or CV effect, like a voltage-controlled reverb freeze (e.g., Mutable Instruments Clouds), distortion (Doepfer A-137), granular FX, or rhythmic sample slicing.

---

## 9. **Intermodulation With Other Generative Modules**

- **Setup:**  
  Use Euclid in tandem with modules like Mutable Instruments Marbles, Ornament & Crime (Hemicube, Acid Curds, etc.), or Turing Machine for cross-patching generative rhythms and melodies.
- **Example:**  
  Use Marbles’ random clock or bias outputs to modulate Euclid’s parameters for complex, self-evolving systems.

---

## Module Type Recommendations

- **Drum/Voice Modules:** Mutable Instruments Plaits, Noise Engineering BIA, TipTop 808/909 modules, Erica Synths Pico Drum.
- **CV/Motion Sources:** Maths, Function, Peaks, Zadar, Batumi.
- **Sequencers:** René, Metropolis, Keystep Pro, SQ-1.
- **Logic/Utility:** Doepfer A-166, Mutable Instruments Branches, Intellijel Plog, XOR, AND logic modules.
- **Clock/Divider:** Pamela’s (New) Workout, 4ms RCD/SCM, Doepfer A-160.
- **Performance:** Tetrapad, Planar2, Sensel Morph, LP1.
- **Effects:** Clouds, Beads, Milky Way, FX Aid, Pico DSP.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)