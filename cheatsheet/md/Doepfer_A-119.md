# Doepfer — A-119

- [Manual PDF](../../manuals/A119_man.pdf)

---

[Doepfer A-119 Manual PDF](https://doepfer.de/a100man/A119_man.pdf)

---

# Doepfer A-119 Ext. Input / Envelope Follower  
**Cheat Sheet**

*The Doepfer A-119 is for integrating external audio (instruments, mics, etc.) into your modular, providing pre-amped audio, an envelope follower, and a gate comparator.*

---

## Inputs

| Jack Label      | Type        | Details                                                         |
|-----------------|-------------|-----------------------------------------------------------------|
| **Asym. In (!) (3.5mm)** | Unbalanced (mono) | For line-level signals (e.g., synths, drum machines). [Gain x0–20] |
| **Symm. In (") (6.3mm)** | Balanced (TRS)   | For mic/instrument-level signals (e.g., guitar, microphone). [Gain x0–500] |

**Note**: Only use one input at a time. If both are used, mixed with a 1:25 ratio.

---

## Outputs

| Jack Label        | Type              | Voltage Range                 | Details                                 |
|-------------------|-------------------|-------------------------------|-----------------------------------------|
| **Audio Out (§/$)** | Unbalanced audio | up to ±10V*                   | Pre-amped signal (2 linked outputs, “mini-mult”). |
| **Envelope Out (%)** | CV (envelope)    | 0–~8V (typical max output)    | Follows amplitude contour of input.     |
| **Gate Out (&)**     | Gate             | 0V (off), +12V (on)           | High when envelope > threshold.         |

\* **Audio Out Overload:** Outputs can clip with input gain set too high; watch Overload LED.

---

## Controls, Buttons, Indicators

| Label             | Type    | Range / Purpose                          |
|-------------------|---------|------------------------------------------|
| **Gain (1)**      | Knob    | Sets input preamp gain (see ranges above)|
| **Thres. (5)**    | Knob    | Sets gate threshold (relative to envelope out)|
| **Overload LED (2)** | LED  | Lights if preamp output >10V (audio clipping)|
| **Envelope LED (3)**| LED   | Indicates current envelope level         |
| **Gate LED (4)**    | LED   | Indicates gate output status (= high)    |

---

## Quick Patching Examples

- **Bring in External Audio:**  
  - Plug audio into **Asym. In** or **Symm. In**  
  - Set **Gain** so Overload LED barely lights on peaks  
  - Take pre-amped signal from **Audio Out (§/$)**

- **Envelope Following (e.g. for VCF/VCAs):**  
  - Use **Envelope Out (%)** for a dynamic CV

- **External Gate Source (e.g. for ADSRs):**  
  - Use **Gate Out (&)** when envelope passes threshold

- **Typical Gate Output Threshold:**  
  - Adjust with **Thres.** until desired triggering

- **Tip:** If Envelope Out (%) is "noisy" with low-frequency inputs (<50 Hz), route through a slew limiter like A-170.

---

## Voltage Ranges

| Output         | Range           |
|----------------|-----------------|
| **Audio Out**  | up to ±10V (clipping past 10V) |
| **Envelope Out**| 0–~8V (typical) |
| **Gate Out**    | 0V (low), +12V (high) |


---

## Additional Notes

- **Use only one input at a time.**
- **Overload LED**: Avoid sustained overload for clean audio.
- **Envelope Out** is a full-wave rectified, low-passed envelope of audio input.
- **Gate Out** is held HIGH as long as the envelope stays above threshold.
- **Two preamp outputs for easy splitting (“mini-mult”).**


---

**Reference:**  
[Doepfer A-119 Manual PDF](https://doepfer.de/a100man/A119_man.pdf)  
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)