# Tiptop Audio — CYMBL909

- [Manual PDF](../../manuals/Tiptop_Audio_CYMBL909_ns.pdf)

---

[CYMBL909 Manual PDF](https://tiptopaudio.com/909-2)

---

# Tiptop Audio CYMBL909 Cheat Sheet

The **CYMBL909** is a dual-voice Eurorack module that clones the iconic TR-909 crash and ride cymbals with extra features for modular use. Each side (Crash and Ride) is controlled independently. Voltage Controlled Tuning and individual Accent inputs allow for highly expressive drum programming.

---

## Panel Overview

### Controls (Per Voice: Crash & Ride)
- **LEVEL**: Sets output level of cymbal voice.
- **TUNE**: Manual frequency tuning.
- **ACCENT**: Adjusts intensity/loudness of the gate trigger; scalable via external accent input or manual setting.
- **VC-TUNE**: Voltage controlled tuning input (responds to CV).

---

## Panel Connections

### Inputs

| Jack        | Function                        | Voltage Range | Notes                                              |
|-------------|---------------------------------|---------------|----------------------------------------------------|
| CR GATE     | Crash Voice Trigger Input       | 5V Gate/Trig  | Receives gates or triggers to play Crash           |
| RD GATE     | Ride Voice Trigger Input        | 5V Gate/Trig  | Receives gates or triggers to play Ride            |
| ACCENT (CR) | Crash Accent Input (CV/gate)    | 0-5V suggested| CV or gate/trigger. Sets accented level, scales gain|
| ACCENT (RD) | Ride Accent Input (CV/gate)     | 0-5V suggested| CV or gate/trigger. Sets accented level, scales gain|
| VC-TUNE (CR)| Crash Frequency CV Input        | -5V to +5V    | For modulating pitch; external LFO/CV recommended   |
| VC-TUNE (RD)| Ride Frequency CV Input         | -5V to +5V    | For modulating pitch; external LFO/CV recommended   |

### Outputs

| Jack    | Function                  | Voltage Range   | Notes                                         |
|---------|---------------------------|-----------------|-----------------------------------------------|
| CR OUT  | Crash Cymbal Audio Output | Typical modular | Audio output level, patch to mixer or VCA     |
| RD OUT  | Ride Cymbal Audio Output  | Typical modular | Audio output level, patch to mixer or VCA     |

---

## Quick Start
1. **Connect GATES:** Patch sequencer outputs to CR GATE and RD GATE.
2. **Patch Outputs:** CR OUT and RD OUT to mixer/sound system.
3. **Set Initial Controls:**
    - ACCENT: Max
    - LEVEL: 12 o’clock
    - TUNE: 12 o’clock (adjust for taste)
4. **Tweak:** Adjust LEVEL, ACCENT, and TUNE for each voice. Sequence/CV via VC-TUNE for animation.

---

## Key Features Explained

- **Independent Accent:** Unlike the original TR-909, both Crash & Ride have their own Accent controls & inputs.
- **Accent Input:** Patch CV/gate for detailed dynamics per cymbal. Without Accent input, GATE is internally routed so ACCENT knob works as fine gain.
- **VC-TUNE:** Modulate pitch manually and with CV (-5V to +5V typical). Sync CV modulation with each gate for creative effects (e.g., patch to envelope or step sequencer).
- **True Analog 909:** Circuit is a close clone of the original, adapted for Eurorack (-12V/+12V power, compatible with most modular systems).

---

## Reference Table: Knobs & Jacks

| Control/Jack  | Type      | Description                  | Voltage Range / Function             |
|---------------|-----------|------------------------------|--------------------------------------|
| LEVEL         | Knob      | Output volume                | -                                    |
| TUNE          | Knob      | Frequency tuning             | - (analog, physical sweep)           |
| ACCENT        | Knob      | Intensity amount             | - (scales incoming accent/GATE)      |
| GATE IN (CR/RD)| Jack     | Triggers Crash/Ride          | 0-5V (gate/trigger)                  |
| ACCENT IN (CR/RD)| Jack   | CV or gate accent control    | 0-5V (suggested)                     |
| VC-TUNE IN (CR/RD)| Jack  | CV frequency modulation      | –5V to +5V typical                   |
| OUT (CR/RD)   | Jack      | Audio                        | Modular audio level                  |

---

## Tips
- **Accent can use any gate or CV; try envelopes for dynamic hits.**
- **VC-TUNE is great for LFO, envelopes, or sequencer-based pitch shifts/ringing sweeps.**
- **Set ACCENT to minimum if using CV to prevent double-scaling.**
- **Internally normalized accent means drum sounds stay loud even with only GATE patched.**

---

**Manual Source & More:** [CYMBL909 Manual PDF](https://tiptopaudio.com/909-2)

**Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)**