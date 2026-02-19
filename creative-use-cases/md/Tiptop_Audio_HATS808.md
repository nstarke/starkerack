# Tiptop Audio — HATS808

- [Manual PDF](../../manuals/Tiptop_Audio_HATS808_ns.pdf)

---

[HATS808 Manual PDF](https://tiptopaudio.com/manuals/TTA_HATS808_UserGuide.pdf)

---

# Creative Eurorack Patch Ideas: **Tiptop Audio HATS808**

The HATS808 is a versatile TR-808-style hi-hat generator with key enhancements for Eurorack integration: VC resonance (Q), independent gain staging, voltage-controllable accent, and filter output. Here are some inventive ways to use it in your modular system, blending both specific and generic module suggestions:

---

## 1. Envelope & LFO Modulation Magic

**Explore VC-Q and Accent:**
- **Patch:** Send an LFO (e.g., Make Noise Maths, Intellijel Quadrax) or envelope generator (e.g., Intellijel Quadra) into the VC-Q CV input.
- **Result:** Sweep resonance dynamically—metallic timbres and wild, percussive morphs. High-frequency LFOs can make inharmonic, glitchy fizzles. Try an envelope with velocity sensitivity for real-time playing expressiveness.
- **Pro Tip:** Modulate Accent input for groove that “breathes,” making some hi-hats hit harder than others in a rhythmic cycle.

---

## 2. Choke Funk with Sequencers

**Classic 808 Style, Techno Flair:**
- **Patch:** Program a gate/CV sequencer (e.g., Erica Synths Black Sequencer, Mutable Instruments Grids) to alternate triggers between OH (Open Hat) and CH (Closed Hat) inputs.
- **Result:** The internal choke circuit gives velocity and groove; rapid-fire hi-hats with call-and-response interplay.
- **Variation:** Disable choke (per manual instructions) for *unbroken splashing hats* layered with tight closed hats on top, then blend them for complexity.

---

## 3. Saturate, Distort, Repeat

**Overdrive Output Signals:**
- Run HATS808’s output hot (Level/Accent maxed) into:
    - a wavefolder (e.g., ST Modular Fold, Intellijel uFold)
    - a saturation/distortion unit (e.g., Erica Synths Fusion Tube VCA/Waveshaper, Intellijel Bifold)
    - or a guitar pedal (via a module like ALM S.B.G. or Befaco Instrument Interface).
- **Result:** Wildly clipped, harmonically rich hats. Shape digital or analog distortion for industrial textures, techno aggression, or lo-fi vibes.

---

## 4. Band-Pass Output: DIY Percussion Lab

**Raw Source for Custom Sound Design:**
- Connect the Band-Pass Out to other filters (e.g., Mutable Ripples, WMD C4RBN) or wave shapers.
- Patch into VCAs (Doepfer A-132-4, Intellijel Quad VCA) with custom envelopes. 
- **Result:** Roll your own cymbals, metallic percussion, or noise-based FX. Add further modulation or spring reverbs for vintage splash.

---

## 5. Audio-Rate Modulation & FM

**Experimental Hat Tones:**
- Patch an audio-rate oscillator (e.g., Make Noise STO, Instruo Ts-L) into the VC-Q input.
- **Result:** FM or AM of the filter’s resonance. Chaotic, metallic, and alien hat splatters. Sculpt mutations with the Q and accent controls.

---

## 6. Rhythmic Layering & Stereo Tricks

**Multi-Module Groove Engine:**
- Combine with other percussion modules (Tiptop SD808, BD808, or any kick/snare modules).
- Pan CH and OH outputs using a stereo mixer (e.g., Intellijel Mixup, Befaco STMix).
- Delay or reverb only the OH, for big-room club hats.
- **Result:** Lively, dynamic drum mixes that move in stereo space and time.

---

## 7. Accented Randomization & Euclidean Patterns

**Algorithmic Drumming:**
- Use a random gate generator (Mutable Marbles) or Euclidean sequencer (e.g., Euclidean Circles) patched to Accent input for ever-changing groove accents.
- **Result:** Humanized, shifting hats, ideal for generative/techno/IDM rhythms.

---

### **Extra Patch Tip**

- **Sidechaining:** Use the Accent gate output as a CV source to duck bass or pads with a VCA or sidechain compressor for tight club-style mixes.
- **Clocked Digital FX:** Route to digital effects (Disting EX, Happy Nerding FX Aid) set to clock-synced delay/reverb for even more rhythmic depth.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)