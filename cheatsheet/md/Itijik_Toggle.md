# Itijik — Toggle

- [Manual PDF](../../manuals/toggle.pdf)

---

[Manual PDF](#)

# Itijik Toggle — Cheat Sheet

## What it is
A **quad flip-flop / logic utility** for Eurorack.  
It gives you **4 identical sections**, each with:
- **SET**
- **RST**
- **CLK**
- **IN**
- **OUT**
- **VERT**

Core idea:
- **OUT** is the flip-flop output.
- **VERT** is the inverted output **unless** you patch something into **IN**, which breaks that normalization.

## Power / Installation
- **+12V:** 37 mA
- **-12V:** 34 mA
- 10-pin ribbon on module: **red stripe to -12V** (bottom of module)
- 16-pin ribbon on bus board: **red stripe to negative side**

## How each section works
Each of the 4 sections is identical.

### Basic behavior
- Send a pulse/gate to **SET** → **OUT goes HIGH**
- Send a pulse/gate to **RST** → **OUT goes LOW**
- Send a pulse/gate to **CLK** → **OUT toggles**
- If **IN is unpatched**, **VERT = inverse of OUT**

### IN jack behavior
- Patching **IN** breaks the normal connection from **OUT** to **IN**
- **VERT** becomes the inversion of the **IN** signal instead of OUT
- So:
  - **IN HIGH** → **VERT LOW**
  - **IN LOW or no signal present at IN** → **VERT HIGH**

## Fast patch ideas
- **Clock divider by 2 / toggle gate**
  - Patch a trigger stream to **CLK**
  - Take output from **OUT**
  - Each pulse flips the state

- **Manual state logic source**
  - Use **SET** and **RST** from two different trigger sources
  - Great for rhythmic state changes

- **Complementary gates**
  - Leave **IN unpatched**
  - Take **OUT** and **VERT** as opposite logic signals

- **Standalone inverter**
  - Patch a gate into **IN**
  - Take inverted gate from **VERT**

---

## Jack Reference

### Inputs per section
| Jack | Function | Notes | Voltage Range |
|---|---|---|---|
| **SET** | Forces **OUT HIGH** on received pulse/gate | Also forces **VERT LOW** if **IN** is unpatched | **Not specified in manual** |
| **RST** | Forces **OUT LOW** on received pulse/gate | Also forces **VERT HIGH** if **IN** is unpatched | **Not specified in manual** |
| **CLK** | Toggles **OUT** on each received pulse/gate | Also toggles **VERT** if **IN** is unpatched | **Not specified in manual** |
| **IN** | Logic input for inverter | Breaks normalization from **OUT** to **IN** when patched | **Not specified in manual** |

### Outputs per section
| Jack | Function | Notes | Voltage Range |
|---|---|---|---|
| **OUT** | Main flip-flop output | Normalized to **IN** for inversion when IN is unpatched | **Not specified in manual** |
| **VERT** | Inverted logic output | Inverts **OUT** if **IN** unpatched; otherwise inverts **IN** | **Not specified in manual** |

## Controls / Indicators
### Controls
- **No knobs**
- **No buttons**
- **No sliders**
- **No toggle switches**

### Indicators
- **LEDs for OUT and VERT** on each section to show logic state

## Important normalization
- **No cable in IN:**  
  **VERT = NOT(OUT)**
- **Cable in IN:**  
  **VERT = NOT(IN)**  
  and the OUT-to-IN normalization is disconnected

## Good to know
The manual does **not specify exact logic voltage thresholds or output voltage levels**, so treat all pulse/gate voltages as **unspecified by manufacturer** in this document.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)