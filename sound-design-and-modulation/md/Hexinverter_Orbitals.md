# Hexinverter — Orbitals

- [Manual PDF](../../manuals/hexinverter-orbitals.pdf)

---

[Orbitals Dual Bipolar Voltage Controlled Step Sequencer – Manual (PDF)](https://hexinverter.net/wp-content/uploads/2016/08/Orbitals-UserManual-v104.pdf)

---

# Creative Patch Tips for the Hexinverter Orbitals Step Sequencer

The Hexinverter Orbitals module is an exceptionally deep step sequencer for eurorack with a range of flexible features: dual 8-step/16-step operational modes, bipolar output, voltage-addressed steps, per-channel length/mode/gate control, and extensive CV/gate routing.

Below, I’ll guide you through patch ideas and modulation concepts to create **distorted percussive sounds**, **crazy basslines** (à la dubstep/DnB), and **haunting atmospheric pads**.

---

## Essentials: Orbitals Modulation Features

**Modulate Orbitals Using:**
- Step CV and gate sequencing (of course).
- Bipolar output switching for sharper/stronger modulations.
- Voltage-controlled step addressing for non-linear, evolving patterns.
- Transpose input for real-time or sequence-driven shifting.
- Per-channel mode switching (random, pendulum, CV, etc.).
- Clock rate modulation, both externally and internally.
- CV and gate outputs to trigger or modulate external sources (VCO, LPG, VCF, etc.).

---

## 1. Distorted Percussive Sounds

### *Patch Strategy:*
- Use one sequencer row (A or B) as a **trigger/gate source** for drum modules or noise/VCAs.
- Patch CV outs into heavily overdriven VCA/VCF or a waveshaper/distortion module.

#### **Modulation Techniques:**
- **Pendulum or Random Mode (MODE knob):** For unpredictable, glitchy rhythms.
- **Gate Length (GATE knob):** Turn up for longer, overlapping pulses—send to a distortion module (wavefolder, bitcrusher, etc.).
- **Bipolar Output:** Flip BIPOLAR on and set output to ±5V for aggressive modulation of distortion drive, filter cutoff, etc.
- **Voltage Address Step Mode (CV/CLK modes via MODE + RST/CV in):** Run a noisy/random LFO into RST/CV; this scrambles step position, creating varied triggers and unevenly spaced events.

#### **Example Patch:**
1. CV OUT → filter cutoff or VCA CV input (post-distortion).
2. GATE OUT → drum module/EG, or trigger noise burst through a VCA.
3. Add a random or stepped LFO to RST/CV in **(CV or CLK mode)** for evolving, broken percussive loops.

---

## 2. Crazy Dubstep / Drum & Bass Basslines

### *Patch Strategy:*
- Sequence VCO/VCF pitch, wavetable selection, or complex waveshaping.
- Use the Transpose input or external CV for bassline interval jumps/riffs.

#### **Modulation Techniques:**
- **16-Step Mode:** Use both rows as one for longer, evolving phrases.
- **Transpose Input:** Plug keyboard for pitch bends/glides; or use a sequenced CV for pitch jumps typical in DnB/dubstep.
- **Reverse Input + Random Mode:** Send gates to the REVERSE input, switching up bassline playback direction for stutter/glitch effects.
- **Bipolar switch with ±10V (jumper):** Get extra pitch range and drive harder VCO FM inputs.
- **Step Gating:** Use switches to mute/enable steps and create syncopation.
- **Length knob:** Unusual loop lengths (e.g., 5 steps) create polyrhythmic movement.

#### **Example Patch:**
1. CV OUT → VCO 1V/OCT (set to deep sine/saw).
2. GATE OUT → sample & hold, or sync envelope for filter cutoff “notches.”
3. TRANSPOSE IN → arpeggiator or modulation, for wild interval jumps.
4. RST/CV IN (CV/CLK mode) → LFO or S&H for pitch-scrambling lines.
5. Experiment with **clock rate modulation** (patch an LFO into clock input).

---

## 3. Haunting Atmospheric Pads

### *Patch Strategy:*
- Use slow rates (RATE knob) for gradual, textural changes.
- Sequence filter cutoffs, FX mix levels, or wavetable positions for evolving sound.
- Double up sequencers for parallel modulation paths (e.g., one for VCF, one for FX/CV).

#### **Modulation Techniques:**
- **Random or Pendulum Mode:** Adds subtle, organic non-repetition.
- **Bipolar Mode on ±2.5V output:** Perfect for gentle LFO-like modulation.
- **Gate shaping:** Long gate times for droning vactrol/VCAs.
- **CLK OUT:** Use to sync slow LFOs/clock dividers for layered atmosphere.
- **Voltage-addressed mode:** Use a wandering S&H or slow random CV to “morph” through scenic step values.

#### **Example Patch:**
1. CV OUT to VCF cutoff, reverb mix level, or wavetable morph input.
2. GATE OUT to control an LFO reset or trigger slow EGs.
3. Run step modes in **random/pendulum** and set rate to very slow values.
4. Summing Orbitals’ CV out with another LFO via a mixer for added modulation complexity.

---

## **Key Bonus Tips**

- Experiment with OUTPUT LEVEL jumpers (**±2.5V, ±5V, 0–5V, 0–10V**) to match/trick your downstream modules! More voltage = wilder modulation.
- Patch external modules (chaos modules, random clocks, audio rate LFOs) to RST/CV and clock inputs for totally bespoke rhythms and motion.
- The SLAVE B>A switch is your secret to instantly layered, evolving 16-step mod sequences—try pairing stepper rhythms or blended gate patterns.

---

For visuals and more context, always consult the [Orbitals PDF Manual](https://hexinverter.net/wp-content/uploads/2016/08/Orbitals-UserManual-v104.pdf).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)