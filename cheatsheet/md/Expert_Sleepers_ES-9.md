# Expert Sleepers — ES-9

- [Manual PDF](../../manuals/es9_user_manual_1.3.pdf)

---

[**Expert Sleepers ES-9 Manual PDF**](https://expert-sleepers.co.uk/es9usermanual.html)

# Expert Sleepers ES-9 – Quick Reference Cheat Sheet

## Power & Installation
- **Power Connector**: Doepfer standard (10-pin).  
  - Red stripe = -12V (bottom of PCB)
- **Power Draw**:
  - +12V: 451 mA (max at 96kHz)
  - -12V: 133 mA
  - 5V: Not used

## Panel Controls

| Control   | Type      | Function                                                                                  |
|-----------|-----------|-------------------------------------------------------------------------------------------|
| Volume Knob | Rotary & Push | Headphone output volume. Push & hold (>1s) toggles between "hosted" and "standalone" configs. |
| LEDs      | 4x        | A: Power / B: USB Data / C: MIDI Out / D: MIDI In                                       |
| Jumpers   | Back Panel| JP1: Forces DFU boot mode for firmware update                                            |

---

## Inputs and Outputs

| Type                | Location      | Count | Connector  | Voltage Range  | Coupling | Notes                         |
|---------------------|--------------|-------|------------|---------------|----------|------------------------------|
| Analogue Inputs     | Front        | 14    | 3.5mm TS   | ±10V (0dBFS)  | DC       | Use for audio or CV           |
| Analogue Outputs    | Front        | 8     | 3.5mm TS   | ±10V max      | DC       | Use for audio or CV           |
| Balanced Outputs    | Front        | 2     | 1/4" TRS   | Line Level    | AC       | Not DC coupled (for monitors) |
| Headphone Output    | Front        | 1     | 1/4" TRS   | Line Level    | DC       | Mix of outs 1/2 & 3/4         |
| S/PDIF In/Out       | Front        | 2     | Optical    | Digital audio | N/A      |                                 |
| MIDI – Expansion    | Rear Header  | 2     | 4-pin IDC  | –             | –        | Use MIDI breakout             |
| ES-5 Expander       | Rear Header  | 1     | 10-pin IDC | –             | –        | For gate/trigger expansion    |

*Socket Illumination*: 3.5mm input/output jacks light RED (positive), BLUE (negative).

---

## USB Host Operation
- **USB C port** connects to DAW; no power drawn from USB bus.  
- No drivers needed for macOS/iOS/Linux; Windows driver available on [Expert Sleepers downloads](https://expert-sleepers.co.uk/downloads.html).

## Audio Channels Mapping (Default, DAW)  
- **Main Outputs (1/4")**: 1/2  
- **Headphone Out**: Mix of 1/2 & 3/4  
- **S/PDIF Out**: 5/6  
- **ES-5 Out**: 7/8  
- **3.5mm Outputs**: 9–16  
- **3.5mm Inputs**: 1–14  
- **S/PDIF In**: 15/16  

---

## Quick-Start Workflow

1. **Install ES-9 in Eurorack** → connect power cable (match -12V to red stripe)
2. **Connect via USB** to your computer (use C-to-A or C-to-C cable).
3. **Confirm DAW Device**: Select ES-9 in your DAW's audio preferences.
4. **Monitor LEDs**: LED below USB C should light when connected.
5. **Configure** with the ES-9 Config Tool ([download here](https://expert-sleepers.co.uk/es9firmware.html); browser app requires Chromium-based browser).
6. **Save Configuration** into either hosted or standalone memory slots.

---

## Advanced Features Cheat Sheet

| Feature                    | Key Details                                                            |
|----------------------------|------------------------------------------------------------------------|
| **Mixers**                 | 8x8 crosspoint (mono) mixers. Can route anything to anything.          |
| **DC Blocking**            | Switchable per input pair; keep ON for audio, OFF for CV.              |
| **Stereo Links**           | Links adjacent mixer channels for stereo processing.                   |
| **EQ**                     | 4 bands per input, several filter types. Consumes DSP resources.       |
| **Mix Smoothing**          | Optional interpolation; use for MIDI-controlled mixing, live use.      |
| **MIDI Control**           | Macro mix controllable via MIDI CC (see manual for CC mapping).        |
| **5-pin DIN MIDI I/O**     | With MIDI breakout; 4-pin header pinout in manual.                     |
| **Firmware Update**        | Use ExpertSleepersDFU tool + .dfu file; see [update page](https://expert-sleepers.co.uk/es9firmware.html) |
| **SysEx Protocol**         | Full SysEx support for config state/automation (see manual).           |

---

## Back Panel Jumpers & Expansion

- **JP1**: Fit jumper to force DFU boot (firmware rescue if normal DFU fails).
- **GT1 (To ES-5)**: 10-pin expansion to ES-5; red stripe down.
- **GT2 (MIDI breakout)**: 4-pin header for 5-pin DIN MIDI.

**Pinout:**

| Pin | Function    |
|-----|-------------|
| 1   | OUT (DIN pin 4) |
| 2   | OUT (DIN pin 5) |
| 3   | IN  (DIN pin 5) |
| 4   | IN  (DIN pin 4) |

---

## Troubleshooting LED Indicators

| LED | Function                                          |
|-----|---------------------------------------------------|
| A   | On = Powered                                      |
| B   | On = USB connected                                |
| C   | MIDI from host → breakout (outbound)              |
| D   | MIDI from breakout → host (inbound)               |
| All | At start: flash twice/sequence = normal.          |

---

## Useful Links
- [**Expert Sleepers ES-9 Manual (PDF/HTML)**](https://expert-sleepers.co.uk/es9usermanual.html)
- [**Firmware & Config Tools**](https://expert-sleepers.co.uk/es9firmware.html)

---

**Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)**