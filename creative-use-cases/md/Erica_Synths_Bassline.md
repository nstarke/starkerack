# Erica Synths — Bassline

- [Manual PDF](../../manuals/BASSLINE_web.pdf)

---

[Erica Synths Bassline Manual PDF](https://www.ericasynths.lv/media/Bassline_manual_1.02.pdf)

---

## Creative Ways to Utilize the Erica Synths Bassline in Your Eurorack Setup

The Erica Synths Bassline is a versatile analog synth voice designed for acid, techno, and experimental basslines. Here's an analysis of its features and creative patching ideas combining it with other modules.

### Key Features Recap

- **Analog VCO (with SAW, PULSE, SUB oscillator)**
- **VCF (Polivoks-inspired, resonance, CV control)**
- **Envelope (ADSR, CV controllable)**
- **Accent In/Out (for classic acid lines)**
- **Gate, CV, Modulation & External Input/Output**
- **Compact 14HP format**

---

## Creative Combinations & Patching Ideas

### 1. **Acid Techno Basslines with Sequencers**
- **Recommended module:** [Mutable Instruments – Yarns / Arturia Beatstep Pro / Intellijel Metropolis]
- **How:** Sequence pitch CV & gate, use **accent CV** from the sequencer or even Pam's New Workout. Add slide with external slew limiter (e.g., Doepfer A-171-2 or Mutable Stages in slew mode) patched before VCO CV in.
- **Result:** Classic squelchy acid, 303-style lines—Slide and accent made easy!

### 2. **Audio Rate Modulation**
- **Recommended module:** Any extra oscillator (e.g., Dixie II+, STO)
- **How:** Patch a fast LFO or VCO into the **Modulation CV input** or **VCF Cutoff CV**.
- **Result:** FM (Frequency Modulation) basses, complex metallic timbres, or formant-like growls.

### 3. **Waveshaping & Distortion Chains**
- **Recommended module:** Wavefolder (e.g., Serge Wave Multiplier, Intellijel uFold) or distortion (e.g., Erica Synths Fusion VCA/Waveshaper).
- **How:** Route the Bassline module’s output through a waveshaper and/or distortion.
- **Result:** Industrial, hard techno-bass or acid with a twist.

### 4. **Dual Basslines & Cross-Modulation**
- **Recommended module:** Another Bassline or a simple analog voice (Doepfer A-111-5 Mini Synth, Dreadbox Hysteria or Make Noise STO)
- **How:** Patch each to their own sequencer line, cross-modulate their VCF cutoff or use the output of one as modulation source for the other.
- **Result:** Poly-rhythmic acid lines, evolving bass textures.

### 5. **External Input Processing**
- **Recommended module:** Drum machine, other synth, or sampler
- **How:** Patch external audio to the **Ext In** of Bassline, use the filter and envelope to process drums, samples, or other synths.
- **Result:** Acidic breakbeats, filtered percussion, or animated sample mangling.

### 6. **Generative Patches with Random CV**
- **Recommended module:** Random module (e.g., Wogglebug, Turing Machine, or Marbles)
- **How:** Send random voltages to Cutoff CV, VCA Env CV, or Tune CV.
- **Result:** Evolving, unpredictable acid bass or weird techno sequences.

### 7. **Clocked Rhythmical Filtering**
- **Recommended module:** Pamela’s New Workout, Malekko Varigate, or Euclidean sequencer.
- **How:** Use a rhythmic clock or gate pattern to modulate accent in or VCF cutoff.
- **Result:** Synchronized filter movements, “bouncing” bass patches, synced to your master clock.

### 8. **Stereo Tricks & Paraphony**
- **Recommended module:** Stereo panner (e.g., Make Noise PanMix), two Bassline modules
- **How:** Run two detuned Basslines, pan hard left/right, sequence each slightly differently.
- **Result:** Huge stereo bass sound, paraphonic effect.

### 9. **Ring Modulation & Amplitude Modulation**
- **Recommended module:** Ring modulator (Doepfer A-114, Intellijel uMod)
- **How:** Sum Bassline output and another VCO output in a ring modulator or use VCA for AM with external CV.
- **Result:** Bell-like, clangorous bass and metallic timbres.

### 10. **Bass Chaining and Signal Routing**
- **Recommended module:** Sequential switch (Doepfer A-151), matrix mixer (Doepfer A-138m)
- **How:** Route the Bassline through switchable effects, or blend various signal-mult combinations.
- **Result:** Live performance possibilities, morphing basslines.

---

### Summary Table of Inputs/Outputs & Creative Patch Ideas

| Bassline Input/Output | Patch Suggestion                   | Example Module                                  |
|----------------------|------------------------------------|-------------------------------------------------|
| Tune CV / VCO FM     | Pitch slides, FM                   | Slew Limiter, Dixie II+                         |
| VCF Cutoff CV        | Rhythmic filter, random mod        | Envelope Generator, Marbles, PNW                |
| Ext In               | Filter drums/other synths          | Anything!                                       |
| Gate In              | Generative rhythm, accent triggering| Trigger sequencer, Marbles                      |
| Accent In            | Dynamic acid lines                 | Sequencer with accent/gate out (Metropolis)     |
| Audio Out            | Chain with effects/distortion      | uFold, Fusion VCA/Waveshaper, Pico DSP          |

---

### Tips

- **Patch Accent Out into Accent In for auto-accented lines.**
- **Self-patch VCA Env or VCF Env outs to mod inputs for feedback madness.**
- **Experiment with very slow modulation for evolving drones.**
- **Combine with add-on CV utilities (attenuators, offset, logic modules) for complex performance control.**

---

**Manual:** [Erica Synths Bassline Manual (PDF)](https://www.ericasynths.lv/media/Bassline_manual_1.02.pdf)  
**Generated With Eurorack Processor:** [https://github.com/nstarke/eurorack-processor](https://github.com/nstarke/eurorack-processor)