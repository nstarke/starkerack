# WMD SSF — Facture

- [Manual PDF](../../manuals/manual_black_fracture.pdf)

---

[Fracture Multi-Particle Percussion Synthesizer Manual (PDF)](https://wmdevices.com/manuals/fracture-manual.pdf)

---

## Creative Modulation Strategies for WMD Fracture

As a Eurorack musician, the **WMD Fracture** is a hugely versatile percussion voice that can be pushed far beyond claps and applause. Here’s how you can patch and modulate it for wild, unique distortion, growling basslines, and eerie pads:

---

### 1. Creating Distorted Percussive Sounds

- **Drive Front End Hard with CV Modulation:**
  - **DENSITY:** Patch a fast, variable random CV or stepped sequencer into the Density CV. At high values, you’ll force the particle oscillator almost into noise territory—distortion arrives as the circuit is overloaded with overlapping particles.
  - **SURFACE:** Modulate Surface with stepped CV or a fast random source to rapidly scan between microsamples, which can glitch out and smear transient details for lo-fi, industrial hits.
- **PUNCH Modes:** 
  - Use the **final PUNCH setting (parallel bandpass)** — PUNCH(⚔) — for boosted mid/high frequency content and extra aggression. Modulate the **FREQ** input (via LFO, envelope follower, or stepped random) for sweeping resonant overtones and biting, synthetic edges.
- **Decay/Envelope Tricks:**
  - Use a **short DECAY** for tight, clipped bursts. Modulate TAIL mode (the mode modulating probability only) for randomized “choke” percussive bursts. Try gating TAIL with an LFO to alternate between classic and janky transient responses.
- **Feedback & External Distortion:**
  - Route one output (say, OUT L) back through distortion or wavefolder, then into a mixer with OUT R — or try subtle feedback through a VCA for chaotic, ringy crunch.
- **INF Mode for Static Clouds:**
  - Enable **INF** and automate DECAY for a cloud of clicks/noise. Slam it through distortion or wavefolders for a wall-of-sound snare/hat.

---

### 2. Basslines for Dubstep/Drum & Bass

- **Low-Pitched Granular Snares/Hit Basses:**
  - Patch a sequencer or envelope into **FREQ** input. Select PUNCH mode that modulates both filter and pitch (PUNCH(⚡)), and set FREQ low. You’ll get punchy, pitched “thunk” and “wob” with metallic qualities—great for basslines that are both percussive and tonal.
  - Use a stepped random or envelope for **SPREAD** to create moving, stereo-wide basslines with microtonal pitch offset on each hit.
- **Glitchy Sub Snares/Growls:**
  - Modulate SURFACE with a fast LFO or sample & hold — when set to lower-pitched surfacers, you will get unpredictable, mutant snares or low-end hits. Try clocking DENSITY to the beat’s subdivision for “machine gun” rolls with timbral morphing.
- **Wobble Automation:**
  - Patch an external LFO or envelope into the PITCH jack, which disables the FREQ knob’s pitch influence and allows for synced or free-running LFO sweeps.
- **Accent for Extra Punch:**
  - Use the ACC input with velocity CV or gate for accented notes – giving that DnB “thwap”.

---

### 3. Haunting, Atmospheric Pad Sounds

- **Clouds of Microgranular Texture:**
  - Patch slow, cycling LFOs and random voltage sources to **DECAY**, **DENSITY**, and **SURFACE**. With DECAY high and TAIL set to modulate both amplitude and probability, you get suspiciously organic pads full of ghostly clicks.
- **Stereo Spread & Modulation:**
  - Max out **SPREAD** for wide panning and pitch scatter. Controlled chaos across the stereo field for enveloping atmospheres.
- **Reverb Wash:**
  - Set REVERB to Hall and modulate after triggering for billowing tails– use envelopes, slow LFOs or random gates for evolving reverberant textures.
- **INF (Infinite) Mode Drones:**  
  - Flip to **INF mode** and use slow automation of DECAY and DENSITY to morph the particle cloud, then filter externally for shifting spectral drones.  
- **External CV Mangling:**
  - Feed audio-rate modulation into FREQ or SURFACE for pseudo-FM textures.  
  - Try audio-rate pings into **TRIG** for chopped, granulated buffer effects—excellent for granular manipulation.

---

#### Patch Example: Dripping Haunted Cave Pad

1. Set TAIL to amplitude+probability mode.  
2. Run moderate, non-repetitive random CV (Wogglebug, Turing Machine, etc) to **SURFACE** and **DENSITY**.  
3. Max SPREAD for stereo.  
4. DECAY high.  
5. REVERB set to Hall.
6. INF enabled.
7. Output to lush stereo FX (delay/shimmer).

---

**Remember:** All CV inputs sum with their panel knobs. Hit the parameters from as many modulation sources as you can for the most organic, lively results!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)