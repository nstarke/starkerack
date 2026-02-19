# Erogenous Tones — VC8

- [Manual PDF](../../manuals/vc8-instructions.pdf)

---

[**VC8 Manual PDF**](https://erogenous-tones.com/erogenous-tones-vc8.html)

---

# Erogenous Tones VC8 – Cheat Sheet

**Erogenous Tones VC8** is an 8-channel DC-coupled linear VCA module featuring individual control over each channel and optional sub-mix grouping.

---

## Quick Reference

### Inputs & Outputs

| Channel | Signal Input | CV Input (LEVEL) | Audio Output | Notes                        |
|---------|--------------|------------------|--------------|------------------------------|
| 1-3     | In 1-3       | CV 1-3           | Out 1-3      | Standard VCA behavior        |
| 4       | In 4         | CV 4             | Out 4        | Can group 1-3 as sub-mix     |
| 5-7     | In 5-7       | CV 5-7           | Out 5-7      | Standard VCA behavior        |
| 8       | In 8         | CV 8             | Out 8        | Can group 5-7 as sub-mix     |

- **All Inputs/Outputs are DC coupled.**
- **Voltage Range (CV Inputs):** 0–+5V fully opens the VCA
- **Audio/Control Voltage Pass-through:** Both CV and audio signals are supported (DC coupled).

---

### Controls per Channel

- **LEVEL (CV Attenuator):** 
  - Attenuates incoming CV signal (0 to full amplitude).
  - Full VCA open at +5V.

- **OFFSET (CV Offset Knob):**
  - Adds/subtracts a fixed voltage to the CV.
  - When no CV is patched, this knob manually opens/closes the VCA.

- **White LED:** 
  - Shows resulting CV level after attenuator and offset adjustments for each channel.

---

### Sub-Mix Features

- **Channel 4 SUBMIX:**
  - When engaged, Out 4 mixes audio from channels 1–3, volume controlled by VCA 4’s controls.
  - 1/2/3 still output their individual signals as normal.

- **Channel 8 SUBMIX:**
  - When engaged, Out 8 mixes audio from channels 5–7, volume controlled by VCA 8’s controls.
  - 5/6/7 still output their individual signals as normal.

---

### Physical & Power

- **Aluminum knobs with knurled edge**
- **Width:** 18 HP
- **Depth:** Skiff Friendly (Shallow)
- **Current Draw:** +12V/80mA, -12V/70mA

---

## Usage Tips

- **For straight VCA:** Patch input + CV, use LEVEL to set response, OFFSET to bias as needed.
- **For mixing:** Engage sub-mix on CH4 or CH8—patch multiple inputs to 1–3 or 5–7.
- **Visual feedback:** White LED helps quickly check what’s open or closed.
- **For DC/CV processing:** Use with sequences, envelopes, or LFOs as it is DC-coupled.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)