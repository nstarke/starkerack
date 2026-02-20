# ADDAC Systems — ADDAC-402 Heuristic Rhythm Generator

- [Manual PDF](../../manuals/ADDAC402_UsersGuide_A_0_web_6500.pdf)

---

[**ADDAC402 Heuristic Rhythm Generator Manual (PDF)**](http://addacsystem.com/sites/default/files/files/ADDAC402%20User%20Guide%20Revision.01.pdf)

---

# Creative Modulation Techniques: ADDAC402 Heuristic Rhythm Generator

The ADDAC402 is a four-voice, algorithmic rhythm generator with extensive CV and manual control, designed for experimentation. Below are creative strategies—directly referencing the module’s features and controls—to sculpt unique, highly-modulated sounds in your Eurorack system: from distorted percussive textures, monstrous bass, to cinematic, eerie pads.

---

## 1. Overview of Modulation Sources

**CV Inputs (per channel):**  
- Fills (Parameter B) CV input  
- Swing/Assign CV input (global, configurable to other parameters)

**Manual Controls:**  
- Knobs (Parameters A/B), with CV override/attenuation  
- Gate/Trigger switches  
- Skip/Reset push buttons

**Assignable Control:**  
- The Swing/Assign knob and CV input can be assigned to Preset changes, Steps, Gate/Trigger state, Skip, Reset, etc. Multiple simultaneous assignments are possible.

---

## 2. Patching for Distorted Percussive Sounds

### **A. Rhythmic Structure Creation**

- Use **Euclidean Mode** or **Game of Life** mode for non-repetitive, algorithmic patterns—activate complex rhythms that go far beyond traditional step-sequencing.
- Modulate **Fills (CV input)** dynamically with an LFO or envelope for morphing between dense and sparse hits.

### **B. Creating Distortion & Crunch**

1. **Patch A Channel’s Gate Output → Drum Module or VCA**  
   (with fast decay envelope)

2. **Use Skip or Reset (via CV or manual mashing) to glitch up the rhythm.**

3. **Mult The Pattern To Distortion/Audio FX Module:**  
   Patch the main or inverted Gate Output to an audio-rate effect strip (distortion, wavefolder, bit crusher). With short gates or triggers, you'll get aggressive transients.  
   
4. **Modulate Swing/Assign with Audio-Rate CV:**  
   Assign the Swing/Assign CV to Steps, Skips, or Reset, then patch in a fast LFO or audio-rate oscillator—this injects pseudo-random clocking for digital distortion/artifacting in the rhythm.

5. **Invert Outputs = Double Triggers:**  
   Send both Gate and Inverted Gate to separate FX chains (overdrive, reverb, ring mod). Their offset will create rapid-fire, jittery percussion.

---

## 3. Synth Bassline Madness (Dubstep/Drum & Bass Inspired)

### **A. Sequenced Sub-Bass Triggers**

- Use the **Footwork Mode** for unpredictable, glitchy patterns. Set STEPS controls for strong “wub” hit placement.
- Patch a Gate Output to a VCA controlling a bass oscillator (through a lowpass or wavetable module for maximum bass character).
- Modulate **Steps CV (via Assign) with an envelope follower** for evolving, syncopated bass phrasing.

### **B. Syncopated "Talking Bass"**

- Assign the **Swing/Assign CV to Skip channel(s)**.
- Feed a sequencer output or random stepped voltage into Swing/Assign—causes patterns to "skip"/rotate rhythmically, driving formant filter/LPG for “growl” effects.
- Mult channel outputs to trigger different sub-patches (FM, pitch-shifted inputs into a distortion pedal, etc.).

### **C. Dubstep Snares & Bass Glitch**

- Use **Probabilistic Mode**: Modulate Probability (Fills) with a slow random LFO.  
- Patch Gate/Trigger outputs into drum and synth voices. Unpredictable hits = complex, stuttering bass and snare rolls.

---

## 4. Haunting Atmospheres/Pad Textures

### **A. Algorithmic Ambient Gates**

- Use **Golomb Rulers**/Game of Life modes for irregular, non-cyclic triggering—perfect for dreamlike pads.
- Patch Gate outputs to slow-attack, slow-decay VCA/envelope paths to create long, overlapping gates into reverb/delay.

### **B. Dynamic Pattern Morphing**

- Assign Swing/Assign to control multiple parameters (e.g., Steps, Skips, Resets), then use a sample & hold, S&H, or drone LFO for organic pattern changes.
- External CV controlling pattern length and Fills = evolving rhythm for drones/pads.

### **C. Multichannel Modulation**

- Use the U-shaped layout to design polyrhythmic patterns on all four channels.  
- Distribute gates to modulate different oscillator/pitch paths through lush FX chains (cloud reverb, resonator, etc.).

---

## 5. Advanced Modulation Tips

- **Preset Morphing:** Assign Swing/Assign to Presets and scrub through patterns with random CV or manually. Pads and basses will drift in unexpected ways.
- **Clock Shifting:** Modulate the clock input with variable sources or clock division/multiplication for off-grid, warped time signatures.
- **Interactive Performance:** Manual button presses—especially Skip/Reset—bring trance-inducing rhythmic shifts during live jams.

---

## 6. Summary Table

| Logical Function         | Modulation Source        | Patch/Assign Example                |
|-------------------------|-------------------------|-------------------------------------|
| Fills/Pattern Density   | CV Input (per channel)  | LFO, envelope, random voltage       |
| Steps/Pattern Length    | Assign+CV               | Slow LFO, keyboard CV               |
| Gate/Trigger Skip/Reset | Assign+CV, Button       | Audio-rate oscillator, manual press |
| Swing                   | Assignable knob+CV      | Humanize rhythms, triplet shuffle   |

---

## 7. External FX & Audio Processing

Remember: The ADDAC402 output is gates/triggers, so to create **audio signals** you must drive oscillators, drum modules, VCAs, and process those sounds with filters, waveshapers, distortion, and FX modules. Layering fast gates, modulated patterns, and applying external distortion/reverb is essential for dirty percussion and atmospheric soundscapes.

---

_For experimentation, consult the: [ADDAC402 User Guide (PDF)](http://addacsystem.com/sites/default/files/files/ADDAC402%20User%20Guide%20Revision.01.pdf)_

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)