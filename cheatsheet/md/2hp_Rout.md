# 2hp — Rout

- [Manual PDF](../../manuals/Rout_Manual.pdf)

---

[**Download the Rout Manual (PDF)**](#) <!-- (Replace # with the actual manual link if available) -->

---

# Rout (2hp) – Cheat Sheet

**What is Rout?**
- *Voltage-controlled gate switch.*  
- Routes one gate/trigger input to any of four outputs.
- Selection via knob or CV input (0–5V).
- Perfect for splitting trigger/gate patterns to multiple voices or modulating patterns with a single gate source.

---

## **Panel Controls and I/O Reference**

### **Inputs**

| Jack/Control | Label   | Function                                              | Voltage Range       |
|:------------:|:--------|:-----------------------------------------------------|:--------------------|
| 1            | INPUT   | Main gate/trigger input to be routed                 | Threshold: 2.5V     |
| 2            | SEL CV  | CV input to control output selection (overrides knob)| 0V – 5V             |

### **Knobs**

| Control | Label | Description                                              |
|:-------:|:------|:---------------------------------------------------------|
| 3       | SEL   | Manual selector for output (far left=OUT 1, far right=OUT 4). CV input overrides knob position. |

### **Outputs**

| Jack | Label  | Description                                           | Voltage Range       |
|:----:|:-------|:------------------------------------------------------|:--------------------|
| 5    | OUT 1  | Gate/trigger output if OUT 1 selected                 | 0V – 5V             |
| 7    | OUT 2  | Gate/trigger output if OUT 2 selected                 | 0V – 5V             |
| 9    | OUT 3  | Gate/trigger output if OUT 3 selected                 | 0V – 5V             |
| 11   | OUT 4  | Gate/trigger output if OUT 4 selected                 | 0V – 5V             |

### **LED Indicators**

| LED  | Corresponds To | Indicates                                    |
|:----:|:--------------|:----------------------------------------------|
| 4    | OUT LED 1     | Shows activity at OUT 1                       |
| 6    | OUT LED 2     | Shows activity at OUT 2                       |
| 8    | OUT LED 3     | Shows activity at OUT 3                       |
| 10   | OUT LED 4     | Shows activity at OUT 4                       |

---

## **Basic Operations**
1. **Input** your gate/trigger signal to INPUT.
2. **Select** one of four outputs using the SEL knob (or use SEL CV for voltage control).
3. Only **one output** is active at a time—the selected output passes the INPUT signal, others are low.
4. Use the **SEL CV** input (0–5V) to automate output switching (e.g., from a sequencer, sample & hold, LFO, etc.).
5. **Monitor** which output is active via the corresponding OUT LED.

---

## **Specs**
- Width: 2 HP
- Depth: 47mm (Skiff friendly)
- Power: +12V = 26mA, -12V = 6mA

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
