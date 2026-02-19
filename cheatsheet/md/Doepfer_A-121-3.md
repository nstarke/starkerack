# Doepfer — A-121-3

- [Manual PDF](../../manuals/A-121-3 12dB Multimode Filter (slim version).pdf)

---

[Doepfer A-121-3 12dB Multimode Filter Slim Line Series Manual](https://doepfer.de/a1213.htm)

---

# Doepfer A-121-3 Cheat Sheet

**Type:** Voltage-controlled multi-mode filter  
**HP:** 4  
**Depth:** 50mm  
**Current Draw:** +40mA (+12V) / -30mA (-12V)  
**Price:** ~€110  
**Cutoff Slope:** -12dB/octave  
**Freq. Range:** ~10Hz–20kHz  
**Features:** Simultaneous LP, HP, BP, Notch outputs

---

## Inputs, Outputs, & Controls

### Inputs

| Jack    | Function                                  | Voltage Range / Notes                    |
|---------|-------------------------------------------|------------------------------------------|
| **In**  | Audio signal input                        | Adjustable with **Level** knob           |
| **CV1** | Filter cutoff control (1V/Oct)            | ~0–8V, no attenuator                     |
| **CV2** | Filter cutoff modulation                  | ~0–8V, has dedicated attenuator (**FCV2**)|
| **CQ**  | Resonance (Q) control voltage             | 0–8V, no attenuator                      |

### Outputs

| Jack    | Output Type                               | Notes                                   |
|---------|-------------------------------------------|------------------------------------------|
| **LP**  | Low-pass filtered output                  |                                          |
| **HP**  | High-pass filtered output                 |                                          |
| **BP**  | Band-pass filtered output                 |                                          |
| **N**   | Notch/Bandsperre filtered output          |                                          |

### Knobs / Controls

| Label     | Function                                | Notes                                   |
|-----------|-----------------------------------------|------------------------------------------|
| **Frequ.**  | Manual cutoff frequency                | Sweeps filter freq. from 10Hz–20kHz      |
| **Q**       | Resonance (manual)                     | Full CW will self-oscillate (sine out)   |
| **FCV2**    | CV2 attenuator (modulation depth)      | Ranges from 0 to full incoming voltage   |
| **Level**   | Audio input gain/attenuator            | Start seeing distortion/clipping >5      |

---

## Quick Reference

- Use **In** for your audio source & adjust **Level** for input gain (beware distortion beyond position 5).
- **Frequ.** sets the base cutoff frequency; **CV1** (1V/oct) and **CV2** (variable depth via **FCV2**) control cutoff via CV.
- Patch an envelope, sequencer, or LFO to **CV1**/**CV2** for animation.
- Patch a CV source to **CQ** for voltage control over resonance (**no attenuator** here).
- **Q** knob manually sets resonance—self-oscillation possible when fully clockwise.
- Simultaneous outputs: LP (Low-pass), HP (High-pass), BP (Band-pass), N (Notch).
- Perfect for compact cases (4HP), similar in sound/function to A-121-2 but smaller (no CQ attenuator).

---

## Voltage Ranges

- **Cutoff frequency CVs (CV1, CV2):** expect standard modular levels (usually 0–8V), 1V/Oct on CV1.
- **Resonance CV (CQ):** 0–8V recommended.
- **Output audio:** Standard modular levels (typically ±5V peak-to-peak).
- **Input audio:** Standard modular levels (adjust with **Level**).

---

### [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)