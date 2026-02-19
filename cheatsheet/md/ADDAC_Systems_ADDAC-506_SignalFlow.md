# ADDAC Systems — ADDAC-506 SignalFlow

- [Manual PDF](../../manuals/ADDAC506_SignalFlow.pdf)

---

[ADDAC506 VC Stochastic Function Generator & Expansion Manual (PDF)](https://addacsystem.com/manuals/addac506_manual.pdf)  
*Cheat sheet generated from reference diagrams and descriptions.*

---

# ADDAC506 VC Stochastic Function Generator & Expansion  
**Quick Reference Cheat Sheet**

---

## OVERVIEW

- **4 Independent function generator/envelope channels**
- **Randomized Rise & Fall times (with min/max limits), voltage controllable**
- **Sum, Average, and Random CV outputs**
- **Flexible operation: Slew/Trigger, Loop/Oneshot, Curve, Amplitude, Offset**
- **Expansion for external random retriggering**


---

## PANEL CONTROLS

### Per Channel (x4):

| Control                  | Type          | Details                                                                            |
|--------------------------|---------------|-------------------------------------------------------------------------------------|
| **Initial**              | Knob          | Manual envelope amount; voltage range per envelope: 0V to 10V                        |
| **CV Input**             | Jack          | Accepts CV, gate, trigger, or audio (Bipolar ±10V typical)                           |
| **CV Input Attenuverter**| Knob          | Amount and polarity of CV input modulation (-1 to +1 range)                          |
| **Rise Time Min**        | Knob & CV     | Sets minimum randomized rise time (0–10V normal range); CV input/attenuverter        |
| **Rise Time Max**        | Knob & CV     | Sets maximum randomized rise time (0–10V); CV/attenuverter                           |
| **Fall Time Min**        | Knob & CV     | Sets min randomized fall time (0–10V); CV/attenuverter                               |
| **Fall Time Max**        | Knob & CV     | Sets max randomized fall time (0–10V); CV/attenuverter                               |
| **Envelope Curve**       | Switch        | Logarithmic ↔ Linear shape selector                                                  |
| **Amplitude**            | Knob          | -10V to +10V envelope level (center = 0V; max span 10Vpp)                            |
| **Offset**               | Knob          | -10V to +10V shift (envelope baseline) (center = 0V)                                 |
| **LEDs**                 | Output        | Visual envelope monitor (bipolar; shows amplitude/polarity)                          |
| **Lock Button**          | Button        | Locks channel Rise/Fall settings from accidental changes                             |
| **Loop / Oneshot**       | Toggle        | Envelope retriggers itself (Loop) or single cycle (Oneshot)                          |
| **Slew / Trigger**       | Toggle        | Slew: follows input CV; Trigger: one-shot envelope cycle per input                   |

---

## GLOBAL CONTROLS

| Control                  | Type          | Details                                                                            |
|--------------------------|---------------|-------------------------------------------------------------------------------------|
| **Speed Range**          | Switch        | Low / Medium / High (overall envelope responsiveness)                               |

---

## JACK REFERENCE

### Per Channel (x4):

| Jack                       | Direction | Details                                     | Voltage Range         |
|----------------------------|-----------|---------------------------------------------|-----------------------|
| **Channel Input**          | Input     | CV, gates, triggers, or audio accepted      | ±10V                 |
| **CV Output**              | Output    | Envelope output                             | -10V to +10V         |
| **Gate Output**            | Output    | HIGH while in rise, LOW otherwise           | 0V/5V                |
| **End of Rise (EOR)**      | Output    | Pulse at end of rise segment                | 0V/5V or Gate (jumper)|
| **End of Fall (EOF)**      | Output    | Pulse at cycle end                          | 0V/5V or Gate        |

### Mixer/Global Outputs:

| Jack                    | Direction | Details                          | Voltage Range      |
|-------------------------|-----------|----------------------------------|--------------------|
| **Average Mix Output**  | Output    | Average of all 4 envelopes       | -10V to +10V       |
| **Summing Mix Output**  | Output    | Sum of all 4 envelopes           | -40V to +40V (all channels maxed)|

---

### Expansion Jacks (per channel):

| Jack                            | Direction | Details                                                       | Voltage Range         |
|----------------------------------|-----------|---------------------------------------------------------------|-----------------------|
| **Random Trigger Input**         | Input     | Re-randomizes Rise & Fall time at any point                   | 0V/5V                 |
| **Random CV Output**             | Output    | Actual random Rise/Fall control CV for the cycle (selectable) | 0V to 10V             |

---

### Miscellaneous

- **Jumper on each Random CV Output:** Selects if jack outputs Rise or Fall random value.
- **Envelope time randomization:** Happens at new cycle trigger or via expansion random input.

---

## OPERATION HINTS

- **Set Rise/Fall Min above Max:** Envelope time is fixed to Min knob (no random).
- **Lock/Unlock Button:** Lock channel settings to tweak only the one you want.
- **Slew mode:** Use as a voltage follower for any signal, not just gates/triggers.
- **Visual feedback:** Use LEDs to watch envelope shape and output.
- **Mix & route:** Combine channels for complex modulation; sum/average/join outputs.

---

## VOLTAGE RANGES

- **Envelope Outputs:** -10V to +10V (bipolar, with amplitude and offset).
- **CV Inputs:** ±10V optimal.
- **Gate/EOR/EOF Outputs:** Typically 0V (inactive) or 5V (active).

---

## PATCH IDEAS

- Use random CV outs for modulating other modules with true cycle-to-cycle randomness.
- Inject audio or noisy CV sources in Slew mode for envelope following/vactrol-like behavior.
- Lock some channels and randomize others for patch variety.
- Use sum/average outputs for macro modulation controls.

---

**Reference:** [Github: Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---