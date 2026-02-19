# Qu-Bit — Nautilus

- [Manual PDF](../../manuals/Nautilus_v1.1.3.pdf)

---

[**Download the Qu-Bit Nautilus Manual PDF**](https://www.qubitelectronix.com/_files/ugd/2d1459_1e95d666b54541e99911603995dd7c3d.pdf)

---

# Qu-Bit Nautilus Eurorack Cheat Sheet

#### **Overview**
- Stereo, underwater-inspired delay network with 8 addressable delay lines (up to 20s each)
- Multi-mode delays: Fade, Doppler, Shimmer, De-Shimmer
- Advanced feedback, filtering, distortion, CV/gate outputs

---

## **Panel and Controls**

### **Knobs**
| Knob       | Function                                                                                   | CV Input (Range)      |
|------------|--------------------------------------------------------------------------------------------|-----------------------|
| **Mix**    | Wet/dry blend                                                                              | Yes (-5V to +5V)      |
| **Resolution** | Delay subdivision/multiplier (div/mult clock rate: 512th to 2 bars)                   | Yes (-5V to +5V)      |
| **Feedback** | Number of repeats; infinite at max                                                       | Yes (-5V to +5V, attenuverter assignable) |
| **Sensors** | Number of delay lines active (1–8)                                                        | Yes (-5V to +5V)      |
| **Dispersal** | Spacing between delay lines (for polyrhythms & strums); fine tune at 1 sensor           | Yes (-5V to +5V, attenuverter assignable) |
| **Reversal** | Controls which delay lines play backwards (per delay line, not just on/off)              | Yes (-5V to +5V)      |
| **Chroma** | Selects internal effect/filter in feedback path                                            | Yes (-5V to +5V)      |
| **Depth**  | Amount of Chroma effect applied                                                            | Yes (-5V to +5V)      |

### **Buttons**
| Button             | Function                                                                              |
|--------------------|---------------------------------------------------------------------------------------|
| **Tap**            | Sets internal clock rate or enters Tap Secondary Functions (see below)                |
| **Freeze**         | Freezes (loops) current buffer—creates beat repeat/glitch effects                     |
| **Purge**          | Clears all delay lines                                                                |
| **Delay Mode**     | Selects delay mode: Fade, Doppler, Shimmer (up), De-Shimmer (down)                   |
| **Feedback Mode**  | Selects feedback network: Normal, Ping Pong, Cascade, Adrift                         |

#### **Tap Secondary Functions (Hold Tap)**
- **+ Purge:** Resets input level/delay mode/feedback mode to default
- **+ Dispersal Attenuverter:** Adjusts input gain (-12dB to +12dB, indicated by left LEDs)

---

## **Inputs & Outputs**

| Jack                      | Function/Type                                  | Range / Notes                                   |
|---------------------------|------------------------------------------------|-------------------------------------------------|
| **Left In**               | Audio Input (left, AC-coupled)                 | 10Vpp                                           |
| **Right In**              | Audio Input (right, AC-coupled)                | 10Vpp (norms from left if none plugged in)      |
| **Left Out**              | Audio Output (left)                            | 10Vpp                                           |
| **Right Out**             | Audio Output (right)                           | 10Vpp                                           |
| **Clock In**              | Gate Input for clock sync                      | Threshold: 0.4V; Range: 0.25Hz–1kHz             |
| **Freeze In**             | Gate (mirrors Freeze button)                   | Threshold: 0.4V                                 |
| **Purge In**              | Gate (mirrors Purge button)                    | Threshold: 0.4V                                 |
| **Mix CV**                | CV control of Mix knob                         | -5V to +5V                                      |
| **Resolution CV**         | CV for subdivision/multiplier                  | -5V to +5V                                      |
| **Feedback CV**           | CV control of Feedback                         | -5V to +5V (attenuverter assignable)            |
| **Sensors CV**            | CV for number of delay lines                   | -5V to +5V                                      |
| **Dispersal CV**          | CV for delay spacing                           | -5V to +5V (attenuverter assignable)            |
| **Reversal CV**           | Which delay lines are reversed                 | -5V to +5V                                      |
| **Chroma CV**             | Chroma internal FX selection                   | -5V to +5V                                      |
| **Depth CV**              | Depth/amount of effect                         | -5V to +5V                                      |
| **Sonar Out**             | Algorithmic CV or gate based on delay topology | CV: 0–5V; Gate: +5V (50% duty cycle); type set via software; patchable as mod source or clock pass-through |

---

## **Chroma Effects**
- **Blue**: Oceanic Absorption – 4-pole lowpass filter
- **Green**: White Water – 4-pole highpass filter
- **Purple**: Refraction Interference – Variable bitcrusher/sample rate
- **Orange**: Pulse Amplification – Soft/warm saturation
- **Cyan**: Receptor Malfunction – Wavefolding distortion
- **Red**: SOS – Heavy distortion

*Depth* knob controls intensity (except bitcrusher is random stepped).

---

## **Delay Modes (Button cycles)**

- **Fade** (blue): Smooth interpolation of delay time (no pitch artifacts)
- **Doppler** (green): Classic vari-speed pitch effect on time change
- **Shimmer** (orange): Octave-up pitch shift in feedback path (configurable semitones via USB)
- **De-Shimmer** (purple): Octave-down pitch shift (configurable)

---

## **Feedback Modes**

| Mode        | Behavior                                                 |
|-------------|---------------------------------------------------------|
| **Normal**  | Standard stereo matched to input                        |
| **Ping Pong**| Alternates left/right in feedback                      |
| **Cascade** | Delays in serial per channel for extra-long delay       |
| **Adrift**  | Cross-channel serial cascade/collage                    |

---

## **Other Features**
- All CV inputs are -5V to +5V; assignable attenuverters for fine CV mapping
- Onboard USB-A for firmware/configuration via Narwhal web app—no drive required to operate, any FAT32 USB sticks supported
- Lifetime free repairs (excl. cosmetic/damage abuse)

---

## **Links**
[**Full Nautilus Manual PDF**](https://www.qubitelectronix.com/_files/ugd/2d1459_1e95d666b54541e99911603995dd7c3d.pdf)  
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)