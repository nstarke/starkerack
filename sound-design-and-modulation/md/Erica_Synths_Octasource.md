# Erica Synths — Octasource

- [Manual PDF](../../manuals/black_octasource_manual.pdf)

---

[**Erica Synths Black Octasource Manual (PDF)**](https://www.ericasynths.lv/media/Black_Octasource_manual_1.1.pdf)

---

# Sound Design Strategies with Erica Synths Black Octasource

As a Eurorack musician, the **Erica Synths Black Octasource** offers rich, multi-output LFO capabilities that transcend conventional modulation roles. Its unique features—such as 8 phase-shifted outputs, waveform morphing, FM, CV control over phase and waveform, external sync, and flexible output modes—open up experimental territories for making powerful percussive, bass-heavy, and ethereal sounds. Below are techniques tailored to your interest in **distorted percussion, aggressive basslines, and haunting pads**.

---

## 1. Distorted Percussive Sounds

### **Techniques**

**A. Audio-Rate Modulation (Turning LFO into Oscillator/Modulator)**
- **Patch:** Crank the *RATE* control into its highest setting (up to 30Hz). Patch one or more outputs into the FM or AM (audio-rate) input of a VCO or a filter.
- **Result:** Fast, phase-shifted LFOs create metallic, clangorous, or broken digital percussion when used as FM sources, especially if the waveform is ramp, S&H, or sharply morphs.

**B. Multi-Output Rhythm Driver**
- **Patch:** Use MULTI mode for different waveforms on each output. Patch 2–3 outputs into several percussion LPGs or envelope generators. Each gets a different rhythmic modulation due to phase shifts.
- **Result:** Generates complex, shifting rhythm beds. If used with VCAs and distortion modules, it produces wildly throbbing, glitched percussion textures.

**C. Unipolar Percussive FM**
- **Tip:** Switch to *unipolar* output (+0V to +5V) for envelope/FM modulation of pitch or cutoff in classic synth drum sounds (see manual: *Set RATE to 12 o’clock + MUL/SING switch 6x*).
- **Result:** Removes unwanted negative voltage "pop," accentuating the attack phase and sharper percussive snap.

---

## 2. Wild Dubstep/Drum & Bass Basslines

### **Techniques**

**A. Sync to Master Clock for Groovy Modulation**
- **Patch:** Patch your DAW or sequencer clock into *SYNC*. Now the LFO modulates in sync (RATE knob freezes modulation except in “freeze” mode).
- **Result:** Ensures your wobbles hit exactly on the beat—vital for modern bass music.

**B. Eight-Phase Wobble Modulation**
- **Patch:** In SINGLE mode, take several outputs (e.g., at 0°, 45°, and 90°) and modulate multiple parameters: filter cutoff, resonance, waveshaper amount, or VCA level.
    - *Example CV Routing:* Output 1 → Filter cutoff, Output 2 → Oscillator FM, Output 3 → VCA CV.
- **Result:** Each parameter modulates with a different phase, yielding morphing, interlocking wobble-bass movement typical of complex dubstep/Drum & Bass lines.

**C. FM Feedback for Aggressive Distortion**
- **Patch:** Patch an Octasource output into its own *FM IN*. Use another output/CV to modulate *FM LEVEL* knob by hand or via CV.
- **Result:** Self-FM introduces pitch warble and chaotic distortion. Tame with downstream filter or distortion for modern, aggressive textures.

---

## 3. Haunting Atmospheric Pads

### **Techniques**

**A. Multi-Parameter Pad Mod**
- **Patch:** Use several Octasource outputs to subtly modulate parameters such as reverb mix, chorus rate, or multiple oscillator levels/panning.
- **Result:** The slow drift between outputs (at sub-audio LFO rates) provides an organic, ever-evolving motion in stereo or surround field—perfect for haunting pads.

**B. Morphing Ambience**
- **Patch:** Choose MULTI mode. Use the *WAVE* knob or CV to morph between outputs, routing them to FM/AM/shaping inputs on digital or analog oscillators.
- **Result:** Smoothly morphing waveforms at different phases create unpredictable artifacts—great for surreal modulated textures under pad layers.

**C. Freeze for Timeless Modulation Snapshots**
- **Patch:** Engage *Freeze* (RATE at 12 o’clock or via external clock). This holds the CV state. Unfreeze for dramatic changes.
- **Result:** Create shimmering, frozen modulations or time-suspending transitions in ambient and cinematic builds.

---

## **Extra Creative Tips**

- **Inter-modulation:** Self-patch the Octasource (output to WAVE CV, PHASE CV, or FM IN) to create evolving feedback LFO patterns.
- **Waveform Selection via Sequencer:** Route a CV sequence to the *WAVE CV* input to create animated, sequencer-driven modulations.
- **LED Metrology:** Use the bipolar LEDs not just as indicators—visually “patch” by rhythm/level feedback for syncing with other modules by eye.

---

## **Further Exploration**

- Experiment with **external quantizers** after the LFO outputs for modular pseudo-random gating/pitching.
- Mix outputs for complex modulations (e.g., sum 0° and 180° outputs for balanced, biphasic CV).
- Use S&H (sample & hold) wave for stepped, glitchy effects—combine with slow morph for unpredictable random voltages.

---

### [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)