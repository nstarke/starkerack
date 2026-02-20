# Xaoc Devices — Batumi

- [Manual PDF](../../manuals/xaoc_batumi2_poti2_manual.pdf)

---

[**Xaoc Devices Batumi II & Poti II Manual** (PDF)](https://xaocdevices.com/manuals/batumi_ii_manual.pdf)

---

# Creative Modulation Techniques for Batumi II (+Poti II)  
_Aimed at distorted percussive sounds, basslines (d&b/dubstep), and atmospheric pads_

**Batumi II** is one of the deepest Eurorack LFO/VCOs, and with the **Poti II** expander you get extensive hands-on and CV modulation options per channel. Here’s how you can squeeze some unique and extreme sounds from them, based on the manual:

---

## 1. Distorted Percussive Sounds

### Extreme Phase Modulation (Pseudo-FM Synthesis)
- **How:** Set Batumi II to **Phase Mode** (yellow LED). Use one channel at audio rate (using slider + CV as VCO), then patch another channel's output into the first channel’s **FRQ/PH/RTO CV input**.
- **Result:** This creates brutal FM-style timbres, perfect for metallic/harsh percussive hits. Modulating phase rapidly can morph sine waves into sharp, distorted clangs. If you have a VCA, use it to rhythmically gate the output for further percussive effect.

### Hard Reset Sync for Glitchy Hits
- **How:** Feed rhythmic triggers (from sequencer or burst generator) into Batumi’s **RESET/SYNC inputs** in Reset Mode (LED off).
- **Result:** This hard-resets the phase, chopping or stuttering the LFO/VCO—perfect for digitally-glitchy clicks, folds, or repeating percussive blips.

### Wavefolding Percussion with Poti II
- **How:** On the **Poti II**, select “Sine Out” for the target channel. Feed audio-rate CV into the corresponding **SHAPE input**.
- **Result:** The sine wave will be wavefolded and amplified dynamically (with auto-amplitude compensation), generating harsh, clangorous, or almost metallic percussion like you might hear in more aggressive modular techno or glitch.

---

## 2. Dubstep/Drum & Bass Basses

### Audio-rate LFO as VCO with V/Oct Tracking
- **How:** Use any channel in **Free Mode** as a VCO, patch sequenced CV (from keyboard/sequencer) into the channel’s CV input—Batumi tracks 1V/oct pretty well.
- **Result:** You get classic sub bass, but with available complex waves (triangle, trapezoid, etc.), and random/smooth random for more experimental tones.

### Bass Wobble via Wave Morph + Phase Sync
- **How:** Assign “asgn” output (triangle, saw, random, etc.) per channel with Poti II. Modulate wave shape by sending LFO or envelope into its **SHAPE input** (switch set to “asgn”).
- **Result:** Morphing between waves can make LFOs that “wobble” the timbre of your bass, giving you those famous dubstep modulated basslines—especially when passed through a filter or distortion.

### Suboscillator Trick: Divide Mode  
- **How:** In **Divide Mode** (blue LED), b/c/d channels become divisions of channel a. Set a to audio rate, others to 1, 2, 4, etc.—run trigs into reset/sync for phase variations.
- **Result:** Create a stack of related suboscillators at subharmonic intervals, dialing in classic reese or layered d&b basses by mixing waves.

---

## 3. Haunting Pads & Atmospheric Sounds

### Multi-channel Random LFOs for Modulation  
- **How:** In **Free Mode**, set b/c/d channels to stepped or smooth random via wave select. Patch their outputs into filter cutoff, VCA CV, reverb, etc.
- **Result:** Non-repeating, uncorrelated modulation lets pads drift, swell, and evolve organically—especially when each channel modulates a different effect.

### Synchronous Morphing Pads in Phase/Divide/Mult Mode
- **How:** In **Phase**/**Divide**/**Mult** modes, all channels sync to channel a; set the others' sliders for phase/frequency offsets. Set each asgn output to a different waveform (using Poti II).
- **Result:** Generate four perfectly interlocked LFOs or VCOs, with each morphing/wobbling its own parameter, for shimmering, spectral pad atmospheres.

### Modulating Wave Shape for Subtle Complexity
- **How:** Use **Poti II SHAPE input** CVs to slowly morph sine to folded or asgn output’s shape; especially on random and trapezoid shapes.
- **Result:** Pads that "breathe" and shimmer as overtones and timbre shift smoothly.

---

## Advanced Tips

- **VCAs after Batumi II:** Process its output with VCAs/envelopes for "pluck" or "hit" envelopes.
- **Cascading Reset:** Patch Batumi II’s outputs into its own or another channel’s reset input for recursive, chaotic modulation.
- **Clock-following LFOs:** Use sync mode to lock Batumi II to external clocks for tempo-synced modulations (great for rhythmic pads and syncopated bounces).

## Patching Scenarios

- **Percussion:** Batumi Sine Out → Wavefolded by SHAPE input → VCA (triggered by sequencer) → Distortion/FX.
- **Dubstep Bass:** Batumi Channel a in audio rate, modulated by Batumi Channel b LFO in phase mode, with asgn set to triangle, routed through filter and distortion.
- **Atmospheric Pad:** Multiple Batumi channels in random mode, each modulating different effect/parameter (reverb wet, filter cutoff, VCA gain, delay time).

---

*Explore self-patching and feedback using Batumi's outputs into each other's CV and reset inputs for unpredictable, living results!*

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
