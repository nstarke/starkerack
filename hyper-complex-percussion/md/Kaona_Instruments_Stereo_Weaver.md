# Kaona Instruments — Stereo Weaver

- [Manual PDF](../../manuals/stereoweaver.pdf)

---

[Download the Stereoweaver Manual (PDF)](https://kaona.fr/wp-content/uploads/2024/02/STEREOWEAVER_MANUAL_EN.pdf)

---

## Using Stereoweaver for Densely Rhythmic, Hyper-Complex Percussion

### 1. Module Context & Approach

The **Kaona Stereoweaver** is an advanced stereo effects module, not a sound source/voice, so it processes your percussion signals rather than generating them. It excels at spatial manipulation—depth, motion, phase shifting, Haas effect (micro-delays), and dynamic width—using psychoacoustic principles.

To enhance **complex, polyrhythmic, or experimental percussion**, patch your **mono drum/percussion mix, single drum voice, or highly complex trigger-based percussion** into Stereoweaver’s input. Its outputs immediately provide a transformed stereo image.

### 2. Techniques for Dense, Punchy Rhythms

#### A. **CV Animation for Sequence Stereoscopy/Texture**
- **Patch rhythmic/clocked/random/Euclidean CV sequencers or internal triggers to Stereoweaver’s CV inputs**:  
  - **Depth CV**: Use triggers or stepped random signals to accentuate or hollow out the perceived space on every beat or subdivision.
  - **Width CV & Move**: Modulate width using Euclidean polyrhythms; have each drum “jump” around the stereo field based on complex trigger/gate patterns.
  - **Phase CV**: Modulate on odd-time pulses (5/8, 7/16) so phase relationships are never static; this can create evolving, lively, and slightly "uneasy" spatial textures perfect for intricate percussion.
  - **Motion CV**: Animate Leslie/rotary effects with LFOs synced to non-standard clock divisions (e.g., 3 against 4), so swirling spatiality is itself polyrhythmic.

#### B. **Articulation and Percussive Punch**
- **Drive the input HARD** for controlled saturation:  
  Use distortion intentionally on each transient-heavy percussion hit. Adjust input gain until the LED blinks in time—let it overload on strong downbeats for added punch, or modulate gain control voltage with trigger envelopes for hit-by-hit “coloration.”
- **Exploit the Haas and Micro-Delay**:  
  Push the Haas setting hard, or modulate with a stepped random or variable clock so different hits or pulses have different stereo delays—this creates a tangled, urgent stereo feel, emphasizing intricate rhythms.

#### C. **Chaos and Unpredictability**
- **Animate ‘Move’ at audio rates or with highly irregular gates**:  
  Patch burst generators, logic patterns, or heavily clock-divided clocks to the Motion/Width CVs. In “Move” mode, this swaps L/R unexpectedly, making your patterns feel “glitchy” and kinetic.
- **Max out Phase + Depth for Micro-Chorus/Phasing**:  
  At extreme settings, your percussive hits can become subtly flanged or phase-shifted. Accent minor notes with these modulations for unique timbral ripples.

### 3. Patch Ideas

- **Breakcore/Jungle**: Use a trigger sequencer sending triggers on both regular and offgrid pulses to the Width and Phase CVs. Stereo image will jump according to rhythmic density.
- **Polyrhythmic Techno**: Assign clocks from different meters (e.g., 5-step and 7-step) to modulate Haas/Width. Layered drums “dance” around the cycle.
- **Electroacoustic**: Pair with acoustic percussion sounds or foley, let complex envelopes modulate Depth and Phase in conjunction with touch/pressure or sensor-based CV, for gestural spatiality.

### 4. General Tips

- **Mult different CV sources** (clock divisions, envelope followers, random gates) to several parameters for hyper-complicated, interconnected rhythmic spaces.
- **Stereo Balance**: Use the independent L/R outputs to further process with stereo compressors or spatializers—Stereoweaver can feed parallel effects chains for even more depth.
- **Visual Feedback**: The on-panel LEDs help you “see” when movement or widening is happening, making precise tuning for rhythmic mapping easy.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)