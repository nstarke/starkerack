# Mutable Instruments — Plaits

- [Manual PDF](../../manuals/Mutable Instruments - Plaits.pdf)

---

[Download Mutable Instruments Plaits Manual (PDF)](https://mutable-instruments.net/modules/plaits/manual.pdf)

---

# How to Use Plaits for Densely Rhythmic & Hyper Complex Percussion

Mutable Instruments Plaits is a digital macro-oscillator that is capable of being a *full percussive voice generator* in addition to more traditional melodic and textural duties. The following strategies, drawing from the manual, will guide you in building music with dense, complex, and polyrhythmic percussion.

---

## 1. **Choose the Right Models**

Plaits includes several synthesis models well-suited for percussion/complex rhythms:

- **Bank 2:** Noisy and Percussive Models.
  - *Drum synthesis models (kick, snare, hihat/cymbals)*.
  - *Physical modeling (mini-Rings: string, bar, tube)*.
  - *Granular noise, dust, filtered noise*.

For percussion, cycle to these models using the model selection buttons. Experiment with the AUX out for alternate timbres.

---

## 2. **Triggering & Polyrhythm Creation**

- **TRIG Input:**  
  Patch distinctly clocked, irregular, or polyrhythmic trigger patterns into the TRIG input.  
  - Use multiple trigger generators—e.g. Euclidean sequencers, clock dividers/multipliers, or step sequencers running at odd divisions (3, 5, 7, etc).
  - Cross-patch clocks from sequencers with different time signatures for polyrhythms.
  
- **LEVEL Input:**  
  Patch envelope generators, sequencer CVs, or accent patterns to LEVEL. This will simultaneously control amplitude and timbral brightness for each hit—introducing variation and punch.

- **TRIG plus unpatched CV Inputs:**  
  If TIMBRE, MORPH, or FM CVs are left unpatched, the respective attenuverters can set how much *internal envelope modulation* affects those parameters. Crank these for hyper-punchy, dynamic timbre with each hit.

---

## 3. **Complex Parameter Modulation**

- **External CV Modulation:**  
  - Use fast, stepped, or even random/noise CV sources to modulate TIMBRE, MORPH, FM, and HARMONICS.  
  - Sequencers running at polyrhythmic divisions can be routed separately to each modulation input.

- **Model Selection CV Input:**  
  Sequence (or randomly modulate) the Model Select CV input in time with (or offset from) your main triggers—Plaits will change drum types/pitched/noise elements on the fly. When patched to trigger, the model only changes on trigger, allowing per-step timbre switching.

---

## 4. **Accentuation & Groove**

- **Accent/Groove:**  
  Send an additional trigger/gate or CV to LEVEL on specific rhythmic steps (e.g. every 4th or 7th). This can function as an “accent” and impact both loudness and tonal brightness.

- **Decay & Envelope Settings:**  
  Hold the first button (A) and use:
  - *MORPH knob:* Set the LPG/envelope decay appropriately—short for sharp, punchy hits, longer for reverb-y, overlapping textures.
  - *TIMBRE knob:* Adjust LPG from VCA (sharpest) to VCFA (more rounded/transient).

---

## 5. **Unusual Voicings and Textures**

- Use additive, wavetable, and granular models—tuned to percussive ranges—by keeping frequency low and modulating wave/harmonic spread for metallic, glitch, or Eraserhead-style percussion.

- Bank the module into speech/voice synthesis for chopped, stuttered, or robotic rhythmic elements, modulating CLOCK/trigger to scan phonemes in rhythm.

- Use “modal resonator” and “inharmonic string” models for organic, quasi-acoustic percussive effects by sending very rapid or irregular triggers.

---

## 6. **Advanced: Firmware & Calibration**

- Configure a tight *frequency knob range* (hold second button; turn HARMONICS) to avoid accidental pitch sweeping that could mess up percussive articulation mid-performance.

- If using as a multi-sound drum voice (model switching via CV/trigger), calibrate Plaits so that 1V/oct CV from a well-calibrated sequencer precisely switches models.

---

### **Creative Tips:**

- **Layer with Other Modules**: Use AUX and OUT for stereo/dual timbral layering, or process separately with differing effects for extra complexity.
- **Silence as Rhythm**: Some models will output silence at certain parameter extremes—sequence these momentary mutes for stutter/shuffle effects.
- **Randomize**: Use sample & hold, stepped random, or Turing machine sources into model or timbre to maintain unpredictability in your percussion.
- **Feedback FM**: Use FM modulation from another Plaits or digital source clocked at a related, but offset, rhythm for cross-modulated percussion.

---

#### **Quick Patch Example**

```text
1. Set model to bank 2 “drum” type.
2. Patch three different Euclidean sequencer outputs (e.g., 5-step, 7-step, 11-step) into TRIG, MODEL select CV, and TIMBRE CV.
3. Set LEVEL to a fast S&H sequence.
4. Modulate DECAY and LPG response for desired percussiveness.
5. Use OUT and AUX for two separate percussion voices in your mix.
```

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)