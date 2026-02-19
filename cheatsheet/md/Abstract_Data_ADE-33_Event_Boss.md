# Abstract Data — ADE-33 Event Boss

- [Manual PDF](../../manuals/ADE33_Manual_v1_0.pdf)

---

[**Download the ADE-33 Event Boss Manual PDF**](https://www.abstractdata.biz/ADE-33/ADE-33-User-Guide-v101.pdf)

---

# ADE-33 EVENT BOSS – CHEAT SHEET

**Rhythm and Pattern Creation and Manipulation Module**  
*By Abstract Data Ltd. – v1.0.1*

---

## Quick Reference Panel Functions

### BUTTONS & CONTROLS

| Control                 | Function                                                                                       |
|-------------------------|-----------------------------------------------------------------------------------------------|
| **MODE SELECT**         | Click: Cycle forward Local/Global Modes <br> Double-Click: Cycle backward <br> Hold: Edit     |
| **GATE A1/A2 SELECT**   | Click: Toggle between IN: GATE A1 and A2 <br> Double-Click: Toggle backward <br> Hold: Edit   |

### INDICATORS

| Indicator               | Meaning                                                                                       |
|-------------------------|-----------------------------------------------------------------------------------------------|
| **MODE LEDs 1-6**       | Selected Local (or Global) Mode                                                               |
| **A1/A2 SELECT LED 1-2**| Displays active input (A1 or A2)                                                              |
| **OUTPUT LED**          | Shows output status (On = High/+5V, Off = Low/0V)                                            |

---

## INPUT / OUTPUT JACKS

| Jack               | Full Name                     | Function                                                  | Voltage Range        |
|--------------------|------------------------------|-----------------------------------------------------------|---------------------|
| **IN: MODE SELECT/ RESET** | Mode Select / Count Reset  | Event: Steps thru Local Modes; CV: Jumps by voltage       | 0 to +5V            |
| **IN: GATE A1**    | Event Input A1               | Event input for all modes                                 | 0 to +5V            |
| **IN: GATE A2**    | Event Input A2               | Event input for all modes                                 | 0 to +5V            |
| **IN: GATE B/CV**  | Event or CV Input            | Event/CV input, function varies by Global Mode            | 0 to +5V            |
| **OUT**            | Output                       | Gate/trigger or clock signal output                       | 0 to +5V            |

---

## OPERATION ESSENTIALS

### GLOBAL & LOCAL MODES

- **6 Global Modes** (e.g. Variables, Multiples, Probability, Logic, Phase, Gates)
- **Each Global Mode has 6 Local Modes** (36 total)
- Mode select by holding both buttons until GLOBAL LED flashes → Change Global → Hold both to exit.  
Then use MODE SELECT button to change Local Mode.

### INPUT HANDLING

- **Events:** Clocks, gates, triggers, square/PWM-LFO or similar
- **CV Input:** Any 0–5V CV source such as LFO, envelope, offset, etc.
  - Most algorithms respond to non-square LFOs or variable CV for dynamic rhythmic changes
- **Output:** High = +5V, Low = 0V

---

## MODE OVERVIEW

| Global Mode | Theme                              | CV/Function Highlights                           |
|-------------|-------------------------------------|--------------------------------------------------|
| **1. Variables** | Variable Rhythmic Patterns           | CV sets <n> (1-8): pattern pass/block variations  |
| **2. Multiples** | Clock Division/Multiplication        | CV sets division/mult (1-12): output tempo scales |
| **3. Probability** | Random/Chance pattern variations      | CV = percentage chance, probability, tie, coin flip|
| **4. Logic** | Logic Functions (AND, OR, XOR etc)            | Dual event logic, switch with CV/A1/A2            |
| **5. Phase** | Phase/Delay/Swing                      | CV sets phase offsets or mark/space ratios         |
| **6. Gates** | Gate/Trigger Manipulation               | Extend, hold, alternate gate logic                |

---

## MODE SHORTCUT REFERENCE

### **Global Mode 1: Variables**  
- **CV @ IN: GATE B/CV:** Sets variable <n> (1-8)
- Patterns: nth Pass, nth Block, n Pass, n Block, toggles

### **Global Mode 2: Multiples**  
- **CV @ IN: GATE B/CV:** Sets division/mult (1-12)
- Modes: Divide /1, Multiply /1, Divide /2, Multiply /2, Divide /3, Multiply /3

### **Global Mode 3: Probability**  
- **CV @ IN: GATE B/CV:** 0–5V for 0–100% probability
- Modes: Pass chance, Block chance, Tie/Pass, Flip-Flop, Inversion

### **Global Mode 4: Logic**  
- **IN: GATE A1/A2** + **IN: GATE B/CV**: Standard two-input Boolean Logic (AND, NAND, OR, NOR, XOR, XNOR)
- **Global Event:** Mutes output

### **Global Mode 5: Phase**  
- **CV @ IN: GATE B/CV:** Sets phase offset (quantized, %, ms)
- Modes: Phase-shift or alter mark/space ratio by CV

### **Global Mode 6: Gates**  
- **CV @ IN: GATE B/CV:** Pattern length/gate logic threshold (1-8 steps or 2.5V logic)
- Modes: n High, n High/Low, Logic Pass/Hold, toggles

---

## POWER

- **10-16 pin ribbon, RED stripe = -12V**
- Doepfer standard; 53mA ( +12V), 35mA ( -12V)

---

## PATCH FLOW EXAMPLES

**Clock in A1 → OUT to Envelope** = rhythmic gate  
**CV in GATE B/CV** = pattern/swing/logic/randomness by mode  
**Second clock in A2** = logic and complex rhythm modes  
**MODE SELECT input/CV** = step through/switch patterns

---

## PDF Manual  
[**ADE-33 User Guide**](https://www.abstractdata.biz/ADE-33/ADE-33-User-Guide-v101.pdf)

---

Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)