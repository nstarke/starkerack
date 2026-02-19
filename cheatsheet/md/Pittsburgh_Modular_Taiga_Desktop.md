# Pittsburgh Modular — Taiga Desktop

- [Manual PDF](../../manuals/Taiga+Desktop+Manual+v2.pdf)

---

[Taiga Desktop Electronic Musical Instrument Manual V2.0 (PDF)](https://pittsburghmodular.com/manuals/taiga_manual.pdf)

# Pittsburgh Modular Taiga Eurorack Module Cheat Sheet

A powerful all-in-one semi-modular analog synthesizer voice with deep MIDI integration, three complex oscillators, mixers, multi-mode filter, dual ADSR, VCA/dynamics, analog delay, and utility modules. Fully eurorack compatible; all internal connections can be overridden via patch cables.

---

## **Power & Setup**
- **Power**: 16-pin Eurorack ribbon, connects to standard +/-12V. **650mA (+12V), 475mA (-12V)**
- **Don't hot-plug**: Always power off your case before plugging/unplugging.
- **-12V stripe line up required**.
- **All connections (except MIDI):** 3.5mm mono jacks; MIDI uses 1/8" TRS to DIN adapter.

---

## **Panel Controls & Sections**
**All button edits:** Hold [Edit] to access secondary (yellow-labeled) button features.

**Main Sections:**  
- Control (MIDI/CV, clock, arp, mod tools)
- 3 Oscillators (complex analog, waveshaping)
- Dual Mixer / Preamp
- Utilities (LFO, noise, S&H, splitter/mixer)
- Multimode Filter (analog state-variable: LP/BP/HP/Notch)
- Dual ADSR
- Dynamics (VCA/LPG/Pluck)
- Analog Delay (BBD)
- Output

### **Knobs & Buttons Reference**

| Function                                 | Knob/Button    | Section          |
|-------------------------------------------|----------------|------------------|
| Glide                                    | 1              | Control          |
| Clock                                    | 2 (Button), 3 (LED)       | Control          |
| ARP/Seq                                  | 4 (LED), 5 (Button)         | Control          |
| Octave Up/Down                           | 8,9,10,11      | Control          |
| Edit                                     | 12 (Button)    | Control          |
| Osc Pitch, Shape, FM, Shape CV           | 13-16,22,23-26,32,33-36,42 | Oscillator      |
| Osc Seed (waveform select)               | 21,31,41       | Oscillator       |
| Mixer Ch 1-4, Preamp Gain/Level          | 43-48          | Mixer/Preamp     |
| LFO Rate                                 | 49             | Utility          |
| Filter Freq, Res, Mode, CV1/CV2          | 51-58          | Filter           |
| ADSR (A, D, S, R) 1 & 2                  | 59-63, 64-68   | ADSR             |
| Dynamics knobs (Resonance, Response, Mode, CV, LPG, Pluck) | 69-78 | Dynamics     |
| Output Volume                            | 79             | Output           |
| Delay (Time, Regen, Mix, Time CV)        | 80-83          | Echos            |

---

## **Jacks Reference (Numbers refer to illustrated panel in manual)**

### **Control**

- **84. Control Clock In/Out**: Input/output, 0V=off, 5V=on (CV/gate).  
- **85. MIDI Input**: Type A 1/8" TRS MIDI in.
- **86. Control Pitch Output**: 1V/oct CV out, 0–5V
- **87. Control Gate Output**: 0/5V gate
- **88. Control Velocity Output**: 0–5V velocity/paraphonic/random
- **89. Control CC/Mod Output**: 0–5V from chosen MIDI CC, LFO, etc.

### **Oscillators 1/2/3**

| Input/Output     | Function                      | Voltage     |
|------------------|------------------------------|-------------|
| Pitch In (90, 96, 102)| 1V/oct CV in           | 0–5V(?) CV  |
| Shape CV In (91, 97, 103) | For wavefolder     | 0–5V CV     |
| FM In (92, 98, 104)      | Linear FM           | Audio-rate  |
| Sync In (94, 100, 106)   | Reset/hard sync     | Any pulse   |
| Sine Out (93, 99, 105)   | Clean sine          | Audio       |
| Audio Out (95, 101, 107) | Shaped output       | Audio       |

### **Mixer/Preamp**

| Input/Output                  | Jack No | Notes        |
|-------------------------------|---------|--------------|
| Mixer Ch 1–4 In               | 112-115 | Normaled to Oscs 1–3, noise |
| Mixer 1+2 Out                 | 116     | Sends Ch 1+2 summed         |
| Mixer Out                     | 117     | Master sum (preamp in norm) |
| Preamp In                     | 108     | For external/excess signal  |
| Preamp Out                    | 109     | Soft clip, normaled to Mixer Out |

### **Utilities**

| Input/Output             | Jack No | Notes                         |
|--------------------------|---------|-------------------------------|
| LFO Triangle Out         | 110     | ±5V                           |
| LFO Square Out           | 111     | ±5V                           |
| Noise Out                | 119     | ±5V, white-pink               |
| S&H Sample In            | 118     | Normaled to noise             |
| S&H Hold In              | 120     | Normaled to clock             |
| S&H Out                  | 121     | As sampled (CV/Audio)         |
| Mixer/Splitter In 1/2    | 130,132 | Unity mix/buff split          |
| Mixer/Splitter Out 1/2   | 131,133 | Unity mix/buff split          |

### **Filter**

| Input/Output                    | Jack No | Voltage           |
|----------------------------------|---------|-------------------|
| Freq CV 1 (attenuator)          | 122     | Bi-polar, ±5V     |
| Freq CV 2 (attenuverter)        | 124     | Bi-polar, ±5V     |
| Audio In                        | 123     | Normaled to mixer |
| Audio Out                       | 125     | Audio             |

### **ADSR (x2)**

| Input/Output     | Jack No | Voltage           |
|------------------|---------|-------------------|
| Gate In          | 126/128 | Trigger/Gate      |
| Envelope Out     | 127/129 | 0–10V             |

### **Dynamics**

| Input/Output             | Jack No | Voltage          |
|--------------------------|---------|------------------|
| CV In                    | 134     | Amplitude CV; 0–10V |
| Resp. CV In              | 136     | Decay/response; ±5V |
| Audio In                 | 135     | Normaled filter out  |
| Audio Out                | 137     | Audio out           |

### **Delay (Echos)**

| Input/Output       | Jack No |  Voltage        |
|--------------------|---------|-----------------|
| Time CV In         | 140     | ±5V or ±10V     |
| Audio In           | 138     | Normaled to dynamics out|
| Audio Out          | 139     | Audio           |

### **Output**

| Input/Output      | Jack No    | Voltage         |
|-------------------|------------|-----------------|
| Input             | 141        | Normaled to delay out |
| Main Out          | 142        | Line-level mono |
| Headphones Out    | 143        | Stereo (mono L/R) |

---

## **Voltage Ranges (by function):**
- **Gate signals**: 0V (off), +5V (on)
- **Pitch (1V/oct)**: 0–5V (standard)
- **ADSR Out**: 0–10V
- **LFO/Mods**: ±5V
- **Velocity/CC/Mod**: 0–5V
- **Mixer, Filter, Dynamics, Delay**: standard modular audio; can soft clip
- **Filter/Dynamics CV inputs:** ±5V preferred for bi-polar/attenuverters

---

## **Panel Labeling Quick Reference**
- **Green**: CV/audio input jacks  
- **White**: output jacks, primary button functions  
- **Yellow**: secondary (Edit) button hold functions

---

## **Digital Function Shortcuts**
- **Arpeggiator, Sequencer, Hold, Octave Shift**: see section 5 for [Edit Button] + combo cheats
- **Random/Clocked parameters**: Hold Seed or Filter Mode + [Clock] for random cycles
- **Paraphonic Mode**: Use Vel out to Pitch in, calibrate as per sec 15  
- **Factory Reset**: Hold [Oct Up] + [Oct Down] + [Dynamics Mode] for 5 seconds

---

## **Notable Defaults / Normalings**
- MIDI→Oscs, Arp, Velocity, Gate via internal (can disable per module)
- Mixer feeds filter, filter→dynamics, dynamics→delay, delay→out
- All major CV ins normaled to internal mod sources (LFO triangle, ADSRs, etc), overridden when patched

---

## **Patch Examples**
- **Basic Subtractive Voice**: Use default internal routing, play from MIDI
- **West Coast**: Patch Velocity out to Osc Pitch, patch S&H/noise/random to modulation ins, LPG mode in dynamics
- **Feedback/Overload**: Patch Output or Preamp out back into Mixer/Preamp in for wild timbral effects

---

### **Useful Links**
- [Taiga Manual PDF](https://pittsburghmodular.com/manuals/taiga_manual.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)