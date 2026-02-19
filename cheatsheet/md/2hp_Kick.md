# 2hp — Kick

- [Manual PDF](../../manuals/2hp_Kick.pdf)

---

[Manual PDF (image reference)](#) <!-- Update with actual link if available -->

---

# **Kick Eurorack Module Cheat Sheet**

## **Summary**
Kick is a flexible analog kick drum synthesizer module. It features CV control over all main parameters, 1V/Octave pitch tracking, and a wide decay/tone range (from sine to overdriven, distorted kicks).

---

## **Panel Controls & Jacks**

| # | Name    | Type   | Function/Range / Notes                                                       |
|:-:|---------|--------|-------------------------------------------------------------------------------|
| 1 | **TRIG**   | Jack   | **Trigger Input:** Accepts gate signals to trigger the kick.                  |
| 2 | **TONE**   | Knob + Jack | **Tone/Character:**<br>Knob - sets from clean sine (center/right) to overdrive (left);<br>CV Input (-5V to +5V) |
| 3 | **DECAY**  | Knob + Jack | **Decay Time:**<br>Knob - sets decay 80ms up to 15s;<br>CV Input (-5V to +5V, adds to pot)        |
| 4 | **V/OCT**  | Jack   | **Pitch CV Input:** 1V/Oct for tonal playing/sequencing;<br>Adds to Pitch knob|
| 5 | **PITCH**  | Knob   | **Pitch Control:** Sets base frequency of drum sound                        |
| 6 | **OUT**    | Jack   | **Audio Output:** Drum audio, 10Vpp (peak-to-peak)                          |

---

### **Voltage Ranges**

- **TONE CV Input:** -5V to +5V  
- **DECAY CV Input:** -5V to +5V  
- **V/OCT (Pitch):** Standard 1V/octave  
- **Audio OUT:** 10Vpp

---

## **Quick Reference Table**

| Control | CV Range | Function |
|---------|----------|----------|
| TONE (knob + jack) | -5V to +5V | Sine (center/right) → Overdrive (left); pitch mod (higher when left/right) |
| DECAY (knob + jack) | -5V to +5V | Decay time 80ms–15s, CV adds to knob |
| V/OCT (jack) | 1V/oct | Tonal pitch/frequency |
| PITCH (knob) | n/a | Base pitch of drum |
| OUT (jack) | 10Vpp | Drum audio output (patch to mixer/FX, etc.) |
| TRIG (jack) | Gate/Trig | Triggers drum envelope |

---

## **Installation**

- **Width:** 2 HP
- **Depth:** 42mm
- **Power:** +12V: 74mA, -12V: 2mA
- **Red stripe:** must face -12V (usually bottom)
- **Secure ribbon to both module and bus board.**

---

## **Suggested Use**

- Sequence via gate/trigger to **TRIG**.
- Sequence pitch via 1V/Oct to **V/OCT** for tuned drums/basslines.
- Modulate **TONE** and **DECAY** for variation and dynamic kicks.
- Run **OUT** to your drum mix, VCA, or FX modules.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)