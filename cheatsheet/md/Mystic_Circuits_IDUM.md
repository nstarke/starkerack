# Mystic Circuits — IDUM

- [Manual PDF](../../manuals/IDUM Manual Draft 7.pdf)

---

[IDUM Official Manual (PDF)](https://www.mysticcircuits.com/manuals/IDUM_Manual.pdf)

# Mystic Circuits IDUM — Eurorack Cheat Sheet

**IDUM** is an intelligent gate/trigger manipulator designed to add probability, ratcheting, clock mangling, and live performance tricks to sequenced rhythms. It’s like an “effects processor” for your gates/triggers.

---

## Panel Reference

### Inputs
| Jack    | Type         | Function                             | Voltage Range      |
| ------- | ------------ | ------------------------------------ |-------------------|
| CL      | Clock In     | External clock                       | 0–5V (Trig ≥ ~1.8V)   |
| TR1–TR4 | Trigger In   | 4 external triggers/gates            | 0–5V (Trig ≥ ~1.8V)   |
| CHANCE  | CV Input     | Probability CV                       | 0–5V               |
| MODE    | CV Input     | Mode Selection CV                    | 0–5V               |
| PARAM   | CV Input     | Parameter CV                         | 0–5V               |
| LENGTH  | CV Input     | Modification length CV               | 0–5V               |
| LOOP    | Gate Input   | Toggles loop mode (see Setup)        | 0–5V               |

### Outputs
| Jack    | Type         | Function                             | Voltage Range  |
| ------- | ------------ | ------------------------------------ |-------------|
| CL      | Clock Out    | Modified clock out                   | 0–5V        |
| TR1–TR4 | Trigger Out  | 4 processed gate/trigger outs        | 0–5V        |

---

## Modes Summary (Selected by MODE Knob)

1. **Hold** — Probabilistically lengthen (CW) or skip/mute (CCW) incoming triggers.
2. **Burst** — Ratchets: Get fast bursts of triggers when a gate is received. PARAM = div/mult of clock.
3. **Multiply/Divide** — Ratchets based on distance between IN triggers. PARAM = div/mult of last trigger interval.
4. **Bouncing Ball** — Triggers speed up (CCW) or slow down (CW), simulating a bouncing ball (unquantized).
5. **Rotate** — Scrambles connections between triggers in/out. PARAM = Swap (CCW) or Rotate (CW).
6. **Gate Delay** — Delays outputs based on recent intervals. PARAM = Delay % (side to side applies delay per channel).
7. **Break** — Selects preset breakbeat-style rhythms (16 patterns via PARAM).
8. **Skip** — Manipulates clock only (not triggers): Step skipping (CCW), Clock ratchet (CW).

> *All modes: CHANCE slider sets probability of effect activating (0–100%), LENGTH sets modification length (1–8 clocks), PARAM function is mode-dependent. GATE/Trigger out is active 0–5V.*

---

## Control Summary

| Control       | Type            | Action/Behavior                                               |
| ------------- | --------------- | ------------------------------------------------------------ |
| MODE          | Large Rotary    | Select active modification mode                               |
| PARAM         | Small Rotary    | Mode-specific parameter (see table above)                     |
| LENGTH        | Slider          | Duration (steps) of modification (1–8, can be CV controlled)  |
| CHANCE        | Slider          | Probability mod applies (0–100%, can be CV controlled)        |
| REMOVE MODE   | Button (top left) | Tap: Remove (bypass) current mode · Long: Enter Setup menu |
| LOOP          | Button (center) | Tap: Toggle looper on/off (or use Loop CV input)              |
| CYCLE         | Switch (2-position) | Up: “Tracks” original clock position (for sequencer sync), Down: Output can drift out of sync |

---

### Output LEDs

- **Blue** = Incoming trigger detected
- **Red** = Modified trigger outputting
- **Pink** = Output is pass-through (not modified)

---

## Looper Mode

- **LOOP Button/Input**: Capture and repeat last 8 steps of triggers + mods. Button toggles loop, input can toggle/momentary (set up in menu).
- While loop is active, panel controls adjust playback parameters:
  * **MODE**: Choose first step (“scrub” steps when length=1)
  * **PARAM**: Loop speed
  * **LENGTH**: Loop length (1–8)
  * **CHANCE**: Probability that the stored mod is applied on each step

---

## Setup Menu (Long Press REMOVE MODE)

_Setup options can restrict step/parameter values, clock bursts, and loop gate behavior._
- **Parameter/Length Resolution**: ODD/EVEN/POW2 steps only
- **Slow Clock**: Slower clock burst for digital sequencers (LED off = slow)
- **16 Step**: (future) Expand to 16 steps
- **Split**: (future) Per-channel mode independence
- **Loop**: Set LOOP input to latching (default) or momentary (LED on)

---

## Cheat Sheet: Using IDUM

1. **Connect** clock/gates and patch outputs to drums, synth, or sequencer.
2. **Set CHANCE slider up** for more effects, down for subtlety.
3. **Set LENGTH slider** for how many steps effect stays on.
4. **Turn PARAM knob** to mode-specific setting.
5. **Select mode** with MODE knob; tap REMOVE MODE to bypass undesired modes.
6. **Engage LOOP** with center button or gate for live remixing.
7. **Use CYCLE switch** up if synchronizing a sequencer to clock out.

---

**For firmware updates, use micro-USB on rear; see the manual or Mystic Circuits GitHub for details.**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)