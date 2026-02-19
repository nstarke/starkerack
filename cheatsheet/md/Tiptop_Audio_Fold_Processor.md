# Tiptop Audio — Fold Processor

- [Manual PDF](../../manuals/Tiptop_Audio_foldprocessor.pdf)

---

[Tiptop Audio Fold Processor Manual (PDF)](https://www.tiptopaudio.com/manuals/TIPTOP_FoldProcessor_Manual.pdf)

---

# Tiptop Audio Fold Processor — Cheat Sheet

## Overview

The Fold Processor is an analog wavefolder and sub-octave generator. It expands simple waveforms into complex harmonics and creates subdivided outputs for thick, harmonically rich tones.

## Quick Start

1. **Patch a sine wave** (from an oscillator or self-oscillating filter) into **IN1**.
2. **OUT:** Connect Fold OUT to your speakers.
3. Sweep the **FOLD** knob to hear folding; adjust **INJECT** to offset the waveform.
4. Experiment with **CV control** over FOLD/INJECT via their respective jacks, using the ATTEN knobs to dial in modulation amount.
5. Try the **SUBDIV OUT** for added lower octave tones; mix subdivisions using the +1, +2, +3, +4 knobs.

---

## Jack Reference

| Jack           | Type        | Description                                                      | Voltage Range (if applicable)            |
|----------------|-------------|------------------------------------------------------------------|------------------------------------------|
| **IN1**        | Input (audio)  | Main audio input for wavefolding/subdivision.                   | ±5V typical eurorack level               |
| **FOLD CV**    | Input (CV)     | Voltage control over amount of folding.                         | 0–+5V (common eurorack CV)               |
| **INJECT CV**  | Input (CV)     | Voltage control over inject offset.                             | 0–+5V                                    |
| **OUT**        | Output (audio) | Folded audio signal output.                                     | ±5V typical                              |
| **SUBDIV OUT** | Output (audio) | Sub-divided output; outputs a blend of original and suboctaves. | ±5V typical                              |

---

## Control Reference

- **FOLD (knob):** Sets amount of wavefolding applied.
- **FOLD ATTEN (knob):** Attenuates/mixes external CV to FOLD parameter.
- **INJECT (knob):** Offsets input signal for further waveshaping.
- **INJECT ATTEN (knob):** Attenuates/mixes external CV to INJECT parameter.
- **1, 2, 3, 4 (DIVISION GAIN knobs):** Level controls for each suboctave mixed into SUBDIV OUT. Suboctaves are spaced at 1-octave intervals.

---

## Usage Tips

- Use pure waveforms (sine, triangle) for classic wavefolding.
- Feed the SUBDIV OUT with all/selected sub-octave gains for bass-rich or complex tones.
- Inject drums, samples, or filtered audio for analog distortion/lo-fi effects.
- Place before/after filters, or patch OUT to a VCO’s FM input for feedback/FM craziness.

---

## Voltage Ranges

- **Audio In/Out:** ±5V standard eurorack
- **CV Inputs (FOLD/INJECT):** 0–+5V unipolar recommended, but will respond to wider ranges with additional effect

---

## Patch Ideas

- *Wavefolder:* VCO sine > IN1, OUT > Mixer.
- *Sub-octaver:* VCO > IN1, SUBDIV OUT > Mixer, use 1/2/3/4 controls to mix octaves.
- *Distortion:* Drum sample > IN1, OUT > Mixer.
- *FM Madness:* OUT > VCO FM IN.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)