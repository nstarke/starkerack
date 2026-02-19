# Erica Synths — Clap

- [Manual PDF](../../manuals/CLAP_manual.pdf)

---

[Erica Synths CLAP Manual PDF](https://www.ericasynths.lv/media/Clap%20drum%20manual_1.pdf)

---

# Erica Synths CLAP — Eurorack Cheat Sheet

**High-quality, analog drum module focused on producing "clap" sounds.**

---

## Controls

| Knob       | Function                                           | Notes                           |
|------------|----------------------------------------------------|---------------------------------|
| TONE       | Master tone control for the clap                   | CV controllable                 |
| DECAY      | Sets the decay time of the clap noise              | Adjusts clap "tail"             |
| TONE CV    | Attenuator for TONE CV input                       | Controls amount of modulation   |

---

## Jacks (Inputs / Outputs)

| Jack         | Type     | Function                                                                              | Voltage Range                |
|--------------|----------|---------------------------------------------------------------------------------------|------------------------------|
| TRIG (Input) | Trigger  | Main trigger input; LED shows trigger activity                                        | Trigger above 2V             |
| ACC (Input)  | CV/Trig  | Accent input; +10V will trigger an accented (louder) clap                            | 0V to +10V                   |
| TONE CV (In) | CV       | CV input for TONE, controlled by the "TONE CV" knob; modulates master tone           | -5V to +5V                   |
| OUT (Output) | Audio    | Main audio out; clap signal output                                                    | -                            |

---

## Additional Information

- **Decay Time Range:** Approx. 120ms – 1100ms
- **Trigger Level:** >2V
- **CV Inputs (Accent, Tone CV):** –5V to +5V
- **Module depth:** 35mm
- **Power consumption:** +32mA/-30mA

---

## Usage Tips

- To generate a clap, patch a trigger to **TRIG**.
- For accented claps (louder), apply a pulse (~+10V) to **ACC**.
- Control the brightness/tone with the **TONE** knob or via CV (**TONE CV IN**).
- Shape the length of the sound using the **DECAY** knob.
- Monitor the clap audio from the **OUT** jack.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)