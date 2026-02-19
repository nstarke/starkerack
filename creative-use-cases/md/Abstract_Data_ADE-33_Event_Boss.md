# Abstract Data — ADE-33 Event Boss

- [Manual PDF](../../manuals/ADE33_Manual_v1_0.pdf)

---

[Abstract Data ADE-33 Event Boss Manual PDF](http://www.abstractdata.biz/docs/ADE-33-User-Guide-v1_0_1.pdf)

---

# Creative Uses for the Abstract Data ADE-33 Event Boss in a Modular Synth Setup

The ADE-33 Event Boss is a deep rhythm/pattern processor capable of transforming simple clock/gate/LFO/CV signals into complex, evolving trigger, gate, and rhythm patterns. With its 6 Global Modes (Variables, Multiples, Probability, Logic, Phase, Gates), each containing 6 Local sub-modes, you can integrate it in countless creative ways with other Eurorack modules to generate and manipulate patterns for percussive, melodic, and modulation purposes.

Here are creative patching ideas:

---

## 1. **Rhythm Humanizer and Variation Maker**
**Combine With:**  
- Mutable Instruments Grids or Delptronics Trigger Man (for trigger/gate pattern sources)
- Mutable Instruments Marbles (randomness/inspiration)
- Any basic clock (from Pamela’s PRO Workout, Tempi, or even a square LFO like Intellijel Dixie)

**Patch Idea:**  
- Feed your main clock or rhythm output into ADE-33 GATE A1.
- Use Marbles’ random stepped output or an LFO into GATE B/CV to modulate the ADE-33’s Probability or Variables modes.
- Send ADE-33 OUT to Triggers for drum voices or sequencing (Tiptop Audio ONE, Erica Synths Pico Drums).
- Live tweaks or CV into Event Boss morph patterns for continually evolving beats.  
**Result:** Your static patterns become dynamic, organic, probability-driven grooves.

---

## 2. **Pseudo-Polyrhythm/Polymeter Creator**
**Combine With:**  
- Pamela’s PRO Workout or ALM Busy Circuits Pam’s New Workout
- 2hp Div, Doepfer A-160-2 Clock Divider/Multiplier
- Anything that requires clocking at different rates: sequencers, quantizers, triggerable synth voices

**Patch Idea:**  
- Run clock into GATE A1 and a divided or multiplied clock into GATE B/CV.
- Use Multiples mode to multiply/divide incoming clocks differently per Local Mode.
- Output unique divisional patterns (e.g. 5 against 4, 7 against 8) to different sequencers or voices for unusual polyrhythms.
- Use reset input to bring complex patterns back in sync occasionally for musical chaos and order!  
**Result:** Polydivisional rhythmic backbones for generative music, IDM, or cinematic scoring.

---

## 3. **Chance-Based Melodic Progressions**
**Combine With:**  
- Sequencers (Make Noise René, Malekko Voltage Block, Hermod, or even basic analog step sequencer)
- Quantizer (Doepfer A-156, Intellijel uScale)
- VCO or Sample Player (for melodic voices)

**Patch Idea:**  
- Send the output of Event Boss in Probability mode (OUT triggers) to the sequencer’s step or reset input.
- Use a random or slowly evolving LFO into GATE B/CV to modulate probability/chance rates.
- This skips or retriggers sequencer steps at random, creating chance-driven melodic contour.
- Use Phase or Gates mode to swing/evolve step triggers for “humanized” play.  
**Result:** Non-repeating, generative arpeggios and melodies—perfect for ambient or Berlin School sequences.

---

## 4. **Logic "Drum Fill" Generator**
**Combine With:**  
- Any drum modules (Noise Engineering Basimilus, WMD Crater, etc.)
- Two unrelated or related clocks/patterns (Pam’s Workout, Tempi, clock output from a sequencer)

**Patch Idea:**  
- Patch two rhythm sources to GATE A1 and GATE B/CV.
- Set Event Boss to Logic mode, cycling between AND, OR, XOR etc., to create fills or accents based on logical combinations of two patterns.
- Use the A1/A2 select input for further live or CV-controlled logic changes.
- Output to drum voice triggers, or re-combine for more complex patterning using another ADE-33 channel!  
**Result:** Smart, math-driven percussion fills and complex pattern interweaves.

---

## 5. **Time-Shifting & Swing Patterns**
**Combine With:**  
- Gate sequencers (Intellijel Steppy, Verbos Sequence Selector)
- Delay modules for CV (ALM Pip Slope as envelope, or Intellijel Quadra/LFO)

**Patch Idea:**  
- Gate sequence into GATE A1, LFO/Envelope/CV into GATE B/CV.
- Use Phase mode to swing, delay, or phase-shift triggers, creating late/early beats, shuffled patterns, or swung hats/snares.
- Output to percussive elements or use as clock for follow-on sequencers needing a swung groove.  
**Result:** Instantly add musical swing and rhythmic complexity—great for live performance jams!

---

## 6. **Performance-Friendly Pattern Morphing**
**Combine With:**  
- CV sources: joystick (Intellijel Planar), sliders (Make Noise Pressure Points), or random voltage (Wogglebug/Tides)
- Output routing, sequential switch (Doepfer A-151 or 2hp Switch)

**Patch Idea:**  
- Use a performer-controllable CV (joystick, envelope, or touch controller) to select Local Mode, GATE A1/A2, or Probability/Variables modes in real time.
- Route OUT to various destinations via a switch for live jamming and rapid pattern mutation.
- Save or recall set-ups via Pamela’s Workout or similar master clocks.  
**Result:** Evolving, hands-on rhythmic manipulation as part of your live sets—great for techno, IDM, or leftfield modular improvisation.

---

## 7. **CV as Rhythmic Modulator**
**Combine With:**  
- Any modulation destination (filter cutoff, wavefolder, FX depth)
- Slewed CV source (Make Noise Maths, Befaco Rampage)

**Patch Idea:**  
- Use Event Boss OUT as a gate to trigger major CV events—filter sweeps, extreme morphs, sample and hold events, etc.
- Pair with Probability, Gates, or Variables modes to make “musical” but unpredictable modulations.
- Don’t restrict yourself to audio circuits; try switching FX, transposing sequences, or switching quantizer scales in time with evolving ADE-33 rhythms.
  
**Result:** "Animate" your entire modular with Event Boss as a master rhythmic brain!

---

### **General Tips**
- Take advantage of the ADE-33’s button edit modes for deep live CV assignment and performance tweaks.
- Use sequencers, random CV, or envelopes to modulate ADE-33 parameters for non-repetitive results.
- Chain the ADE-33 with logic or switching modules to further expand rhythmic complexity.

---

### **Selected Module-Type Recommendations**
- **Gate/Trigger Sequencer**: Intellijel Steppy, Make Noise René, Tiptop Audio Circadian Rhythms
- **Random/Chaos Source**: Mutable Marbles, Make Noise Wogglebug, SSF Ultra-Random Analog
- **Clock Dividers/Multipliers**: Doepfer A-160-2, 4ms Rotating Clock Divider/Multiplier
- **Logic Processors**: Doepfer A-166, Ladik S-180, Erica Synths LOGIC
- **VCOs and Drum Sound Sources**: Noise Engineering, WMD, Erica Synths, Tiptop
- **Slew/Envelope Generators**: Maths, Stages, Rampage, Quadra

---

## [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
