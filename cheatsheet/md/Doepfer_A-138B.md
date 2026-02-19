# Doepfer — A-138B

- [Manual PDF](../../manuals/A138_man.pdf)

---

[Doepfer A-138 Mixer Manual PDF](https://doepfer.de/a100man/a138_man.pdf)

---
# Doepfer A-138 System A-100 Mixer
**Type:** 4-channel mixer (audio & CV)

---

## Panel Reference

| Label      | Function                                             | Voltage Range         |
|------------|------------------------------------------------------|----------------------|
| In 1       | Input 1 (also offset generator, see below)           | Audio/CV ±10V        |
| In 2       | Input 2                                              | Audio/CV ±10V        |
| In 3       | Input 3                                              | Audio/CV ±10V        |
| In 4       | Input 4                                              | Audio/CV ±10V        |
| Out        | Mixed Output                                         | Depends on input     |

### Knobs/Controls

| Label    | Function                                            |
|----------|-----------------------------------------------------|
| In 1     | Level (attenuator) for Input 1                      |
| In 2     | Level (attenuator) for Input 2                      |
| In 3     | Level (attenuator) for Input 3                      |
| In 4     | Level (attenuator) for Input 4                      |
| Out      | Master output level                                 |
| lin/exp  | Module type:                                          
               - **A-138a:** Linear pots (CV mixing)
               - **A-138b:** Logarithmic pots (Audio mixing)      |

### Internal Jumper (JP4, mid-2004 and later only)

- **No jumper:** Offset disabled
- **Jumper at edge:** Input 1 knob generates +0...+5V offset (if nothing is patched to In 1)
- **Jumper near panel:** Input 1 knob generates  0...-5V offset (if nothing is patched to In 1)

---

## How To Use

### Audio Mixing (A-138b recommended)

1. Patch audio sources to In 1–4
2. Set individual levels with In 1–4 knobs
3. Adjust mix output with Out knob
4. Take final mix from Out jack

### CV Mixing (A-138a recommended)

1. Patch up to 4 CV sources (LFO, ADSR, etc) to In 1–4
2. Set individual CV levels with In 1–4 knobs
3. Adjust summed CV mix with Out knob
4. Output to target CV input (e.g. VCF, VCO)

### Use as Offset Generator (Modules built mid-2004 onwards)
- Leave In 1 unpatched; configure JP4 for desired offset polarity.
- Use In 1 knob to set offset voltage, available at Out jack.

---

## Cheat Sheet Summary

- **Inputs (4):** Accept audio or CV, ±10V typical range.
- **Outputs (1):** Mixed sum, level set by "Out" knob.
- **Type:** Linear (A-138a) for CV, Logarithmic (A-138b) for audio.
- **Manual Output Level Control:** Yes, via Out knob.
- **Offset Generator:** Available for Input 1 via jumper.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)