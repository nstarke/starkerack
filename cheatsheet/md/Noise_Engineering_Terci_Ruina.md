# Noise Engineering — Terci Ruina

- [Manual PDF](../../manuals/Terci Ruina - Noise Engineering Documentation.pdf)

---

[**Terci Ruina Manual (PDF)**](https://manuals.noiseengineering.us/tr/)

---

# Terci Ruina Cheat Sheet

**Noise Engineering Terci Ruina**  
*Three Classic Distortions in 4HP (Eurorack)*

---

## Quick Start

1. **Power Off** your case before installing.
2. **Align Red Stripe** on ribbon cable with -12V on the module *and* your power bus.
3. **Screw In** module before powering on!
4. **Patch Your Audio Source** to any input (`In 1`, `In 2`, `In 3`).
5. **Patch Output** from any output (`Out 1`, `Out 2`, `Out 3`) to a mixer or destination.
6. **Turn Knobs** (FB, FF, FZ) to taste and explore the range of distortions!

---

## Panel Controls & Connections

### Inputs & Outputs

| Jack      | Type     | Description                                                                                      | Voltage Range         |
|-----------|----------|--------------------------------------------------------------------------------------------------|-----------------------|
| In 1      | Audio In | First distortion input. Normaled to previous output if nothing patched.                          | Audio (~±5V typical)  |
| In 2      | Audio In | Second distortion input. Normaled to output of FB stage if nothing patched.                      | Audio (~±5V typical)  |
| In 3      | Audio In | Third distortion input. Normaled to output of FF stage if nothing patched.                       | Audio (~±5V typical)  |
| Out 1     | Audio Out| Output of first distortion stage (FB). Normaled to In 2 if nothing patched.                      |                 |
| Out 2     | Audio Out| Output of second distortion stage (FF). Normaled to In 3 if nothing patched.                     |                 |
| Out 3     | Audio Out| Output of third distortion stage (FZ). Final output if all three are in series.                  |                 |

> **Note:** Inputs/Outputs are audio-rate only; there is *no* CV control or voltage processing in this module.

---

### Knobs

| Knob | Description                                                                              |
|------|------------------------------------------------------------------------------------------|
| FB   | Distortion 1 Drive: Bipolar transistor with diode-feedback clipping. Asymmetric, wild.    |
| FF   | Distortion 2 Drive: Op-amp with feedforward diode clip. Ranges from soft clip to hard.    |
| FZ   | Distortion 3 Drive: Two-stage bipolar transistor fuzz. Blends phase sections (LP→HP resp.).|

---

## Patching Tips

- **FB → FF → FZ (default)**: Patch audio into In 1, Out 3 to mixer for max carnage.
- **Re-Order/Isolate Stages**: Use In/Out jacks to break normalization and explore each stage's sound individually or in custom order.
- **Stack with Filters**: Use before/after a filter for classic overdriven bass/acid sounds.
- **Perfect for Drums**: Try on drum machines or acoustic drums for crunchy distortion.
- **Dynamic Control**: Add a VCA after (e.g., Sinc Bucina) for envelope-shaped distortion.
- **Noisy by Design**: Expect and embrace noise, chaos, odd radio pickup.

---

## Power Requirements

- **+12V:** 30 mA  
- **-12V:** 25 mA  
- **Connector:** 2x5 Eurorack standard  
- **Depth:** 0.8 inches (shallow skiff friendly)

---

## Reference

- **Type:** Triple analog distortion (4HP)
- **Voltage Control:** None (manual knobs only)
- **Patch Flexibility:** Fully series, parallel, or per-stage patching
- **Primary Use:** Brutal distortion, aggressive waveshaping, noise

---

For full details, troubleshooting, and warranty:  
[**Terci Ruina Full Manual**](https://manuals.noiseengineering.us/tr/)

---

*Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)*