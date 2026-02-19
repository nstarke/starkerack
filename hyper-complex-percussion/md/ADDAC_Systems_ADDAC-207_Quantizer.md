# ADDAC Systems — ADDAC-207 Quantizer

- [Manual PDF](../../manuals/ADDAC_207_Quantizer_REV05.pdf)

---

[**ADDAC207 Intuitive Quantizer Manual PDF**](https://www.addacsystem.com/Manuals/ADDAC207-Intuitive-Quantizer-User-Guide.pdf)

---

# Using the ADDAC207 Intuitive Quantizer for Densely Rhythmic, Hyper-Complex Percussion Sequences

As a Eurorack artist, the ADDAC207 is a powerful tool to introduce advanced rhythm, timing, and tonal complexity into your percussion programming. Here’s a focused strategy to use it for hyper-complex, polyrhythmic percussion:

---

## 1. **Module Overview in Percussion Context**
- **Type:** Multi-channel CV quantizer (not a voice or effect, but a pitch/voltage processor—can act as a rhythmic switch/logic utility for percussion).
- **Key Features for Rhythm:**
  - Four independent quantizer channels (Voices), each with its own inputs and GATE output.
  - Flexible scale/key selection, user-chosen intervals, microtonal options.
  - Per-channel Gate Length control (10ms to 10s+!).
  - External Trigger/Gate Inputs for each channel (for sync or retriggering).
  - Assignable CV input for menu functions (remote, sequencer, or LFO modulation).

---

## 2. **Building Polyrhythms & Complex Patterns**

### **A. CV-to-Gate Percussion Triggering**
- **Voice Outs → Percussion Modules:**  
  Patch the GATE OUT of multiple voices (1–4) to percussion module trigger inputs (kick, snare, hats, etc).
- **Multiple Gate Lengths:**  
  Assign each output a different gate length for each percussive voice, using the Intuitive Menu (Button 6). This can create “flams,” rolls, ratchets, or ghost notes.
- **Asymmetric Triggering:**  
  Quantize multiple asynchronous CV sources (different sequencers, random patterns, S&H, or LFOs) into the four voices. With each quantized to a different scale or interval, it forces the triggers (Gate Outs) into unique timing grids.
- **Polymeter/Polyrhythm:**  
  Route clock-divided signals into each channel’s Gate Input. Voice 1 = /4, Voice 2 = /5, Voice 3 = /7, Voice 4 = /9 divisions—a fast way to create fluid polyrhythmic triggers.

### **B. Quantizer as a Creative Clock Divider/Mangler**
- **Trigger Inputs:**  
  Send complex, irregular clocks or Euclidean pulses to the Gate In jacks. Each channel quantizes only on incoming gates (gated quantization), generating new rhythms driven by your external logic/gates.

### **C. Complicated Melodic Percussion**
- **Assign Intervals:**  
  Use interval assignment for Voice 2–4 (chord modes). Set Voices 2–4 to intervals like 7th, 9th, 11th, 13th. Send CV from a trigger sequence to the first voice. Each percussion hit can have multiple, controlled harmonic variations, generating tuned percussion chords or clusters.
- **Transpose Inputs:**  
  Use the ASSIGN input with an LFO or further random/stepped CV to shift the root or intervals. Modulating this with fast stepped random can cause quantizer pattern “rotation,” instantly creating complex fills, tuplet divisions, and breakbeats.

---

## 3. **Techniques for Unique, Punchy Percussion**

### **A. Microtonal & Temperament Mode**
- **Non-Standard Scales:**  
  Set the quantizer to Bohlen-Pierce, Just, or Exotic temperaments (Buttons 5–9 in Tuning Menu). Passing noisy or random CV through these scales, then using gates for triggers, produces unexpected “off-grid” events—great for glitch or experimental percussion.

### **B. Gate Length & Gate-Off Condition**
- **Gate Off for Syncopation:**  
  Set long gate lengths (>500ms) on one or more voices, use the “Gate Off Condition” (Button 12 in Gate Length Menu) so new triggers only happen when gate is low: this delays and “pushes” notes in time, making the rhythm uneven/complex.
- **Fast Chops & Ratchets:**  
  Run GATE OUT to a fast analog envelope into percussive VCAs—use shortest gate times for rapid-fire percussion.

### **C. CV Assign for Live / Algorithmic Mutation**
- **Automated Pattern Morphing:**  
  Use an LFO or random stepped voltage into the ASSIGN CV jack, assign to “Change Preset” (Button 12) or “Quantization Type” (Button 5), so the module’s whole rhythmic/interval logic is switched or morphed mid-sequence.

### **D. Modular "Keyboard Mode" Tricks**
- **Monophonic Keyboard as Percussion Selector:**  
  Hold Button 1 to enter Keyboard Mode. Use manual button jabs or a voltage-addressed switch to trigger specific rhythm voices, playing percussive melodies or fills live.

---

## 4. **Patch Example: Dense Polyrhythmic Percussion Grid**

- **Sequencer 1 (slow random):** → CV IN 1 (Voice 1): Quantizes to Dorian scale, GATE OUT 1 → Perc Module 1 (Kick)
- **Sequencer 2 (faster, odd clock):** → CV IN 2 (Voice 2): Quantizes to Just scale, GATE OUT 2 → Perc Module 2 (Snare)
- **LFO (audio rate, bursty):** → CV IN 3 (Voice 3): Bohlen-Pierce scale, GATE OUT 3 → Perc Module 3 (Bongos)
- **Stepped Random:** → ASSIGN CV (set to Preset Change & Gate Length): Mutates patterns, fills, breaks.
- **All Gate OUTs:** Go to VCAs with short attack—shaping each percussion hit for extra punch.

---

## 5. **Advanced: ADDAC207 as Meta-Pattern Modulator**

- **Preset Switching:**  
  Rapid/cv-driven preset switching for sudden metric/time signature changes—makes the grid “breathe” and stumble in intentional ways.
- **Negative Octave Offset:**  
  Set certain voices to negative octave offset, forcing extremely low-frequency triggers (subsonics) mixed with higher, on-grid triggers.

---

## 6. **Summary Table: Unique Rhythmic Approaches**

| Feature         | Use Case for Percussion             |
|-----------------|------------------------------------|
| Gate In         | Sync with other complex trigger sources & clocks |
| Gate Out        | Directly pings drum modules/VCAs for percussive structure |
| Multiple Voices | Each quantized differently → multi-instrument polyrhythms |
| Interval Assign | Chorded/rippled triggers for complex accents |
| CV Assign       | Remote mutation of quantizer logic (for fills/chaos/variation) |
| Gate Length     | "Ratchet," roll, or extend percussion articulation |
| Nonstandard Scales | Glitchy, off-grid, experimental hits |
| Keyboard Mode   | Live-reassign any drum voice by hand or with voltage switching |

---

## 7. **Keep It Unique, Punchy, and Percussive**
- Use fast, short gates for tight transients.
- Leverage microtonality/temperaments to make “gridless” snare fills or rimshots.
- Harness polyrhythm via asynchronous triggers into each channel.
- Automate menu changes with the Assign input for evolving, “alive” drum programming.

---

> If you want more ideas or patch recipes, [grab the manual here (PDF)](https://www.addacsystem.com/Manuals/ADDAC207-Intuitive-Quantizer-User-Guide.pdf).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)