# Pittsburgh Modular — "Generator"

- [Manual PDF](../../manuals/Generator - Pittsburgh Modular Synthesizers.pdf)

---

[Manual PDF / Source](https://pittsburghmodular.com/generator)

# Pittsburgh Modular Generator — Cheat Sheet

**Type:** Dual oscillator / FM voice  
**Status:** No longer in production  
**Size:** 10 HP  
**Depth:** 35 mm  
**Power:** 30 mA

## What it does
Generator is a **2-oscillator FM-focused sound source** built around two **triangle-core wide-range oscillators**. It excels at:
- internal FM tones
- metallic percussion
- harsh modulation
- drones / textures
- noise / glitchy digital-like sounds

A key concept: **Oscillator 1 feeds an internal VCA (“Index”) whose output internally FM-modulates Oscillator 2.**

It is **not 1V/oct** and **not temperature compensated**, so think of it more as an **FM/timbre oscillator** than a precision melodic VCO.

---

## Quick start
1. Patch **OUT** or **2** to your mixer/VCA.
2. Set both oscillators to **Mid** or **High** range.
3. Adjust **GEN1 RANGE** and **GEN2 RANGE** for base pitch.
4. Turn **INDEX** to control how much Osc 1 internally FM’s Osc 2.
5. Sweep **SHAPE** to morph both oscillators’ waveforms.
6. Use **EXTERNAL IN** plus its attenuverter to add more FM to either osc.
7. For dynamic timbre, patch an envelope or LFO into **INDEX CV**.

---

## Signal flow
- **Generator 1 output (“1”)** = raw Oscillator 1, **pre-Index VCA**
- **Index VCA** controls Generator 1 level
- **OUT** = Oscillator 1 **post-Index VCA**
- **OUT** is also the **internal FM source** sent to Generator 2
- **Generator 2 output (“2”)** = Oscillator 2 audio output
- **EXTERNAL IN** can FM either Generator 1 or 2 depending on destination switch

---

## Controls

## GEN1 row
### EXP jack
Exponential CV input for **Generator 1** frequency.  
- Exponential response
- **Does not track 1V/oct**
- Voltage range: **not specified in manual**

### 3-way range switch
Coarse frequency range for Generator 1:
- **Left = Low**
- **Center = High**
- **Right = Mid**

### RANGE knob
Fine frequency control for Generator 1.

---

## EXTERNAL row
### INPUT ATTENUVERTER knob
Controls amount/polarity of **EXTERNAL IN** modulation.
- Full left: inverted modulation, max amount
- 12 o’clock: 0
- Full right: positive modulation, max amount

### DESTINATION switch
Chooses which oscillator gets modulated by **EXTERNAL IN**:
- **Up = Generator 1**
- **Down = Generator 2**

### EXTERNAL IN jack
Accepts CV or audio-rate signals as FM/modulation source.  
- Voltage range: **not specified in manual**

---

## GEN2 row
### EXP jack
Exponential CV input for **Generator 2** frequency.  
- Exponential response
- **Does not track 1V/oct**
- Voltage range: **not specified in manual**

### 3-way range switch
Coarse frequency range for Generator 2:
- **Left = Low**
- **Center = High**
- **Right = Mid**

### RANGE knob
Fine frequency control for Generator 2.

### Internal FM note
Generator 2 is internally FM’d by **Generator 1 Index Out**. The amount is controlled by:
- **INDEX knob**
- **INDEX CV**

---

## SHAPE row
### SHAPE knob
Morphs both oscillators’ waveforms simultaneously:

- **Full left**
  - Generator 1 = **Square**
  - Generator 2 = **Triangle**

- **Full right**
  - Generator 1 = **Triangle**
  - Generator 2 = **Square**

### 1 jack
Audio output for **Generator 1**, **pre-Index VCA**.  
- Voltage range: **not specified in manual**

### 2 jack
Audio output for **Generator 2**.  
- Voltage range: **not specified in manual**

---

## INDEX row
### CV jack
CV input for the **Index VCA**.  
This controls Generator 1’s VCA, which in turn controls:
- **OUT level**
- amount of **internal FM sent to Generator 2**

Voltage range: **not specified in manual**

### OUT jack
**Post-Index VCA Generator 1 output**.  
Also serves as the source for internal FM to Generator 2.  
Voltage range: **not specified in manual**

### INDEX knob
Gain control for Generator 1 Index VCA:
- **Full left = 100% gain**
- **Full right = 0% gain**

Important: this knob is **not** a normal CV attenuator.  
- Full left gives full output regardless of CV
- Full right allows strongest effect from incoming **INDEX CV**

---

## Jack reference

| Jack | Type | Function | Voltage range |
|---|---|---|---|
| **GEN1 EXP** | CV input | Exponential frequency control for Generator 1 | **Not specified** |
| **EXTERNAL IN** | CV/audio input | External FM/modulation source for selected oscillator | **Not specified** |
| **GEN2 EXP** | CV input | Exponential frequency control for Generator 2 | **Not specified** |
| **1** | Audio output | Generator 1 output, pre-Index VCA | **Not specified** |
| **2** | Audio output | Generator 2 output | **Not specified** |
| **INDEX CV** | CV input | Controls Index VCA / internal FM amount | **Not specified** |
| **OUT** | Audio output | Generator 1 post-Index VCA output; internal FM source to Gen2 | **Not specified** |

---

## Control reference

| Control | Type | Function |
|---|---|---|
| **GEN1 RANGE switch** | 3-way toggle | Gen1 coarse range: Left Low / Center High / Right Mid |
| **GEN1 RANGE knob** | Knob | Gen1 fine frequency |
| **EXTERNAL ATTENUVERTER** | Knob | Amount/polarity of external modulation |
| **DESTINATION switch** | Toggle | External modulation target: Up Gen1 / Down Gen2 |
| **GEN2 RANGE switch** | 3-way toggle | Gen2 coarse range: Left Low / Center High / Right Mid |
| **GEN2 RANGE knob** | Knob | Gen2 fine frequency |
| **SHAPE** | Knob | Simultaneous waveform morph for both oscillators |
| **INDEX** | Knob | Gain of Generator 1 Index VCA / internal FM amount to Gen2 |

---

## Practical patch tips

### 1. Internal FM voice
- Listen to **2**
- Set both oscillators in **Mid**
- Use **INDEX** to add internal FM
- Sweep **SHAPE** for timbre changes

This is the core Generator sound.

### 2. Metallic percussion
- Patch an envelope to **INDEX CV**
- Listen to **OUT** or **2**
- Put **GEN1** in **Low**
- Put **GEN2** in **Mid**
- Fine-tune both frequency knobs

This matches the manual’s suggested percussion approach.

### 3. Cross-mod style patch
- Patch **2** into **EXTERNAL IN**
- Set destination switch **Up** to modulate **GEN1**
- Use **INDEX CV** for animated internal FM
- Listen to **OUT** or **2**

Great for chaotic, aggressive, unstable FM.

### 4. Separate dual oscillator use
- Take **1** and **2** as two independent audio sources
- Keep **INDEX** lower if you want less internal FM interaction
- Use **SHAPE** as a dual timbre control

---

## Important caveats
- **Not a precision pitch VCO**
- **No 1V/oct tracking**
- **No voltage ranges given in the manual** for I/O
- Best treated as an **experimental FM oscillator / sound generator**

---

## Best-use summary
Use Generator when you want:
- brutal FM
- percussion and clangs
- shifting drone textures
- unstable digital-ish sounds from analog circuits
- one compact module that can act as both sound source and modulation source

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)