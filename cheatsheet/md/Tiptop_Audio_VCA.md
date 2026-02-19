# Tiptop Audio — VCA

- [Manual PDF](../../manuals/Tiptop Audio VCA user manual_6.pdf)

---

[Tiptop Audio VCA Manual PDF](http://tiptopaudio.com/vca/)

---

# Tiptop Audio VCA Eurorack Cheat Sheet

A single-channel, variable-slope Voltage Controlled Amplifier (VCA) with full morphing between Logarithmic, Linear, and Exponential curves. Suitable for clean amplification, modulation, FM index control, audio/CV mixing, and sidechaining.

---

## Controls Overview

| Control     | Type   | Description                                                                                                   |
|-------------|--------|---------------------------------------------------------------------------------------------------------------|
| **LEVEL**   | Knob   | Sets output volume (post-VCA gain). Useful for gain staging or matching shapes.                               |
| **SHAPE**   | Knob   | Continuously morphs the CV response curve: Logarithmic ← Linear → Exponential.                               |
| **OFFSET**  | Knob   | Adds offset to CV, manually opens/closes the VCA, or shifts bipolar mod sources for full bipolar modulation.   |
| **CV IN**   | Knob   | Attenuates incoming CV (from CV IN jack). Helps prevent CV clipping.                                          |

---

## Input/Output Reference

| Jack        | Type   | Function                                                                             | Voltage Range       |
|-------------|--------|--------------------------------------------------------------------------------------|---------------------|
| **CV IN**   | Input  | CV control of the VCA or for Amplitude Modulation with audio-rate CVs.               | ±10V recommended    |
| **Audio IN**| Input  | Audio or CV signals to be amplified/processed.                                       | Up to ~20Vpp*       |
| **Audio OUT**| Output | Final amplified/processed audio/CV signal.                                            | Up to ~20Vpp*       |

\*Precise limits not stated, but standard for Eurorack; incoming signal clipping is indicated with a red LED.

---

## LED Indicators

| LED             | Location   | Indicates                         |
|-----------------|------------|-----------------------------------|
| **CV Clip LED** | Panel      | CV IN signal is clipping          |
| **Audio Clip LED** | Panel   | Audio IN signal is clipping       |

---

## Typical Voltage Ranges

- CV IN: Designed for ±10V (unipolar envelopes, LFOs, or bipolar LFOs). Envelope peaks should avoid clipping as indicated by the CV LED.
- Audio IN: Typical Eurorack audio (±5V, 10Vp-p).

---

## Key Functions

- **Dynamic Volume Control**: Control over audio amplitude via envelopes, LFOs, sequencers, etc.
- **CV Attenuation and Offset**: Tune incoming control signals for mod depth and baseline.
- **SHAPE Morphing**: Sweep through log/lin/exp responses for nuanced dynamics or CV shaping.
- **Amplitude Modulation (AM)**: Use audio-rate CVs for audio AM effects.
- **FM Index Control**: Use VCA to modulate amount of FM sent to other oscillators or destinations.
- **Sidechaining**: Invert envelope CV for “ducking” effects.
- **FX Send Automation**: Dynamically automate effect sends.

---

## Quick Start

1. Set SHAPE to center (linear).
2. Patch audio to Audio IN, Audio OUT to sound system.
3. LEVEL to max, OFFSET up to bring signal through.
4. Patch envelope/LFO to CV IN, adjust CV IN knob for modulation amount.
5. Adjust SHAPE to hear curve differences.

---

## Calibration Trimmers (on module rear, factory set)

| Trimmer      | Function                                                         |
|--------------|------------------------------------------------------------------|
| BIAS ADJ TR2 | Matches output level across shape morphing                      |
| OTA OFFSET T1| Minimizes DC offset at output                                   |
| CV OFFSET T3 | Minimizes bleed when VCA is “closed”                            |

---

## Patch Tips

- **Linear:** Best for controlling CV/mod signals.
- **Exponential:** Best for audio amplitude (matches human hearing).
- **Logarithmic:** Creative modulation source shaping or special effects.
- **OFFSET**: Center for bipolar LFOs, LEFT for silence, adjust for sustained S&H/no silence envelopes.
- **CV IN+LEVEL:** Both affect final gain; use together for precise control.

---

## Example Uses

- **Envelope-controlled VCA**: Patch envelope to CV IN to shape amplitude of incoming audio.
- **Modulated Filter FM**: VCA controls modulation amount into filter cutoff.
- **Audio-rate AM/FM**: Send VCO to CV IN for ring/AM/FM effects, index controlled by OFFSET or envelope.
- **Automated FX Sends**: Sequence wet/dry FX amounts via CV automation.
- **Sidechaining**: Invert envelope for ducking audio during drum hits.

---

## Module Inputs/Outputs & Controls Table (Summary for Quick Reference)

| Label   | Jack/Control | Function                            | Typical Voltage Range         |
|---------|--------------|-------------------------------------|------------------------------|
| LEVEL   | Knob         | Output level                        | N/A (audio gain)             |
| SHAPE   | Knob         | Morph between log/lin/exp curves    | N/A                          |
| OFFSET  | Knob         | Adds DC to CV in                    | N/A                          |
| CV IN   | Knob         | Attenuates CV input                 | N/A                          |
| CV IN   | Jack         | Control voltage input (CV or audio) | ±10V                         |
| Audio IN| Jack         | Audio or CV in                      | ±5V to ±10V typical          |
| OUT     | Jack         | Audio or CV out                     | Module powered output        |

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)