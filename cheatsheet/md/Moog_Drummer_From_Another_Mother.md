# Moog — Drummer From Another Mother

- [Manual PDF](../../manuals/DFAM_Manual.pdf)

---

[Download the Moog DFAM Manual PDF](https://www.moogmusic.com/sites/default/files/2018-03/DFAM_Manual_0.pdf)

---

# Moog DFAM (Drummer From Another Mother) Eurorack Cheat Sheet

### Eurorack Specs
- **Width:** 60HP  
- **Max Depth:** 26mm  
- **Power Draw:** +12V (230mA max), -12V (Not used)  
- **Ribbon:** 10-pin  
- **All signals: ±5V (10Vpp) Eurorack compatible**

---

## Quickstart

- **Power On:** No power switch; powered when adapter is connected or installed in rack.
- **Warm-up:** Allow a few minutes after power-on for oscillator/frequency stability.

---

## Controls Overview

### Knobs
- **VCO 1 Frequency, VCO 2 Frequency:** Set pitch of both oscillators
- **VCO 1/2 EG Amount:** Bipolar, amount of envelope to VCO pitch (-/center/+)
- **VCO Decay:** Envelope decay for VCO mod.
- **VCO 1/2 Level:** Mixer volume for each oscillator
- **Noise/Ext Level:** Level for noise generator or external input
- **Filter Cutoff:** Master cutoff frequency for filter
- **Resonance:** Filter resonance; self-oscillation in LP
- **VCF EG Amount:** Bipolar, amount of envelope to cutoff
- **VCF Decay:** Envelope decay for filter
- **Noise/VCF Mod:** Amount of noise (or CV) modulating filter cutoff
- **VCA Decay:** Overall output envelope decay
- **Mixer Volume:** Output gain

- **8x Pitch Knobs:** Step pitches for sequencer
- **8x Velocity Knobs:** Step velocity for sequencer

- **Sequencer Tempo:** Global tempo

---

### Switches/Toggles
- **VCO 1 Wave, VCO 2 Wave:** Triangle / Square 
- **Hard Sync:** Off/On (Osc 2 phase resets to Osc 1)
- **Seq Pitch Mod:** [VCO 1&2 / Off / VCO 2]
- **Filter Mode:** [Low Pass / High Pass]
- **VCA EG:** [Fast/Slow] (Envelope attack speed)

---

### Buttons
- **Run/Stop:** Start/stop sequencer
- **Advance:** Manually advance sequencer (step)
- **Trigger:** Trigger selected step (no advance)

---

## Patchbay Reference

> **All jacks: 3.5mm.  Inputs: 0–+5V or ±5V, Outputs: ±5V (unless noted).**  
> _(Eurorack ±5V = 10Vpp modular standard)_

### Inputs

| Jack Name         | Description                                  | Voltage Range        |
|-------------------|----------------------------------------------|----------------------|
| **TRIGGER**       | Fires ENV (all 3 EGs) @ selected velocity    | 0–+5V Pulse/Gate (+10V toler) |
| **VCA CV**        | Add'l CV for amp level (summed w/ EG)        | 0–+8V |
| **VELOCITY**      | Step ENV max amp                             | 0–+5V                |
| **VCA DECAY**     | Controls VCA envelope decay                  | -5V to +5V           |
| **EXT AUDIO**     | Audio in (replaces noise in mixer)           | 10Vpp                |
| **VCF DECAY**     | Controls VCF envelope decay                  | -5V to +5V           |
| **NOISE LEVEL**   | CV for noise/external audio level            | 0–+8V                |
| **VCO DECAY**     | Controls VCO EG decay                        | -5V to +5V           |
| **VCF MOD**       | CV for filter cutoff (replaces noise)        | -5V to +5V           |
| **VCO 1 CV**      | 1V/octave control for Oscillator 1           | -5V to +5V           |
| **1→2 FM AMT**    | Mod amount CV (linear FM, VCO1→VCO2)         | 0–+8V                |
| **VCO 2 CV**      | 1V/octave control for Oscillator 2           | -5V to +5V           |
| **TEMPO**         | 1V/oct (audio-rate possible)                 | -5V to +5V           |
| **RUN/STOP**      | Gate for sequencer (- off, + on)             | 0–+5V Gate (+10V tol)|
| **ADV/CLOCK**     | Clock / advance input (external clock)       | 0–+5V Clock (+10V tol)|

### Outputs

| Jack Name         | Description                                  | Voltage Range        |
|-------------------|----------------------------------------------|----------------------|
| **VCA**           | Main audio out (pre volume knob)             | -5V to +5V audio     |
| **VCA EG**        | ENV out for VCA                              | 0–+8V CV (unipolar)  |
| **VCF EG**        | ENV out for Filter                           | 0–+8V CV (unipolar)  |
| **VCO EG**        | ENV out for VCO pitch                        | 0–+8V CV (unipolar)  |
| **VCO 1**         | Raw signal out (wave chosen by switch)       | -5V to +5V           |
| **VCO 2**         | Raw signal out (wave chosen by switch)       | -5V to +5V           |
| **TRIGGER**       | Sequencer clock output                       | 0–+5V (1ms pulse)    |
| **VELOCITY**      | Step velocity CV out                         | 0–+5V                |
| **PITCH**         | Step pitch CV out                            | -5V to +5V           |

---

## Signal Path (Summary)

1. **VCO 1 & VCO 2**: Select tri/square waveform, tune frequency, hard sync, FM.
2. **Mixer**: Blend VCOs and/or Noise/External In.
3. **VCF**: HP/LP, cutoff, resonance, modulation (EG + Noise/CV).
4. **VCA**: EG-controlled amplitude, velocity and decay variation.
5. **Sequencer**: 8 steps, each with pitch & velocity; analog clock & patchable.

---

## Tips & Tricks

- All EG amount knobs are bipolar (negative at left, neutral at center, positive at right).
- Set pitch modulation with SEQ PITCH MOD toggle.
- Use the patchbay to sequence or modulate ANY parameter via CV.
- Noise/EXT Jack can be replaced with external audio (removes noise).
- Filter self-oscillates in low-pass mode with high resonance; can be used as an additional tone source.
- Perfect for cross-modulation (“FM Toys” patch: VCO2 FM’ing filter cutoff!).
- Both Osc1 and Osc2 pitch can be externally controlled (1V/oct).
- Sequencer can act as CV or trigger source for other gear via patch outputs.
- Designed to immediately fit 60HP Eurorack systems.
- All inputs/outputs Eurorack voltages.

---

## Troubleshooting

- **No Sound?**  
  - Check VCO FREQ, EG AMT, Filter cutoff/resonance, patch section for dead-end connections.
- **Levels too low?**  
  - EXT IN expects modular level (10Vpp). Amplify external line-level sources.

---

## Useful Links

- [Moog DFAM Official Manual PDF](https://www.moogmusic.com/sites/default/files/2018-03/DFAM_Manual_0.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)