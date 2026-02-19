# Noise Engineering — Basimilus Iteritas Alia

- [Manual PDF](../../manuals/Basimilus Iteritas Alia Manual - Noise Engineering Documentation.pdf)

---

[**Basimilus Iteritas Alia Manual PDF**](https://manuals.noiseengineering.us/bia/)

---

# Basimilus Iteritas Alia Cheat Sheet

> **Analog-inspired digital drum/percussion & synth voice. 6 oscillators (additive/FM), extreme wavefolding, morphing waveforms, multi-algorithm, patchable.**

---

## I/O Jack Summary

| Jack         | Function                                    | Voltage Range      | Notes                      |
|--------------|---------------------------------------------|--------------------|----------------------------|
| **Trig**     | Envelope trigger input                      | > +1.8V threshold  | Accepts gates/triggers     |
| **Pitch CV** | Oscillator pitch (1V/octave)                | -2V to +5V         | Alia version only          |
| **Env Out**  | Envelope output                             | 0V to +5V          | Matches internal envelope  |
| **Out**      | Main audio output                           | 14Vpp max          | Level depends on patch     |
| **Decay CV** | Decay control CV input                      | 0 to +5V           | Offsets Decay knob         |
| **Attack CV**| Attack control CV input                     | 0 to +5V           | Offsets Attack knob        |
| **Morph CV** | Waveform morphing CV input                  | 0 to +5V           | Offsets Morph knob         |
| **Fold CV**  | Wavefolder threshold CV input               | 0 to +5V           | Offsets Fold knob          |
| **Harmonic CV**| Harmonic/partials blend/decay CV input    | 0 to +5V           | Offsets Harm knob          |
| **Spread CV**| Inharmonicity/spacing CV input              | 0 to +5V           | Offsets Spread knob        |

---

## Controls Reference

| Control           | Description                                                                |
|-------------------|----------------------------------------------------------------------------|
| **Pitch (Encoder)**| Fine (turn) & coarse (press+turn) frequency tuning                        |
| **Decay**         | Adjusts decay time for all oscillators; CV offsets this knob               |
| **Attack**        | Left: Adds noise, Center: Analog "pop", Right: Slows attack; CV offsets    |
| **Morph**         | Waveform morphs (sine → tri → saw → square); CV offsets                    |
| **Fold**          | Active wavefolder; adds harmonics; top ¼ mixes pulse train; CV offsets     |
| **Harmonic**      | Partial/harmonic decay blend; from single tone → many; CV offsets          |
| **Spread**        | Inharmonicity; spreads partials; CV offsets                                |
| **S/L/M Switch**  | Skin (additive), Liquid (additive + pitch env), Metal (FM/phase mod) algo  |
| **B/A/T Switch**  | Bass/Alto/Treble: pitch offset by octaves                                  |
| **Hit Button**    | Manual trigger for envelope/oscillator hit                                 |

---

## Sound Design Shortcuts

- **Kick**: Low Pitch/Bass, Skin or Liquid mode, quick Attack/Decay.
- **Snare**: Higher Pitch, Skin or Liquid, moderate noise via Attack left, Harm for snappier tone.
- **Hat/Cymbal**: High Pitch/Treble, Metal or Liquid for noisier, short Decay, Fold for brightness.
- **Clap**: Middle pitch, Metal mode, rapid Decay, fold for metallic snap.
- **Supersaw/Leads**: Spread and Harmonic for detuning, Morph for waveform blending, tune via Pitch input.

---

## Calibration, Firmware, & Power

- **Autocalibration:** Just power on with nothing patched to Pitch CV for self-cal (Alia only).
- **Firmware Swap:** Connect USB (back header) & use [Noise Engineering Portal](https://noiseengineering.us/portal/firmware/).
- **Power:** 2x5pin ribbon; +12V (105mA), -12V (10mA); align red stripe to -12V.
- **Pitch Input:** 1V/oct tracking.

---

## Voltage Ranges (Alia)

- Trigger in: > +1.8V
- Pitch CV: -2V to +5V
- All CVs: 0V to +5V (except pitch)
- Envelope Out: 0V to +5V
- Audio Out: up to 14Vpp

---

## Quick Reference – Controls & Jacks

```
[ In: Trig | Pitch CV | Decay CV | Attack CV | Morph CV | Fold CV | Harmonic CV | Spread CV ]
[ Out: Audio | Envelope ]
Controls: Pitch(encoder), Decay, Attack, Morph, Fold, Harmonic, Spread, S/L/M (Skin/Liquid/Metal algo), B/A/T (octave switch), Hit (manual trig)
```

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)