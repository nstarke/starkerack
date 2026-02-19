# Tiptop Audio — MIXZ

- [Manual PDF](../../manuals/Tiptop_Audio_mixz.pdf)

---

[Tiptop Audio MIXZ Manual PDF](https://tiptopaudio.com/manuals/mixz.pdf)

# Tiptop Audio MIXZ Cheat Sheet

## Overview
- **Type:** Low-noise, dual 4-channel mixer with Tiptop Bus Mix integration
- **Formats:** Audio, CV, and Gate signals (excellent linearity)
- **Special Feature:** Tiptop Bus Mix allows cable-free connection from supported Tiptop modules via the bus board.

---

## Front Panel Reference

### Mixer A (Left Side)
- **IN 1–4** (Jacks) – 4 input channels (audio/CV/gate)
- **GAIN 1–4** (Knobs) – Per-channel gain control
- **OUT A** (Jack) – Output for Mixer A
  - **Note:** If OUT A is patched, Mixer A is isolated and not summed into Mixer B.

### Mixer B (Right Side)
- **IN 5–8** (Jacks) – 4 input channels (audio/CV/gate)
- **GAIN (Master Knob)** – Single overall gain for Mixer B
- **OUT B** (Jack) – Output for Mixer B
  - **Input Summing:** Sums IN 5–8, Mixer A output (if OUT A not patched), and Bus Mix signal (if enabled via switch).

### BUS MIX (for Tiptop Bus Mix)
- **BUS ON/OFF** (Toggle Switch) – Enables/Disables mixing of Bus Mix channel into Mixer B.
  - **Keep OFF if not using Bus Mix** to reduce system noise.
- **BUS MIX INPUT** (Hidden, Internal) – Receives signals from enabled modules over the power bus board (using rear jumpers).

---

## Inputs/Outputs & Voltage Ranges
- **All mixer inputs support audio, CV, and gate signals**
- **Inputs:** AC or DC (compatible with typical Eurorack voltage ranges, ±10V)
- **Outputs:** Standard Eurorack audio/CV levels

### Inputs
| Jack | Label    | Type        | Notes                    |
|------|----------|-------------|--------------------------|
| 1    | IN 1     | A, CV, Gate | Mixer A, Channel 1       |
| 2    | IN 2     | A, CV, Gate | Mixer A, Channel 2       |
| 3    | IN 3     | A, CV, Gate | Mixer A, Channel 3       |
| 4    | IN 4     | A, CV, Gate | Mixer A, Channel 4       |
| 5    | IN 5     | A, CV, Gate | Mixer B, Channel 1       |
| 6    | IN 6     | A, CV, Gate | Mixer B, Channel 2       |
| 7    | IN 7     | A, CV, Gate | Mixer B, Channel 3       |
| 8    | IN 8     | A, CV, Gate | Mixer B, Channel 4       |

### Outputs
| Jack | Label    | Type        | Notes                    |
|------|----------|-------------|--------------------------|
| 1    | OUT A    | Audio/CV    | Mixer A output           |
| 2    | OUT B    | Audio/CV    | Mixer B summed output    |

---

## Rear/Bus Connections

- **Bus Mix Jumpers (on compatible Tiptop modules):**
  - Place jumper on both pins to enable module signal on the bus (Bus Mix).
  - **Bus Mix is only received by MIXZ when BUS MIX switch is ON.**
  - If using multiple MIXZ modules, only activate BUS MIX on one per bus board row.

---

## Controls Summary
| Type             | Location      | Function                                                             |
|------------------|--------------|----------------------------------------------------------------------|
| 4 x Gain Knobs   | Mixer A       | Per-channel input gain for IN 1–4                                    |
| 1 x Gain Knob    | Mixer B       | Master gain for Mixer B (IN 5–8, A in, Bus Mix)                      |
| 1 x Toggle       | Mixer B       | BUS MIX ON/OFF (enables Bus Mix signals on Mixer B)                  |

---

## Usage Tips
- **Patch OUT A** if you want to use Mixer A independently from Mixer B.
- **Leave OUT A unpatched** to sum Mixer A output into Mixer B.
- **Toggle BUS MIX ON (only one MIXZ per row),** to receive bused signals from Tiptop modules.
- **Keep BUS MIX OFF** if not using Bus Mix to minimize potential noise.
- **Cannot use on Doepfer CV/GATE bus row unless BUS MIX is OFF.**
- **Max Bus Mix channels:** ~16 per bus board, subject to practical limitations.

---

## Noise & Best Practices
- **Bus Mix adds some noise**—panel inputs are quieter.
- **CP909 and similar modules may add bus noise due to internal noise sources.**
- **Only sum Bus Mix with one MIXZ per row.**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)