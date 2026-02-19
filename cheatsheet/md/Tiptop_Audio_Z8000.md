# Tiptop Audio — Z8000

- [Manual PDF](../../manuals/Tiptop_Audio_z8000.pdf)

---

[Z8000 Matrix Sequencer Official Manual (PDF)](https://tiptopaudio.com/manuals/z8000.pdf)

---

# Z8000 Matrix Sequencer "Cheat Sheet"

The Tiptop Audio Z8000 is a powerful, compact matrix sequencer offering **10 separate sequencer outputs** (eight 4-step and two 16-step). You can clock, reset, and control the direction of each sequencer independently to create complex, polyrhythmic modulation and pitch patterns.

---

## FRONT PANEL JACK & CONTROL REFERENCE

### Inputs

| **Input Jack**     | **Function**                                       | **Voltage Range**       |
|--------------------|----------------------------------------------------|-------------------------|
| CLK (Clock)        | Advances sequencer steps                           | Gate, any Pulse         |
| DIR (Direction)    | Sets direction; Low=Forward, High=Backwards        | Gate, any logic-level   |
| RT (Reset)         | Resets to step 1 on high                           | Gate, any logic-level   |

- **Notes:**
    - Each of the 10 sequencers (8x 4-step, 2x 16-step) has individual DIR, RT, and CLK inputs.
    - The 4-step sequencers’ CLK jacks are **normalized** in groups of four, so one jack can drive up to four rows/columns unless patched individually. DIR & RT are not normalized.

### Outputs

| **Output Jack** | **Function**                        | **Voltage Range**          |
|-----------------|-------------------------------------|----------------------------|
| CVx             | Stepped CV output for each sequencer| 0–10V (default), 0–5V (jumper-selectable) |

- **8x** 4-step sequencer CV outs (horizontal: 1-4, vertical: A-D)
- **2x** 16-step sequencer CV outs (one aggregates all horizontal, one all vertical)
- **Labeling matches panel graphics**

---

## KNOBS & CONTROLS

### Knobs (16 total)
- Set the voltage for each step in the 4×4 grid (steps 1–4, A–D).
- The active step is indicated by LEDs.

---

## LED INDICATORS

- **Red**: Active step in 4-step sequencers (8 total).
- **Green**: Active step in 16-step sequencers (2 total).
- **Yellow**: LED intersection—when a step is active in both a 4-step and 16-step sequence. Increases in brightness if two 4-step sequencers coincide.

---

## CV OUT RANGE (JUMPER CONFIGURATION)

- **Factory Default**: 0–10V on all outputs.
- **Change to 0–5V:** Remove the corresponding jumper(s) on the rear labeled "CV RANGE" for desired sequencers.
- **10 jumpers total:** 2 for 16-step, 8 for 4-step sequencers.

---

## BASIC USAGE

1. **Patch CV Out:** Choose a sequencer output (CVx) and connect to your destination (VCO for pitch, VCF for modulation, etc.).
2. **Patch Clocks:** Send clock signal(s) to CLK input(s). Use normalization for grouped 4-steps, or separate clocks for polyrhythms.
3. **Set Direction/Reset:** Patch in gates to DIR for forward/backward or to RT for reset-to-step-1.
4. **Adjust Steps:** Set voltages for each step with the corresponding knob in the matrix grid.
5. **Monitor LEDs:** Use red/green/yellow LEDs for visual sequence position and overlaps.
6. **Advanced:** Quantum/quasi-quantized with external quantizer; create polyrhythms by patching multiple clocks; patch CV outs to clock ins for generative rhythms.

---

*For more patch ideas, consult the [full manual (PDF)](https://tiptopaudio.com/manuals/z8000.pdf)*

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)