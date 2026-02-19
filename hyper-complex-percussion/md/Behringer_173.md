# Behringer — 173

- [Manual PDF](../../manuals/QSG_BE_0720-AAL_173 QUAD GATE-MULTIPLES_WW.pdf)

---

[Behringer 173 Quad Gate/Multiples Manual PDF (Quick Start Guide)](https://mediadl.musictribe.com/media/PLM/data/docs/P0DHV/173%20QUAD%20GATE_MULTIPLES_QSG_WW.pdf)

---

## Using the Behringer 173 Quad Gate/Multiples for Hyper-Complex Percussion in Eurorack

### Module Overview

The Behringer 173 Quad Gate/Multiples is not a sound-producing voice or effect in itself. Instead, it provides:

- **4 Gate circuits** (each with Gate In, Gate Out, Gate CV in)
- **6 sets of 4-way passive multiples** for distributing signals.

**Roles In Rhythm Generation:**
- **Gate processing**: Control the presence or shape of rhythm signals.
- **Multiples**: Distribute clocks, triggers, or CV/gates to multiple modules for tight, intricate synchronization.

This makes it a **utility module** ideal for routing, shaping, and complexifying trigger/gate signals—crucial for hyper-rhythmic and polyrhythmic patches.

---

### **Strategies for Hyper-Complex Percussion Patching**

#### 1. **Gate Shaping for Polyrhythms**

- **Multiple Gate Inputs**: Take several rhythmic triggers (from sequencers, clock dividers, Euclidean rhythm generators, etc.) and process them through the 173’s GATE sections.
- **Gate CV Input**: Patch another independent rhythm or random gate to the CV in—using active high (non-inverting) or active low (inverting). This allows one rhythm to modulate the output from another, effectively *multiplying* or *masking* polyrhythms, as one gate will only pass when the CV is high.

##### Example:
- **Trigger 1**: 5/8 rhythm pulse to GATE IN 1.
- **Trigger 2**: 4/4 clock, but running at 2x speed, to GATE CV 1.
- **Result**: You get a complex, composite rhythm at GATE OUT 1, combining both patterns with unusual overlaps.

#### 2. **Using Multiples for Complex Timing**

- **Flow Routing**: Use the multiples to split a master clock or trigger into several destinations.
- **Pattern Interleaving**: Stack several sources (e.g., clock divisions/multiplications) via multiples, then route these to various GATE INs and CVs. Each gate path can selectively shape when and how often a trigger passes, letting you layer odd and even time signatures together.

#### 3. **Percussive Variability via Gate Length Manipulation**

- Feed envelopes or variable-length triggers into GATE IN/CV, letting sustain/decay on the input affect how long the percussive voice is open.
- Use the inverting and non-inverting CV inputs to alternate between *open* and *muted* percussive “hits” depending on your signal polarity.

#### 4. **Mute/Slice/Cut Triggers On The Fly**

- Use manual or pattern-based gates to quickly silence or reactivate voice channels.
- Feed a hand-controlled or performance-based gate into CV—this allows you to bring layers in and out for dynamic live rhythms.

#### 5. **Unique Routing Exploits**

- **Stacking Gates**: Patch several rhythmically related gates together in a multiple, then use them to modulate different CV ins on the 173 gates.
- **Triggered Muting**: Create improvised breaks or fills by gating your main voices with a complex CV rhythm (from something like a Turing Machine, random looped sequence, etc.).

---

### **Example Patch for Hypercomplex Percussion**

1. **Sequencer A** (polyrhythmic odd time) → GATE IN 1
2. **Sequencer B** (straight 4/4, faster clock) → GATE CV 1 (non-inverting)
3. **GATE OUT 1 → Kick Drum Module**
4. **Euclidean Rhythm Generator (3 against 8)** → GATE IN 2
5. **Random Trigger Output (with swung rhythm)** → GATE CV 2 (inverting)
6. **GATE OUT 2 → Snare/Clap Module**
7. Use multiples to fan out main/fill/break rhythms to additional percussion voices (hi-hats, glitch percussion, etc.), modulating their “mutes” or “accents” by further complex gate patching.

---

### **Tips for Density and Punch**

- Chain the 173’s gates for sequential rhythmic gating—output of one gate into the next’s gate or CV input for chained logical rhythmic logic.
- Use sharp digital or analog envelopes to accentuate percussive attack, then gate those signals with the 173 for extra control.
- Experiment with cross-patching—gate A controls the length or presence of gate B, etc.
- Use the inverting CV option to subtract or “cut” holes in regular patterns, making for irregular and unpredictable grooves.

---

> For more creative patching tools, browse [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)  
