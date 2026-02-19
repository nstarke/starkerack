# Qu-Bit — Synapse

- [Manual PDF](../../manuals/Synapse.pdf)

---

[Qu-Bit Synapse Manual PDF](https://qu-bit-electronix.com/files/synapse_manual.pdf)

# Qu-Bit Synapse Cheat Sheet

A powerful crossfade switch with digital routing/mixing, memory presets, DC modulation, LFOs, and flexible CV control for Eurorack.

---

## Controls Reference

### Knobs & Encoders

| Name         | Function                                                                                                                                                          |
|--------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Crossfade (4x)** | Set blend between A and B inputs per channel. CV controllable (`-5V` to `+5V`).                                                                             |
| **Terminal Encoder** | Shifts channel outputs to different output jacks (routing). Press to reset positions. CV controllable (`-5V` to `+5V`).                                    |
| **Memory Knob**      | Selects memory bank (8 total); load preset crossfade positions. Bypass memory fully CCW. Also sets LFO phase relationship and DC offset in edit modes.     |
| **Inertia Knob**     | Sets slew/smooth (0–5s), affects fader, memory, and CV changes. Also controls LFO frequency in edit mode. Also enables click-less switching in edit mode. |

### Buttons

| Name      | Function                                               |
|-----------|--------------------------------------------------------|
| **Save**     | Store current crossfade/routing to memory bank.        |
| **Scatter**  | Shuffle output channel positions.                      |
| **Advance**  | Move all outputs one to the right (sequential switch). |

---

## Inputs & Outputs

### Inputs

| Jack         | Type         | Voltage Range  | Description                                                        |
|--------------|--------------|----------------|--------------------------------------------------------------------|
| **A (4x)**   | Signal In    | Audio/CV (DC)  | Main per-channel input                                             |
| **B (4x)**   | Signal In    | Audio/CV (DC)  | Alternate per-channel input, can be normalled to +5V offset        |
| **Crossfade (4x)** | CV In   | `-5V` to `+5V` | Crossfader per channel; adds to knob position                      |
| **Terminal** | CV In        | `-5V` to `+5V` | Shifts output routing                                              |
| **Advance**  | Trigger/Gate | N/A            | Steps all outputs one to the right                                 |
| **Scatter**  | Trigger/Gate | N/A            | Randomizes output routes                                           |

### Outputs

| Jack         | Type           | Description                                                            |
|--------------|----------------|------------------------------------------------------------------------|
| **Out (1–4)**| Audio/CV Out   | Final output of each switch channel post crossfade and routing         |
| **1+2**      | Sum Out        | Sum of output from Out 1 and Out 2                                     |
| **3+4**      | Sum Out        | Sum of output from Out 3 and Out 4                                     |
| **Sum**      | Sum Out        | Pre-switch sum of each crossfade channel output                        |

---

## Special/Shift Functions (Hold + Action)

| Hold...   | While Turning...           | Action                                     |
|-----------|---------------------------|--------------------------------------------|
| Terminal  | Crossfade knob            | Per-channel master volume                  |
| Terminal  | Memory knob                | +5V DC offset to B inputs (center point on/off) |
| Terminal  | Inertia knob               | Click-less switching on/off                |
| Terminal  | Scatter button             | Set linear/constant loudness fade curve    |
| Terminal  | Save button                | Factory reset                              |
| Save      | Scatter button             | Randomize memory positions                 |
| Save      | Terminal button            | Reset all memory to A only                 |
| Scatter   | Crossfade knob             | Set LFO amplitude per channel              |
| Scatter   | Memory knob                | Set LFO phase relationships                |
| Scatter   | Inertia knob               | Set LFO frequency                          |
| Scatter   | Terminal button            | Reset LFOs to default                      |
| Scatter   | Save button                | Randomize internal modulation (LFOs)       |

*LEDs will indicate status for certain functions.*

---

## Voltage Control Summary

- **All CV Inputs:** Range `-5V` to `+5V`
- **Crossfade:** CV adds/subtracts from knob position
- **Terminal:** CV positive = right, negative = left output shift

---

## Quick Operation Examples

- **Crossfade between A/B:** Turn crossfade knob per channel, or patch CV.
- **Sequencer Mode:** Enable +5V DC offset to B inputs; modulate crossfade with CVs.
- **Switch outputs:** Turn Terminal knob or use Terminal CV input.
- **Shuffle/Advance routing:** Use Scatter or Advance buttons/inputs.
- **Save/Recall Scene:** Set crossfades/routing, select memory slot, press Save.
- **LFO Modulation:** Hold Scatter, turn crossfade knob for per-channel LFO amount; adjust inertia for speed.

---

For more advanced usage, see [Qu-Bit Synapse Manual PDF](https://qu-bit-electronix.com/files/synapse_manual.pdf).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)