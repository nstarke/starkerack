# Robaux — DCSN-3

- [Manual PDF](../../manuals/robauxDCSN3Manual.pdf)

---

[Robaux Decision Tree (DCSN3) Manual PDF](https://robaux.io/assets/decision_tree_manual.pdf)

---

# Robaux Decision Tree (DCSN3) Eurorack Module Cheat Sheet

**Type:** Randomized Gate/Trigger Router & Clock Divider  
**Power:** ±12V (30mA on +12V)  
**Width:** (Check official specs)  
**Depth:** (Check official specs)  

---

## **Panel Reference**

```
   b   c   d
  / \ / \ / \
 e f g h i j k l m
         n (Knob)
         o (Button)
```

---

## **Inputs**

| Jack | Function                                  | Voltage Range                |
|------|-------------------------------------------|------------------------------|
| a    | Main gate/trigger or clock input          | 0-5V or 0-10V (typical)      |
| m    | Hidden Reset input (in certain modes)     | 0-5V or 0-10V (typical)      |

*Note: The specified voltage range isn't detailed in the manual. Generally, 0-5V triggers/gates are expected for this type of module.*

---

## **Outputs**

| Jack | Function (depends on mode)                              | Output Voltage                |
|------|--------------------------------------------------------|-------------------------------|
| b, c, d    | Main gate/trigger outputs (random or divided clock)      | 0-5V (typical)                |
| e, f, g    | Sub-outputs for main output b                      | 0-5V (typical)                |
| h, i, j    | Sub-outputs for main output c                      | 0-5V (typical)                |
| k, l, m    | Sub-outputs for main output d                      | 0-5V (typical)                |

- **Random/Pattern Mode:** Trigger signals routed randomly or via patterns to these outputs.
- **Clock Divider Modes:** Each output carries clock divisions as per chosen divider mode.

---

## **Controls**

| Control          | Type       | Description                                                                                                          |
|------------------|------------|----------------------------------------------------------------------------------------------------------------------|
| n                | Rotary knob| Interpolates between fully random and 16-step repeating patterns. Used with o to select modes.                       |
| o                | Button     | Tap for new random sequence. Hold + Turn n to select mode; hold on power up for debug mode.                         |

---

## **Operation & Modes**

### Basic Gate/Trigger Routing  
- **Send a trigger/gate to input a.**
- The module randomly routes to one (or more, in poly modes) of b, c, or d, then randomly to one of their 3 sub-outputs.

### Mode Selection (while power is on)  
1. **Hold o (Freeze button)**
2. **Turn rotary knob n**  
   Visual pattern (via LEDs) shows selected mode:
   - **Mono/Mono:** Random single path
   - **Poly/Mono:** Randomly to one or more main outs, each to one sub
   - **Poly/Poly:** Random polyphonic through all outs
   - **Latch** modes: As above, but output is held until new input/clock

### Randomness vs. Pattern  
- **Turn n:** Left = fully random, Right = repeating 16-step pattern  
- **Tap o:** Generate a new random sequence.

---

### Clock Divider Modes (selected by turning o knob in main mode)  

| Position of o  | Mode             | Output Assignments                                          |
|----------------|------------------|-------------------------------------------------------------|
| Fully left     | Classic Divider  | b: /2, e: /4, f: /8, g: /16. c-h-m: 8-step sequencer.      |
| Center         | 2/3/5 Divider    | b-e-f-g: /2,4,8,16; c-h-i-j: /3,6,12,24; d-k-l-m: /5,10,20,40|
| Fully right    | Spread           | Successive integer divisions: /2, /3, /4, /5, /6, /7, ...   |

---

### Reset & Debug

- **Auto-reset:** If input pauses, resets to first step.
- **Hidden Reset Input:** m jack can act as a reset in loop mode; enable in debug mode.
- **Debug Mode:** Hold o on power-up; outputs & LEDs will cycle for testing.

---

## **Quick Mode/Modes Reference**

- **Mono/Mono:** Random single path b/c/d → e-g/h-j/k-m
- **Poly/Mono:** Randomly to several b/c/d, each picks one sub-out
- **Poly/Poly:** Poly trigger through all main + sub-outs
- **Latch variants:** Out is held till next gate/trigger
- **Clock Divider:** See divider modes above

---

**General Tips:**
- **Modes are visually indicated via LEDs for intuitive feedback.**
- **Combines random logic, clock dividing, and switch routing in one compact module.**
- **Excellent for generative rhythms, randomized sequence distribution, or complex clocking.**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)