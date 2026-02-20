# 2hp — Brst

- [Manual PDF](../../manuals/Brst_Manual.pdf)

---

[Download the 2hp Brst Manual (PDF)](https://www.2hp.com/docs/Brst_Manual.pdf)

---

# Creative Modulation Tips for 2hp Brst
*By a Eurorack Modular Synth Musician*

The **2hp Brst** is a voltage-controlled burst generator and trigger delay—compact, yet capable of injecting wild rhythmic mayhem, off-kilter grooves, and evolving textures into your modular system. Here's how you can modulate the Brst for unique sound design, with a focus on **distorted percussion**, **crazy basslines (dubstep, DnB)**, and **haunting atmospheric pads**.

---

## Core Panel Controls Recap

- **TRIG (1):** Trigger/gate input (2.5V threshold)
- **PULSES CV (2):** Modulate burst count (1-32)
- **PULSES (3):** Sets burst count
- **RATE CV (4):** Modulate timing between pulses (10ms–500ms)
- **RATE (5):** Sets timing between pulses
- **TRIG TOGGLE (6):** Include/exclude initial trigger
- **BURST LED (7):** Visual feedback
- **OUT (8):** Burst output (0–5V triggers)

---

## 1. Distorted Percussive Sounds

### **Patch Idea**
Use Brst to create rapid, glitchy trigger streams for a drum module, then distort the resulting audio.

#### **How to Modulate**
- **Clock Sync:** Send a clock or sequencer gate into TRIG for tempo-locked bursts.
- **Rate & Pulses CV:** Send an LFO, envelope, or stepped random source into RATE CV and/or PULSES CV. Try using a fast, intense LFO to RATE CV for pseudo-flams, ratchets, or metallic textures.
- **Audio-Rate Modulation:** Feed audio-rate signals (e.g., from another oscillator) into RATE CV for extreme stuttering/tearing rhythmic effects.
- **Distortion:** After your drum sound is triggered, process it with distortion, wavefolder, or bitcrusher for extra grit and character.

**Pro tip:** Rapid bursts (low RATE, high PULSES) into a snare or metal percussion voice + heavy distortion = *brutalist industrial snares*.

---

## 2. Crazy Basslines (Dubstep/Drum & Bass)

### **Patch Idea**
Use Brst bursts to create complex syncopated envelopes for bass VCF/VCA, sidechaining, or FM hits.

#### **How to Modulate**
- **Modulated Burst Rhythm:** Patch a sequencer or random gate source to TRIG. Modulate PULSES with a CV pattern in sync with your beat, so some notes have single, others rapid multi-triggers.
- **RATE Automation:** Send a stepped or smooth CV pattern (S&H, random, or LFO) to RATE CV to vary the speed of bursts, keeping bass hits unpredictable.
- **Bass Movement:** Use Brst OUT to trigger a fast envelope, which in turn modulates your bass synth’s filter cutoff, VCA, or FM amount on each burst.
- **Accent Triggers:** Use the TRIG TOGGLE to sometimes omit the first pulse, creating funky edits and fills.

**Pro tip:** Extreme PULSES/RATE modulation on bass filter envelopes with follow-up distortion = *neurofunk bass growls & wobbles*.

---

## 3. Haunting Atmospheric Pads

### **Patch Idea**
Use Brst to inject subtle, evolving rhythmic texture into long, droning pad sounds.

#### **How to Modulate**
- **Randomization:** Patch a slow random source (Wogglebug, Turing Machine, etc.) into both PULSES CV and RATE CV, making bursts unpredictable—tiny blips, long clusters, etc.
- **Envelope Triggers:** Use Brst’s OUT to trigger percussive envelopes or LPGs controlling textures, noise, grains, or filter parameters in your pad chain. 
- **Sparse Mode:** Set RATE high (long delays between pulses), PULSES low or under voltage control, to create ghostly or “rain drop” style trigger events mapped to reverb, delay sends, or granular samplers.
- **Layering:** Mult Brst’s OUT to several destinations so different pad and effect parameters change slightly on each burst.

**Pro tip:** Try “bursting” clouds of plucked string or bell tones deep in a reverb, modulating RATE and PULSES for an ever-evolving spectral wash.

---

## Patch Examples

| Sound Type            | TRIG Source   | PULSES CV                | RATE CV                      | Output Goes To     |
|-----------------------|--------------|--------------------------|------------------------------|--------------------|
| Distorted Snare       | Clock        | Envelope or LFO          | Audio-rate Osc/LFO           | Drum module/env    |
| DnB Bass Envelope     | Seq. gates   | Sequencer CV             | Stepped random/LFO           | Fast env for VCF/VCA|
| Haunting Pad Texture  | Slow random  | Smooth random            | Slow LFO or S&H              | LPG/filter/noise   |

---

## Advanced Modulation Tips

- **VCA Before CV Inputs:** Place a VCA or CV processor before RATE/PULSES CV for dynamic control over burst patterns via pressure (CV) or automation.
- **Inter-modulation:** Use Brst’s own output, via attenuverter, back into its RATE/PULSES CV for self-modulating, feedback-style randomization.
- **Burst Layering:** Use two Brst modules in parallel, cross-modulating each other's CVs for chaotic polyrhythms.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)