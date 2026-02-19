# Doepfer — A-130-1

- [Manual PDF](../../manuals/A1301_man.pdf)

---

[**Doepfer A-130/A-131 VCA Manual (PDF)**](https://doepfer.de/a100man/A130_A131_man.pdf)

---

# Doepfer A-130 / A-131 VCA — Cheat Sheet

## Overview
- **A-130:** Linear voltage-controlled amplifier (VCA), best for control voltages.
- **A-131:** Exponential VCA, best for audio signals.
- Both modules are otherwise functionally identical (jacks and knobs).

## Controls

| Label  | Function                                               | Range     |
|--------|--------------------------------------------------------|-----------|
| Gain   | Overall gain (offset) control                          | 0–10      |
| CV2    | Attenuator for CV 2 (modulates amount of CV2 applied)  | 0–10      |
| In 1   | Attenuator for Audio In 1                              | 0–10      |
| In 2   | Attenuator for Audio In 2                              | 0–10      |
| Out    | Attenuator for output signal (audio level out)         | 0–10      |

---

## Inputs & Outputs

| Jack         | Function                     | Voltage Range     |
|--------------|-----------------------------|-------------------|
| CV1          | Control Voltage In 1         | 0–+5 V (lin/exp)* |
| CV2          | Control Voltage In 2         | 0–+5 V (lin/exp)* |
| Audio In 1   | Audio Input 1                | Typical line lvl  |
| Audio In 2   | Audio Input 2                | Typical line lvl  |
| Audio Out    | Audio Output                 | +/-5 V (typical)  |

- *CV1 and CV2 are summed; +5 V = max amplification, 0 V = closed. CV2 has an attenuator, CV1 does not.*

---

## Response Curves

- **A-130:** Linear response (best for control voltages).
- **A-131:** Exponential/logarithmic response (best for audio for natural loudness perception).

---

## Usage Tips

- **For audio signals**: Use exponential mode (A-131).
- **For CV/modulation**: Use linear mode (A-130).
- **Gain Control**: At 0, no signal passes (unless CV present). Increase for baseline amplification or when using bipolar CV sources.
- **CV Inputs**: Bring envelope generators or LFOs to CV1/CV2. For maximum VCA response use up to +5 V.
- **Distortion**: If output distorts, lower In 1/In 2 attenuators.
- **Output Level**: Adjust Out attenuator to set final module volume.

---

## Patch Examples

- **ADSR to VCA:** Envelope shapes volume/dynamics of sound source.
- **LFO to VCA:** Amplitude modulation for tremolo or AM effects.
- **Keyboard CV to VCA:** Keyboard tracking for dynamic response based on pitch.
- **Inverse Tracking:** Use a voltage inverter before the CV input.

---

## Patch Sheet Tip

- Use the front panel diagrams to log your settings and favorite patches with marker.

---

**Manual Reference:** [Doepfer A-130/A-131 VCA Manual (PDF)](https://doepfer.de/a100man/A130_A131_man.pdf)  
**Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)**