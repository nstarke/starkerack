# Intellijel — Atlantix

- [Manual PDF](../../manuals/atlantix_manual_2024.09.12.pdf)

---

[Atlantix Manual (PDF)](attachment://manual.pdf)

# Atlantix Eurorack Synth Voice Cheat Sheet

## Overview

- **Standalone analog dual-VCO synth voice** (VCO A + B)
- Extensive normalization and modulation routing, full patch override
- Mixer with noise/sub/aux routing, multi-mode filter (VCF/Phaser), ADSR + linear VCA, S&H/T&H, Expander
- **All signals and modulations available via jacks.**

---

## Quick Reference Guide

### 1. **VCO A** (Oscillator 1)
| Control              | Function/Range                                                  |
|----------------------|-----------------------------------------------------------------|
| **[1.1] OCTAVE A**   | 8-position coarse tune (octaves)                                |
| **[1.2] PITCH A**    | Fine tune (~±1 semitone), tracks **PITCH A IN** (1V/Oct)        |
| **[1.3] IM slider**  | FM index mod source amount (default: Envelope)                  |
| **[1.4] INDEX**      | Base FM1 amount (depth)                                         |
| **[1.5] FM2**        | FM2 depth (Exponential FM, default: Envelope)                   |
| **[1.6] PWM**        | Pulse width mod amount, default: VCO B sine or Envelope         |
| **[1.7] PWM SRC**    | PWM modulation source select                                    |
| **[1.8] PW**         | Pulse width setting (50%–~95%, full mod to 100% = silence)      |
| **[1.9] PULSE POS**  | Center/Edge pulse position switch                               |
| **[1.10] TZFM/EXP**  | Linear Thru-Zero FM or Exponential FM                          |
| **[1.11] AC/DC**     | DC = deeper, AC = accurate (only for linear FM)                 |
| **[1.12] SYNC TYPE** | Hard / None / Soft sync selection                               |
| **[1.13] SYNC SRC**  | VCO B Saw or GATE default for sync src                         |

#### VCO A Jacks
| Jack            | Function                        | Range                |
|-----------------|---------------------------------|----------------------|
| **[1.A] PITCH A IN** | 1V/Oct pitch CV input            | 0–+5V typical        |
| **[1.B] SYNC A IN**  | Sync input (Ext overrides norm)  | Logic/Audio signal   |
| **[1.C] IM IN**      | FM index mod CV (FM1 depth)      | ±5V                  |
| **[1.D] FM1 IN**     | Linear/Exp FM input              | ±5V                  |
| **[1.E] FM2 IN**     | Exponential FM input             | ±5V                  |
| **[1.F] PWM IN**     | Pulse width modulation           | ±5V                  |
| **[1.G] SINE OUT**   | Sine output                      | 10Vpp                |

---

### 2. **VCO B** (Oscillator 2 / LFO)
| Control                | Function/Range                                |
|------------------------|-----------------------------------------------|
| **[2.1] OCTAVE B**     | 8-position coarse tune                        |
| **[2.2] PITCH B**      | Fine tune, tracks **PITCH B IN** (1V/Oct)     |
| **[2.3] PITCH SRC**    | Pitch A + B or B only                         |
| **[2.4] VCO/LFO**      | Switch: audio rate or LFO (50s cycle)         |
| **[2.5] Indicator**    | Bi-color LED shows polarity/rate              |

#### VCO B Jacks
| Jack              | Function                            | Range             |
|-------------------|-------------------------------------|-------------------|
| **[2.A] PITCH B IN** | 1V/Oct pitch CV input                 | 0–+5V typical     |
| **[2.B] FM B IN**    | Exponential FM input                  | ±5V               |
| **[2.C] SYNC B IN**  | Hard sync input                       | Logic/Audio       |
| **[2.D] SPIKE OUT**  | Spike waveform out                    | 10Vpp             |

---

### 3. **MIXER**
**Mixes: VCO A Pulse/Saw, Sub, Noise, AUX1 (Tri/Square), AUX2 (Sine/Saw, route to MIXER or VCA)**  
**Sub, Noise, and AUX waveforms selectable by switches**

| Control                | Function                                         |
|------------------------|--------------------------------------------------|
| **[3.1] PULSE**        | VCO A pulse level                                |
| **[3.2] SAW**          | VCO A saw level                                  |
| **[3.3] SUB**          | SUB level, type: -1/-2/OR                        |
| **[3.4] NOISE**        | Noise level, type: WHITE/PINK                    |
| **[3.5] AUX1**         | AUX1 level, source: VCO A TRI/B SQUARE           |
| **[3.6] AUX2**         | AUX2 level, source: VCO A SINE/B SAW, routing    |
| **[3.7] AUX2 ROUTE**   | Route AUX2 pre/post filter (MIXER/VCA)           |
| **[3.8-3.11] Switches**| Set Noise/Sub/AUX1/AUX2 source types             |

#### MIXER Jacks
| Jack            | Function                        | Range                |
|-----------------|---------------------------------|----------------------|
| **[3.A] AUX1 IN**    | External input to mixer           | ±5V                 |
| **[3.B] AUX2 IN**    | External input (pre/post VCA)     | ±5V                 |
| **[3.C] MIXER OUT**  | Mixed output (default to VCF in)  | 10Vpp               |

---

### 4. **VCF / Phaser**
| Control                | Function/Range                                           |
|------------------------|---------------------------------------------------------|
| **[4.1] FM1**          | FM1 depth (default: MOD Y)                              |
| **[4.2] FM2**          | FM2 depth (default: VCO A pitch), polarity switchable   |
| **[4.3] ENV**          | Envelope FM depth, polarity switchable                  |
| **[4.4] FREQ**         | Cutoff freq                                             |
| **[4.5] Q**            | Resonance (CV offset at Q IN)                           |
| **[4.6] Mode**         | LP/BP/HP (High = always 4-pole), PHZ/Filter toggle      |
| **[4.7] 4P/2P**        | 2/4 pole (LP/BP mode only)                              |
| **[4.8] PHZ/Filter**   | Phaser/Filter switch                                    |
| **[4.9] FM2 Polarity** | Invert FM2 CV                                           |
| **[4.10] ENV Polarity**| Invert envelope CV                                      |

#### VCF Jacks
| Jack            | Function                        | Range                |
|-----------------|---------------------------------|----------------------|
| **[4.A] FM1 IN**      | Filter CV 1 (attenuated)         | ±5V               |
| **[4.B] FM2 IN**      | Filter CV 2 (attenuated)         | ±5V               |
| **[4.C] VCF IN**      | Main audio in (defaults to mixer)| 10Vpp             |
| **[4.D] Q IN**        | Resonance CV                     | ±5V               |
| **[4.E] VCF OUT**     | Main filter audio out            | 10Vpp             |

---

### 5. **ENVELOPE / VCA**
**Classic ADSR, routed to VCA, FM, PWM, filter**
| Control                   | Function/Range                                  |
|---------------------------|-------------------------------------------------|
| **[5.1] A**               | Attack time (time varies by **RATE** switch)    |
| **[5.2] D**               | Decay time                                      |
| **[5.3] S**               | Sustain level (0–5V)                            |
| **[5.4] R**               | Release time                                    |
| **[5.5] RATE**            | Envelope speed: FAST/MED/SLOW                   |
| **[5.6] ENV/GATE**        | VCA controlled by ENV or GATE                   |
| **[5.7] DRIVE**           | VCA drive: Sym/None/Asym                        |
| **[5.8] MAN GATE**        | Manual gate trigger (momentary button)          |

#### Envelope/VCA Jacks
| Jack           | Function                        | Range      |
|----------------|---------------------------------|------------|
| **[5.A] GATE IN**     | Gate trigger input                | Gate/Trigger |
| **[5.B] RETRIG**      | Retrigger (while gating)          | Trigger      |
| **[5.C] LEVEL**       | Envelope output VCA (defaults 5V) | 0–5V CV      |
| **[5.D] ENV OUT**     | Envelope out                      | 0–5V         |
| **[5.E] INV ENV OUT** | Inverted envelope                 | 0–-5V        |
| **[5.F] VCA IN**      | VCA signal in (defaults to VCF O) | 10Vpp        |
| **[5.G] OUT**         | Main audio output                 | 10Vpp        |

---

### 6. **MODS (X, Y, S&H, Noise)**
| Control                    | Description                                           |
|----------------------------|------------------------------------------------------|
| **[6.1/6.5] MOD X/Y SRC**  | 8-way selector: VCO B (Sine, Tri, Saw, Sq), S&H, Noise, VCF, (X: VCA; Y: Mixer) |
| **[6.2/6.6] UNIPOLAR**     | UP: unipolar (0–5V); DOWN: bipolar (-5–+5V)          |
| **[6.4/6.8] POLARITY**     | UP: normal, DOWN: inverted                           |
| **[6.9] HOLD SRC**         | S&H hold: VCO B Sq or Gate                           |
| **[6.10] S&H/T&H**         | S&H (sample-hold rising edge), T&H (track-hold low)  |

#### MOD Jacks
| Jack                 | Function                        | Range      |
|----------------------|---------------------------------|------------|
| **[6.A] S&H HOLD**   | S&H sample trigger/gate         | Gate/Clk   |
| **[6.B] S&H SAMP**   | S&H input (default: WhiteNoise) | ±5V        |
| **[6.C] S&H OUT**    | S&H output                      | -5V to +5V |
| **[6.D] NOISE OUT**  | Dedicated noise out             | ±5V        |
| **[6.E] MOD X OUT**  | X source out (audio or CV)      | ±5V        |
| **[6.F] MOD Y OUT**  | Y source out (audio or CV)      | ±5V        |

---

### 7. **ATLX Expander Jacks**
- **[X.A] LP OUT:** Lowpass out      | **[X.B] HP OUT:** Highpass out  
- **[X.C] BP OUT:** Bandpass out     | **[X.D] PHZ OUT:** Phaser out  
- **[X.E] SUB OUT:** Sub osc out     | **[X.F] RING OUT:** Ring mod out  
- **[X.G/H] X/Y IN:** Ring mod inputs (default: A/B Sine)  
- **[X.I-X.L] A outputs:** Sine, Tri, Saw, Pulse  
- **[X.M-X.P] B outputs:** Sine, Tri, Saw, Square  

---

## **Voltage Ranges**

- **CV Inputs:** Most use ±5V, envelopes/sources generally 0–5V, outputs 10Vpp audio
- **Gate/Trigger:** Standard 5V logic
- **Keep CV within ±12V for safety when patching external gear.**

---

## **Key Internal Normalizations**
- Patch points override normaled routing.
- Envelope, MOD X/Y, and default oscillator and modulator connections pre-wired.
- Mixer output normalled to filter, filter output normalled to VCA, VCA to OUT.

---

## **Tips**

- Use **VCO B** as audio or LFO in mod matrix; Exponential/Linear FM available
- **Drive** switch on VCA for saturation/color
- **AUX2** can be routed post-filter (VCA) for parallel processing
- **MODS**: Noise, S&H, VCO/VCF/MIX sources as mod or audio
- **Expander** gives direct outs for advanced patching (filter breakouts, ring mod, etc)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)