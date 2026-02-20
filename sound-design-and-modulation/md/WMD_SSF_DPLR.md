# WMD SSF — DPLR

- [Manual PDF](../../manuals/DPLRmanual1.3.pdf)

---

[WMD/SSF DPLR Official Manual (PDF)](https://wmdevices.com/products/wmd-ssf-dplr)

---

## Eurorack Sound Design with the WMD/SSF DPLR Dual Delay

The **WMD/SSF DPLR** is a rich stereo/dual delay module with several modulation points, unique XTALK (crosstalk) modes, and analog-style filtering. Here’s how you can use it to craft unique, hard-hitting, and atmospheric synth sounds.

---

### General Modulation Points

- **DELAY AMOUNT CV** (`DLY CV`): Modulate delay time for pitch-shifting, tape-wobble, and glitch effects.
- **SPREAD CV** (`SPRD CV`): Modulate to create stereo movement or ping-pong delay effects.
- **REGEN CV** (`RGN CV`): Modulate feedback for recursive, evolving, or self-oscillating textures.
- **Manual Controls**: All main controls are also voltage-controllable and performable for real-time tweaks.

---

### 1. Distorted Percussive Sounds

**Goal:** Glitchy, crunchy, or broken delay tails suited for techno, IDM, or experimental percussion.

#### Tips:
-:
- **Crank the REGEN:** Turn up feedback for intense repeats; automate with a stepped or envelope CV for build-ups or bursts.
- **Delay Amount:** Modulate rapidly with an envelope triggered by your drum hit (cv from envelope follower or gate to envelope into `DLY CV`). This produces broken pitch jumps and unique decays.
- **Heavy Filtering:** Hold `MODE SELECT` to toggle to the strongest filter slopes—this reduces delay brightness, emphasizing thump and crackle.
- **XTALK Modes:** Step through cross talk (crosstalk; RED-RED for classic dual delay, BLUE for most chaotic bleed between channels). The higher the XTALK, the noisier and more affected each tap is by the other.
- **SPREAD Jumps:** Punch Spread/B at specific intervals (even with a random voltage or S&H LFO) for polyrhythmic, offset delay taps.

**Patch Example:**
```plaintext
Drum Module --> DPLR IN
Envelope Follower from Drum --> DLY CV in
Short Envelope or Stepped S&H --> RGN CV in
Modulated LFO or S&H --> SPRD CV in
OUT A / OUT B --> Mixer/VCAs
```

---

### 2. Crazy Dubstep/Drum & Bass Basslines

**Goal:** Growling, resonant, or moving basslines with stereo interest and heavy feedback artifacts.

#### Tips:
- **Feed Bass into Delay:** Route a saturated bassline through DPLR; use OUT A/B for stereo width.
- **REGEN for Roar:** Push REGEN CV high for runaway feedback bursts—sync this via MIDI clock or LFO for predictable destruction.
- **Delay Time Modulation:** Fast, sharp LFO shapes or sequencer gates into `DLY CV` produce FM-style, robotic glitches or formant-like "vocal" movement. Try quantized S&H for stepped madness.
- **Use SPREAD:** Add panning motion or create offbeat echoes with modulating SPREAD. An envelope or fast, bipolar LFO works best.
- **XTALK for Unpredictability:** Use crosstalk modes above minimum for stereo chaos—great for building tension.
- **Filter Settings:** Dial in less filtering for more grit, or max filtering for dark, focused bass.

**Patch Example:**
```plaintext
VCO/Distorted Bass Synth --> DPLR IN
Fast LFO/Random CV --> DLY CV in
Clocked LFO --> SPRD CV in
Envelope/LFO --> RGN CV in
Try OUT B for the grittier, more modulated signal
```

---

### 3. Haunting Atmospheric Pads

**Goal:** Evolving, lush backgrounds with ghostly delay trails, perfect for ambient, cinematic, or horror genres.

#### Tips:
- **Long Delay Times:** Set DELAY AMOUNT high (towards 700ms). Modulate gently for subtle pitch/texture wobble.
- **Gentle Feedback:** Keep some REGEN for long, evolving repeats—but automate with a slow LFO to swell the feedback over time.
- **XTALK for Texture:** Moderate XTALK adds movement and spectral interest without muddying the pad.
- **Heavy Filtering:** Max filter for dark, ghostly echoes; lighter filter for shimmering, noisy repeats.
- **SPREAD Automation:** Slowly modulate SPREAD to move echoes across the stereo field, enhancing immersion.
- **Amount Control:** Mix dry and wet with modulation for movement within the pad soundscape.

**Patch Example:**
```plaintext
Pad/Waveshape VCO/Granular Source --> DPLR IN
Slow LFO/S&H --> DLY CV in
Long, slow LFO --> RGN CV in
Random LFO --> SPRD CV in
Cyclic pressing of MODE/XTALK for live transitions
OUT A and B --> Stereo output
```

---

### Pro Patch Tricks

- **Self-Oscillate:** Maximize feedback (REGEN) and use a short impulse to "tune" the DPLR as a bizarre kick or snare drum sound source.
- **Stereo Cross Patch:** Use OUT A + OUT B for dual parallel processing—route one to reverb, one through additional effects for maximal texture.
- **Live Knob Twiddling:** Combine CV modulation with live tweaks for maximum chaos and performance feel.

---

#### [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)