# Omnitone — Rhythmi

- [Manual PDF](../../manuals/Rhythmi_Information_Package.pdf)

---

[**Rhythmi Eurorack Drum Sequencer Manual (PDF)**](attachment:image)

---

# Creative Rhythmi Modulation Strategies
*For Distorted Percussion, Dubstep/Drum & Bass Basslines, and Haunting Atmospheric Pads*

---

Rhythmi is a deep, generative drum sequencer tailored for both quick, evolving grooves and mod-heavy explorations. Here’s how you can patch and modulate it for wild sound-design inspiration within your own modular setup—whether you’re after aggressive percussion, crazy modulated basslines, or spacious, shifting pads.

## 1. Creating Distorted Percussive Sounds

**General Strategy:**
- Use Rhythmi to produce complex, evolving percussion patterns with heavy syncopation and energy.
- Run audio outputs (Kick, Snare, Tom, Hat, Crash) through distortion, wavefolders, bitcrushers, or feedback devices outside the module.
- Modulate parameters for ever-changing distortion character.

### ***Step-by-Step:***
- **Energy Macro Control:**  
  - **Crank up the Energy** to drive density on kick, snare, and toms.  
  - Hit the red cursor for crash triggers—patch this to gate further distortion or external event (e.g., toggle feedback).
- **Syncopation (Synco) & Density:**  
  - **Max out Syncopation** for hats and snares—creates unpredictable off-grid percussive triggers.
  - **Increase Density** to pack the beats per drum voice.
- **Evolve Parameter:**  
  - **Slowly modulate Evolve** (CV or manually) for patterns that morph over time. Go further by randomizing Evolve for wildly asymmetrical fills.
- **Short loops:**  
  - Run 2–8 step loops for glitchy, stuttering patterns ideal for heavy distortion.  
- **Patch Suggestion:**  
  - HI-HAT output to a gated fuzz/bitcrusher.
  - SNARE output to a short delay/reverb plus overdrive.
  - CRASH output to a distortion + filter—use crash as a rhythmic “reset” or spiky accent.
- **External Modulation:**  
  - Use a fast LFO or envelope to modulate Energy or Evolve via CV, so pattern intensity and fill rate constantly shift.

---

## 2. Creating Crazy Basslines (Dubstep/DnB Style)

**General Strategy:**
- Rhythmi’s TOM output is both rhythm and pitch! Quantized to a minor pentatonic scale with 1V/oct, you can use this for basslines.
- Pair evolving rhythms with external bass voice for heavy, wobbly, or tearing effects.

### ***Step-by-Step:***
- **TOM CV Out:**  
  - Send TOM CV output to a VCO/VCO-sub combo set low for sub bass.  
  - Use the **Tom Amount** knob to set the “note pool” size—more notes for more melodic fills, fewer for steady riffs.
- **TOM Trigger:**  
  - Also patch TOM TRIG out to a fast envelope or VCA, gating the bass oscillator.
- **Energy Macro Control:**  
  - As you **raise Energy**, TOM triggers cluster at the fill phase (end of loop), creating classic fill/roll effects.
  - Go beyond the red threshold so crash = baseline “reset” accent.
- **Swing:**  
  - Push SWING to near 90% for delayed off-grid stabs.
- **Evolve:**  
  - Automate Evolve (with randomization!) for glitching or pitch-rising fills.
- **External Patch Ideas:**  
  - Use a distortion or formant filter after the bass for DnB “talking” basslines.  
  - Modulate these post-effects with the CRASH trigger, or use HI-HAT gates as envelope triggers for filter/FX motion.

---

## 3. Creating Haunting, Atmospheric Pads

**General Strategy:**
- While Rhythmi is designed for rhythmic triggers, its evolution, syncopation, and density controls can generate organic “pulses” for granular or ambient soundscapes.
- Use slow, sparse patterns to trigger layers of long-attack/release envelopes.

### ***Step-by-Step:***
- **Slow Clock/External Sync:**  
  - Set Rhythmi to a SLOW loop (low speed, long lengths) or clock from a divided LFO for ambient tempo.
- **Low Energy, Sparse Density:**  
  - **Turn Energy low**, density knobs low—few triggers, lots of space.
- **Syncopation for Randomness:**  
  - Modulate Synco slowly (with LFO or random voltage) on SNARE and TOM for unpredictable, ghostly hits.
- **Pad Sound Source:**  
  - Patch TOM or SNARE triggers to envelope generators with long attack and release—these EGs then modulate filters/VCAs of your pad voices (synths or samplers).  
  - Use TOM CV out to shift pad pitch in a scale-locked way.
- **Evolve + Randomization:**  
  - Apply evolving/randomization to keep patterns shifting gently.  
- **Swing:**  
  - Dial in extra swing for ethereal delay/diffusion—spread attacks out in wonky ways.
- **Layering:**  
  - Mult outputs to modulate other parameters (e.g., send CRASH trigger to reverb “freeze” or shimmer FX).

---

## ***General Patching/Modulation Tips***

- **CV Control Everything:**  
  - Connect LFOs, envelopes, or random CVs to Evolve, Energy, Syncopation, or Length for hands-off textural changes.
- **Pattern Automation:**  
  - Use CV-enabled randomization for unpredictable bursts/fills—great for filling space in pads or sudden energy spikes in percussion.
- **Base Pattern Changes:**  
  - Long-press the encoder to flip the base pattern—use in performance or automate with external hands.

---

## ***Summary Table: Parameter-Driven Sound Design***

| Goal                       | Parameter Focus              | CV Modulation (External)     | Output Destinations           | Suggested Processing     |
|----------------------------|-----------------------------|------------------------------|-------------------------------|-------------------------|
| Distorted Percussion       | High Energy, Density, Synco | Evolve, Energy, Syncopation  | KICK/SNARE/TOM/HI-HAT/CRASH   | Distortion, Bitcrush, FX|
| Modulated Basslines        | Tom CV/Trig, Swing, Evolve  | Evolve, Length, Energy       | TOM CV/Trig, Crash            | Filter, Distortion, Glitch|
| Atmospheric Pads           | Low Energy, Slow Clock      | Evolve, Syncopation          | TOM/SNARE/HI-HAT triggers, TOM CV | Long EG, Modal/Granular FX|

---

[**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)