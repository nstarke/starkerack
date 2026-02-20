# Tiptop Audio — CYMBL909

- [Manual PDF](../../manuals/Tiptop_Audio_CYMBL909_ns.pdf)

---

[Tiptop Audio CYMBL909 Manual PDF](https://tiptopaudio.com/manuals/manual-cymbl909.pdf)

---

# Creative Modulation Ideas for Tiptop Audio CYMBL909

The **Tiptop Audio CYMBL909** is a dual-voice (Crash & Ride) Eurorack drum module that offers both the iconic 909 crash/ride sounds AND extensive voltage control for powerful sound shaping. Below are modulation strategies for crafting distorted percussion, wild basslines, and atmospheric sounds beyond typical drum machine duties.

---

## 1. Distorted Percussive Sounds

**Patch Suggestions:**
- **Accent as Distortion Source**:  
  - Patch an LFO, sequencer, or stepped random CV (e.g., from a S&H) into the ACCENT input while keeping the ACCENT knob at high settings.
  - This will cause the VCA/envelope of the crash/ride voice to "slam" inconsistently, adding witchy peaks and dynamic tear to the envelope—great for dirty, off-kilter percussion.
- **VC-TUNE Modulation Mayhem**:
  - Use a fast envelope, gated random, or chaotic LFO (e.g., Make Noise Wogglebug or Mutable Instruments Tides) into the VC-TUNE input.
  - Crank the TUNE knob for maximum range and let the modulator sweep the sample playback pitch for bit-crushed, metallic, and distorted overtones.
- **Overdrive Post-Processing**:
  - Route CR OUT/RD OUT directly into a wavefolder, distortion, or input-overdriven mixer channel. The sharp transients (especially with max accent) will push the distortion for crispy, thunderous results.

---

## 2. Creating Dubstep/Drum & Bass Basslines

While the CYMBL909 is a cymbal/ride module, extreme processing can transform its metallic resonance into reese-like movement or grinding bass.

**Patch Suggestions:**
- **Sub-Bass with Frequency Drop**:
  - Multi the gate signal. One path triggers the module. The other fires a very fast-decaying envelope into VC-TUNE.  
    - Set VC-TUNE to sweep downward quickly. This "sinks" the cymbal’s pitch into the bass range for a gnarly hit—process this with filtering/distortion for a bassy thunk.
- **Wobble Bass**:  
  - Patch an LFO synced to song tempo into VC-TUNE.  
    - Keep TUNE at its lowest. Let the LFO sweep up and down percussively—post-process with a lowpass filter modulated for additional movement.
- **Layer with Sub Oscillator**:
  - Blend CR/RD OUT with a basic sine or triangle sub-oscillator for thunderous impact and weighty bass.

---

## 3. Haunting Atmospheric Pad Sounds

Don’t overlook the atmospheric potential of metallic source material!

**Patch Suggestions:**
- **Extreme VC-TUNE Modulation**:
  - Slowly modulate VC-TUNE with a drifting, unsynced LFO (e.g., Batumi, Zadar).
  - Hold the module’s envelope open by gating it constantly (e.g., via a held gate from a keyboard or long manual press), letting the shimmer ring indefinitely.
- **Granular or Reverb Processing**:
  - Send the outputs into heavy delay/reverb (e.g., Mutable Instruments Clouds, Make Noise Mimeophon).
  - Consider modulating ACCENT with an LFO for undulating volume swells through the effects.
- **Negative Feedback/Resampling**:
  - Route one output through a filter/EQ and back into a CV input (VC-TUNE/ACCENT) for feedback-style, evolving metallic pads.

---

## Key Points from the Manual

- **ACCENT** can be modulated by gate/CV for dynamic loudness and attack; it acts as a VCA.
- **VC-TUNE** replaces the TR-909’s original digital rate with an **analog VCO** for deep, voltage-controllable pitch sweeps—making it far more expressive.
- Use both manual knobs and CV for combining real-time modulations (hand tweaks) with sequenced/unpredictable changes.

---

### Resources

- [Tiptop Audio CYMBL909 Manual PDF](https://tiptopaudio.com/manuals/manual-cymbl909.pdf)
- Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)