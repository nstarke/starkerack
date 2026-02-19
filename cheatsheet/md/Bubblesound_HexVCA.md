# Bubblesound — HexVCA

- [Manual PDF](../../manuals/bubblesound.pdf)

---

[HEXvca Manual PDF](https://www.bubblesound-instruments.com)

---

# HEXvca (Bubblesound) Cheat Sheet

**Overview:**  
The Bubblesound HEXvca is a 7HP eurorack module featuring 6 independent VCA channels with flexible mixing and voltage-controlled features. Suitable for both audio and CV signal processing.

---

## Quick Start

- **Channels:** 6 independent VCAs
- **Mix Outs:** 3 mix outputs (1-3, 4-6, and all 1-6)
- **CV Response:** Switchable per channel (Linear/Exponential)
- **CV Normalization:** Jumpers on the back to chain CV control over multiple VCAs
- **Expansion:** Back header allows for ribbon cable connection with HEXar (triggers VCAs), future-proofed audio input header for cableless connection

---

## Controls

### Front Panel

- **(Assumed Typical) Per Channel:**
    - **Input Jack:** Patch in your audio or CV signal
    - **CV In Jack:** Patch control voltage (envelope, LFO, etc.) here  
      - *Typical voltage range:* 0V (off) to +5V (unity/max VCA response)
    - **CV Response Switch:** Toggle between Linear and Exponential VCA behavior
    - **Output Jack:** VCA output for each channel

- **Mix Outputs:**
    - **1-3 Mix Out:** Sums channels 1, 2, 3
    - **4-6 Mix Out:** Sums channels 4, 5, 6
    - **1-6 Mix Out:** Sums all six channels

### Rear Panel / Internal Jumpers

- **CV Normalize Jumpers:** Set for cascading gate/EG control between VCAs
- **Ribbon Cable Header:** Connect to HEXar for gate/trigger control (no patch cables needed)
- **6-pin Audio Input Header:** For future expansions

---

## Signal & Voltage Reference

- **All VCAs are DC-coupled:** Accept audio and CV signals
- **CV In Range:** 0–5V (typical – check for max input in module test)
- **VCA Response:**  
    - **Linear:** Best for CV and control purposes  
    - **Exponential:** Ideal for audio dynamics (musical VCA behavior)

---

## Power & Mechanical

- **Width:** 7HP
- **Depth:** 30MM
- **Power Consumption:** +50mA / -45mA

---

### Inputs & Outputs Reference

| Jack                 | Function                                   | Typical Voltage Range   |
|----------------------|--------------------------------------------|------------------------|
| Channel IN (1-6)     | Audio or CV input                          | -10V to +10V (typical) |
| Channel CV IN (1-6)  | Voltage control over VCA gain              | 0V to +5V              |
| Channel OUT (1-6)    | Individual channel output                  | -10V to +10V           |
| 1-3 MIX OUT          | Mix of channels 1, 2, 3                    | -10V to +10V           |
| 4-6 MIX OUT          | Mix of channels 4, 5, 6                    | -10V to +10V           |
| 1-6 MIX OUT          | Mix of all 6 channels                      | -10V to +10V           |

---

## How To Use

- Patch audio/CV sources to Channel IN jacks.
- Patch CV (envelope, LFO, step) sources to Channel CV INs.
- Select desired VCA response (linear/exp) per channel.
- Take outputs from individual OUTs or from MIX OUTs as needed.
- For advanced chaining, use rear jumpers/ribbon for CV normalization or expansions.

---

### [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)