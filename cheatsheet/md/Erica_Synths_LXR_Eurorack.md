# Erica Synths — LXR Eurorack

- [Manual PDF](../../manuals/LXR_eurorack_manual.pdf)

---

# Erica Synths x Sonic Potions LXR Eurorack Module Cheat Sheet

**Manual PDF:**  
[Erica Synths LXR Eurorack Manual PDF (official)](https://www.ericasynths.lv/storage/products/LXR_eurorack/LXR-EURORACK-OWNERS-MANUAL.pdf)

---

## **Module Overview**

The **Erica Synths x Sonic Potions LXR Eurorack Module** is a 6-voice digital drum synthesizer with deep sound shaping, modulation, and performance capabilities. Each voice is highly programmable and can simulate classic analog drum sounds or venture deep into digital territory.

---

## **Panel Reference – Jacks, Knobs, Buttons**

### **Input & Output Jacks**

#### **Audio Outputs (2nd Row, L→R):**
- **OUT 1 – 4 (4 jacks)**: Assignable, DC-coupled, 10Vpp, Output Impedance: 100 Ω
- **Stereo out possible as two pairs, or as 4 mono outputs**
- **FX Bus:** Assign voices to FX-processed output

#### **Trigger Inputs (Top Row, L→R):**
- **DRUM1 – DRUM3, SNARE, CLP/CYM, CL HH, OP HH:** 7x 3.5mm jacks, 5V trigger

#### **Accent Inputs:**
- **ACC1 – ACC6:** 6x 3.5mm jacks, 5V for velocity/accent per-voice

#### **CV Inputs:**
- **CV1 – CV5:** 5x 3.5mm jacks, assignable to almost any parameter via the mod matrix
    - **Voltage Range:** -5V to +5V

---

### **Controls:**

#### **Knobs & Encoder:**
- **4 Endless Pots** below screen: Adjust highlighted parameter values
- **Encoder:** Navigate menus, push to enter/exit parameter detail edit

#### **Buttons:**
- **MENU BUTTONS (Labeled EDIT, PERFORM, MOD, FX, DATA, etc.):** Select module operating mode
- **7 SELECT Buttons:** Switch between parameter menu sections or select voices (when holding DRUM button)
- **DRUM Button:** Hold + SELECT to change the active voice
- **SHIFT Button:** For secondary functions (e.g. SHIFT + FX for FX, SHIFT + SAVE/LOAD for global settings)
- **SAVE/LOAD:** Load or save kits

---

### **Modes & Menu Navigation**

#### **EDIT Mode:**
- Edit parameters for each voice
- DRUM + SELECT = choose active voice
- SELECT alone = change to a menu section (OSC, AEG, MOD, FM, CLICK, FIL, MIX)

#### **PERFORMANCE Mode:**
- Jam mode (no editing), trigger sounds or morph between kits

#### **MODULATION Menu:**
- Assign 3 slots per voice:
    - Sources: 5 CVs, 6 LFOs, 6 Accent inputs
    - Destinations: Any voice parameter, 1V/Oct support for tonal play (src: "v/o", amt: 100%)

#### **LFOs:**
- 6 LFOs, classic shapes (sin/tri/saw/sqr/rnd/xup/xdn)
- Assign via MOD menu, retrigger available

#### **FX Mode:**
- 1 global FX at a time: Drive (distortion), Ringmod, Compressor, Delay
- Route voices to FX via MIX page

---

## **Quick Reference: Parameter Pages**

| Menu Page | Key Parameters                  | Description                                 |
|-----------|---------------------------------|---------------------------------------------|
| **OSC**   | coa, fin, wav, pwm              | Oscillator freq/waveform                    |
| **AEG**   | att, dec, slp, rpt (clap)       | Amplitude envelope (attack, decay, shape)   |
| **MOD**   | dec, slp, mod, vol              | Extra envelopes, accent to volume           |
| **FM**    | amt, frq, wav, mod              | FM Osc, mode, ratio                        |
| **CLICK** | wav, vol, frq                   | Transient generator, snappy/offset/sample   |
| **FIL**   | frq, res, typ, drv              | Filter (freq, type: LP, HP, BP, etc.)       |
| **MIX**   | vol, pan, sr, drv, out          | Volume, panning, FX/output routing          |

---

## **Saving & Loading Kits**

- **Load:** Press SAVE/LOAD, use encoder to select, press encoder to confirm
- **Save:** SHIFT + SAVE/LOAD, select slot, confirm and name/edit

---

## **Global Settings**

- **SHIFT + SAVE/LOAD**: Access settings (when both are pressed).
    - **Screensaver**: On/Off
    - **CV Routing:** Global/per-kit

---

## **Firmware Update**

- Copy latest `.img` file to SD root, power up holding encoder, follow prompts on display

---

## **Electrical/Mechanical Specs**

- **Audio Output:** 10Vpp, 100 Ω unbalanced
- **CV Inputs:** -5V to +5V
- **Power Draw:** +12V (88mA typical, 160mA peak), -12V (10mA typ, 12mA peak)
- **Triggers/Accent:** 5V
- **Physical:** 28HP wide, 35mm deep

---

## **Tips**

- Use performance mode to morph between sounds live.
- Modulate any parameter (including 1V/Oct pitch) with CV.
- Use envelopes, filter types, repeat, transients, FX for deep drum shaping.

---

## **Links**

- **[Official Manual PDF](https://www.ericasynths.lv/storage/products/LXR_eurorack/LXR-EURORACK-OWNERS-MANUAL.pdf)**
- **[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**

---

**Happy patching!**