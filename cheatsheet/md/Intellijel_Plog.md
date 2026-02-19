# Intellijel — Plog

- [Manual PDF](../../manuals/plog_manual.pdf)

---

[Download the Plog rev 1.0 Manual PDF](https://intellijel.com/downloads/manuals/plog_manual.pdf)

---

# Intellijel Plog Cheat Sheet

**Plog** is a flexible, voltage-controlled logic processor module with two 3-input logic blocks (A & B), a toggle flip-flop (T), and a data flip-flop (D). Useful for creating complex patterns, clock/trigger manipulation, and experimental generative sequences.

---

## Panel Controls & Features

### Logic Blocks (A & B)
- **TYPE Button**  
  - Press: Cycle logic type (AND, OR, NOR, XOR, NAND, XNOR) for selected block  
  - Hold (1 sec): Load preset from memory

- **TYPE CV Attenuator (A & B)**  
  - Mini knobs to scale incoming CV to TYPE A/B CV inputs

- **SELECT Button**  
  - Press: Select which logic block (A or B) to edit  
  - Hold (1 sec): Save current logic states to memory

- **OUT A / OUT B (Outputs)**  
  - Main logic block outputs

- **TYPE A/B CV Input ([±5V], bipolar)**  
  - Controls which logic type is selected for each block  
  - LEDs indicate selected logic type  
  - Typical logic types per CV:  
    - AND, OR, NOR, XOR, NAND, XNOR

- **X, Y, Z Inputs (Channel A & B, [0-5V logic], protected ± overvoltage)**  
  - X and Y of A are normalled to X and Y of B  
  - Z is normalled to Y unless patched  
  - 0V = logic LOW; 5V = logic HIGH; comparator threshold ≈3V

---

### Flip-Flop Section

- **TRIGGER Button**  
  - Press: Sends trigger to Toggle input (T Flip-Flop)  
  - Hold (1 sec): Enter tap-tempo mode, tap to set clock, hold again to exit

- **TOGGLE Input (T, [0-5V logic], protected)**  
  - Trigger for Toggle flip-flop  
  - TRIGGER button normalled to this jack  
  - Jumper on back: can normal OUT B here

- **OUT T (Output, [0-5V pulses])**  
  - Output of the Toggle flip-flop  
  - In tap-tempo mode: tempo clock output (square pulses)

- **CLK (Clock Input, [0-5V logic])**  
  - Clock input for Data (D) flip-flop  
  - OUT T normalled to here

- **DATA (Input, [0-5V logic])**  
  - Data input for Data (D) flip-flop

- **OUT D (Output, [0-5V pulses])**  
  - Output of the Data flip-flop

---

## Logic Types and Truth Tables
| Logic Type | Description                           |
|------------|---------------------------------------|
| AND        | High only if all inputs are High      |
| OR         | High if any input is High             |
| NOR        | High if all inputs are Low            |
| XOR        | High if odd number of inputs are High |
| NAND       | High unless all inputs are High       |
| XNOR       | High if even number of inputs are High|

See manual Tables 1 & 2 for detailed truth tables for 3 or 2 input modes.

---

## Usage Ideas
- **Clock Dividing:** Use the flip-flops as /2, /4 clock dividers  
- **Randomized Triggers:** Patch random and quantized sources into logic blocks for "real-time quantizer" effects  
- **Pattern Mutation:** Use CV over logic type inputs to morph gate patterns  
- **CV Addressed Logic:** Modulate TYPE A/B CV for evolving logic operations

---

## Voltage Ranges
- **Logic inputs:** 0-5V pulses/gates/clocks (comparator @ 3V threshold, accepts non-square inputs)  
- **CV TYPE inputs:** ±5V (bipolar, for logic type selection)
- **Outputs:** 0-5V (unipolar pulses/gates/clocks)

---

## Technical Specs (from manual)
- 8HP, 29mm depth  
- +12V 55mA / -12V 11mA

---

## Example Patch (Quantized LFO)
- Set A to AND  
- Random triggers (e.g. square LFO) → X  
- Clock (e.g. drum machine/sequencer) → Y  
- OUT A → Envelope → VCA  
- Modulate TYPE A CV for extra variation

---

> [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)