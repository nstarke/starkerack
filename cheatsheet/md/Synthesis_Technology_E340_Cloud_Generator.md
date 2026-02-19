# Synthesis Technology — E340 Cloud Generator

- [Manual PDF](../../manuals/E340_manual.pdf)

---

[**E340 Cloud Generator Manual (PDF)**](http://www.synthtech.com/docs/E340manual.pdf)

---

# E340 Cloud Generator (Synthesis Technology) Cheat Sheet

## OVERVIEW

- **Dual-output VCO** with up to 8 stacked "cloud" VCOs, each with detune and chaos modulation.
- Outputs super-saw and super-sine oscillations for fat, swarm-like timbres.
- No built-in CV attenuators—CVs should be attenuated externally if needed.
- CVs: -5V to +5V range for all modulation inputs.

---

## Panel Controls & Jacks Reference

### KNOBS & SWITCHES

| Control       | Function                                                                                       |
|---------------|------------------------------------------------------------------------------------------------|
| **COARSE**    | Main frequency, spans 8 octaves.                                                              |
| **FINE**      | Fine frequency, spans ~0.5 octave.                                                            |
| **FM AMT**    | Attenuates FM CV input.                                                                        |
| **SPREAD**    | Detunes cloud VCOs relative to base pitch (exponential spread, center position = off).         |
| **CHAOS**     | Adds filtered noise (FM) to detuning, making each VCO "wiggle."                               |
| **CHAOS BW**  | Sets bandwidth (speed) of chaos-noise in 6 steps (left = slow, right = fast).                  |
| **DENSITY**   | Toggles active VCO count: **2, 4, or 8** VCOs. More VCOs = reduced amplitude to avoid clipping.|

### INPUT JACKS

| Jack           | Voltage Range | Function                                                                |
|----------------|--------------|-------------------------------------------------------------------------|
| **1V/OCT CV**  | -5V to +5V   | Pitch control for all VCOs (use for standard keyboard/gate CV).          |
| **FM IN**      | -5V to +5V   | Frequency modulation, mod depth set by FM AMT knob.                      |
| **SYNC**       | >+0.25V      | Hard sync input. Resets all VCOs to -5V.                                |
| **SPREAD CV**  | -5V to +5V   | Modulates SPREAD detune, added to knob value.                            |
| **CHAOS CV**   | -5V to +5V   | Modulates CHAOS depth, added to knob value.                              |
| **CHAOS BW CV**| -5V to +5V   | Modulates CHAOS BW (speed), added to knob value.                         |

### OUTPUT JACKS

| Jack         | Voltage Range | Function                         |
|--------------|--------------|----------------------------------|
| **SAW OUT**  | -5V to +5V   | Sum of detuned saw waves (DC-coupled). |
| **SINE OUT** | -5V to +5V   | Sum of detuned sine waves (DC-coupled).|

---

## QUICK START

1. **Patch 1V/OCT** to sequencer/keyboard CV.
2. **OUT to VCA/Mixer:** Choose **Saw Out** or **Sine Out**.
3. **Tune** with coarse/fine knobs.
4. **Set DENSITY:** Choose 2, 4, or 8 VCOs.
5. **SPREAD:** Turn up for "cloud" detune effect; patch external CV to sweep amount.
6. **CHAOS/CHAOS BW:** Add and shape random "wiggle" for extra thickness.
7. **Sync:** For hard-edge tones, patch clock/square LFO to SYNC.
8. **FM:** Patch external CV source/noise/LFO/another VCO for classic FM effects. Use FM AMT for depth.

---

## POWER

- **Eurorack:** +12V @ 55mA, -12V @ 25mA.
- **MOTM:** +15V @ 45mA, -15V @ 15mA.
- **All panel CV inputs:** -5V to +5V nominal, DC to 8kHz.

---

## TIPS

- Overdriving inputs can shift pitch—keep input levels within -5V/+5V if possible.
- Each control voltage input is summed with associated knob for total effect.
- Use external attenuators if finer CV control is needed.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)