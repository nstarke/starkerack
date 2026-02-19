# 2hp — MMF

- [Manual PDF](../../manuals/2hp_MMF.pdf)

---

**[MMF Eurorack Filter Module Manual PDF](#)**
*(No actual link provided, please insert manual link if available)*

---

# MMF Eurorack Filter Cheat Sheet

**Overview:**  
The MMF is a compact (2HP) analog multimode filter module for Eurorack systems. It features simultaneous low pass, high pass, and band pass outputs, with voltage control over cutoff frequency and resonance.

---

## Panel Controls & Jacks

| Label   | Type     | Function/Description                                                  | Voltage Range (if applicable)      |
|---------|----------|-----------------------------------------------------------------------|------------------------------------|
| INPUT   | Jack     | Modular-level audio signal input                                      | N/A                                |
| FREQ    | Knob + Jack | Cutoff frequency control knob, with CV input jack below            | CV Input: -8V to +8V (added to knob)|
| RESO    | Knob + Jack | Resonance amount control knob, with CV input jack below            | CV Input: -5V to +5V (added to knob)|
| LP      | Jack     | 2-pole low pass filter output                                        | N/A                                |
| HP      | Jack     | 2-pole high pass filter output                                       | N/A                                |
| BP      | Jack     | 2-pole band pass filter output                                       | N/A                                |

*There are no buttons, sliders, or toggle switches on this module.*

---

## Inputs

- **Audio Input:** Accepts modular-level audio signals.
- **FREQ (CV):** Modulates filter cutoff, -8V to +8V range.
- **RESO (CV):** Modulates filter resonance, -5V to +5V range.

## Outputs

- **LP (Low Pass):** Filtered output, 2-pole, 12dB/oct slope.
- **HP (High Pass):** Filtered output, 2-pole, 12dB/oct slope.
- **BP (Band Pass):** Filtered output, 2-pole, 12dB/oct slope.

---

## Usage Tips

- Patch your audio signal to **INPUT**.
- Select either **LP**, **HP**, or **BP** output (or all simultaneously) based on desired filter type.
- Adjust **FREQ** knob for manual cutoff control, or patch modulation CV for dynamic cutoff movement.
- Adjust **RESO** knob for resonance, or patch modulation CV for dynamic resonance sweeps (self-oscillation is not specified).
- Use simultaneous outputs for creative parallel or serial filtering.

---

**[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**