# Access Virus — TI Snow

- [Manual PDF](../../manuals/Virus_TI_Snow_Quickstart.pdf)

---

It appears the images provided are of the Access Virus TI Snow Quickstart Manual, which is not a eurorack module, but a desktop digital synthesizer. The Virus TI is a powerful synth, but it is **not a eurorack module**, nor does it have typical eurorack features (patch points, ±5V CV, trigger/gate ins/outs, etc).

If you want a cheat sheet **for the Virus TI Snow**, I can create a quick-reference guide focused on its controls, ins/outs, and operation for music production.

If you meant to provide a different file or want a cheat sheet for a **eurorack module**, please clarify or upload the correct manual.

---

## Access Virus TI Snow Cheat Sheet
[Full Manual PDF Link Not Available — based on uploaded pages]

---

### Overview

- **Type**: Desktop Digital Synthesizer (not a eurorack module)
- **Polyphony**: Variable, typically 10–30 voices depending on patch complexity
- **Multi-timbrality**: 4 parts
- **Integration**: Hardware synth with deep VST/AU/RTAS plugin integration (TI: "Total Integration")

---

## Panel Controls & Reference

### Front Panel Controls

- **LCD Display**: Shows parameters and patch info
- **Soft Knobs (Below LCD)**: 3 rotary encoders for context-sensitive editing (parameters change per menu)
- **Edit/Shift Button**: Accesses editing menus or acts as shift for alternate functions
- **Mode/Exit Button**: Changes between Single, Multi, and Sequencer modes; exit to main menu
- **Value +/- Buttons**: Increment/decrement selected values
- **Parameter < / > Buttons**: Move to previous/next parameter within a menu

### Patch Selection
- **Bank Button**: Choose RAM or ROM bank (8 of each, 64 patches/bank)
- **Patch Buttons**: Select patch numbers; use upper row for batch, lower for preset

### Additional Buttons
- **Tap Tempo**: Tap to set global tempo; [Shift+Tap]: Panic (all notes off)
- **Part Button**: Select active part (Multi/Sequencer mode)
- **Store**: Save patch or multi
- **Audition**: Preview current sound

### Knobs (General Purpose)
- **Volume**: Master output level
- **Soft Knobs (also below LCD)**: Assigns to parameters (e.g., Oscillator settings, Filter cutoff, Env, etc.)
    - [Shift + Knob]: Access 'secondary' parameters (e.g., Patch Volume, Pan, Envelope, etc.)

---

## Rear Panel Connections

| Jack           | Type           | Function                                            | Characteristics               |
|----------------|----------------|----------------------------------------------------|-------------------------------|
| MIDI In        | 5-pin DIN      | Accepts external MIDI signals (notes, CCs, clock)  | MIDI standard                 |
| MIDI Out/Thru  | 5-pin DIN      | MIDI output/Thru signal                            | MIDI standard                 |
| USB            | USB-B          | Computer connection for TI integration              | Audio/MIDI interface, driver required         |
| Left Output    | 1/4" TS        | Main audio output left                             | Line level (+4dBu nominal)    |
| Right Output   | 1/4" TS        | Main audio output right                            | Line level (+4dBu nominal)    |
| Left Input     | 1/4" TS        | Audio input left (for FX processing, etc)          | Line level                    |
| Right Input    | 1/4" TS        | Audio input right                                  | Line level                    |
| Power          | Barrel 12V DC  | Connects to supplied adapter                       | 12V DC, specific adapter only |

**Note:** There are no eurorack-type patch points or CV/gate jacks.

---

## Voltage References

- **CV Inputs/Outputs**: None (this device is not for eurorack, has no ±5V or 0-10V CV compatibility)
- **MIDI**: Standard MIDI voltage
- **USB**: Digital audio/MIDI via driver and plugin only
- **Audio IO**: Standard line level (Do NOT patch eurorack-level signals directly)

---

## Quick Operation Reference

1. **Power On/Off**: Plug in supplied adapter. Use [Shift+Part] to enter/exit standby.
2. **Patch Select**: [Bank] → choose bank (RAM/ROM via top/bottom row) → choose preset via patch buttons.
3. **Mode**: [Mode] switches between Single, Multi, Sequencer.
4. **Editing**: [Edit/Shift] + [menu button] to access menus (oscillator, filter, env, mod, FX, etc). Use soft knobs to adjust.
5. **Store Patch**: [Store] to save; follow prompts for RAM location and patch name.
6. **USB Use**: Requires driver & TI Software Suite (do **not** use USB hub!). Allows plugin use in DAW for full integration.

---

## Menu/Parameter Reference (Soft Knob Assignments)

- **Osc 1 (Classic/HyperSaw/Wavetable/Formant)**
  - Shape, Pulse Width/Wave Select/Index, Balance, Density, Detune, F-Shift, etc.
- **Osc 2**
  - Similar to Osc 1, but Value 3 = FM Amount/Sync (depending on mode)
- **Filters**
  - Cutoff, Filt 2 Offset, Saturation, Osc Volume (pre/post filter)
- **Mod**
  - LFO1/2/3 rates (free/clock)
- **Envelope**
  - Amp Attack, Filter Attack, Filter Envelope Amt
- **FX**
  - Delay Send, Reverb Send, Phaser Mix
- **Arp**
  - Mode, Pattern, Step length
- **Common**
  - Key Mode (Poly/Mono/Hold), Portamento time, Transpose

---

## Polyphony Tips

- More effects, Unison voices, complex oscillators, or reverb reduce available voices.
- Reduce complexity for more notes/polyphony.

---

## Further Help

- Press `?` in Virus Control plugin or consult included documentation for advanced editing or integration.
- Visit [Access Music Website](http://www.access-music.de) for updated OS and support.

---

*This synth is not directly compatible with eurorack systems (no CV/Gate), but can be integrated via MIDI-to-CV if needed.*

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)