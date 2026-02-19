# Erica Synths — Stereo Reverb

- [Manual PDF](../../manuals/black_stereo_reverb_Manual.pdf)

---

[Erica Synths Black Stereo Reverb Manual (PDF)](https://www.ericasynths.lv/media/Black_Stereo_Reverb_manual_1_01.pdf)

---

# **Erica Synths Black Stereo Reverb – Cheat Sheet**

A high-end stereo reverb based on Tape, BBD, and Digital emulations with CV control of key parameters and 10 preset slots.

---

## **INPUTS & OUTPUTS**

| Jack/Button   | Function                                              | Voltage Range         |
|---------------|-------------------------------------------------------|----------------------|
| R IN          | Right signal audio input                              | up to 16 Vptp        |
| L (MONO) IN   | Left signal audio input (Mono normalized to R)        | up to 16 Vptp        |
| SIZE CV       | CV input – alters SIZE knob (1V/oct tracking)         | **-5V to +5V**       |
| TONE CV       | CV input – alters TONE/SPN knob                       | **-5V to +5V**       |
| FBK CV        | CV input – alters FEEDBACK knob                       | **-5V to +5V**       |
| PATCH         | CV input – switches between preset patches            | **-5V to +5V**       |
| FREEZE (Trig) | Gate/Trigger input for FREEZE/unfreeze loop           | +5V trigger/Gate     |
| R OUT         | Right audio output                                    | -                    |
| L OUT         | Left audio output                                     | -                    |


## **KNOBS, BUTTONS, SWITCHES & THEIR FUNCTIONS**

| Control                    | Description                                                           |
|----------------------------|-----------------------------------------------------------------------|
| **SIZE**                   | Adjusts simulated room size; also selects preset slots (with SHIFT)   |
| **SIZE CV (Attenuator)**   | Attenuates incoming SIZE CV signal                                    |
| **FEEDBACK**               | Adjusts reverb feedback amount (self-oscillates fully CW)             |
| **TONE/SPN**               | Sets reflective tone or "spins" reverb across stereo field            |
| **DRY/WET**                | Manually set blend; full analog dry/wet circuit                       |
| **SHIFT (button)**         | Hold for alternative actions (preset save/recall, spin control)       |
| **FREEZE (button)**        | Trigger to freeze/unfreeze buffer; also used for saving presets       |
| **SAVE (TAP/SAVE, button)**| Save preset to selected slot (hold SHIFT, rotate SIZE, hold SAVE 1s)  |
| **TYPE (toggle 3-pos)**    | Tape, BBD, "Dirty BBD" algorithms                                     |
| **MODE (toggle 3-pos)**    | Room, Hall, Cathedral (early/late reflection mixes)                   |

## **PRESET MANAGEMENT**

- **Save:** Hold SHIFT, rotate SIZE to pick slot (LEDs show slot), then hold SAVE for 1s.
- **Recall:** Hold SHIFT, rotate SIZE to slot, press TAP to load.
- **Spin reflections:** Hold SHIFT and rotate TONE/SPN knob.
- **Presets:** 10 slots, chosen via SIZE when SHIFT held (LED bar shows both levels & presets).

## **FREEZE FUNCTION**

- **Manual:** Press FREEZE button.
- **CV:** Patch gate/trigger to FREEZE jack.
- **Playback rate in FREEZE:** Use SIZE knob or SIZE CV.

## **FIRMWARE UPDATE**

1. Download firmware audio.
2. Connect audio out to L(MONO) IN, set TYPE to D.
3. Hold SHIFT + FREEZE, power on (5 right-side LEDs blink).
4. Play audio (left LEDs = input level; at least 3 on).
5. FREEZE blinks during update; SHIFT lights if error.
6. Restart rack after update.

---

## **Reference Table**

| Feature        | Voltage/CV Range         | Notes                                            |
|----------------|-------------------------|--------------------------------------------------|
| Audio inputs   | up to 16Vptp            | Left input normalled to right if mono            |
| CV ins         | -5V to +5V              | SIZE input tracks 1V/oct                         |
| Audio outs     | -                       | Stereo out                                       |
| Power Usage    | +12V: 120mA / -12V: 39mA|                                                  |
| Module Width   | 12HP                    |                                                  |
| Depth          | 35mm                    |                                                  |

---

## **Quick Start**

1. Patch audio to L(MONO) IN (R IN for stereo).
2. Output: L OUT and R OUT to mixer/speakers.
3. Select reverb TYPE and MODE.
4. Set SIZE, FEEDBACK, and TONE/SPN (use corresponding CVs for modulation).
5. Adjust DRY/WET to taste.
6. Use FREEZE to hold reverb tail/freeze buffer.
7. Save/recall presets with SHIFT + SIZE + SAVE/TAP.

---

**Manual:** [https://www.ericasynths.lv/media/Black_Stereo_Reverb_manual_1_01.pdf](https://www.ericasynths.lv/media/Black_Stereo_Reverb_manual_1_01.pdf)  
**Generated With Eurorack Processor**: [https://github.com/nstarke/eurorack-processor](https://github.com/nstarke/eurorack-processor)