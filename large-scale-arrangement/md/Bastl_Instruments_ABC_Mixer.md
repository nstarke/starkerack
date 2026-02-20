# Bastl Instruments — ABC Mixer

- [Manual PDF](../../manuals/manual-abc-web.pdf)

---

[**Bastl Instruments ABC 6 Channel Mixer Manual (PDF)**](https://bastl-instruments.com/content/manuals/ABC_manual.pdf)

---

# Using the Bastl Instruments ABC 6-Channel Mixer to Build Full Length Eurorack Songs

## Overview

The [Bastl Instruments ABC](https://bastl-instruments.com/products/abc) is a six-channel mixer specifically aimed at combining audio or CV signals in a compact 5HP format. It provides two summed outputs — A+B+C and D+E+F — and includes flexible normalization and solder jumpers for AC (audio) or DC (CV) mixing.

## Key Features for Song Creation

- **6 Audio or CV Inputs** (A, B, C, D, E, F)
- **Two Summing Outs:** A+B+C & D+E+F; can become a single 6-channel mix
- **Normalization Jumpers:** Useful for stereo mixing or layer splitting
- **Individual Gain for Each Channel**
- **DC Coupling Option:** Lets you mix CVs for parameter control/morphing

---

## Creative Uses for Full-Length Song Construction

### 1. **Dynamic Submixing of Groups (Song Parts)**
Use the module as two 3-channel mixers for grouping instrumental layers:
- **A+B+C:** Drums/perc, main synth, bass
- **D+E+F:** Pads, leads, FX

**Live Song Structure Tactic:**  
Patch all voices into the mixer, then perform transitions/muting by turning channel gains up & down or by patching in/out the group outputs. This helps create intros, breakdowns, drops, and outros by fading groups in/out.

---

### 2. **Manual Performance/Automation**
Assign mixer channels to various song sections:
- Channel A: Verse synth
- Channel B: Chorus synth
- Channel C: Bridge FX

**Performance tip:**  
Use active muting (by turning the gain knob fully down) to bring parts in/out by hand—even if your sequencers are firing all patterns at once. This is a tactile way to “arrange” live.

---

### 3. **Morphing Between Song Sections Using CV Mixing**
By modifying the mixer for DC coupling (solder jumpers), you can mix LFO/envelope CVs that control other modules (VCAs, filters, effect sends).

**Example:**  
- Channel A: Envelope for verse intensity
- Channel B: LFO for transitions
- Channel C: Envelope for breakdown FX

Sum these, then send the output to modulate effects or VCAs—the evolving CV shapes can “morph” your song structures automatically.

---

### 4. **Stereo/Fake-Stereo Arrangements**
Use the normalization jumpers on the back to pair:
- A→D, B→E, C→F  
Send different signals to the L/R outputs; pan drums left, synths right, FX center—giving your songs a sense of movement over time.

---

### 5. **Scene Switching with Shared Outputs**
When nothing is plugged into A+B+C, this mix is summed into D+E+F.  
- **Patch D+E+F to a master VCA or FX send:** This lets you crossfade between full arrangement (all 6 channels) and subgroup (3 channels only), building in/outro sections.

---

### 6. **Performance Combinations**
**Patch Scenario:**
- A: Kick
- B: Snare
- C: Hats
- D: Bass
- E: Chord synth
- F: Lead melody

**Full Mix to Output:** All channels
**Drop to Drums + Bass Only:** Mute E, F (turn down)
**Breakdown:** Kill A, B, D (only hats + chords remain)
**Drop:** Bring all channels back
**Outro:** Fade down each group

---

### Practical Workflow for Full-Length Songs

1. **Pre-Patch Sections:** Pre-patch all instruments; decide what channels group into which song section.
2. **Manual or Automated Muting:** Use mixer channel knobs to “write” your arrangement in real-time.
3. **Send Mixes to Effects or Sidechains:** For further variation, patch outputs to FX modules or sidechains for builds and drops.
4. **Layer with Additional Automation:** Use CV mixing to organically morph sections (volume, modulation, FX sends).

---

## Conclusion

The ABC mixer is not just utility—it’s a hands-on performance and arrangement tool that lets you shape your eurorack jams into coherent, evolving full-length songs. Combine channel assignments, mutes, fades, CV mixing, and stereo tricks to perform or multitrack entire arrangements with structural change and dynamic interest.

---

**For more utilities and generative eurorack workflows, check out:**  
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)