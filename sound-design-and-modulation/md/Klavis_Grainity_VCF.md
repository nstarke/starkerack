# Klavis — Grainity VCF

- [Manual PDF](../../manuals/Klavis_-_Grainity_User_Manual.pdf)

---

[**Klavis Grainity Granular VCF User Manual (PDF)**](https://www.klavis.com/Grainity_Granular_VCF_User_Manual_RevA_EN.pdf)

---

# Creative Modulation Techniques for Klavis Grainity

As a eurorack musician, the Klavis Grainity offers unique tools to sculpt intensely modulated, analog-filtered sounds. With its dual-section (granular and multimode VCF) architecture, myriad CV inputs, and granular structure concepts, it’s a goldmine for percussive distortion, seething basslines, and eerie atmospheres. Here’s how to get the most out of it for these applications:

---

## **1. Distorted Percussive Sounds**

**Core Strategy:**  
Leverage the Grainity’s cycling detection with chaotic sources and unusual structure/division settings to impose broken, glitchy, or razor-sharp flavor on drums and noise.

### **Patching Tips:**
- **Input:** Feed in rich percussive audio or noise.
- **Detect Input:** Patch the drum’s trigger (or an LFO clock, or even a fast envelope) to the Detect input.  
  - *Result:* The granular filter cycles step on each hit or at a rhythmic subdivision, "slicing" the effect differently for every hit.

- **Structures & Division:**  
  - Use longer Structures (4–8 steps) and high Division settings (`Div pot` fully clockwise or CV modulated).  
  - Try random structures (`r` bank) for unpredictable filter movement across drum transients.

- **Phase/Track Modulation:**  
  - CV the Φ/Frq pot with an LFO, envelope, or stepped random to add phase-shifting and flanging on the attack.

- **Multimode Blend:**  
  - Use the Mix output and voltage control it, automating the blend between G.VCF and M.VCF for rapid timbral changes per hit.

- **Resonance Abuse:**  
  - Push Q into self-oscillation territory for barking, almost metallic artifacts layered with percussion.

### **Result:**  
*Percussion is fragmented, reshaped into lo-fi digital grit, or undergoes stuttering filter jumps reminiscent of old breakcore/digital glitches, but with a wholly analog snap.*

---

## **2. Crazy Dubstep & Drum & Bass Basslines**

**Core Strategy:**  
Use the granular engine’s frequency tracking, structure cycling, and external CV to create the hyper-complex, modulated basses common in modern bass music.

### **Patching Tips:**
- **Source:**  
  - Route a harmonically rich, detuned saw/sub heavy oscillator or two (e.g., through a wavefolder) into the main input.

- **Power Move: Sync Tracking to Pitch**
  - Patch your melody-line V/Oct to both the VCO(s) and the Grainity V/Oct input. This ensures filter movement tracks every note change, making modulation tightly musical.

- **Activate Track Mode:**  
  - Use the Track button + CV the Φ/Frq pot for riotously detuned or harmonically ambiguous sweeps.
  - Sweep the Track knob with an envelope for each bass note for quick, talking filter movement.

- **Structure & Division:**
  - Select a 3- or 4-step Structure for additive harmonics.
  - Automate Division with random/modulated CV for “wobble” or syncopated filter changes in time to your bass rhythm.

- **FM Input:**  
  - Patch an LFO, envelope, or audio-rate oscillator into the FM input, and tweak the FM knob for classic dubstep growl—or go negative for reverse-mod dynamics.

- **Q Modulation:**  
  - Patch a sharp envelope to Q for punchy, roaring resonance on each note.

- **Phase Inversion:**  
  - Toggle phase inversion when using the Mix output for hollow, “comb-filtered” bass flavors or to make bass jump in the stereo field (if spreading G.VCF and M.VCF to hard left/right).

### **Result:**  
*Create gnarled, metallic, or vowel-like basses that move dynamically with your performance, with formant and subharmonic content impossible with conventional VCFs.*

---

## **3. Haunting Atmospheric Pads**

**Core Strategy:**  
Exploit slow, evolving granulation cycles, random structures, gentle phase sweeps, and subtle blend of analog filter paths for ethereal movement.

### **Patching Tips:**
- **Source:**  
  - Use a soft, sustained pad (layered VCOs, chords, or audio snippets).

- **Granular Structures:**  
  - Choose long, random Structures (`r`) for evolving, shifting spectral content.
  - Use high Division settings (e.g., `b`, `c`, `d`) to slow down the progression, washing the filtering over long stretches.

- **Detect Input Options:**  
  - Experiment with LFOs, noise, or external random clocks in the Detect input, causing slow, unpredictable filter shifts independent of the original pad’s timing.

- **Phase Modulation:**  
  - Slowly sweep Φ/Frq with a complex LFO for dreamy phasing/flanging.
  - Modulate with a slewed random or sample-and-hold for organic, tape-warbly movement.

- **Q and FM:**  
  - Set Q just below self-oscillation to avoid harshness, but enhance airiness.
  - Subtly modulate FM with a slow, gently-moving CV source for extra shimmer.

- **Stereo Potential:**  
  - Send M.VCF and G.VCF outputs hard L/R for wide, spectral motion.
  - Alternatively, automate phase inversion for evolving stereo or comb-like textures.

### **Result:**  
*Pads billow and morph, with ghostly formants and moving harmonics, perfect for ambient, cinematic, or horror soundscapes.*

---

## **General Modulation Suggestions**

- **Random/Stepped CV Sources:**  
  - Greatly increase unpredictability and motion by patching random CVs to Structure, Division, Mix, or Phase.
- **Sequencer or S&H:**  
  - Sequence Division or Structure values to create patterns with each trigger, especially for hyper-evolving drum and bass or industrial beats.
- **Envelope Follower:**  
  - Feed the output of a loudness-tracking envelope follower (from your percussion or pad or external audio) into any CV input for organic, input-reactive modulation.

---

> **Explore, experiment, and abuse the CV-modulatable parameters on the Klavis Grainity—especially Structure, Division, FM, Q, and Phase/Track modes—using classic eurorack tools (LFOs, S&H, random voltages, gates, switches) for totally novel, musical results.**  

---

[**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)