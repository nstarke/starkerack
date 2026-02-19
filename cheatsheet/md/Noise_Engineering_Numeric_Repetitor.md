# Noise Engineering — Numeric Repetitor

- [Manual PDF](../../manuals/NR_manual.pdf)

---

[Noise Engineering Numeric Repetitor Manual (PDF)](https://www.noiseengineering.us/manuals/NumericRepetitorManual.pdf)

---

# Noise Engineering Numeric Repetitor – Cheat Sheet

**Type:** Rhythmic Gate Generator  
**Size:** 8HP Eurorack  
**Depth:** 0.8"  
**Power:** 2x5 Eurorack, +12V: 50mA, -12V: 5mA

---

## What is Numeric Repetitor?
A binary-arithmetic-based rhythmic gate generator. It outputs four related rhythmic patterns based on a selected core rhythm ("Prime") and up to three rhythm modifiers ("Factor") using multiplication and binary logic.

---

## Quick Start

1. **Patch a clock (trigger/gate) to `BEAT`.**
2. **Patch `PRIME` and `PRODUCT 1-3` outputs to drum modules, envelopes, etc.**
3. Rotate the `PRIME` knob to pick a core rhythm; adjust `FACTOR 1-3` to create variations.
4. Patch CV or gates to `PRIME CV` or `FACTOR CV 1-3` for dynamic variations.
5. Optionally patch a reset (start of bar) pulse to `MEASURE`.

---

## Controls and Jacks Reference

| Label         | Type         | Function                                                 | Voltage Range           |
|---------------|--------------|----------------------------------------------------------|-------------------------|
| **PRIME**     | Knob         | Selects prime pattern (main rhythm)                      | -                       |
| **PRIME CV**  | CV In        | Modulates `PRIME` pattern selection                      | 0–5V typical            |
| **FACTOR 1-3**| Knobs        | Selects variation factor for each PRODUCT output         | -                       |
| **FACTOR CV 1-3** | CV In    | Modulates each `FACTOR` knob                             | 0–5V typical            |
| **SET**       | Toggle/Switch| Selects bank of rhythms                                 | -                       |
| **BEAT**      | Trigger In   | Clock input; advances step on rising edge                | Standard gates/triggers |
| **MEASURE**   | Trigger In   | Resets sequence to start of measure                      | Standard gates/triggers |
| **RST**       | Button       | Pauses time; resets to start when released               | -                       |
| **PRIME**     | Gate Out     | Main rhythm (core pattern gate)                          | 0V (low), 6V (high)     |
| **PRODUCT 1-3** | Gate Out   | Three rhythm variations based on factors                 | 0V (low), 6V (high)     |

---

### Output Voltage
- All gate outputs are 0V (low) and 6V (high).
- Low impedance, compatible with most gate-driven modules.

---

## Patch Suggestions
- **Basic:** Clock -> BEAT; PRIME/PROD1-3 -> Percussion Gates
- **Variation:** Use CV/gates on `PRIME` or `FACTOR` for related, evolving patterns (e.g., send a random gate or modulated LFO to a FACTOR CV input).
- **Measure Reset:** Trigger `MEASURE` to keep everything in sync with your main clock.
- **Creative CV:** Divide clock, use sequencers or random sources to modulate FACTOR or PRIME CVs for pattern variation.

---

## Notes on Patterns
- 32 handpicked rhythmic patterns ("Primes")—all 16 steps, always start on step 1, musically valid (see manual for detailed grid).
- Each `FACTOR` applies different binary arithmetic for human-friendly variations.

---

### Tips
- Turning FACTORs or applying CVs creates time offsets, fills, syncopations, and other pattern variations.
- Use SET bank switch for expanded pattern selection.

---

**Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)**