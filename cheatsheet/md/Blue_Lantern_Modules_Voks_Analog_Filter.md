# Blue Lantern Modules — Voks Analog Filter

- [Manual PDF](../../manuals/BLM Voks Analog Filter.pdf)

---

[BLM Voks Analog Filter Manual (PDF)](https://www.bluelanternstore.com/store/p133/BLM_Voks_Analog_Filter.html#/)

---

# **BLM Voks Analog Filter – Cheat Sheet**

**Type:** Analog VCF (Voltage Controlled Filter)  
**Format:** Eurorack (6HP)  
**Current draw:** +13mA, -13mA  
**MSRP:** $103 (blowout), originally $150  
**Design:** Based on classic Polivoks filter, modernized parts with improved sweep.

---

## **Panel Overview & Controls**

### **Inputs**
| Label         | Type          | Description                                            | Voltage Range         |
|---------------|---------------|-------------------------------------------------------|----------------------|
| `IN (LEVEL)`  | Audio/CV      | Attenuated audio input via Level knob                 | Audio ±5V typical    |
| `CV IN`       | CV            | Direct filter cutoff modulation input                 | CV 0-5V              |
| `FM` (bi-polar CV) | CV        | Frequency modulation (bi-polar) input, depth controlled | CV ±5V               |
| `1 IN`        | Audio         | Direct, unattenuated audio input                      | Audio ±5V typical    |

### **Outputs**
| Label         | Type          | Description                                            | Voltage Range         |
|---------------|---------------|-------------------------------------------------------|----------------------|
| `LPF`         | Audio         | Low Pass Filter output (12dB/oct, amplified)           | Audio ±5V            |
| `BPF`         | Audio         | Band Pass Filter output (6dB/oct, amplified)           | Audio ±5V            |

### **Switches & Buttons**
| Label / Type      | Function                                 | Notes                  |
|-------------------|------------------------------------------|------------------------|
| 2-way Toggle      | Filter Mode: **Normal / Unstable Brite** | Brite: unstable/edgy   |
| 2-way Toggle      | Limiter Diode in circuit: **On / Off**   | For added saturation   |

### **Knobs**
| Knob        | Function                              | Range         |
|-------------|---------------------------------------|---------------|
| LEVEL       | Controls input gain (attenuates "IN") | 0 → Max input |
| FM Amount   | Controls depth of bi-polar FM         | 0 → Max depth (unlabeled, but present)      |

---

## **Feature Recap**
- **Modes:**  
  - **Normal:** Classic Polivoks timbre.  
  - **Unstable Brite:** More aggressive/edgy, less predictable resonance.
- **Limiter Diode:** Soft clipping/saturation switch for character and taming levels.
- **Outputs:**  
  - **LPF (12dB/oct):** Steeper, classic lowpass filter.  
  - **BPF (6dB/oct):** Gentler bandpass flavor.
- **Inputs:**  
  - **Two audio ins:**  
    - One level-controlled via the panel knob.  
    - One direct, full strength.
- **CV Control:**  
  - **Direct CV input for cutoff.**  
  - **FM input for wild modulations (bipolar).**

---

## **General Use Tips**
- For classic filtering, use `IN` with the LEVEL knob, `LPF` out, switch in Normal/Diode off.
- For wild, unstable tones/noisy sweeps, use Unstable Brite mode and experiment with FM and Limiter engaged.
- Use both LPF and BPF outs for parallel or stereo effects.
- Bi-polar FM accepts full audio-rate CV for aggressive timbres.

---

## **Reference Links**

[BLM Voks Analog Filter Manual (PDF)](https://www.bluelanternstore.com/store/p133/BLM_Voks_Analog_Filter.html#/)

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)