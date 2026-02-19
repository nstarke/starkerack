# 2hp — Pluck

- [Manual PDF](../../manuals/2hp_Pluck.pdf)

---

[2hp Pluck Manual (PDF)](https://2hp.com/wp-content/uploads/2019/09/PluckManual.pdf)

---

## Using 2hp Pluck for Dense, Hyper-Complex Percussion Patterns

The **2hp Pluck** is a Karplus-Strong physical modeling voice module with four-voice polyphony, making it a powerful and flexible percussion source for dense, evolving rhythmic music—especially when combined with sophisticated modulation and sequencing. Here are some strategies and ideas to get the most out of Pluck in the context of polyrhythms, complex meters, and unique percussion:

---

### Core Techniques

#### 1. **Triggering Complex Rhythms**

- Use multiple trigger/gate sequencers or clock dividers/multipliers to feed the **TRIG** input with overlapping or non-aligned rhythm streams.
  - For polyrhythms, send triggers from different divisions (e.g., 3/4/5 over 4/4 grid).
  - Probability or pattern generators (e.g., Euclidean sequencers, Marbles, Zularic Repetitor) are particularly effective.
- With four-voice polyphony, closely spaced or overlapping triggers won't choke each other—notes will sustain and overlap, adding to density.

#### 2. **Voice Parameter Animation**

- **DAMP** and **DECAY** dramatically shape the percussive quality. Modulate these using fast or stepped CV patterns synced to your triggers.
  - Map DAMP to the output of a fast LFO, random voltage, or stepped sequencer for shifting timbres (from muted thuds to snappy, metallic blips).
  - Similarly, automate DECAY for evolving sustain and harmonic content.
- Use **CV modulation** (especially from sources like clocks, gates, or stepped random) for per-step variation, emulating a live drummer's dynamics.

#### 3. **Pitch as a Percussive Parameter**

- Don't just use pitch for melody—try sequencing pitch per hit, or use dramatic pitch sweeps for toms, claves, blips, or synthetic snare effects.
  - Play with microtonal intervals for intentionally "off-kilter" metallic percussion patterns.
- Animate the **Pitch Knob** with slow LFO or envelopes for evolving tone during note sustain.

#### 4. **Output Processing**

- **Patch the audio OUT to...**
  - Waveshapers, bitcrushers, or distortion for more grit.
  - High-pass, band-pass, or comb filters to accentuate attack and make the timbre even sharper & punchier.
- Use a **VCA with velocity/velocity emulation** by modulating amplitude per trigger for varied accents.

---

### Advanced Patch Concepts

#### **A. Polyrhythmic Triggering Example**

- Use a clock divider set to 7 and another to 5, feeding both into a trigger combiner (logic OR or diode mixer). Send the combined triggers to **TRIG** for dense, unpredictable patterns.
- Assign separate DAMP/DECAY CVs stepped from two sequencers running at different clock rates for ever-morphing percussive timbres.

#### **B. Percussive Melodic Sequence**

- Program a sequence where **Pitch CV** and **TRIG** are decoupled (e.g., random pitch per hit, but regular rhythmic triggers), to generate Gamelan or prepared-piano–like textures.
- Modulate DAMP or DECAY for variety between short, woodblock-like hits and long, metallic resonances—great for fills and transitions.

#### **C. Manual Performance/Glitching**

- Manually tweak the **DAMP** and **DECAY** knobs during sequence playback to create fills, mutes, or sudden tonal shifts.
- Use a pressure-sensitive controller or touch plate to control DAMP CV, enabling real-time expressive playing.

---

### Tips for Unique, Punchy Percussion

- **Short DAMP + Short DECAY + High Pitch = Clicky/Glitchy Drums**
- **Long DAMP + Short DECAY = Metal Plate/Clang**
- **Short DAMP + Long DECAY = Plastic/Muted Bass Drums**
- **Vary all three—trigger, CV, and manual—to keep drums unique on each hit instead of repetitive.**

---

### Integration

Pair Pluck with gate-delay or logic modules to create "flams," ratchets, or rolls, and with random CV for ever-changing drum 'kits' from a single module.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
