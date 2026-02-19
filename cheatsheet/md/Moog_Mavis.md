# Moog — Mavis

- [Manual PDF](../../manuals/MAVIS_MANUAL_V2_06.27.2022.pdf)

---

[Moog Mavis User Manual PDF](https://www.moogmusic.com/sites/default/files/2022-05/Manual_Mavis_v2.2_WEB.pdf)

---

# Moog Mavis Eurorack Module Cheat Sheet

## Power & Installation
- **Eurorack Power**: 44 HP wide; draws 175mA from +12V only (does not use -12V)
- Connect 10-pin ribbon (pin 1/-12V red stripe UP, but only uses +12V)
- Max depth: ~26mm

---

## Panel Controls

### Oscillator (VCO)
- **PITCH**: Coarse pitch (8Hz – 8kHz)
- **VCO WAVE**: Fade Saw⬄Pulse
- **PULSE WIDTH**: Pulse duty (5%-50%)
- **VCO MOD MIX**: LFO⬄EG modulation mix to VCO
- **PITCH MOD AMT**: Mod amount to Pitch
- **PWM AMT**: Mod amount to Pulse Width

### Filter (VCF)
- **CUTOFF**: 4-pole LPF cutoff (30Hz–20kHz)
- **RESONANCE**: Add resonance/self-oscillation
- **VCF MOD MIX**: LFO⬄EG modulation mix to filter
- **VCF MOD AMT**: Bipolar mod amount to Cutoff (center=off, left=invert, right=normal)

### LFO
- **LFO RATE**: 0.1–550Hz (audio-rate capable)
- **LFO WAVE**: Fade Tri⬄Square

### EG (Envelope Generator)
- **ATTACK**: (0.8ms–5.5s)
- **DECAY**: (3ms–18s)
- **SUSTAIN**: 0–8V level
- **RELEASE**: (3ms–18s)

### VCA
- **VOLUME**: Output/headphones level
- **VCA MODE [TOGGLE]**: DRONE (on)/normal EG control

### Keyboard Section
- **13-button C-to-C keyboard**
- **KB SCALE**: 1V/octave (1 octave) to 5V/octave (5 octaves)
- **GLIDE**: Portamento time (max ~9s)

### Utilities
- **FOLD**: Amount of wave folding (wavefolder)
- **ONE LVL**: Mixer ch.1 Level (ONE input)
- **ATTENUATOR**: Attenuate +5V or input signal

---

## Patchbay Jack Reference

| Label     | Type     | Row/Col | Function & Voltage Range                  |
|-----------|----------|---------|-------------------------------------------|
| /VCA      | Out      | R1;C1   | Main audio/headphone out: -5V/+5V         |
| KB CV     | Out      | R1;C2   | Keyboard 0–1V (CCW KB scale), 0–5V (CW)   |
| FOLD IN   | In       | R1;C3   | Wavefolder input: -5V/+5V                 |
| 1V/OCT    | In       | R2;C1   | Pitch CV: -5V/+5V                         |
| PWM       | In       | R2;C2   | Pulse Width CV: -5V/+5V                   |
| ONE (-5)  | In       | R2;C3   | Mixer ch.1 in: -10V/+10V                  |
| ONE       | Out      | R3;C3   | Mixer ch.1 out: -8V/+8V                   |
| LFO RATE  | In       | R3;C1   | LFO rate CV: -5V/+5V                      |
| CUTOFF    | In       | R3;C2   | Filter cutoff CV: -5V/+5V                 |
| TWO       | In       | R4;C3   | Mixer ch.2 in: -10V/+10V                  |
| GATE      | In       | R4;C1   | EG gate in: 0V=OFF, +5V=ON (1.5–3.5V)     |
| VCA CV    | In       | R4;C2   | VCA level: 0V–8V                          |
| ONE+TWO   | Out      | R5;C3   | Mixer sum out: -8V/+8V                    |
| VCO       | Out      | R5;C1   | Raw oscillator out: -5V/+5V               |
| S+H (VCO) | In       | R5;C2   | S+H sample input: -5V/+5V                 |
| LFO       | Out      | R6;C1   | LFO out: -5V/+5V                          |
| S+H GATE  | In       | R6;C2   | S+H clock in: 0–+5V, rising edge          |
| ATTN (+5) | In       | R6;C3   | Attenuator in: -10V/+10V                  |
| EG        | Out      | R7;C1   | Envelope out: 0–8V                        |
| S+H       | Out      | R7;C2   | S+H out: -5V/+5V                          |
| ATTN      | Out      | R7;C3   | Attenuator out: -10V/+10V                 |
| MULT      | In       | R8;C1   | Passive mult in: any CV/audio             |
| MULT 1    | Out      | R8;C2   | Passive mult out (copy of MULT in)        |
| MULT 2    | Out      | R8;C3   | Passive mult out (copy of MULT in)        |

---

## Internal Modules (Patchable via Patchbay)

- **Wavefolder**: Patch-in via FOLD IN, enable with FOLD knob.
- **Mixer**: Inputs: ONE (-5), TWO; Output: ONE+TWO (balance ONE LVL knob).
- **Attenuator**: ATTN (+5) in, ATTN out, set amount via knob.
- **Sample+Hold**: S+H (VCO) in, S+H GATE in, S+H out. Defaults: sample VCO, gate from LFO.
- **MULT**: 1 in, 2 outs.

---

## Patch Examples (Quick Reference)
- **Engage Wavefolder**: VCO out → FOLD IN
- **Add S+H filter modulation**: S+H out → CUTOFF in
- **Mixer as audio sum**: LFO (audio rate) → ONE in, VCO out → TWO in, ONE+TWO out → signal path
- **MULT**: One source (e.g., S+H) to two destinations (e.g., pitch and cutoff)
- **External pitch**: CV/gate controller → 1V/OCT in & GATE in

---

## Voltage Ranges (Quick Reference)
- **Patchbay Inputs**: Most -5V/+5V (mixer/attenuator -10V/+10V)
- **Pitch CV**: 1V/oct standard
- **Gate in**: rises >3.5V triggers EG, drops <1.5V releases EG
- **All outputs (audio/CV)**: labeled per jack above

---

For more detail, see the [official manual PDF](https://www.moogmusic.com/sites/default/files/2022-05/Manual_Mavis_v2.2_WEB.pdf).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)