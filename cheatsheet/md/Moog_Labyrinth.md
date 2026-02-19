# Moog — Labyrinth

- [Manual PDF](../../manuals/Labyrinth Manual.pdf)

---

[Moog Labyrinth User’s Manual PDF](https://cdn.shopify.com/s/files/1/0274/7781/4651/files/Labyrinth_Manual_Web.pdf)

---

# Moog Labyrinth Eurorack Module Cheat Sheet

### OVERVIEW  
**Moog Labyrinth** is a semi-modular, parallel generative analog synthesizer with dual sequencers, two parallel audio paths (VC wavefolder & state-variable filter), individual VCAs, dual decay envelopes, extensive patching, and advanced generative sequencing features.

---

## Quickstart

1. **Power Up**: Plug in the +12 VDC power supply (draws ~290 mA in Eurorack), or use included wall adapter.
2. **Audio Out**: Patch the rear AUDIO OUT (1/4” TS) to a mixer or active speaker. Use the VOLUME knob to adjust.
3. **Warm Up**: Allow a few minutes for analog tuning stability.
4. **Initialize**: Hold `BUFFER + RESET` for 1 sec to clear sequencers.
5. **Sequencer**: Enable steps with `BIT FLIP`. Use `RUN/STOP` to start and hear sound. Adjust pattern using LENGTH, BIT SHIFT, CV RANGE, and CORRUPT knobs.
6. **Sound Shaping**: Wavefolder (VCW) and filter (VCF) paths are mixed/crossfaded via BLEND.  
Set ORDER:  
- PARALLEL: VCW and VCF run side by side
- VCW>VCF: VCW feeds into VCF  
- VCF>VCW: VCF feeds into VCW

---

## Controls Summary

### Oscillators

| Knob/Button        | Function                                                                                |
|--------------------|----------------------------------------------------------------------------------------|
| VCO FREQUENCY      | Main sine VCO pitch (~20 Hz - ~5 kHz)                                                  |
| VCO EG1 AMT        | Bipolar env (EG1) to VCO pitch                                                         |
| VCO SEQ1 AMT       | SEQ1 amount (set to QTZ for quantized)                                                 |
| MOD VCO FREQUENCY  | Mod/triangle VCO pitch (LFO–~1.3kHz, below audio range = LFO/Drums)                    |
| MOD VCO EG1 AMT    | Bipolar env (EG1) to MOD VCO                                                           |
| MOD VCO SEQ2 AMT   | SEQ2 amount (set to QTZ for quantized)                                                 |
| MOD VCO FM AMT     | Amount of FM from MOD VCO to VCO (thru-zero for proper tuning)                         |

### Mixer Section

| Knob      | Function                                        |
|-----------|-------------------------------------------------|
| VCO LVL   | Sine VCO level (+ overdrives past 12:00)        |
| RING MOD LVL | Ring mod level (adds metallic tones)         |
| MOD VCO LVL | MOD VCO level                                 |
| NOISE LVL | Noise level                                     |
| NOISE TONE| Noise HF/LF tilt                                |

### Wavefolder (VCW) Section

| Knob      | Function                                                    |
|-----------|-------------------------------------------------------------|
| VCW FOLD  | Depth of wavefolding (clean left, max right)                |
| VCW EG1/CV AMT | Bipolar env or CV to VCW FOLD (patch breaks EG1 norm)  |
| VCW SEQ1 AMT   | SEQ1 amount to VCW FOLD                                |
| VCW BIAS       | DC bias (for asymm. folding)                           |

### Filter (VCF) Section

| Knob      | Function                                         |
|-----------|--------------------------------------------------|
| VCF CUTOFF| Filter cutoff frequency (~20 Hz - 20 kHz)        |
| VCF EG1/CV AMT | Bipolar env or CV to cutoff (patch breaks)  |
| VCF SEQ2 AMT   | SEQ2 amount to VCF cutoff                   |
| RESONANCE | Adds peak at cutoff (no bass loss)               |
| FILTER MODE | LP↔BP crossfade left→right                     |

### Blending/VCAs

| Control   | Function                                                               |
|-----------|------------------------------------------------------------------------|
| BLEND     | Crossfades VCW ↔ VCF paths                                             |
| VOLUME    | Final output and VCA out patch bay level                               |
| ORDER     | Routing: PARALLEL/VCW-VCF/VCF-VCW                                      |
| U MIX 1 LVL| Level for utility submixer 1 (normalled to ringmod, patch breaks)     |

### Envelopes

| Knob/Button   | Function                                                     |
|---------------|--------------------------------------------------------------|
| EG1 DECAY     | Percussive envelope 1 decay (mod, VCO, VCF, VCW)             |
| EG2 DECAY     | Envelope 2 decay (controls both built-in VCAs by default)     |
| EG TRIG MIX   | Trig blend between SEQ1 and SEQ2 triggers to envs             |
| TRIGGER (btn) | Manually triggers both EG1 and EG2                            |

### Sequencer (per SEQ1, SEQ2)

| Knob/Button   | Function                                                              |
|---------------|-----------------------------------------------------------------------|
| RUN/STOP      | Start/stop sequencer                                                  |
| BUFFER        | Save buffer state (hold 1s for save, short press to reload)           |
| CHAIN SEQ     | Chain SEQ1 & SEQ2 for 16-step sequence                               |
| ADVANCE       | Move play/write heads ahead one bit                                   |
| LENGTH        | Sequence step length (1–8, cycles)                                    |
| BIT SHIFT     | Rotates active bits                                                   |
| BIT FLIP      | Flips current write head's bit on/off (generates random voltage)      |
| CORRUPT       | Probabilistic mutation of step voltages/bits                          |
| CV RANGE      | Attenuates voltage span of sequence (-5V...+5V in, scales down)       |
| RESET         | Resets play head to step 1                                            |
| Various combos| Quantizer, shift offsets, special ops (see Button Combos ref)         |

**Sequencer Button Combos:**  
See p.37 for list—hold/combine BIT SHIFT, ADVANCE, etc. to offset, reset, select quantizer, etc.

---

## Patch Bay Reference

**32 x 3.5mm Jacks (20 IN, 12 OUT), all Eurorack compatible**

### Inputs (White text, Black Body)
| Jack                | Function                                             | Voltage Range    |
|---------------------|-----------------------------------------------------|------------------|
| VCO 1V/OCT          | VCO pitch control (sum with panel)                  | -5V to +5V       |
| M VCO 1V/OCT        | MOD VCO pitch control (sum)                         | -5V to +5V       |
| M VCO SYNC          | Resets triangle MOD VCO                             | 0V to +5V        |
| BLEND               | Crossfader VC for BLEND                             | -5V to +5V       |
| VCW IN              | Audio in to wavefolder                              | -5V to +5V       |
| FOLD                | CV in for fold depth                                | -5V to +5V       |
| VCW VCA CV          | VCA level for VCW side                              | 0V to +8V        |
| VCF IN              | Audio in to VCF                                     | -5V to +5V       |
| CUTOFF              | VCF cutoff CV (sum)                                 | -5V to +5V       |
| VCF VCA CV          | VCA level for VCF side                              | 0V to +8V        |
| U MIX 1 (RING)      | Utility mixer 1 input (default: ring mod)           | -5V to +5V       |
| U MIX 2             | Utility mixer 2 input                               | -5V to +5V       |
| EG2 TRIG            | Triggers EG2 envelope (rising edge)                 | 0V to +10V       |
| CLOCK 1             | Ext clock SEQ1 (or both if 2 is unpatched)          | 0V to +10V       |
| BIT FLIP 1          | Digital in, flips current write step for SEQ1       | 0V to +10V       |
| CLOCK 2             | Ext clock SEQ2 (norm: from 1)                       | 0V to +10V       |
| BIT FLIP 2          | Digital in, flips current write step for SEQ2       | 0V to +10V       |
| MIDI                | 3.5mm MIDI In (Clock, Note On, Start/Stop/Continue) | MIDI signals      |
| TRIGGER             | Triggers both EGs (rising edge), unless EG2 patched | 0V to +10V       |
| RESET               | Resets sequencer play head to step 1                | 0V to +10V       |

### Outputs (Black text, White Body)
| Jack                | Function                                | Voltage Range   |
|---------------------|-----------------------------------------|-----------------|
| VCA                 | Mono main output (Eurorack level)       | -5V to +5V (10Vpp)|
| M VCO               | MOD VCO triangle out                    | -5V to +5V      |
| NOISE               | Noise generator out                      | -5V to +5V      |
| MIXER               | Mixer output (raw: VCO, MOD VCO, etc.)   | -5V to +5V      |
| EG1                 | Envelope 1 out                          | 0V to +8V       |
| EG2                 | Envelope 2 out                          | 0V to +8V       |
| U MIX 1+2           | Utility mixer summed output              | -5V to +5V      |
| SEQ1 CV             | Sequencer 1 CV (attenuated, quantized)   | -5V to +5V      |
| SEQ1 TRIG           | Sequencer 1 trigger out (step is on)     | 0V to +5V       |
| SEQ2 CV             | Sequencer 2 CV (attenuated, quantized)   | -5V to +5V      |
| SEQ2 TRIG           | Sequencer 2 trigger out                  | 0V to +5V       |
| CLOCK               | Labyrinth clock out/MIDI clock out       | 0V to +5V       |

---

## Quantizer Modes

- 15 built-in scales, plus unquantized (see manual p. 38 for mappings).
- Select quantization mode by `BIT SHIFT` + `BIT FLIP` (SEQ1) while running.

---

## Reference: Voltages & Ranges

- Most CV/audio: **-5V to +5V** (Eurorack norm)
- Envelope outs: **0V to +8V**
- Triggers/gates: **0V to +5V** (5V logic)
- VCA CV inputs: **0V–+8V**
- Clock/Trig in: works with **0V–+5/10V**
- Main output: **-5V to +5V (10Vpp)** for modular, [1/4” rear audio out] for line level

---

## Pro Tips

- Each path (VCW/VCF) has its own VCA (EG2 by default).
- Use PATCH BAY to break normals and customize routing.
- The sequencer is truly generative; use CORRUPT and BUFFER for evolving/locking patterns.
- U MIX allows you to submix and process external signals.
- BLEND can be CV modulated—try crossfading via envelope or sequencer.
- All parameters bolded in the manual correspond to actual knobs, sliders, buttons, or toggles.

---

## Links

- Full [Moog Labyrinth User’s Manual PDF](https://cdn.shopify.com/s/files/1/0274/7781/4651/files/Labyrinth_Manual_Web.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---