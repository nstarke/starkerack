# 2hp — Unity

- [Manual PDF](../../manuals/2hp_Unity.pdf)

---

[Unity Manual PDF](#)  
*(You may need to supply the actual PDF link)*

---

# 2hp Unity Mixer – Cheat Sheet

A dual unity-gain mixer for Eurorack, allowing for flexible mixing of both audio and CV signals in three different summing modes.

---

## Controls

| # | Label         | Type   | Function                                                                                     |
|---|--------------|--------|---------------------------------------------------------------------------------------------|
| 1 | MODE         | Toggle | 3-position switch to select between Averaging, Unity, or Split mode                         |

### Mode Toggle Behavior
- **Averaging Mode (UP):** All inputs = gain of 1/3. Best for mixing audio, preserves relative loudness.
- **Unity Mode (MIDDLE):** All inputs = gain of 1. Best for mixing control voltages (CV).
- **Split Mode (DOWN):** Top mixer = gain 1; Bottom mixer = gain 1/3. Mix CV on top, audio on bottom.

---

## Inputs and Outputs

| # | Label    | Type         | Description & Normalization                                                    | Voltage Range              |
|---|----------|--------------|-------------------------------------------------------------------------------|----------------------------|
| 2 | Top 3 jacks | IN        | Inputs to Mixer 1. Summed and sent to OUT 1. Each jack accepts audio or CV.    | ±10V CV / Audio typical    |
| 3 | OUT (top)   | OUT       | Output of Mixer 1 (top 3 inputs). If patched, Mixer 1 only goes here; if unpatched, also sums to OUT 2. | Up to input sum max        |
| 4 | Bottom 3 jacks | IN     | Inputs to Mixer 2. Summed and sent to OUT 2. Each jack accepts audio or CV.    | ±10V CV / Audio typical    |
| 5 | OUT (bottom)| OUT       | Output of Mixer 2 (bottom 3 inputs). If OUT 1 unpatched, includes sum of both sections. | Up to input sum max        |

---

## Quick Reference Operation

- **6-to-1 Mixer:** Leave OUT 1 unpatched; OUT 2 will output sum of all 6 inputs (based on mode).
- **2x3-to-1 Mixer:** Patch both OUT 1 and OUT 2. Each OUT is the sum of their respective 3 inputs.
- **Split Mode:** Mix CV with unity gain (top 3 jacks → OUT 1), audio with averaging gain (bottom 3 jacks → OUT 2).

---

## Power & Specs

- **Width:** 2 HP
- **Depth:** 39.5 mm
- **+12V:** 10mA
- **-12V:** 6mA

*Install with red stripe (cable) down for -12V as per standard Eurorack orientation.*

---

## Typical Use Cases

- Combine multiple modulation (CV) sources.
- Mix several audio sources without loss of amplitude (Averaging mode).
- Run hybrid CV+audio patching (Split mode).
- Simple, clean, and compact mixing utility.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)