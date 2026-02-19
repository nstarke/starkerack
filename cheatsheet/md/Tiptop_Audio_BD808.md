# Tiptop Audio — BD808

- [Manual PDF](../../manuals/Tiptop_Audio_BD808_ns.pdf)

---

[Tiptop Audio BD808 Manual PDF](https://www.tiptopaudio.com/808-2)

---

# Tiptop Audio BD808 Eurorack Module Cheat Sheet

The **Tiptop Audio BD808** is a direct clone of the Roland TR-808 bass drum circuit, optimized for Eurorack modular systems with some modern enhancements (notably gain staging and independent accent control).

---

## **Panel Controls**

| Control     | Type   | Description                                                                                                 |
|-------------|--------|-------------------------------------------------------------------------------------------------------------|
| **LEVEL**   | Knob   | Sets output level. High settings can overdrive external devices. 0–100%.                                    |
| **TONE**    | Knob   | Sets the cutoff frequency of the internal low-pass filter. Low = darker, silky. High = punchy, "basketball".|
| **DECAY**   | Knob   | Sets the length of the bass drum tail. High = longer; too high can cause self-oscillation in some units.    |
| **ACCENT**  | Knob   | Sets how much the accent voltage (or normalized GATE) affects the amplitude/attack of the sound.            |

---

## **Inputs and Outputs**

| Jack             | Type      | Function                                                                                                                                         | Voltage Range                 |
|------------------|-----------|--------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------|
| **GATE IN**      | Input     | Trigger signal to play the bass drum.                                                                                                            | Standard modular gate (~5–12V)|
| **ACCENT IN**    | Input     | Optional accent trigger. If unpatched, GATE IN is normalized here. If patched, sets accent independently.                                        | Gate/trigger (~5–12V)         |
| **BD OUT**       | Output    | Audio output for the bass drum. Hot output level—can reach up to 20Vp-p at max LEVEL and ACCENT.                                                 | Up to 20Vp-p                  |

---

## **Usage Tips**

- **Basic Use**:  
  Patch a trigger or gate source into **GATE IN**, and **BD OUT** to your mixer/sound system. Start with **LEVEL** at ~50%.

- **Accents**:  
  - For dynamics, patch a trigger into **ACCENT IN** for accented hits.
  - With no cable patched to ACCENT IN, the BD808 "self-accentuates" (GATE IN is normalized to ACCENT).
  - Use the **ACCENT** knob for fine control over hit strength and volume.

- **Drive and Loudness**:  
  Max **LEVEL** and **ACCENT** produce an extremely hot output (up to 20Vp-p). Watch gain-staging when feeding interfaces.

- **Decay Self-Oscillation**:  
  If DECAY is at maximum, some units may self-oscillate (constant low tone). Reduce slightly if this occurs.

- **Sound Design**:
  - Short DECAY, high LEVEL/TONE/ACCENT = tight, punchy kicks.
  - Long DECAY, low TONE = booming, sub-heavy 808s.
  - Experiment processing **BD OUT** with filters, distortions, or external modulation for unique results.

- **Inconsistent Sound**:  
  If DECAY is longer than your trigger interval, sounds may overlap and become inconsistent—reduce DECAY.

---

## **Voltage Ranges**

- **Inputs (GATE/ACCENT):** Standard modular gates/triggers (typically respond to 4V+, safe up to 12V).
- **Output (BD OUT):** Up to 20Vp-p in extreme settings. Typical professional line level inputs clip around 10Vp-p!

---

## **Patch Ideas**

- Process **BD OUT** through wavefolders/distorters for grit.
- Use another module's output into **ACCENT IN** for dynamic/probabilistic accents.
- Mix with other Tiptop 808-series drums for full classic kits.

---

**Manual Reference:** [Tiptop Audio BD808 Manual PDF](https://www.tiptopaudio.com/808-2)

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
