# Qu-Bit — Cascade

- [Manual PDF](../../manuals/Getting_Started_Cascade.pdf)

---

[**Cascade Manual (PDF)**](https://www.qubitelectronix.com/shop/cascade)

# Cascade Eurorack Module Cheat Sheet

_Cascade by Qu-Bit Electronix: Ratcheting envelope generator, VCA, sound source, compressor, and envelope follower._

---

## BASIC OPERATION

- **Powerful envelope generator normaled to a high-fidelity analog VCA (2164-based)**
- **Ratcheting, AD, ASR, ADSR, Envelope Follower & Compressor modes**
- **Internal sound sources**: White noise, 808 hi-hat, 808 kick, hi-frequency sine
- **Snappy envelopes down to 0.5ms, envelope/CV out: 0–10V**
- **Digital control with analog signal path**

---

# 1. PANEL CONTROLS

## **Knobs**
| Knob           | Function                                                                             | CV Input   | Range                      |
| -------------- | ------------------------------------------------------------------------------------ | ---------- | -------------------------- |
| **Attack**     | Envelope attack time                                                                 | Yes        | 0.5 ms – 5 s               |
| **Decay**      | Envelope decay/release time                                                          | Yes        | 0.5 ms – 10 s (or 5 s)     |
| **Curve**      | Changes envelope curve (logarithmic–linear–exponential/response)                     | Yes        |                            |
| **Repeats**    | Ratchet (# repeats, clock multiplier, or loop)                                       | Yes        | 1–16/infinite loop, 1x–16x |
| **Level**      | Envelope output level                                                                | Yes        | 0–10V                      |
| **Offset**     | DC offset to envelope                                                                | Yes        | 0–10V                      |
| **Sustain**    | (ADSR mode only) Sustain level                                                       | No         | 0V–Level knob setting      |
| **Threshold**  | (Follower/Compressor) Signal threshold                                               | No         |                            |
| **Ratio**      | (Compressor) Compression ratio                                                       | No         |                            |

## **Buttons**
| Button    | Function                                                                                       |
|-----------|-----------------------------------------------------------------------------------------------|
| **Trig**  | Manually trigger envelope                                                                     |
| **Invert**| Flip envelope (maintains selected voltage range, Green LED on)                                |
| **Mode**  | Cycle through main modes (AD/ASR/ADSR/Follower/Compressor/Ratcheting, etc)                    |
| **Shift** | Shift for Edit/secondary functions                                                            |

---

# 2. JACKS (Inputs & Outputs)

| Jack        | Type          | Function                                                                              | Voltage Range      |
| ----------- | ------------- | ------------------------------------------------------------------------------------- | ------------------ |
| **Trigger** | Input         | Triggers the envelope/controls repeat tempo                                           | Gate/Trigger (0–5V/10V) |
| **VCA In**  | Input         | Audio input to VCA (feeds internal VCA and Follower/Compressor modes)                | Audio/CV           |
| **VCA CV**  | Input         | Overrides envelope out for external VCA control                                      | 0–10V CV           |
| **Invert**  | Input         | CV for inverting envelope                                                            | 0–10V              |
| **GATE**    | Output        | Configurable: gate/trigger (varies by Edit Function)                                 | 0–10V              |
| **VCA Out** | Output        | Audio out (external/internal source, enveloped/compressed etc.)                      | Audio/CV           |
| **ENV**     | Output        | Envelope CV out bundle                                                               | 0–10V              |

---

# 3. MODES OVERVIEW

| Mode                  | Unique Controls/Notes                                              |
|-----------------------|--------------------------------------------------------------------|
| **Ratcheting AD**     | Repeats ratcheted, clock-multiplied envelopes                     |
| **AD**                | Basic Attack/Decay envelope (optionally looped)                   |
| **ASR**               | Gate controls sustain; loopable                                   |
| **ADSR**              | Classic four-stage envelope                                       |
| **Envelope Follower** | Follows input amplitude, outputs CV/gate                          |
| **Compressor**        | Audio compression w/ virtual sidechain trigger                    |

---

# 4. EDIT FUNCTIONS (Hold **Shift**)

### **Sound Source Select**
- White Noise
- 808 Hi-Hat
- 808 Kick
- High Frequency Sine

### **Gravity Modes (Envelope Scaling)**
- No Gravity (standard)
- Amplitude Gravity (amplitude follows gravity)
- Amplitude & Time Gravity

### **Gate Output Modes**
- 6ms trigger at start of every envelope
- **EOD Mode:** Gate HIGH except during decay
- **EOA Mode:** Gate HIGH except during attack

---

# 5. QUICK PATCH EXAMPLES

- **AD Envelope**: Patch trigger source to `trigger`, take env to VCA CV or modulators.
- **VCA Control**: Patch audio to `vca in`, enveloped audio is at `vca out`.
- **Use Internal Sound Source**: Nothing patched to `vca in`—use internal sound from edit menu.
- **Compressor/Env Follower**: Patch audio to `vca in`, configure in mode, audio out at `vca out`, envelope/CV at `env`.

---

##### For more examples and advanced setups visit the [product manual PDF](https://www.qubitelectronix.com/shop/cascade).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)