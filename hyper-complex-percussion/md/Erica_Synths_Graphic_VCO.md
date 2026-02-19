# Erica Synths — Graphic VCO

- [Manual PDF](../../manuals/graphic_vco_manual_web.pdf)

---

[**→ Erica Synths Graphic VCO Manual PDF**](https://www.ericasynths.lv/media/Graphic_VCO_manual_2020.pdf)

---

# Using Erica Synths Graphic VCO for Hyper-Complex Percussive Rhythms

The Erica Synths **Graphic VCO** is a digital oscillator with advanced wavetable, morphing, and effects capabilities. It is fundamentally a voice module, capable of producing a wide variety of unique and punchy sounds—especially effective for crafting percussive and rhythmically dense sequences in Eurorack modular setups.

Below are strategies, patch tips, and creative ideas for using the Graphic VCO to create densely rhythmic, polyrhythmic, and hyper-complex percussion:

---

## 1. **Waveform Creation for Percussion**

- **Draw Custom Percussive Waves:**  
  Use the wave drawing/editing features (p. 8–11) to sculpt sharp, transient-heavy waveforms reminiscent of envelopes or drum clicks. Sine-based with steep rises and falls, or squares with very short cycle spikes, can be extremely impactful.
- **Harmonics for Snap:**  
  Directly manipulate harmonics to emphasize high-frequency content, adding snap or click to your percussive voices.
- **One-Cycle Drums:**  
  Create single-cycle drum ‘hits’ and store them in wavetables, then use rapid retriggering and CV scanning for rolls/fills.

---

## 2. **Wavetable and Morphing for Rhythmic Variation**

- **Rhythmic Wavetable Scanning:**  
  Use external CV sources (step sequencers, trigger sequencers, polyrhythmic clocks, random voltages) to rapidly scan or step through custom wavetables of percussive waveforms.  
  - For complex rhythms, use polyrhythmic (odd division) clocks to modulate the **Morph CV** and/or **Wavetable Matrix X/Y** position.
- **Morphing ‘Gestures’:**  
  Manually morph between two selected percussive waves or automate movement with CV for evolving drum timbres—perfect for rhythmic fills or varied phrasing.

---

## 3. **FM, Phase Distortion, and FX for Percussive Character**

- **FM Percussion:**  
  The built-in FM can generate clangorous, metallic, or bell-like hits when modulated with audiorate oscillators. For polyrhythmic clangs, clock or sequence the FM AMOUNT and FM carrier ratio via external CV.
- **Ring Modulation/Phase Distortion:**  
  Use internal or external modulation at polyrhythmic rates for shifting overtones—useful for digital-sounding snares, hi-hats, or “broken glass” percussion.
- **Wavefold/Wavewrap/Bitcrush:**  
  These FX are especially effective for glitch percussion. Modulate their intensity and character at rhythmic or irregular intervals (using gate sequences, random modulation, or Euclidean generators).
- **Apply to Main Voice:**  
  FX are placed before main output (not the suboscillator out), so consider parallel processing for added complexity (e.g., dry/wet blending).

---

## 4. **Suboscillator for Layered Beats**

- **Pitch Offsets/Detuning:**  
  Use the suboscillator for ‘body’ or ‘thump’ beneath clicky main percussive textures. Detune or pitch-offset by non-octave/semitone intervals for off-grid/complex feeling rhythms.
- **Layering:**  
  Mix main and subosc outputs for stacked percussive voices (e.g., click + woof), with blend set via MIX% parameter.

---

## 5. **External Rhythmic Control**

- **Bipolar/Unipolar CVs & Matrix Navigation:**  
  Patch multiple clock divisions/multiplications, Euclidean rhythm clocks, or stepped random voltages into Morph, FX Parameter, FX Amount, or Matrix X/Y CVs to introduce rhythmic complexity.  
  - **-10V...+10V Bipolar CV acceptance** offers flexible mapping of rhythmic voltage patterns.
- **Use as a Digital Drum Voice:**  
  Patch triggers into your envelope/decay generators, then to the VCA for typical drum voice architecture—but use the Graphic VCO for the oscillator (for digital, metallic, or noisy timbres).
- **Snapshot Recall:**  
  Save complex setups as snapshots and recall on the fly for live changes to rhythm profiles or sound banks.

---

## 6. **Live Performance and Modulation**

- **Manual Tweaking:**  
  All parameters can be turned, moved, or scanned live for glitchy, stuttered, or IDM drum effects.
- **Oscilloscope Feedback:**  
  Use built-in visual feedback to fine-tune shapes for maximum “punch” and “snap”.

---

## 7. **Advanced Tips for Unique Rhythms**

- **Microtiming Tricks:**  
  Modulate Morph or FX CVs with unconventional LFOs (sample & hold, skewed sines, etc) and reset at non-grid intervals.
- **Pseudo-Granular:**  
  By rapidly changing wavetables in response to rhythmic CV, you can approximate digital granular effects for tight, evolving hat and snare textures.
- **Custom Wavetable Banks:**  
  With the Wavetable Matrix, create banks with patterns of ‘hits’ and ‘spaces’ to sequence percussive bursts via CV-stepping in multiple directions (matrix navigation via different clocks).

---

## 8. **Patch Example**

**Complex Percussion Machine:**
1. **Draw**: Multiple short, ‘click’ and ‘clap’ waveforms, plus a few noisy digital ones, and save them as a wavetable.
2. **Patch**: 
   - Master clock → Tempi/Ornament+Crime/Euclidean sequencer.
   - Different clock divisions/multiplications to Morph CV, Matrix CV (X/Y), FX Param CV, and trigger drum envelopes.
3. **Sequence**: At least one slow moving and one fast moving CV through Matrix axes for nested polyrhythms.
4. **FX**: Animate FM ratio or amount with a skewed or randomized clock for IDM “glitch” edges.
5. **Layer**: Mix suboscillator out for an underlying bass transient, use main out for sharp attack.

---

## 9. **Patch Starters**

- **Euclidean Kicks & Snares:**  
  Use Euclidean trigger sequencer to vary Morph CV: blend between kick-tuned waveform and snare-tuned waveform inside one bank.
- **Time-Shifting Snares:**  
  Modulate FX parameters with off-beat LFOs to make the snare timbre evolve at a different rate than the main clock.
- **Hats & Clicks**:  
  Load very short, sharp waveforms; crush/bitcrush further with rhythmic triggers on FX Amount CV.

---

**[Full Manual PDF for More Details](https://www.ericasynths.lv/media/Graphic_VCO_manual_2020.pdf)**

---

> **Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)**
