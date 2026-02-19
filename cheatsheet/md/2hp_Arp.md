# 2hp — Arp

- [Manual PDF](../../manuals/2hp_Arp_Manual_2023.pdf)

---

[Download the 2hp Arp Manual (PDF)](https://twohp.com/modules/arp)

---

# 2hp Arp Cheat Sheet

**Gate-Driven Arpeggiator Module (2HP, Depth: 45mm)**

## **Inputs & Outputs Reference**

| Jack             | Function                                                                               | Voltage Range   |
|------------------|----------------------------------------------------------------------------------------|-----------------|
| **TRIG**         | Advances the arpeggio when > 0.4V                                                      | Gate/Trigger    |
| **RESET**        | Restarts the arpeggio at the root note when > 0.4V                                     | Gate/Trigger    |
| **ROOT CV IN**   | CV input for the Root knob (selects chord root)                                        | 0 to +5V        |
| **CHORD CV IN**  | CV input for the Chord knob (selects chord type)                                       | 0 to +5V        |
| **OUT**          | V/Oct arpeggio output                                                                  | 0 to +5V        |

---

## **Controls**

| Control (Knob)   | Function                                                                  | Notes                         |
|------------------|---------------------------------------------------------------------------|-------------------------------|
| **ROOT**         | Sets the initial pitch offset (chord's root note)                         | Manual or voltage controlled  |
| **CHORD**        | Selects which chord is arpeggiated; LEDs indicate active chord            | Manual or voltage controlled  |
| **MODE**         | Selects arpeggio playback mode                                            | 8 modes (see below)           |

---

## **Chord Types and LED Indications**

| Type                    | M/m LED | 7TH LED | * LED            |
|-------------------------|---------|---------|------------------|
| Major                   | ●       |         |                  |
| Major 7                 | ●       | ●       |                  |
| Dominant 7              |         | ●       |                  |
| Minor                   |         |         | ●                |
| Minor 7                 |         | ●       | ●                |
| Diminished              | ● (Off) |         | ● (Off)          |
| Half Diminished 7       |         | ●       | ● (Off)          |
| Full Diminished 7       |         |         | Blinking         |
| Augmented               |         | ●       | Blinking         |
| Augmented 7             | ●       | ●       | Blinking         |
| Sus 4                   |         |         | Blinking         |
| Sus 4 Maj 7             |         | ●       | Blinking         |
| Sus 4 Min 7             | ●       | ●       | Blinking         |

---

## **Arpeggio Modes (Mode Knob)**

- Ascending (1 octave)
- Ascending (2 octaves)
- Descending (1 octave)
- Descending (2 octaves)
- Pendulum (1 octave)
- Pendulum (2 octaves)
- Random (1 octave)
- Random (2 octaves)

---

## **Power Consumption**

- +12V: 40mA  
- -12V: 3mA  
- +5V: 0mA

---

## **Installation Tips**
- 2HP wide; align the red stripe on the power cable with the white line on the module’s PCB.
- Connect either row of 5 pins (if using a 10-pin cable) but always check alignment.
- Mount securely before powering on your rack.

---

## **Quick Workflow**

1. **Patch your clock or gate to the TRIG input.**
2. **Select chord root (ROOT knob or ROOT CV IN) and chord type (CHORD knob or CHORD CV IN).**
3. **Choose arpeggio mode and range using the MODE knob.**
4. **Patch OUT to your VCO or voice.**
5. *(Optional)* Use RESET to jump the arpeggio back to the root.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)