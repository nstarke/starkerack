# Intellijel — Atlantix

- [Manual PDF](../../manuals/atlantix_manual_2024.09.12.pdf)

---

[Atlantix Manual PDF](https://intellijel.com/downloads/manuals/Atlantix_Manual.pdf)

---

# Atlantix: Techniques for Generating Hyper-Complex Percussion and Dense Rhythmic Patterns

## Introduction

The **Atlantix** is an analog dual-oscillator synthesizer voice with extensive internal and external patching, making it a fantastic building block for advanced, rhythmically-percussive music in Eurorack systems. Here are strategies focused on rhythmic density, polyrhythms, and punchy percussive textures—both within the Atlantix and by integrating it with the rest of your modular setup.

---

## 1. **Leverage the Internally-Patched Voice Architecture**

### **Fast Envelope Modulation for Maximum Punch**

- Set the **ENVELOPE RATE** switch `[5.5]` to **FAST** for snappy attacks.
- Use short Attack and Decay on the envelope and set Sustain very low or zero, treating Atlantix as a percussive voice (think kick, snare, click, tom).  
- If using Gate Mode (`[5.6]`), the VCA acts like a digital/organ-style clicker, perfect for hats, claps, and blips.

### **Layering and Stacking Percussive Tones**

- Patch **AUX 1/2** inputs with internal or external modulation. Route VCOs, envelopes, or even noise into these and use their routing switches to stack sounds pre- or post-filter for hybrid percussive textures.
- Leverage the **SUB oscillator**: set it to -1 or -2 octaves for heavy, punchy bass drums, or logical OR for unique pulse shapes.

---

## 2. **Exploit Waveform Mixing & Phase Relationships**

### **Pulse Position Modulation**

- Switch `[1.9]` between **Center** and **Edge** trigger for subtle but essential attack-phase differences. Center can sound rounder and more stable, edge can sound sharper, punchier, and more sync-friendly.

### **Noise Types and Percussive Noise Hits**

- Use the **NOISE TYPE** switch `[3.8]` to select **white** for aggressive hats/claps/snaps, or **pink** for deeper, woody or tom-like percussion.
- Inject noise both into the **mixer** and as modulation for dynamic, constantly shifting timbres.

---

## 3. **Samplers, Modulation, & S&H for Algorithmic/Rhythmic Disruption**

### **Sample & Hold for Algorithmic Rhythms**

- Use **S&H/T&H** circuit as a stepping source: feed in clocked triggers or complex clocks for HOLD, random/sample-varying signals for Samp (default is white noise).
- Patch MOD X/Y outs (with S&H) to control FM, filter, or VCA, creating mixing and probability/randomness in rhythmic sequences.

### **LFO as Clock Divider/Pattern Generator**

- Set **VCO B** `[2.4]` into **LFO** mode; outputs at different phases (square, tri, saw) can become rhythmic CVs for pulse width, FM, filter, or mixer mod inputs—especially at non-integer, unsynced rates for polyrhythm.

### **Complex Time & Polyrhythm: Sync and Modulation**

- VCO B can sync (hard/soft) to polyrhythmic clocks, then modulate VCO A’s pitch, FM, PWM, or cutoff to create shifting rhythms or microtiming.
- Use the **MOD source selectors** `[6.1]/[6.5]` to select appropriate waveforms for rhythmic modulation, e.g., S&H for unpredictable fills, or triangle/square for regular clocking.

---

## 4. **Self-Patching for Evolving Polyrhythms**

- **Patch ENVELOPE OUT** `[5.D]` into VCO A FM or PWM for dynamic pitch or timbre modulation—each hit changes the drum’s "tone."
- **Patch MOD X** to VCA CV input for amplitude modulation—enables complex stutter, mute, or envelope bursts.
- **Feed GATE or external clock patterns** into S&H hold input. With external clock dividers/multipliers, this gives you changing percussive shapes at non-standard subdivisions.

---

## 5. **Tone Shaping & Uniqueness**

### **Ring Modulation via ATLX Expander**

- Feed VCO A and B to the expander’s ring mod for metallic, clangorous percussion—classic for bells, digital-sounding hats, or FM toms.

### **Filter Modes for Drum Character**

- Rapidly switch between **LP**/**BP**/**HP** in performance or with CV for live-evolving drum timbres (snare to tom to shaker).
- The **PHZ (phaser)** mode can create zappy, FM-like percussion—especially when modulated/struck by S&H or rapidly moving LFO.

### **Drive Circuits**

- **VCA DRIVE** (`[5.7]`): Use “SYM” for hard, even clipping (techno drums), and “ASYM” for saturated, broken-up artifacts (lo-fi/IDM percussives).  
- Combine envelope pings with maximum DRIVE for "snapping" attacks.

---

## 6. **Integration With External Rhythm Utilities**

- **Clock or pattern generators** (Pamela’s New Workout, Grids, etc.) can drive Atlantix’s gate, retrigger, and S&H HOLD inputs directly. Feed complex/triplet/quintuplet clocks into different points for phase-shifting rhythmic relations.
- **External sequencers** can provide evolving, polymetric CV for oscillator pitch, PWM, INDEX, or filter FM for drum voices that drift and morph with your sequencer’s time base.

---

## Example Hypercomplex Patch Flow

1. **VCO A** in mid/high register (for rimshot/snare), set pitch CV from a stepped random S&H out.
2. **VCO B** in LFO or low audio, triangle out to MOD X, MOD X to VCA LEVEL input; MOD X set to triangle or to clocked S&H out for organic amplitude modulation.
3. **Envelope** in FAST, short A/D, GATE input clocked by complex, multi-divided clock pattern or trigger sequencer.
4. **NOISE** in mixer + route to filter. Filter in PHZ mode, ENV or MOD Y (sampled LFO) to cutoff, accenting the harmonic splash of percussive hits.
5. **Drive** ON for aggressive impact.
6. **Ring mod with Sub oscillator** (ATLX): out to aux percussion layer.

---

## Design Tips

- **Waterfall routing**: Internally, Atlantix normalizes many CV/audio connections, so you can create feedback, recursive, and branching patterns with minimal patching.
- **Performance**: Modulate the MOD X/Y source selectors and filter modes live to inject structure and progression into organic or algorithmic percussion tracks.
- **A/B Layering**: Use independent ENV, VCA, and filter sequences between main and aux mixer paths—one for punch, one for sizzle or hiss.

---

For the full manual (essential for detailed patch diagrams and parameter options):  
[Atlantix Manual PDF](https://intellijel.com/downloads/manuals/Atlantix_Manual.pdf)

---
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)