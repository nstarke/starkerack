# Moog — Mother 32

- [Manual PDF](../../manuals/Mother_32_Manual.pdf)

---

[Moog Mother-32 User Manual (PDF)](https://www.moogmusic.com/sites/default/files/2019-02/Mother-32-Manual-v4.pdf)

---

# Moog Mother-32 — Eurorack Cheat Sheet

A semi-modular analog synthesizer & sequencer in 60HP. Includes 32-point patchbay, 100% analog signal path, and patchable control voltage inputs/outputs.

---

## Panel Controls

**Knobs:**
- **VCO FREQUENCY**: Coarse tune oscillator (±1 octave)
- **PULSE WIDTH**: VCO pulse wave duty cycle (2%-98%)
- **VCO MOD AMOUNT**: Modulation depth for selected mod source/destination
- **LFO RATE**: LFO frequency (0.1Hz – 350Hz normal, 600Hz max via CV)
- **MIX**: Blend VCO wave (CCW) vs Noise/EXT AUDIO (CW)
- **CUTOFF**: VCF cutoff frequency (20Hz–20kHz)
- **RESONANCE**: VCF feedback / self-oscillation (CW > 3 o’clock)
- **VCF MOD AMT**: Amount of modulation applied to VCF cutoff
- **ATTACK**: Envelope generator attack time (fast←→slow)
- **DECAY**: Envelope generator decay time (fast←→slow)
- **GLIDE**: Portamento time (smooth note transitions)
- **VOLUME**: Final output level

**Switches/Toggles:**
- **VCO WAVE**: Sawtooth or Pulse wave output
- **VCO MOD SOURCE**: LFO, EG, or External
- **VCO MOD DEST**: Frequency or Pulse Width
- **LFO WAVE**: Square or Triangle
- **VCF MODE**: Low Pass or High Pass
- **VCF MOD SOURCE**: LFO or EG
- **VCF MOD POLARITY**: + or –
- **VCA MODE**: EG or ON (drone)
- **SUSTAIN**: EG sustain enabled/disabled

**Buttons:**
- 13-note keyboard (C–C)
- 8 Step buttons (pattern editing/selection)
- LEFT/RIGHT arrows (octaves/pages)
- SHIFT
- PATTERN (pattern select)
- RUN/STOP
- HOLD/REST
- RESET/ACCENT
- REC

---

## Patchbay

### Inputs  
*(all 3.5mm unless noted, all unipolar CVs are 0 to +5V unless indicated)*

| Label         | Function                                             | Range          |
|---------------|------------------------------------------------------|----------------|
| EXT AUDIO     | Audio in (replace noise in mixer)                    | ±5V typical    |
| MIX CV        | Mixer crossfade CV                                   | –5V to +5V     |
| VCA CV        | VCA level (mod for tremolo, etc.)                    | EG: 0–+8V / ON: ±5V  |
| VCF CUTOFF    | Filter cutoff                                         | –5V to +5V     |
| VCF RES       | Filter resonance                                      | –5V to +5V     |
| VCO 1V/OCT    | Main pitch CV input                                   | –5V to +5V     |
| VCO LIN FM    | Linear FM input                                       | –5V to +5V     |
| VCO MOD       | VCO mod (overrides MOD switch, goes through attenuator) | –5V to +5V     |
| LFO RATE      | LFO speed                                            | –5V to +5V     |
| MIX 1         | VC MIX input A (default 0V)                          | –5V to +5V     |
| MIX 2         | VC MIX input B (default +5V)                         | –5V to +5V     |
| VC MIX CTRL   | VC mix crossfade                                     | –5V to +5V     |
| MULT IN       | Buffer/splitter input                                | –5V to +5V     |
| TEMPO         | Clock/Tempo in (see manual for DIN/clock/CV modes)   | –5V to +5V     |
| GATE IN       | Envelope trigger (0/+5V, up to +10V tolerated)       | 0V or +5V      |
| RUN/STOP      | Gate: run seq while +5V                              | 0V or +5V/up to +15V |
| RESET         | Gate: resets seq to step 1 while +5V                 | 0V or +5V/up to +15V |
| HOLD          | Gate: repeats current seq step while +5V             | 0V or +5V/up to +15V |

### Outputs

| Label         | Function                                             | Range          |
|---------------|------------------------------------------------------|----------------|
| VCA OUT       | Post-VCA (pre-volume)                                | ±5V            |
| NOISE         | White noise                                          | ±5V            |
| VCF OUT       | Post-filter audio                                    | ±5V            |
| VCO SAW       | Sawtooth wave                                        | ±5V            |
| VCO PULSE     | Pulse wave                                           | ±5V            |
| LFO SQUARE    | LFO square                                          | ±5V            |
| LFO TRIANGLE  | LFO triangle                                        | ±5V            |
| VC MIX OUT    | VC mixer blended output                              | ±5V            |
| MULT 1/2      | MULT outputs (buffered copy of MULT IN)              | ±5V            |
| ASSIGN        | 16 programmable outputs (clock, accent, MIDI CC, random, etc.) | See manual   |
| EG OUT        | Envelope (env gen) output                            | 0 to +7.5V     |
| KB OUT        | Keyboard/sequencer/MIDI CV out                       | –5V to +5V     |
| GATE OUT      | Keyboard/sequencer/MIDI gate (note ON)               | 0V or +5V      |

---
## Performance/Sequencer

- 32-step sequencer (8 banks x 8 patterns)
- Two input modes: Keyboard (KB) for step record/play, or Step mode for direct editing
- Pattern editing: notes, rests, ties, gate length, accents, glide, ratchets (1–4 per step), swing
- Save/recall 64 patterns (Hold SHIFT+RUN/STOP, then specify bank/location)
- MIDI IN (5-pin DIN): Notes, clock, CC, program change, etc.
- **Preset Functions:** Reset, restore factory patch, transpose, live accent/mute/ratchet, rotate patterns

---

## Typical Patch Examples

- **Basic Patch:** VCO → VCF → VCA → OUT (all internally routed)
- **Blend VCO/Noise:** MIX knob
- **Modulate PWM:** LFO to VCO MOD, switch to Pulse Width
- **Filter FM:** VCO to VCF CUTOFF input
- **Audio-rate modulation:** LFO or VCO to VCO LIN FM input
- **Process external audio:** EXT AUDIO IN, MIX knob CW

---

## Voltage & Eurorack Details

- Power: +12V DC, 230mA max ([Red Stripe] -12V, not used)
- Input CVs typically –5V to +5V (unless stated)
- Audio IO: ±5V = Euro standard
- Patch cables: 3.5mm TS

---

> **Manual Reference:** [Moog Mother-32 User Manual PDF](https://www.moogmusic.com/sites/default/files/2019-02/Mother-32-Manual-v4.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
