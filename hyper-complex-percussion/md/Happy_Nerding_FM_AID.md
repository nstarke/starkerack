# Happy Nerding — FM AID

- [Manual PDF](../../manuals/FM-AID-USERS-GUIDE_2020.pdf)

---

[Download the FM AID 2020 Version Manual (PDF)](https://happynerding.com/manuals/FM_Aid_manual.pdf)

---

# Making Complex, Percussive, and Polyrhythmic Music with FM AID

As a Eurorack musician aiming for dense, polyrhythmic, and hypercomplex percussion underpinned by the FM AID module, you are in perfect territory for both precision and wild experimentation. Below is a practical guide to get the most out of this module within the boundary-pushing world of advanced rhythms.

---

## 1. Understanding & Context: FM AID as a Percussive Voice

FM AID isn’t just a waveshaper/folder; it’s a full-fledged through-zero linear FM engine that can process *any* waveform and repurpose it in surprisingly rhythmic, rich, and abrasive ways. By manipulating both carrier and modulator signals (which can be percussive, rhythmic, or free-running), you can morph the module into a drum voice, a metallic burst generator, or a rhythmically modulating timbre source.

## 2. Core Techniques for Percussion & Rhythmic Complexity

**a. Carrier and Modulator as Percussive Sources**  
- Use envelopes, decaying LFOs, or short, snappy function generators as the *Carrier*. Fast transients will become "attacks"—snare hits, rimshots, claps, etc.
- Patch triggers/gates, audio-rate pulses or *already rhythmic sources* as the *Modulator* for instant rhythmic interaction.

**b. Polyrhythms & Time Signatures**  
- Feed different triggers (e.g., one at 3/16, one at 4/16) into Carrier and Modulator, so FM depth and tone changes only when both coincide—instant interlocking polyrhythms!
- Use rhythmically clocked envelopes/LFOs at different clock divisions for Carrier and Modulator to generate patterns beyond standard 4/4.

**c. Modulation for Rhythmic Movement**  
- Patch complex and/or stepped modulation (random generators, sequencer CVs) into the *CV* input. Sudden voltage jumps slice through the FM AID's timbral state, creating glitchy, stuttering, or precisely sequenced metallic/wooden percussive colors.

## 3. Unique, Punchy, Percussive Sound Design Techniques

### **A. Feedback for Aggressive Percussion**
- Feed one of FM AID’s outputs (e.g., Square or Sine) BACK into the Modulator input.
- This can add digital-like metallic noise, sizzle, or trashy hats and cymbal-style energy, especially if you use short envelopes or bursts as the Carrier.

### **B. Strengthen Impact**
- Use the “Strengthen the Low End” tips:
    - Try lowering the pitch of the Carrier for heavy, punchy kicks.
    - Use triangle or sine waves as the Modulator for rounder, less harsh transients.
    - Dial in the FM knob to taste for just enough aliasing/noise or clean body.

### **C. Output Selection**
- Use SINE output for low, punchy kicks or toms.
- SQUARE/SW outputs will have extra bite, useful for snares, metallic hits, and hi-hats.
- TRAINGLE is in-between: good for thocks, congas, and woodblocks.

### **D. Sequencing for Pattern Complexity**
- Use clock dividers/multiplier modules to send sequenced patterns to FM AID’s various inputs, constantly shifting the internal polyrhythms.
- Step modulate the FM and CV inputs by clocked or probability-based sequencers for evolving time signatures and pattern density.

### **E. CV and FM Index Over Time**
- Use fast envelopes, stepped random, or even *audio rate* signals into the CV input: The timbral changes can become part of your rhythm.
- Automate “FM” and “CV” knob movement with slow LFOs or manual performance for dramatic rhythm/timbre interplay.

## 4. Additional Patching Tricks

- **Self-Patch for Useful Mayhem:** Patch SQUARE or SINE output into the MOD input for digital FM feedback squeals; clock or trigger the Carrier for sharp, metallic handclaps or hi-hat bursts.
- **Clocked Modulation:** If you send clock pulses/divided triggers into the Mod input, you get sharp FM artifacts/rhythmic stutters; combine with sloped envelopes for dynamic shape.
- **Layer Multiple Outputs:** Mix SINE and SQUARE out for a hybrid, complex percussion sound, or pan them for stereo drum ‘spread.’

## 5. Calibration Note
Before recorded tracks or performance, calibrate the module for your typical oscillator(s) per the manual—reduces artifacts and keeps percussion crisp.

---

### Summary
With smart patching and creative CV routing, FM AID is a secret weapon for rhythmically sophisticated, highly unique, and brutally punchy percussion, easily supporting polyrhythms, microtiming, and experimental grooves. Experiment with sources, modulations, and feedback—FM AID isn’t just an effect: it’s a rhythm machine at the core of the rack!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)