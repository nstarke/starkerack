# Tiptop Audio — Fold Processor

- [Manual PDF](../../manuals/Tiptop_Audio_foldprocessor.pdf)

---

[Fold Processor Manual (PDF)](https://tiptopaudio.com/manuals/FoldProcessor_UserManual.pdf)

---

# Modulating the Tiptop Audio Fold Processor for Creative Sound Design

The Tiptop Audio Fold Processor is a versatile analog wavefolder and sub-octave divider that can generate everything from classic West Coast folding tones to brutal digital-esque wave carving and octave ‘thunder’. Below, I’ll break down modulation suggestions for each of your target sound areas: **distorted percussion, wild basslines, and evolving pads**.

---

## 1. **Distorted Percussive Sounds**

- **Input Source:** Use snappy drum samples (e.g., from Tiptop ONE) or short envelopes and noise bursts.
- **Patch Suggestion:**  
  - Drum output → IN 1  
  - OUT or SUBDIV OUT → VCA (with fast envelope) → Mixer/Output
- **Modulation Ideas:**
    - **FOLD CV:** Use a fast, snappy envelope (e.g., from Maths or Z4000) to modulate the Fold CV. This will dynamically increase folding as your percussion strikes, adding aggressive transient-driven distortion.
    - **INJECT CV:** Modulate with an LFO or random stepped source for ever-shifting timbres.
    - **Attenuverters:** Tune the Atten knobs to control modulation depth. Brutal, clicky, overdriven sounds tend to result from medium-to-high Fold/Inject settings.
    - **SUBDIV Out:** Mix in the sub-divided output for metallic, chime-like harmonics—set different divisions to pulse with the original voice.

---

## 2. **Crazy Basslines (Dubstep/DnB Wobble, Growl, etc.)**

- **Input Source:** Use a pure sine or triangle from a VCO, or a self-resonant filter output (as described).
- **Patch Suggestion:**  
  - VCO (Sine/Triangle) → IN 1  
  - OUT → Filter (optional for taming) → VCA → Output
- **Modulation Ideas:**
    - **FOLD CV:** Envelope follower from a kick drum or sidechain LFO/wobbler for rhythmic bass growls.
    - **FOLD CV/INJECT CV:** Assign separate LFOs at different speeds (sync to clock for rhythm, free-running for chaos) for evolving overtones. Try audio-rate modulation for AM/FM timbres.
    - **Atten Knobs:** Tune to taste—more depth = more destruction.
    - **SUBDIV Out:** Mix subtle amounts for added sub-bass grit and “robotic” artifacts. Use extreme settings for octave jumps/buzzy effects.
    - **Post-Processing:** Run the Fold output into a delay or reverb (e.g., Z-DSP) for resonance or chamber-style bass.

---

## 3. **Haunting Atmospheric Pad Sounds**

- **Input Source:** Slow-moving waveforms—stacked VCOs (detune for width), or triangle/saw outputs.
- **Patch Suggestion:**  
  - Mix or sum VCOs → IN 1  
  - OUT → Reverb/Delay → Mixer
- **Modulation Ideas:**
    - **FOLD CV/INJECT CV:** Modulate slowly with drifting LFOs (non-synced, natural movement). Use envelope modulation for gentle dynamic sweeps.
    - **Atten Knobs:** Small depth for subtle morphing, larger depth for evolving spectral timbre.
    - **SUBDIV Section:** Very slow modulation of SUBDIV levels for shifting octave content (“ghostly” undercurrents and shimmer).
    - **External CV:** Use random voltages for “haunted castle” vibes—randomly shifting tonalities and crackles.
    - **Post FX:** Feed the OUT or SUBDIV OUT into long reverb/delay.

---

## **Pro Tips (`get creative!`)**
- Try **feedback** loops by sending Fold OUT back into itself via mixer or via a filter.
- Use voltage-controlled crossfading between OUT and SUBDIV OUT for morphing timbres.
- Place the Fold Processor **before/after filters** for pre/post distortion coloring.
- Patch the OUT to FM input of a VCO for chaotic, self-destructive modulations.

---

For more ideas, [download the full manual PDF here](https://tiptopaudio.com/manuals/FoldProcessor_UserManual.pdf).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
