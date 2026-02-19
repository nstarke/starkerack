# SSF — Autodyne

- [Manual PDF](../../manuals/Autodyne - Steady State Fate.pdf)

---

**[Steady State Fate Autodyne Manual (Webpage)](https://steadystatefate.com/products/autodyne)**

---

# **SSF Autodyne Eurorack Module Cheat Sheet**

## **Overview**
Autodyne is a 4hp analog auto-compressor/distortion featuring:
- Simple single-knob compression/gain control
- Switchable sidechain filtering for transparent low end
- NY-style parallel compression blend
- Capable of both clean and characterful/distorted compression

---

## **Inputs & Outputs**

| Jack Name      | Type            | Function                                                      | Voltage Range              |
|----------------|-----------------|---------------------------------------------------------------|----------------------------|
| **IN**         | Audio/CV Input  | Main audio input                                              | ±10V typical audio range   |
| **OUT**        | Audio Output    | Compressed (and/or blended) audio output                      | ±10V typical audio range   |
| **SIDE CHAIN IN** | CV/Audio Input  | Optional external sidechain detector input (overrides normal) | ±10V typical audio/CV      |

---

## **Front Panel Controls**

| Control                 | Type    | Function                                                                                   |
|-------------------------|---------|--------------------------------------------------------------------------------------------|
| **COMP**                | Knob    | Ratio, Threshold, Gain all in one. <br> Below center = subtle; above center = extreme comp.|
| **GAIN**                | Knob    | Final output level; fully clockwise gives heavy distortion.                                |
| **HPF BLEND**           | Knob    | Blends dry (uncompressed) and wet (compressed) signal (NY parallel). Fully CCW = dry only. |
| **SIDE CHAIN FILTER**   | Toggle  | Engages triple slope high pass on sidechain (better for bass preservation).                |
| **BYPASS**              | Unsure* | Not mentioned as a dedicated switch/footwitch – bypass via HPF Blend fully CCW.            |

> \*Compression is effectively bypassed by turning the HPF BLEND control fully counterclockwise.

---

## **Quick Start Workflow**
1. **Patch Audio**: IN → your signal. OUT → next module/mixer.
2. **Set COMP Knob**:
    - Noon = neutral/dynamic.
    - >12:00 = heavier squash/compression.
    - <12:00 = more transparent.
3. **Set GAIN**: Level match or drive for distortion.
4. **HPF BLEND**: Use to set dry/compressed balance (parallels NY compression).
5. **Sidechain Filter Switch** (if needed): **ON** for bassy material (prevents low-end pumping).
6. **Sidechain Input**: Patch an external signal to shape compression based on a different audio/CV.

---

## **Stereo Use**
- Use two matched modules.
- Controls easy to mirror for dual-mono/stereo applications.

---

## **Power Requirements**
- **Width**: 4hp
- **Depth**: 23mm
- **Current**: +12V @ 85mA, -12V @ 90mA

---

## **Key Points**
- Simple workflow, one big COMP knob for quick vibe changes.
- *Audiophile* quality analog components & Burr-Brown opamps.
- Not gated/noise reducing: strictly compression & tame distortion.

---

## **References**
- [Steady State Fate Autodyne Manual/Product Page](https://steadystatefate.com/products/autodyne)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
