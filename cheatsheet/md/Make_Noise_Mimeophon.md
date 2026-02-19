# Make Noise — Mimeophon

- [Manual PDF](../../manuals/mimeophon-manual.pdf)

---

[Mimeophon Manual PDF](https://manuals.plus/m/d57a4b3e9a25ed99c839fd7a80abb03c2b680482fccb46d25c39523d9c6931b4.pdf)

---

# Make Noise Soundhack Mimeophon Cheat Sheet

Stereo, multi-zone, color audio repeater (echo, delay, looping, flanger, Karplus-Strong, chorus, more).

---

## Signal Flow Overview

- **Inputs:** L (mono), R (stereo), CV control inputs
- **Outputs:** L, R, trigger rate out

---

## Front Panel I/O, Knobs, Buttons

### Audio Inputs/Outputs
| Jack                | Function                                                            | Voltage Range |
|---------------------|---------------------------------------------------------------------|--------------|
| **L (Mono) In**     | Left channel/mono audio input (right is normalled to left)          | ~10Vpp       |
| **R In**            | Right channel audio input                                           | ~10Vpp       |
| **L Out**           | Left channel audio output                                           | ~10Vpp       |
| **R Out**           | Right channel audio output                                          | ~10Vpp       |

### Main Knobs & Associated CVs
| Panel Control    | Description                                                           | CV Input           | CV Range   | CV Notes               |
|------------------|-----------------------------------------------------------------------|--------------------|------------|------------------------|
| **Mix**          | Dry/Wet blend or attenuates Mix CV if patched                        | Mix CV             | 0–8V       | Normalled to 8V        |
| **Repeats**      | Number of repeats, sets repeat start when HOLD is engaged            | Repeats CV         | 0–5V DC    |                        |
| **Halo**         | Smears repeats in stereo space                                       | Halo CV            | 0–5V DC    |                        |
| **Zone**         | Selects delay/echo length zone (see "Zones" below)                   | Zone CV            | 0–5V DC    | Bipolar attenuverter    |
| **Color**        | Timbre/character (tape>digital>oilcan>dark/warm/BBD/etc.)            | Color CV           | 0–5V DC    | Bipolar attenuverter    |
| **Rate**         | Frequency (time) of repeats within current zone                      | Rate CV            | 0–5V DC    | Bipolar attenuverter    |
| **μRate (micro)**| Dedicated Doppler modulation (1V/oct in Zone 0; linear 1–7)          | μRate In           | ±3V        | Unity gain             |

### Time/Sync/Reverse/Loop Controls
| Label         | Type     | Function                                                        | IO Type    | Voltage/Usage           |
|---------------|----------|-----------------------------------------------------------------|------------|-------------------------|
| **HOLD**      | Button/In| Freezes the audio buffer (indefinite repeats; non-destructive)  | Gate In    | ≥2.5V = ON              |
| **REPEATS**   | Knob     | Sets # of repeats (1 to ∞) / start during HOLD                  | -          | -                       |
| **FLIP**      | Button/In| Reverses audio buffer/repeats playback (real-time or "Karplus" style in short zones) | Gate In | ≥2.5V = ON/flip      |
| **TEMPO**     | In       | External clock input (for tempo-synced delays)                  | Clock In   | ≥2.5V, 0.25–50Hz        |
| **RATE OUT**  | Out      | Triggers/clock at current repeat rate, both L + R (OR'ed)       | Gate Out   | 0V/8V pulses            |
| **SKEW**      | Button   | Skews L/R times/panning; hold to enable Ping Pong/Swap          | -          | -                       |

---

## Core Features

### Mix Section
- Set incoming signal (dry) vs repeated (wet) echoes
- When Mix CV is patched, knob acts as attenuator for the CV signal

### Zones  
- Choose delay time range (Zone 0: <2ms, to Zone 7: up to 42s)
- Instant switching: no Doppler (pitch) shift!
- Delay ranges overlap, moving up reveals ever-larger history

### Rate  
- Change repeat time *within zone* (Doppler pitch with feedback, unless clocked)
- Rate CV input modulates this; microRate is for small "vibrato/flange/chorus" mod

### Skew & Ping Pong  
- **Skew:** Offsets L/R repeat times in opposite directions for stereo spread
- **Ping Pong:** (Hold Skew, Zone window flashes) Sums input mono, bounces repeats L/R
- **Swap:** If Skew ON, holding also swaps feedback paths for phase-y stereo

### Flip  
- Reverse the buffer for "reverse" playback, or protonic buffer-distortion in short zones

### Hold  
- Freezes the buffer/loop, making it "infinite"
- Repeats knob while held sets *start point* in loop

### Color & Halo  
- **Color:** Alters echo timbre from dark/dirty to clean/bright
- **Halo:** Adds stereo spatial "smear" to echoes, especially dramatic at high settings

### Tempo Sync  
- Use TEMPO input for syncing delays to external clock
- Rate = clock division/multiplier in any zone; no pitch shift when modulating
- After two tempo pulses, module keeps timing till Rate knob is moved

---

## Voltage Controlled Inputs/Outputs

| CV Input/Output     | Function                                  | Range             |
|---------------------|-------------------------------------------|-------------------|
| Mix CV              | Wet/dry blend                             | 0–8 V             |
| Repeats CV          | Number of repeats                         | 0–5 V             |
| Halo CV             | Stereo smear                              | 0–5 V             |
| Zone CV             | Delay time zone select                    | 0–5 V             |
| Color CV            | Echo timbre                               | 0–5 V             |
| Rate CV             | Delay/repeat speed                        | 0–5 V             |
| μRate In            | Micro pitch/chorus/flange/vibrato         | ±3 V              |
| TEMPO In            | External clock                            | ≥2.5 V / 0.25–50Hz|
| HOLD, FLIP Inputs   | Trigger/gate for Hold/Flip                | ≥2.5 V = on       |
| RATE OUT            | Clock/trigger at repeat rate (OR'ed L/R)  | 0 or 8V pulse     |

---

## Input Gain Level / Hidden Function

- **Adjustment:** Hold FLIP + HOLD
- **Zone Window:**  
  - Blue = -3dB  
  - Green = 0dB (unity, default)  
  - Orange = +3dB  
  - Red = +6dB  
  (Release both buttons to confirm selection.)

---

## Quick Patch Ideas

- **Tempo Echo:** Tempo in → Z4/5, set Mix/Repeats to mid, Skew for stereo.
- **Dub Delay:** Z3–5, Halo/Color up, hand-ride Rate/Repeats for feedback washes.
- **Karplus/Flange:** Z0, fast triggers in, μRate with pitch, tweak Color/Halo for metallics.
- **Chorus:** Z1–2, slow LFO to μRate, Skew ON, high Halo/Repeats.
- **Reverse:** Flip ON, Z4 (vocals) for "reversed" speech at native cadence.
- **Sampler:** Use Hold to freeze, Zone to browse, Repeats shifts start point.
- **Sound-on-Sound:** High Repeats/Hold, manipulate Zone/Color for layered textures.

---

## Firmware Notes

- Recent firmwares add buffer clear (mp70), saves input gain on power cycle (mp82), lower noise floor (mp86).
- Check manual/website for current updates and installation: [Make Noise Firmware](http://www.makenoisemusic.com/firmware/﻿)

---

### More Resources

- [Mimeophon Manual PDF](https://manuals.plus/m/d57a4b3e9a25ed99c839fd7a80abb03c2b680482fccb46d25c39523d9c6931b4.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---