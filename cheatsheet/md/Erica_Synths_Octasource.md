# Erica Synths — Octasource

- [Manual PDF](../../manuals/black_octasource_manual.pdf)

---

[Erica Synths Black Octasource Manual (PDF)](https://www.ericasynths.lv/media/BLACK_OCTASOURCE_manual_1.02.pdf)  <!-- This is a direct link to the official manual for reference. -->

---

# Erica Synths Black Octasource Cheat Sheet

## Overview

The **Erica Synths Black Octasource** is an ultra-flexible LFO with 8 simultaneous outputs, advanced phase and waveform morphing, and extensive CV control. It can be the “heart and brain” of modulation in your modular system.

---

## Controls, Inputs & Outputs

### Front Panel Diagram (Reference)
- **RATE (Large Knob):** Manual LFO speed control. At 12 o’clock, freezes current values on outputs. CW increases LFO rate and shifts phase CW; CCW increases rate and shifts phase CCW.
- **WAVE (Knob):** Selects principal waveforms and morphs between them. In MULTI mode, shifts waves between outputs.
- **MULTI/SINGLE (Toggle Switch):**
  - **MULTI:** 8 different waves on 8 outputs, WAVE knob shifts assignment.
  - **SINGLE:** Same wave on all outputs, phase-shifted (by 45° steps or CV control).
- **FM LEVEL (Small Knob):** Attenuates FM control voltage (see FM IN).
- **OUTPUT LEDs:** Bi-color, display signal level and output mode.
- **SYNC (Jack):**  Clock input to sync LFO frequency externally (disables RATE except at freeze).
- **FM IN (Jack):**  Frequency modulation input (-5V to +5V).
- **WAVE CV (Jack):**  Voltage control of waveform selection/morphing (-5V to +5V).
- **PHASE CV (Jack):**  Voltage control of phase shifting per output (-5V to +5V).
- **OUTPUTS (8x Jacks):** Phase shifted/unshifted LFO outputs (-5V to +5V bipolar, switchable to 0V to +5V unipolar).

---

## Input/Output Voltage Ranges

| Jack        | Function                  | Voltage Range      |
|-------------|---------------------------|-------------------|
| SYNC        | LFO Sync Input            | Clock / Trigger   |
| FM IN       | LFO FM Control Voltage    | -5V to +5V        |
| WAVE CV     | Wave Selection CV         | -5V to +5V        |
| PHASE CV    | Phase Shift CV            | -5V to +5V        |
| OUTPUTS     | LFO Output (default)      | -5V to +5V (bipolar) <br>0V to +5V (unipolar, see below) |

---

## Features Reference

- **LFO Rate:** 0.03 Hz – 30 Hz
- **Output Amplitude:** 10Vpp (bipolar: -5V to +5V, unipolar: 0V to +5V selectable, see below)
- **CV Inputs:** All full sweep at ±5V
- **8 Simultaneous Outputs:** Each 45° phase apart (or 8 different waveforms in MULTI mode)
- **Waveforms:** Sine, ramp, inverted absolute sine, triangle, pulse, absolute sine, saw, S&H (plus morphing between)
- **Sync:** External clock input for LFO rate
- **Freeze:** Set RATE to 12 o’clock in Sync mode or for output freeze
- **LED Indicators:** Show signal amplitude and mode
- **Phase, Wave, Rate:** All manually and CV controllable

---

## Unipolar/Bipolar Output Mode

- **Switching Output Mode:**
  1. Set RATE knob to 12 o’clock ("freeze" position).
  2. Flip the MULTI/SINGLE switch **6 times**.
  - **Unipolar (0V to +5V):** All LEDs blink same color.
  - **Bipolar (default, -5V to +5V):** LEDs blink two colors.

---

## Safety & Other Notes

- DO NOT use in wet or humid environments.
- DO NOT expose to temps above +50°C or below -20°C.
- Only ship in original packaging for warranty/repair.

---

## Quick Workflow

1. **Patch Outputs:** Use any of the 8 outputs for LFO modulation.
2. **Rate:** Adjust main speed with RATE knob or apply clock to SYNC jack for external sync.
3. **Waveform:** Manually select/morph between waveforms with WAVE knob or via CV.
4. **Phase:** Control phase rotation per output with knob or CV.
5. **MULTI/SINGLE:** Choose mode for “8 different” waves or “1 shifted wave.”
6. **FM/Modulation:** Patch into FM IN for CV LFO frequency control, attenuate with FM LEVEL.

---

## Useful Links

- [Erica Synths Black Octasource Manual PDF](https://www.ericasynths.lv/media/BLACK_OCTASOURCE_manual_1.02.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)