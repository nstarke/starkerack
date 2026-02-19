# Vermona — Melodicer

- [Manual PDF](../../manuals/melodicer manual en 1.1 web.pdf)

---

[**Download the full meloDICER Manual (PDF)**](https://www.vermona.com/fileadmin/vermona/downloads/manuals/melodicer_user_guide_en.pdf)

---

# Vermona meloDICER – Eurorack Cheat Sheet

**meloDICER** is a stochastic (probability-based) melody and rhythm sequencer module for Eurorack, with intuitive per-step and probability controls.

---

## Inputs and Outputs — Reference

| Jack         | Function                  | Voltage Range           | Description                                                        |
|--------------|---------------------------|-------------------------|--------------------------------------------------------------------|
| **CLK IN**   | Clock input               | 0…+12V (Thresh: +2V)    | External quarter note clock. Overrides internal clock.              |
| **CV IN 1**  | Pitch control input       | 0…+5V (max 12V)         | Adds/transposes sequence or modulates pitch range.                  |
| **CV IN 2**  | Rhythm control input      | 0…+5V (max 12V)         | Modulates rhythm section parameters (except NOTE VALUE/VARIATION).  |
| **GATE IN 1**| Gate/trig input           | 0…+12V (Thresh: +2V)    | Various assignable functions (toggle dice, re-dice, restart, etc).  |
| **GATE IN 2**| Gate/trig input           | 0…+12V (Thresh: +2V)    | Mutes sequencer, and other assignable functions.                    |
| **GATE OUT** | Gate out                  | +10V                    | Triggers your envelope/voice.                                       |
| **1V/OCT**   | CV out (pitch sequence)   | 0…+5V                   | Standard pitch voltage output.                                      |

---

## Controls

### Knobs & Sliders

- **NOTE VALUE** (Knob): Sets base step length (1/16, 1/8, quarter note, etc.)
- **VARIATION** (Knob): Probability of alternate step lengths (left = longer, right = shorter).
- **LEGATO** (Knob): Probability of notes sliding (no retrigger) between steps.
- **REST** (Knob): Probability of silent (rest) steps.
- **RANGE (Faders/Sliders 2 & 8):** Set lowest and highest note of scale.
- **SEMITONE FADERS (C–B):** Probability of each semitone in pattern (higher = more likely).
- **Rotary Encoder:** Sets pattern position, chooses banks/steps in menus.
- **Pattern Length Buttons (to right of encoder):** Set first and last step of pattern range (hold & turn).

### Buttons

- **DICE (Rhythm & Melody):** New random dice for rhythm/melody pattern. Hold to switch to “realtime” random.
- **M (Mute):** Mutes gate out. Blinks when muted.
- **LOCK:** Freeze parameter updates—edits will not be applied until unlocked.
- **S (Save):** Store current pattern in memory slot.
- **L (Load):** Recall pattern.
- **E (Edit):** Access/edit global parameters and input/gate routing.

### LEDs

- Around encoder: Shows pattern position in 16 steps.
- Button LEDs: Indicate active settings, modes, and states.

---

## Operating Basics

1. **Connect Gate Out** to your voice’s envelope input and **1V/OCT Out** to your oscillator’s pitch input.
2. **Set initial faders/knobs** (see manual fig. 1).
3. **Clock internally** (TAP button) or externally (CLK IN, 0–+12V, 1 PPQN).
4. **Set NOTE VALUE** and optionally add VARIATION.
5. **Adjust LEGATO & REST** for expressive/random rhythms.
6. **Set octave and desired scale** using lowest (2) and highest (8) faders and semitone faders.
7. **Dice pattern(s)**: Tap DICE (rhythm/melody) for new random value set (or hold for realtime probability).
8. **Store/Recall patterns**: Use S/L and rotary encoder.
9. **LOCK mode:** Toggle LOCK to stage edits before applying.

---

## Pattern and Storage

- **Patterns** are the sum of all knob, fader, step, and mode settings, NOT explicit sequences.
- Storage: Up to 16 user patterns.
- **Saving:** S → Select slot (encoder) → Press encoder.
- **Loading:** L → Select slot → Press encoder. Loads in LOCK mode.

---

## Modes (Hold E, then A/B/C/D):

- **A:** Full sequencer — default & all features.
- **B:** Seq+Gate (melody from melody section, triggered by gate at GATE IN 1).
- **C:** Quantizer 1 (CV IN 2 quantized by fader scale, outputs 1V/OCT).
- **D:** Quantizer 2 (gate at GATE IN 2 determines sample/hold of quantized CV IN 2).

---

## Edit Menu (press E)

- Use encoder (1–7) to scroll; A/B/C/D to set options per parameter.
- Typical assignments:
    - **CV IN 1:** Add/Transpose sequence, modulate range
    - **CV IN 2:** Modulate rhythm section (except NOTE VALUE/VARIATION in firmware R19)
    - **GATE INs:** Toggle Dice (rhythm/melody), Re-dice, Mute, Restart
    - **MUTE mode:** Continue (A) / Restart pattern (B)
    - **NOTE VARIATION:** Limit allowed step lengths for VARIATION knob

---

## Quick Reference: voltages

- **Inputs:** 0…+5V for CV, up to +12V signal tolerated, +2V threshold for triggers/gates.
- **Outputs:** 0…+5V 1V/OCT pitch, +10V gate.

---

## Quick Tips

- **Internal clock = TAP tempo.** External clock overrides.
- **Mute:** Press M (button B) or GATE IN 2.
- **Pattern restart:** Push rotary encoder or GATE IN 1 (if assigned).
- **LOCK mode:** Stage edits before applying.
- **Probability faders:** Only semitones within pitch range (set by 2/8) are available.
- **Realtime mode:** Hold DICE to enable, disables set pattern and generates on the fly.

---

**Manufacturer:** [Vermona – meloDICER product page](https://www.vermona.com/en/products/modules/product/melodicer/)

---

[**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)