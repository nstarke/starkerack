# Mutable Instruments — Braids

- [Manual PDF](../../manuals/Manual - Mutable Instruments Braids Documentation.pdf)

---

[Mutable Instruments Braids Manual PDF (v1.8)](https://mutable-instruments.net/modules/braids/manual_v18.pdf)

---

# Using Mutable Instruments Braids for Dense, Rhythmic, and Hyper-Complex Percussion

Mutable Instruments **Braids** is a versatile digital macro-oscillator for Euroack that excels as a percussive sound source when creatively patched. While not a dedicated drum module, its synthesis models and interface invite deep experimentation with rhythm, texture, and timbre. Below are strategies, patch ideas, and manipulation techniques for using Braids as the foundation of densely layered, complex, and punchy percussive music—including recommendations for fostering unique, hyper-detailed rhythm structures.

---

## 1. **Braids as a Percussive Source**

Braids is primarily a **voice**, capable of generating a variety of synth and drum sounds depending on the selected model. Relevant percussive/physical models include:

- **PLUK** (Plucked String)
- **BOWD** (Bowed String)
- **BELL**
- **DRUM**
- **KICK**
- **SNAR**
- **CYMB**
- **NOIS** (Filtered Noise)
- **TWNQ** (Resonant Bandpass)
- **CLOU/PRTC** (Granular/Particle)

### **Rhythmic Density & Complexity**

#### a. **External Triggering & Event Density**
- **Patch** tightly clocked or irregular (Euclidean, polyrhythmic) trigger/gate signals to the **TRIG** input. Many of Braids’ percussive models are event-triggered for each new percussive hit.
- Use multiple gate/trigger sources (like clock dividers, logic, burst generators, or random gate sequencers) sending rapidly interleaved and offset pulses.

#### b. **Internal AD Envelope Modulation**
- Activate the internal AD envelope generator via the TRIG input and use the menu options (**|FM, |TIM, |COL, |VCA**) to modulate pitch, timbre, color, and VCA amplitude per hit. Set **|\ATT** and **|\DEC** to very short settings for snappy, punchy articulations, or longer for more evolved hits.
- Use Braids’ menu to route this envelope to different destinations per patch or even modulate multiple destinations simultaneously for evolving percussion with each trigger event.

#### c. **Model Morphing (META Mode)**
- In **META** mode, you can morph through different synthesis models using incoming CV into the **FM** (now model select) input. With a rhythmic stepped, sampled, or sequenced CV, you can switch between drum sounds on a single voice to achieve complex, "meta-kit" style polyrhythms.
- Use envelope followers, stepped random voltage, or precision adders to manipulate this meta-model morphing in time with your sequence.

#### d. **Trigger Source (TSRC) Options**
- Set **TSRC** to **AUTO** to generate triggers from V/OCT jumps, letting you create percussive events using melodic CV/gate sequencing—even from monosequencers which might lack dedicated triggers. This aids in generating percussive events with pitch information interlocked with your melody.

---

## 2. **Polyrhythms and Irregular Time Signatures**

- Use sequencers, clock dividers/multipliers, or modules like Pam’s New Workout or Euclidean generators to create complex polyrhythmic gate/trigger streams patched to **TRIG**.
- For even higher complexity, combine several rhythmic sources with logic modules (AND/OR/XOR) before they reach Braids' TRIG. Each composite event can trigger entirely new drum sounds when combined with META/model morphing.
- Patch random gates or algorithmic rhythms to the **META/FM** input in META mode to rhythmically “remap” which model is played at each step for heterogenous drum lines.

---

## 3. **Techniques for Unique, Punchy Percussion**

### **Sound Design Approaches:**
- **Modulate** **Timbre** and **Color** with stepped and smooth random voltages for each trigger—sample-and-hold sources work well.
- **Attenuvert** the **FM, TIMBRE, and COLOR** mod inputs for precise dynamic control over punch and character of drum hits. Negative and positive modulation opens up subtle or dramatic differences.
- **Utilize internal versus external AD envelopes:** Stack both for multi-stage modulation on drum attacks (e.g., external envelope modulates pitch decay, internal modulates harmonic content).
- **Run granular and physical drum models (KICK, SNAR, DRUM, CYMB, PRTC, CLOU)** at audio rate or near-audio rate triggering for glitchy, high-speed percussion or near-metallic clusters.

### **Tips for Distinction and Punch:**
- **Decrease bit depth (via BITS option)** for lo-fi, punchy, or digital grit.
- **Switch RATE to lower settings:** Sometimes, lower DAC refresh rates produce grittier, digital transients.
- **Activate FLAT/DRFT/SIGN** for microdetuning, oscillator drift, or purposeful glitch/waveform error for a dirtier, less clinical sound.
- **Use the comb filter model (/|/|_|_|_)** and aggressively modulate the feedback for flams and metallic clustering.

---

## 4. **Advanced Rhythmic Texture: Layering and Sampling**

- **Layer** Braids with additional drum voices, modulating it with cross modulation FM from decay envelopes or from other rhythm-generating modules for percussive overtones or syncopation.
- **Resample** "meta-kits" built from rapid model morphing as new drum loops, then chop and re-sequence these in a sampler module for recursive complexity.

---

## 5. **Calibration and Tuning for Precise Percussion**

- Use **FREE** range for drum work when not sequencing pitch traditionally—this keeps tuning intuitive.
- Use **TDLY** (trigger delay) if complex clocking/sequencer combinations result in timing errors or flams between modules.

---

## 6. **Patch Example: Polyrhythmic Drum Machine With Braids**

```text
[Pam's New Workout] (output 1, 5-step division, polyrhythm A) --> [Braids TRIG]
[Pam's New Workout] (output 2, 7-step division, polyrhythm B) --> [Braids FM (in META Mode), via attenuverter]
[Mutes or Logic]                   --> [Braids TIMBRE and COLOR CV]
Sequencer OR S&H                   --> [Braids V/OCT (optional)]
```
- Use one clock for regular kicks/snare, a second for hi-hat glitches (e.g., with **CYMB/NOIS** models), and another to rhythmically morph models and parameters.
- Tweak mod attenuation and decay curves per pattern for flexible, evolving, extremely dense drum lines.

---

For **maximum punch and distinction**, combine fast external envelopes (VCA after Braids; not just Braids’ own), analog wavefolder/saturators post Braids, or stereo processing with different models per left/right channels (if using two Braids).

---

*Experimentation is key*: Use both the percussive models and pitched ones (with heavy pitch+decay modulation) for unique, inharmonic drum timbres. Don't forget that even melodic models become punchy with aggressive envelopes, random triggers, and hard sync.

---

[Manual PDF](https://mutable-instruments.net/modules/braids/manual_v18.pdf)  
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)