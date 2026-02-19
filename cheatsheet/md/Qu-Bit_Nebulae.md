# Qu-Bit — Nebulae

- [Manual PDF](../../manuals/Nautilus_v1.1.3.pdf)

---

```markdown
[**Qu-Bit Nautilus Manual PDF**](https://manuals.qubitelectronix.com/nautilus/Nautilus%20Manual%20v1.1.3.pdf)

# Qu-Bit Nautilus Cheat Sheet

## Overview
- **Nautilus** is a multi-tap, complex delay processor with 8 configurable delay lines and extensive modulation capabilities.
- Inspired by underwater acoustics and sonar systems, it provides stereo IO, deep feedback/routing, pitch/delay manipulation, and unique topography-based CV/gate out.

---

## Panel Controls Quick Reference

### Knobs (All CV-controllable, range: -5V to +5V unless noted)
| Knob         | Function                                                             | CV Input (range)         |
|--------------|----------------------------------------------------------------------|--------------------------|
| Mix          | Dry/Wet blend                                                        | -5V to +5V               |
| Resolution   | Delay clock div/mult from 512nd note to 2 bars                       | -5V to +5V               |
| Feedback     | Delay feedback amount, has assignable attenuverter                   | -5V to +5V               |
| Sensors      | Number of active delay lines (1–4 per channel, up to 8 total)        | -5V to +5V               |
| Dispersal    | Spacing between delay taps (attenuverter assignable)                 | -5V to +5V               |
| Chroma       | Internal FX type selector (see below)                                | -5V to +5V               |
| Depth        | Amount of effect applied by Chroma                                   | -5V to +5V               |
| Reversal     | How many (and which) delay lines are reversed                        | -5V to +5V               |

### Buttons
| Button      | Function                                                              |
|-------------|-----------------------------------------------------------------------|
| Freeze      | Locks current delay buffer (max 10s), acts as beat repeat             |
| Purge       | Clears/bypasses all delay lines                                       |
| Tap         | Sets internal clock with tap tempo; hold for secondary functions      |
| Delay Mode  | Select: Fade, Doppler, Shimmer, De-Shimmer (pitch up/down)            |
| Feedback Mode | Select: Normal, Ping Pong, Cascade, Adrift                         |

#### Tap + (Secondary Functions)
- **Tap + Purge**: Factory reset (input level, delay mode, feedback mode to default)
- **Tap + Turn Dispersal Attenuverter**: Set input gain (-12dB to +12dB, L Kelp LEDs display)

### Chroma FX Types (Color-coded by LED)
- **Blue:** Lowpass Filter (“Oceanic Absorption”)
- **Green:** Highpass Filter (“White Water”)
- **Purple:** Bitcrusher/SR Reduction (“Refraction Interference”)
- **Orange:** Saturation (“Pulse Amplification”)
- **Cyan:** Wavefolder (“Receptor Malfunction”)
- **Red:** Heavy Distortion (“SOS”)

---

## Inputs & Outputs

### Audio Inputs
| Jack             | Function                                                      | Range             |
|------------------|---------------------------------------------------------------|-------------------|
| Left Input       | Left audio input, normals to right when right is unpatched    | 10Vpp (AC)        |
| Right Input      | Right audio input                                             | 10Vpp (AC)        |

### Audio Outputs
| Jack             | Function                                                      | Range             |
|------------------|---------------------------------------------------------------|-------------------|
| Left Output      | Left channel out                                              | 10Vpp             |
| Right Output     | Right channel out                                             | 10Vpp             |

### CV & Gate Inputs
| Jack/Control     | Function                                                      | Threshold/range      |
|------------------|---------------------------------------------------------------|----------------------|
| Mix CV           | Modulate dry/wet balance                                     | -5V to +5V           |
| Resolution CV    | Modulate clock division/multiplication                       | -5V to +5V           |
| Feedback CV      | Modulate delay feedback attn/invert assignable               | -5V to +5V           |
| Sensors CV       | Modulate number of active delay lines                        | -5V to +5V           |
| Dispersal CV     | Modulate spacing between delays, attn/invert assignable      | -5V to +5V           |
| Reversal CV      | Modulate reversal of delay lines                             | -5V to +5V           |
| Chroma CV        | Modulate chroma FX type                                      | -5V to +5V           |
| Depth CV         | Modulate chroma FX amount                                    | -5V to +5V           |
| Clock In         | Sync to external clock or gate                               | Gate: >0.4V, 0.25Hz–1kHz |
| Freeze           | Gate to engage buffer freeze                                 | Gate: >0.4V           |
| Purge            | Gate to clear buffer                                         | Gate: >0.4V           |

### CV & Gate Outputs
| Jack             | Function                                                      | Range               |
|------------------|---------------------------------------------------------------|---------------------|
| Sonar            | Topography-derived stepped CV or gate output                  | CV: 0V–5V, Gate: +5V, 50% duty|

---

## Additional Features

- **USB (Type A)**: For config, updates, and power (500mA max, consider PSU!).
  - Used with "Narwhal" web configurator [here](https://nautilus.qubitelectronix.com/nautilus/configure).
  - Place **options.json** on USB drive and insert to configure.
- **Assignable Attenuverters**: Attenuverter knobs can assign to any CV input.
- **Sonar Output Config**: Options: stepped CV, master/variable clock, ping generator.

---

## Delay Modes
- **Fade**: Smooth time changes
- **Doppler**: Classic delay-time pitch bends
- **Shimmer**: Pitch up (default: +12 semitones, configurable)
- **De-Shimmer**: Pitch down (default: –12 semitones, configurable)

## Feedback Modes
- **Normal**: Stereo matches input
- **Ping Pong**: Stereo bouncing
- **Cascade**: Serial chaining of delay lines (ultra long delays)
- **Adrift**: Cascade with alternating L/R routing

---

## Quick Usage Tips

- **Freeze** creates beat repeats; **change Resolution** for rhythms.
- **Dispersal + Sensors** alter rhythmic complexity and stereo spreads.
- **Chroma + Depth** create everything from filtering to heavy distortion on repeats.
- **Reversal** gives reverse delays (per-line, not simple FX).
- **Sonar out** can modulate other modules or self-patch for wild effects.

---

## Reference

- **Power**: +12V: 151mA, –12V: 6mA
- **Size**: 14HP, 22mm deep
- **Internal/external clock sync**: Internal (tap), External (clock in)
- **Audio**: True stereo, 48kHz/24-bit, Burr-Brown converters

---

- [Original Nautilus Manual PDF](https://manuals.qubitelectronix.com/nautilus/Nautilus%20Manual%20v1.1.3.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
```