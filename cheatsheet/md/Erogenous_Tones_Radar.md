# Erogenous Tones — Radar

- [Manual PDF](../../manuals/radar-instructions.pdf)

---

[Manual PDF](http://erogenous-tones.com)

# Erogenous Tones RADAR — Cheat Sheet

## What it is
**RADAR** is an **8-channel AD/AR/repeating envelope generator**.  
“RADAR” = **Repeating, AD, or AR**.

It has **3 system modes**:
- **Envelope Mode**: 8 independent envelopes
- **Quad Mode**: two 4-phase groups, or one 4-phase group + 4 independent envelopes
- **Oct Mode**: one 8-phase group

---

## Quick Start

### 1) Pick a system mode
Use the **SYSTEM MODE** switch:
- **Envelope**
- **Quad**
- **Oct**

### 2) Per-lane basic behavior
Each lane can be set to:
- **R** = Repeating / LFO
- **AD** = Attack-Decay
- **AR** = Attack-Release

### 3) Trigger it
In **Envelope Mode**, each lane has a **trigger input**.  
Trigger inputs are **normalized downward** to the next lane.

### 4) Set timing and shape
For each lane, adjust:
- **Attack**
- **Release**
- **Shape**: **LOG ↔ LIN ↔ EXP**

### 5) Watch the LED
- **Blue** = rising
- **Purple** = hold in AR mode
- **Red** = falling

---

## Modes

## Envelope Mode
Use when you want **8 independent envelope channels**.

### Triggering
- Each lane has its own **trigger input**
- Trigger is **normalized to the next channel below**

### AD vs AR
- **AD**: on rising gate/trigger, runs full **Attack**, then full **Release**
- **AR**:
  - In **analog modeling mode**, envelope rises only as long as gate stays high
  - If gate is short, it may never reach full level before releasing
  - In **digital mode**, short gate/trigger behaves more like **AD**

### Gate behavior
If gate stays high longer than attack time:
- envelope rises
- stays high
- releases when gate goes low

### Repeating mode
Acts like an **LFO**.
- In **digital mode**, retrigger resets waveform to zero
- In **analog mode**, reset only happens if lane is in release; restart begins from current level/release point

---

## Modeling modes
Lanes are controlled in **pairs of 2** for modeling mode and envelope shape mode.

### Digital
- Retrigger **resets envelope to zero** from anywhere in cycle
- Creates classic digital discontinuities/snaps
- Repeating/LFO frequency is **constant**

### Analog modeling
- Does **not** reset unless in decay/release
- Attack starts from current level
- Behaves more like capacitor charging/discharging

---

## Shape behavior
### Shape knob / CV
Continuously morphs:
- **LOG**
- **LIN**
- **EXP**
- and everything between

### E/O switch
Controls whether decay/release shape is:
- **E** = Equal to attack shape
- **O** = Opposite of attack shape

Example:
- LOG rise + **O** = EXP fall

If attack is linear, both sides remain linear.

---

## Composite outputs
Only in **Envelope Mode**:

### Lane 4 output switch
Can change lane 4 output to a **composite max output** of:
- **Lane 3 and Lane 4**

### Lane 8 output switch
Can change lane 8 output to a **composite max output** of:
- **Lane 6, 7, and 8**

Notes:
- In composite mode, the LED is always **purple**
- This is a **max-value** combination, not a sum

---

## Quad Mode
Lets you use:
- **2 quad envelopes**, or
- **1 quad envelope + 4 normal envelope lanes**

Use the **lane 4 output switch** to choose the behavior for lanes **1–4**.  
Composite/max output modes do **not** exist in Quad Mode.

### Quad behavior
For each 4-lane group:
- lanes are **90° apart**
- **lane 1** and **lane 5** set rise/fall time for their whole group
- **E/O** also comes from lane 1 / lane 5
- works in **digital mode only**
- reset on first lane resets all lanes and restores phase relationships

### Extra CV functions in Quad Mode
The **2nd, 3rd, and 4th lanes** of each quad group can take on special CV roles:

- **SPEED**
- **GRAVITY**
- **SDELTA**

Their switch behavior:
- **R position** = CV off
- **AD/AR** = off/on respectively via switch or AD/AR input level

#### SPEED
Modulates overall rate of all 4 channels together.

#### GRAVITY
Warps timing relationship of 90°/180°/270° lanes relative to the 0° lane.

#### SDELTA
Offsets/interpolates shape differences from first lane to last lane.

Caution: steep modulation can cause jumps because shape curves differ by time/value.

---

## Oct Mode
Same concept as Quad Mode, but:
- all **8 lanes**
- each lane is **45° apart**

---

## LFO / Repeating speed notes
Fastest frequencies mentioned in manual:

### Analog mode
At fastest settings:
- around **1.18 kHz** with **EXP** shape
- around **610 Hz** with **LIN**
- around **1.18 kHz** with **LOG**

### Digital mode
- max about **591 Hz**

---

# Controls Reference

## Global controls
### SYSTEM MODE switch
Selects:
- **Envelope**
- **Quad**
- **Oct**

---

## Per-lane controls
Each lane has:

### RADAR mode switch
Selects:
- **R** = repeating/LFO
- **AD**
- **AR**

### Attack control
Sets rise time.

### Release control
Sets fall time.

### Shape control
Morphs:
- LOG ↔ LIN ↔ EXP

### Shape CV input
Offsets shape knob setting.

### Trigger/Gate input
Used to start or control envelopes.

### Output jack
Envelope or repeating waveform output.

### LED
Shows stage:
- Blue = rise
- Purple = hold / composite indication
- Red = fall

---

## Shared / grouped controls
### Modeling mode switch
Per pair of lanes:
- **Digital**
- **Analog modeling**

### E/O switch
Per pair of lanes:
- **Equal**
- **Opposite**

### Lane 4 output switch
- Envelope Mode: normal output or max(lane 3, lane 4)
- Quad Mode: selects quad configuration for lanes 1–4

### Lane 8 output switch
- Envelope Mode: normal output or max(lane 6, lane 7, lane 8)

---

# Jack Reference

> Note: The provided manual pages do **not specify exact voltage ranges** for most inputs/outputs. Where range is not explicitly stated, it is marked **Not specified in provided manual**.

## Inputs

### Per-lane Trigger/Gate inputs
- **Function**: trigger envelope, gate AR behavior, reset repeating waveform
- **Normalization**: each trigger input is normalized to the lane below
- **Voltage range**: **Not specified in provided manual**

### Per-lane Shape CV inputs
- **Function**: offsets shape knob position
- **Tip**: use an external attenuator to limit modulation amount
- **Voltage range**: **Not specified in provided manual**

### AD/AR input
- **Function**: can select/activate AD vs AR based on input level in relevant modes
- **Voltage range**: **Not specified in provided manual**

## Outputs

### Per-lane envelope outputs
- **Function**: envelope or repeating/LFO waveform output
- **Voltage range**: **Not specified in provided manual**

### Composite outputs
Available only when lane output switch is set appropriately:
- **Lane 4 output** = max of lanes 3 and 4
- **Lane 8 output** = max of lanes 6, 7, and 8
- **Voltage range**: **Not specified in provided manual**

---

# Practical Patch Tips

## Classic 8-envelope patch
- Set **System Mode = Envelope**
- Put each lane in **AD** or **AR**
- Feed separate triggers to each lane
- Use different shape settings for percussion vs slow modulation

## Cascaded triggers
Because triggers normalize downward:
- patch a trigger into an upper lane
- leave lower inputs unpatched
- get repeated use of same trigger source across lanes

## Organic envelopes
- Use **Analog modeling**
- Use **AR**
- Send variable gate lengths
- Great for plucks, struck tones, and less “snappy” modulation

## Clocked LFO bank
- Set some lanes to **R**
- Use **digital mode** for stable repeating rate
- retrigger/reset from a clock or pulse source

## Composite modulation
In Envelope Mode:
- switch **lane 4** or **lane 8** to composite output
- use resulting “max” contour as a more complex envelope

## Quadrature modulation
In **Quad Mode**:
- use the 4 outputs as phased modulation
- ideal for panning, scanning, vector movement, filter banks, and animation

## 8-phase modulation
In **Oct Mode**:
- use all 8 outputs as a rotating modulation set
- good for sequenced spatial movement or distributed CV animation

---

# Gotchas
- **Shape CV is an offset**, not absolute control
- Use an **external attenuator** for shape CV
- **Digital mode** hard-resets envelopes to zero
- **Analog mode** preserves continuity unless in release
- **Composite output modes** exist only in **Envelope Mode**
- **Quad/Oct** are **digital only**
- In **Quad/Oct**, only the lead lane of the group controls shared timing/shape behavior

---

# Missing from provided manual pages
The provided 2-page excerpt does **not explicitly list**:
- exact **input voltage ranges**
- exact **output voltage ranges**
- exact trigger/gate threshold voltages
- exact attack/release time ranges
- full front-panel jack-by-jack labeling

If you want, I can also turn this into a **one-page performance-oriented quick reference** or a **full panel control map** based on the module photo.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)