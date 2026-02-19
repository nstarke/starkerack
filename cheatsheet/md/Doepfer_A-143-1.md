# Doepfer — A-143-1

- [Manual PDF](../../manuals/A1431_man.pdf)

---

[Doepfer A-143-1 Manual PDF (Doepfer Website)](https://doepfer.de/A1431_tec_eg.pdf)

---

# Doepfer A-143-1 Quad AD/LFO Quick Reference Cheat Sheet

## SUMMARY

**The A-143-1 is a quad Attack/Decay envelope/LFO module**  
Each generator can operate as a triggered AD envelope or a free-running exponential LFO. All controls and jacks are repeated for each of the 4 channels.  
Generators can be linked (daisy-chained) internally for complex multi-stage envelopes or LFOs.

### Basic Operation Modes:
- **AD:** Functions as a standard envelope (fires on trigger input)
- **LFO:** Functions as a free-running exponential LFO (use dummy cable in Trig. In to prevent retriggering from previous channel)

---

## FRONT PANEL CONTROLS & INDICATORS

| Control/Jack    | Type         | Description                                          | Voltage Range             |
|-----------------|--------------|------------------------------------------------------|---------------------------|
| 1. AD/LFO Switch | Toggle       | AD = Envelope, LFO = Free-running LFO                | -                         |
| 2. Attack        | Knob         | Controls attack (rise) time                          | -                         |
| 3. Decay         | Knob         | Controls decay (fall) time                           | -                         |
| 4. Mix Polarizer | Knob         | Level/polarity of channel in mix output (center = 0; left = negative; right = positive add) | -                         |
| 5. Threshold     | Knob         | Sets level for comparator output “Cp Out”            | -                         |
| 6. Env LED       | LED          | Envelope activity visual indicator                   | -                         |
| 7. Cp Out LED    | LED          | Comparator state visual indicator                    | -                         |

---

## ALL INPUTS AND OUTPUTS SUMMARY

| Jack              | Type       | Description                                                                                   | Voltage Range             |
|-------------------|------------|----------------------------------------------------------------------------------------------|---------------------------|
| ! Trig. In        | Input       | Gate/trigger starts envelope or retriggers LFO. Internally normalled in a 4-stage chain.     | Gate: >2.5V for trigger   |
| " EOA (EndOfAttack)| Output      | Goes **high** at end of attack stage, **low** during attack. Can be used to trigger others.  | Digital logic (0V/8V)     |
| § Env x           | Output      | Envelope/LFO output                                                                          | 0...+8V (AD); +0.5...+8V (LFO) |
| $ Cp x (Comp Out) | Output      | Comparator. **Low** when envelope exceeds threshold; **high** otherwise.                     | Digital logic (0V/8V)     |
| % Mix Out         | Output      | Mixer sum (sum of all envelopes/LFOs, level and inversion set by polarizers).                | Sum of 4 envs, up to ±32V?*     |

> *Maximum summed voltage at Mix Out depends on how channels are set and mixed.

### INTERNAL SIGNAL FLOW

- Trig. In is normalled to the previous channel's Cp Out (default chaining: #1↔#4, #2↔#1, #3↔#2, #4↔#3)
- Envelope Out is pre-polarizer by factory default (can be configured internally to post-polarizer)
- Mix Out sums polarizer-processed envelope outputs from all channels

---

## TIPS & PATCH IDEAS

- **4 Independent AD Envelopes:** Set all switches to AD, patch triggers to Trig. In as required, take outputs from § Env x.
- **Complex Multi-Stage Envelope:** Leave Trig. In #1 open, set all to AD, send trigger to input 1; others are chained for 4-stage envelope.
- **Free-running Multi-stage LFO:** Switch to LFO mode, insert dummy jacks if you don’t want internal retrigger, patch from Mix Out or § Env x.
- **Creative Modulation:** Use Envelope Outs or Mix Out to modulate VCOs, filters, VCAs, etc.
- **Comparator/EOA Outputs:** Use EOA or Cp Outs as logic triggers for sequencing or rhythmical effects.
- **Mix Polarizer:** Invert selected envelopes in the mix for complex waveforms or movement.

---

## VOLTAGE RANGES

- Envelope output:  
  - AD: **0...+8V**  
  - LFO: **+0.5...+8V**
- Cp Out, EOA Out: **0V (low) or +8V (high)**
- Input Trig. In: (Gate/trigger): **>2.5V** threshold typical

---

## MECHANICAL/POWER

- Width: **28 HP / 141.9 mm**
- Depth: **Approx 65 mm**
- Power: **70 mA**

---

More details in the [Official Manual PDF (Doepfer)](https://doepfer.de/A1431_tec_eg.pdf)  
Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)