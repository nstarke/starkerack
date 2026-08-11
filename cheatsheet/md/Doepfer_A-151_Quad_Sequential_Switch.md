# Doepfer — A-151 Quad Sequential Switch

- [Manual PDF](../../manuals/A151_man.pdf)

---

[Manual PDF](https://doepfer.de/a100_man/A151_man.pdf)

# Doepfer A-151 Quad Sequential Switch — Cheat Sheet

## What it does
The **A-151** is a **4-step sequential switch**: each trigger advances the connection between the **common jack** and the next one of **4 switched jacks**.

Think of it as an electronic rotary switch for:
- **4 inputs → 1 output**, or
- **1 input → 4 outputs**

It is **bi-directional**, so either use case works.

## Core behavior
- **Each rising edge at Trigger In** advances to the next step.
- Steps cycle:
  - **1 → 2 → 3 → 4 → 1**
- **Reset In** immediately returns the switch to **step 1**.
- **LEDs 1–4** show the active step.
- **Version 2** modules add a **2/3/4 step selector**.

## Controls / Indicators

### LEDs
- **LED 1–4**: show which **I/O 1–4** is currently connected to the common jack.

### Switch
- **Steps switch** *(Version 2 only)*:
  - **2** = alternate between I/O 1 and 2
  - **3** = cycle through I/O 1–3
  - **4** = full 4-step cycle

## Jack Reference

### Inputs
- **Trig. In**
  - Function: advances the switch one step on each **rising edge**
  - Type: trigger input
  - Voltage range: not explicitly stated for trigger threshold in the manual

- **Res. In**
  - Function: resets immediately to **I/O 1** on rising edge
  - Type: reset input
  - Voltage range: not explicitly stated for reset threshold in the manual

### Common jack
- **O/I**
  - Function: common **output/input**
  - Connects to the currently active **I/O 1–4**
  - Signal direction is patch-dependent
  - **Voltage range:**
    - **Version 1:** **-8 V to +8 V**
    - **Version 2:** **-12 V to +12 V**

### Switched jacks
- **I/O 1**
- **I/O 2**
- **I/O 3**
- **I/O 4**

Each is a bidirectional switched jack connected in sequence to **O/I**.

**Voltage range for all I/O jacks:**
- **Version 1:** **-8 V to +8 V**
- **Version 2:** **-12 V to +12 V**

## How to patch it

### 1) Switch between 4 signal sources
Patch:
- 4 different signals into **I/O 1–4**
- Take output from **O/I**
- Send clock/triggers to **Trig. In**

Result:
- Each trigger selects the next source.

Good for:
- Oscillator waveform switching
- Selecting different modulation sources
- Switching among filter outputs

### 2) Send 1 signal to 4 destinations
Patch:
- Signal into **O/I**
- Destinations from **I/O 1–4**
- Clock into **Trig. In**

Result:
- One source is routed to a different destination each step.

Good for:
- Sending one CV to different modulation targets
- Distributing gates or modulation in sequence

### 3) Shorter repeating sequences
Use either:
- **Version 2 Steps switch** to set **2, 3, or 4** steps, or
- **Reset In** to force return to step 1

Example:
- With reset timing, you can create **1 → 2 → 3 → 1...**

## Musical uses from the manual
- **Waveform sequencing:** switch between VCO waveform outputs
- **Audio-rate switching:** very fast triggering can create new timbres / audio-rate modulation effects
- **Envelope sequencing:** cycle through different envelopes affecting a filter
- **Filter mode stepping:** switch among multimode filter outputs per note

## Important notes / gotchas
- The module is **bi-directional**: there is no fixed “input side” vs “output side” for the audio/CV path.
- On **Version 1**, signals outside **-8 V to +8 V** may cause malfunction.
- **Version 2** supports the full A-100 signal range: **-12 V to +12 V**.
- Very fast triggers can push the switch into **audio-rate behavior**, which can be creatively useful.

## Quick reference

| Element | Type | Function | Voltage Range |
|---|---|---|---|
| Trig. In | Input | Advance one step on rising edge | Not specified |
| Res. In | Input | Reset to step 1 on rising edge | Not specified |
| O/I | Bidirectional jack | Common jack connected to active step | V1: -8 to +8 V, V2: -12 to +12 V |
| I/O 1 | Bidirectional jack | Step 1 jack | V1: -8 to +8 V, V2: -12 to +12 V |
| I/O 2 | Bidirectional jack | Step 2 jack | V1: -8 to +8 V, V2: -12 to +12 V |
| I/O 3 | Bidirectional jack | Step 3 jack | V1: -8 to +8 V, V2: -12 to +12 V |
| I/O 4 | Bidirectional jack | Step 4 jack | V1: -8 to +8 V, V2: -12 to +12 V |
| LED 1–4 | Indicator | Show active step | — |
| Steps switch | Toggle/selector | Limit cycle to 2, 3, or 4 steps | Version 2 only |

## In one sentence
Use the **A-151** whenever you want a clocked, resettable way to **cycle one signal through 4 destinations** or **cycle through 4 sources into one destination**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)