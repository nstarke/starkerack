# Doepfer — A-140

- [Manual PDF](../../manuals/A140_man.pdf)

---

[Doepfer A-140 ADSR Manual (PDF)](https://doepfer.de/a100man/a140_man.pdf)

---

# Doepfer A-140 ADSR Cheat Sheet

The **Doepfer A-140 ADSR** is a classic envelope generator for the Eurorack modular system. It outputs a voltage envelope shaped by Attack, Decay, Sustain, and Release (ADSR) stages, and is a modulation source for VCAs, VCFs, VCOs, and more.

---

## Quick Operation

1. **Connect a Gate** (from sequencer, keyboard, LFO, etc.) to the **Gate** ( ! ) input or use internal INT.GATE.
2. **Set A, D, S, R** knobs to your desired envelope shape.
3. **Patch Output** ( § or $ ) to the destination to modulate (VCA, VCF, etc.).
4. (Optional) Use **Retrig** ( " ) to re-trigger the envelope while the gate is high (great with LFOs/clocks).
5. **Select envelope time range** (H, M, L) with the 3-way switch.

---

## Panel Control Reference

| # | Control/Input      | Type           | Description                                         | Range / Details                  |
|---|--------------------|----------------|-----------------------------------------------------|----------------------------------|
| 1 | **A (Attack)**     | Knob           | Sets the attack time                                | 0~10; ms to minutes (L-H range)  |
| 2 | **D (Decay)**      | Knob           | Sets the decay time                                 | 0~10; ms to minutes (L-H range)  |
| 3 | **S (Sustain)**    | Knob           | Sets the sustain level (hold voltage)               | 0~10; 0V to max (approx. +8V)    |
| 4 | **R (Release)**    | Knob           | Sets the release time                               | 0~10; ms to minutes (L-H range)  |
| 5 | **ADSR Control**   | LED            | Visual indicator of envelope activity               | -                                |
| 6 | **Time Range**     | 3-way Switch   | Sets overall envelope time scale                    | H (hours), M (mid), L (<100 µs)  |

---

## Inputs & Outputs

| Symbol | Jack Name      | Type      | Description                                      | Typical Range              |
|--------|---------------|-----------|--------------------------------------------------|---------------------------|
| !      | Gate          | Input     | Starts envelope on rising edge                   | Threshold: +0.8V / > 2V   |
| "      | Retrig        | Input     | Retriggers attack while gate is high              | >+2V pulse recommended    |
| §, $   | Output        | Output    | Normal (positive) envelope voltage               | 0V (rest) to +8V typ, up to +12V |
| %      | Inverse Output| Output    | Inverted envelope voltage                        | 0V (rest) to -8V typ      |

*Each output simultaneously provides the same envelope. Both outputs ( §, $ ) are available for patch flexibility.*

---

### Voltage Ranges

- **Envelope Out/Inverted Out**:  
  - Normal: 0V (rest) up to approx. +8V (max, up to +12V)  
  - Inverse: 0V (rest) down to approx. -8V (min)
- **Gate/Trig Inputs**:  
  - Triggered at +0.8V ("gate on" >+2V safe)
  - Retrig: >+2V pulse recommended

---

## User Examples

- **ADSR → VCA:**  Volume envelope for dynamic articulation.
- **ADSR → VCF:**  Moving filter envelope for sweeps.
- **ADSR → VCO PWM:**  Modulates pulse width, giving timbral movement.
- **ADSR → VCO Pitch:**  Creates pitch swoops/attack transient effects.
- **ADSR → Effects (Phase, LFO freq):**  Modulates FX or LFO for evolving patches.

---

## Patch Notes

- Gate input is normalled to INT.GATE (from system bus/keyboard) unless a cable is inserted.
- Retrig re-triggers attack phase on each pulse received, while gate is high.
- Use the three time ranges to fit applications from percussive plucks (L), standard synth envelopes (M), to very slow pads (H).
- Inverse output can be used for complementary modulation.

---

**Reference: [Doepfer A-140 ADSR Manual (PDF)](https://doepfer.de/a100man/a140_man.pdf)**

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)