# Tiptop Audio — MA808

- [Manual PDF](../../manuals/Tiptop_Audio_MA808_ns.pdf)

---

[Tiptop Audio MA808 Manual PDF](https://tiptopaudio.com/808-2)

---

# Tiptop Audio MA808 Cheat Sheet

## Overview
The **MA808** is a Eurorack adaptation of the Roland TR-808 Maracas sound engine, with additional controls and Eurorack-friendly features including white noise out, independent accent control, and an extra **Attack** parameter to adjust sound character.

---

## Panel Controls & Jacks Reference

### Knobs
- **LEVEL**: Master output volume of maracas sound.
- **ATTACK**: Adjusts the envelope attack time.
  - **Counter-clockwise**: Sharper, snappier, more hi-hat like.
  - **Clockwise**: Slower, softer, delayed maraca sound.  
  - **Dot position**: Classic 808 sound.
- **ACCENT**: Sets the amount of dynamic accent (how much louder accented hits will be).

### Input Jacks
| Jack       | Function                              | Details/Voltage Ranges               |
|------------|---------------------------------------|--------------------------------------|
| ACCENT IN  | Gate/trigger for dynamic accent       | Standard 5V trigger/gate             |
| GATE IN    | Gate/trigger to play maracas sound    | Standard 5V trigger/gate             |

### Output Jacks
| Jack       | Output                               | Details/Voltage Ranges               |
|------------|--------------------------------------|--------------------------------------|
| MA OUT     | Maracas main audio out               | Line level Eurorack modular audio    |
| 808 W-NOISE| Raw analog white noise out           | Line level audio (use for other patching) |

---

## Quick Start
1. **Patch a gate/trigger (5V, ~>2ms) to GATE IN**.
2. **Patch MA OUT** to mixer or audio interface.
3. Set **LEVEL** to 12 o’clock, **ACCENT** full up, **ATTACK** at the dot.
4. Trigger and you’ll get the classic 808 maraca sound.
5. Adjust:
   - **ATTACK** counter-clockwise for sharper/hi-hat like tone.
   - **ATTACK** clockwise for slower maraca with delayed onset.

---

## Feature Tips
- **White Noise Out**: Use **808 W-NOISE** output as raw noise source for other drum synthesis or modulation.
- **Accent**:
  - No patch to **ACCENT IN**: Gate is normalized to accent, **ACCENT** knob becomes a fine volume control.
  - Patch a gate to **ACCENT IN**: Independent control of accented notes; **ACCENT** knob scales accent amount.
- **Classic 808**: Dot on **ATTACK** = original 808 behavior.

---

## Voltage Control
- **Gates/Triggers**: Standard 5V logic. Higher voltage up to 12V usually safe for gate inputs.
- **Audio Outputs (MA OUT, 808 W-NOISE)**: Modular level audio (~10Vpp typical).

---

## Creative Patching Suggestions
- Run **808 W-NOISE** into filters, VCAs, or envelopes for custom hats/snares.
- Use **808 W-NOISE** as random modulation or to clock sequencers (random bursts).

---

**Manual:** [https://tiptopaudio.com/808-2](https://tiptopaudio.com/808-2)

**Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)**