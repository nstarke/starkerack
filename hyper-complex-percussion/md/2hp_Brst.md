# 2hp — Brst

- [Manual PDF](../../manuals/Brst_Manual.pdf)

---

[Brst Manual PDF](https://2hp.com/wp-content/uploads/Brst.pdf)

---

## Using the 2hp Brst for Complex Rhythmic Percussion & Polyrhythms

The 2hp Brst is not a sound source or effect itself—it's a **voltage controlled burst generator and trigger delay**. Its power lies in creating trigger streams in rapid, customizable, and controlled bursts, making it an exceptional utility for **advanced rhythmic creation**. Here's how you can leverage it to construct hyper complex percussion and polyrhythms:

---

### Core Techniques for Dense Rhythmic Patterns

#### 1. **Polyrhythmic Trigger Layers**
- **Patch** one or more Brst units to drum or percussive modules' trigger inputs (e.g. kick, snare, hats, metallic noise, etc.).
- Use **different PULSES and RATE settings** per Brst, so that each drum voice gets a different burst rhythm. This naturally generates superimposed, interlocking rhythms (polyrhythms), especially when you send them triggers divided or multiplied from your main clock.

#### 2. **Complex Time Signatures & Ratcheting**
- Use an external sequencer or clock divider as the source for TRIG input.
- Manipulate the **PULSES knob/CV** for odd numbers (e.g. 5, 7, 11) to inject bursts corresponding to tuplets and unusual subdivisions.
- Vary the **RATE knob/CV**, especially using CV modulation via step sequencers or random sources, so each burst can have evolving speed and feel (ratcheting).

#### 3. **Hyper-Percussive Pattern Generation**
- Combine Brst bursts with other rhythmic modules (Euclidean sequencers, logic modules, clocked LFOs).
- Use **envelope followers or random stepped voltages** patched to RATE CV or PULSES CV for organic, shifting percussive patterns.
- Stack Brst outputs via logic OR combiners to make composite triggers for layered sounds.

---

### Advanced Usage: Manipulation & Sonic Tips

#### **Uniqueness & Punch**
- Since Brst only creates triggers, combine with envelopes and **VCAs** to sculpt the attack and decay of percussive sources for extra punch.
- Alternate PULSES and RATE ranges between very short bursts (staccato blips) and slower flurries for rhythmic contrast and dynamic buildup.
- Use the TRIG TOGGLE creatively:
  - Include the initial trigger for tight "ratchet-like" sounds.
  - Omit to shift the burst onset for syncopated, more humanizing feel.

#### **Humanizing Rhythms**
- Slightly modulate the RATE CV input with slow LFOs or sample & hold modules to add micro-timing fluctuations.
- Use attenuated random sources (e.g. Wogglebug, Turing Machine) for "groove" or swing in trigger timing, making machine rhythms feel more "played."

#### **Percussion Not Possible with a Plain Clock**
- Brst excels at molding generic clock triggers into rolling bursts—perfect for simulating realistic drum rudiments (rolls, flams, ghost notes) with only simple trigger outputs.
- Insert Brst into hi-hat or snare lines to add "machine gun" effects or detailed ghost note patterns impossible by hand or with plain clocking.

---

#### **Chaining & Layering**
- Chain two Brst modules: feed output of one into the TRIG input of another for **nested bursts** and even more complex cascades.
- Interleave Brst outputs with probabilistic gates (Mutable Branches, Doepfer A-150, etc.) to enhance randomness and variation.

---

## Example Patch

> **Goal:** IDM/Glitch Drums With Dense Polyrhythms  
> - Clock source → Brst TRIG  
> - Brst OUT → Snare drum's trigger  
> - Modulate Brst's PULSES CV with stepped random  
> - Modulate Brst's RATE CV with clock-synced LFO  
> - Main clock / 2 → Hi-hat  
> - Second Brst with different settings for rimshot/woodblock  
> Result: Polyrhythms and glitchy rolls interplay with regular patterns.

---

#### **Further Expansion**

- Mult Brst OUT to trigger multiple percussion modules at once for dense, coordinated bursts.
- Sequence RATE and PULSES CVs for evolving, morphing percussive textures through a performance.

---

> [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)