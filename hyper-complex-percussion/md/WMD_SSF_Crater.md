# WMD SSF — Crater

- [Manual PDF](../../manuals/Kick_Manual.pdf)

---

[Download the CRATER Eurorack Module Manual (PDF)](https://wmdevices.com/manuals/CraterManual_WEB.pdf)

---

# Exploring Hyper-Complex Rhythms with the WMD CRATER Kick Drum Module

## Overview

The **WMD CRATER** is a hybrid kick drum voice tailored for dense, modern electronic percussion. With its sound design flexibility (analog-digital hybrid, envelope shaping, clipping, and more), it's exceptionally suited for creating dense, rhythmic, and polyrhythmic percussion sequences. Below are actionable ideas and advanced tips for using CRATER in the pursuit of hyper-complex rhythms, especially in Eurorack modular systems.

---

## Fundamental Uses in Complex Percussion

### 1. **Kick Drum as Percussive Voice for Polyrhythms**
- **Gate/Trigger Input:**  
  Patch separate polyrhythmic gate/trigger sources (such as Euclidean sequencers, clock dividers, or custom trigger machines) into the **TRIGGER/ACCENT** and/or **ACCENT** inputs. This lets you layer accented and non-accented kicks on different rhythmic grids.
- **Layer With Variation:**  
  Chain multiple CRATERs, or use other percussion modules for cross-rhythms, but make CRATER the "pulse anchor" by feeding it complex gate patterns that don't line up traditionally (e.g., 5 vs 4, 7 vs 3).

### 2. **Complex Time Signatures**
- Use sequencers (like the Make Noise Rene, or vector-style sequencers) to generate odd-length gate patterns, piped directly into CRATER's trigger input. Reset the sequencer to different bar lengths for evolving time signatures.
- Feedback accent triggers on off-beats or shifting metric accents to create intricate accents and off-kilter multifold patterns.

---

## Manipulating Crater for Unique, Punchy Percussion

### 1. **Dynamic Tone Shaping with CV**
- **Pitch:**  
  Sequence the **PITCH** input using stepped or smoothly random CV to shift fundamental frequency for every trigger. This creates ever-morphing low-end emphasis, making patterns sound both organic and unpredictable.
- **Sustain:**  
  Use gated envelopes or LFOs to alter the **SUSTAIN** over time. With long sustains, CRATER morphs from a percussive thump to a bassline "rumble," especially when triggered by longer gate lengths.
- **Clipping & Saturation:**  
  Use the **CV control of SATURATION** before clipping for intense, morphing distortion effects. Patch in a stepped random or fast LFO voltage for evolving overtones.
- **Click Timbre & Decay:**  
  Modulate **CLICK TIMBRE** and **CLICK DECAY** using random sample & hold or slow CVs, cycling through the 14 click types on the fly for extreme timbral diversity.

### 2. **Envelope & Pitch Envelope Magic**
- **Pitch Envelope Amount/Decay:**  
  Use fast, snappy pitch envelopes for tight, FM-like cracks. Slow the envelope for timbale or tom-style polyphonic lines. Modulate the **Amount** & **Decay** for every hit via CV for unpredictable, 'living' percussion.

---

## Further Sound Design Techniques

### 1. **Accent for Ghost Notes & Microswings**
- Use **TRIGGER** and **ACCENT** creatively:  
  - Non-accented triggers for ghost notes.
  - Random or humanized triggers to **ACCENT** for shifting, dynamic impact within your complex rhythms.

### 2. **Layered Digital Clicks**
- Dial in a noisy click on offbeats, or use irregular clock sources to trigger just the click section (by modulating **CLICK LEVEL**, **TIMBRE**, or **DECAY**) for intricate high-frequency detail within your groove.

### 3. **Visual Feedback**
- Use the **LED Display** to visually correlate impact and density—helpful for fine-tuning exceptionally fast or nested patterns.

---

## Patch Inspiration: "Hyper Complex Modular Polyrhythm"

- **Step 1:** Chain CRATER’s trigger to a Euclidean sequencer's output set to 7 triggers per 16 steps.
- **Step 2:** Patch a second Euclidean or clock divider (say, 5 per 16) to ACCENT for a crisscrossing accent grid.
- **Step 3:** Modulate PITCH or CLICK TIMBRE with a random S&H triggered at yet another odd division.
- **Step 4:** Put a stepped LFO or envelope generator into the **SATURATION CV** for constantly shifting drive character.
- **Step 5:** Sequence SUSTAIN to shift between ultra-short and long ‘rumble bass’ sections, and automate the CLIPPING knob between clean and gabber-distortion mode during breakdowns or fills.
- **Result:** Asymmetrical, ever-changing, and deeply detailed kick patterns ideal for IDM, broken beat, glitch, or advanced industrial techno.

---

## Tips for Uniqueness & Punch

- Use **negative CV on SATURATION** for elegant transient softening or blend in mid-pattern.
- **Pair with clock-skipping utilities** or probabilistic gates to make the pattern less predictable but still tight.
- **Crosspatch envelope outputs to other percussion modules**—let CRATER be both pulse and modulator for further orchestrated polyrhythms.

---

**As always, the key to maximal percussive complexity lies in combining advanced triggering, modulation, and hands-on tweaking!**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)