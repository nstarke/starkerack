# Cute Lab — Messed Up

- [Manual PDF](../../manuals/messed-up-manual-rev2.pdf)

---

Certainly! Here is a concise cheat sheet for the **CuteLab Messed Up: Metrically Modulating Clock Generator** eurorack module, based on the manual you provided.

---

### [Messed Up User Manual PDF](Upload-the-manual-to-a-public-link/if-available.pdf)

---

## Messed Up Cheat Sheet

### 🏷️ **Quick Overview**
- **Type:** Modulating Clock Generator
- **Use:** Generates flexible clock/divide rhythms and stretchable tempos for advanced metric modulation, polyrhythms, and synced clocking.  
- **Clocks:** Internal or external.
- **Unique:** Truncation and modulation for complex rhythmic changes.

---

## ⚡ **Inputs, Outputs, Controls: Quick Reference**

### Inputs (CV, Gate, or Clock Jacks)
| # | Jack/Input Name | Function | Range/Notes                |
|---|-----------------|----------|----------------------------|
|2  | **Clock In**        | External clock input               | Standard 0-5V or higher for modular clocks |
|14 | **Modulate In**     | Trigger input for metric modulation| Rising edge triggers modulation   |
|13 | **Beat CV In**      | CV to beat value                  | ±5V typical (manual unspecified)  |
|16 | **Divide CV In**    | CV to divide value                | ±5V typical; attenuvertable (see control 12) |
|15 | **Truncate CV In**  | CV to truncation                  | ±5V typical                      |

### Outputs (Gate/Clock Out)
| # | Jack/Output Name | Function / Voltage  | Description                              |
|---|------------------|---------------------|------------------------------------------|
|21 | **Beat Out**         | Gate out (0-5V)      | Fires for each beat                       |
|20 | **Divide Out**       | Gate out (0-5V)      | Fires for divided beats                   |
|19 | **Truncate Out**     | Gate out (0-5V)      | Fires with truncation                     |
|17 | **Downbeat Out**     | Gate out (0-5V)      | Fires for 1st beat of each measure        |
|18 | **EoM Out**          | Gate out (0-5V)      | End of Modulation trigger                 |

### Knobs, Encoders, and Button Controls
| # | Control                | Function                                      |
|---|------------------------|-----------------------------------------------|
|1  | **Tap Tempo Button**   | Sets/holds tempo, shows BPM, clock start/stop |
|5  | **Divide Encoder**     | Adjust divide value (int or CV), push: latch  |
|6  | **Beat Encoder**       | Adjust beat value (int or CV), push: latch    |
|4  | **Modulate Button**    | Triggers modulation, queues modulation        |
|10 | **Truncate Knob**      | Sets truncation position                      |
|12 | **Divide CV Attenuverter** | Scales/inverts divide CV in                |

### Toggles & Indicators
| # | Toggle/Switch/LED           | Function                            |
|---|-----------------------------|-------------------------------------|
|11 | **Free Mod. Toggle**        | Free/latched modulation to measure  |
|9  | **Round Trip Mod. Toggle**  | Enable/disable round trip modulation|
|7  | **Divide Latch LED**        | Red: divides changes latched        |
|8  | **Beat Latch LED**          | Red: beat changes latched           |

### Display
| # | Display Component | Function |
|---|-------------------|----------|
|3  | 7-Segment Display | Shows tempo, settings, or config menu value |

---

## 🎚️ **Features & Workflow**

### Basic Patch & Use
- **Simple clock**: Clock In → Beat Out, Drive sequencers/drums.
- **Set tempo**: Tap clock button or hold and use encoders.
- **Change signature:** Set "Beat" and "Divide" for custom meters/ratios.
- **Modulation:** Press Modulate button, or external trigger, to "stretch" tempo into a new ratio.
  - **Round Trip:** Toggle up for A→B→A switching.
  - **Free:** Toggle modulation to next measure or immediate (beat aligned).
- **Truncate:** Add rhythmic variation using truncate knob or CV.
- **Latch:** Encoders can queue changes to the next downbeat.

### Voltage Ranges
- **All Logic/Gate outs:** 0V (low), 5V (high) typical.
- **CV Inputs:** ±5V (noted, use external attenuators if needed).
- **External Clock:** Accepts typical modular gates/clocks 0-5V up.

### Configuration Menu (Hold Divide encoder to enter)
- **Input Clock Divider:** Adjust input clock scaling 1:1–1:9
- **Clock Stop:** Module stops if no external clock.
- **Beat/Divide Output Multiplier:** Send more clock pulses (1, 2, 4, or 8 PPN)
- **Duty Cycle Mode:** 50% or short pulse (10ms)
- **Beat Input Reset:** Use Beat CV jack as reset instead of CV
- **Modulation Style:** After mod, outputs can sync, stay, or flip roles.

### Presets
- Save/recall all current settings (tempo, beat, divide, options) to one of 9 presets.
- (Hold Beat encoder to enter preset mode.)

### Firmware
- Update via USB mini on back PCB. See [CuteLab Github](https://github.com/nstarke/eurorack-processor) for files/instructions.

---

## 🎶 **Concepts/Best Practices**
- **Metric Modulation:** Use different beat/divide values then modulate, changing the rhythmic grid.
- **Truncation:** Great for syncopation or subtle groove changes.
- **Latch:** Smooth live performance changes by quantizing to the measure.
- **Sync Outputs:** Use Downbeat or EoM out to sync other modules to modulation or measure start.

---

## 💾 **References**

- [Manual PDF (add your link here!)](Upload-the-manual-to-a-public-link/if-available.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---

**Tip:** Experiment with unusual Beat/Divide values, modulate and use truncation for polyrhythms that are tight but breathe!

If you have questions about a specific use case, just ask!