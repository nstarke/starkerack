# WMD SSF — Facture

- [Manual PDF](../../manuals/manual_black_fracture.pdf)

---

[Download the WMD Fracture Manual PDF](https://wmdevices.com/content/Fracture_Manual.pdf)

---

## Creative Eurorack Patch Ideas With WMD Fracture

The WMD Fracture is a multi-particle percussion synthesizer module, particularly well-suited for creating claps, applause, and an array of percussive textures. Its granular engine can be modulated in multiple ways, yielding a wide spectrum of rhythmic and textural results. Below are some creative approaches to integrating Fracture with your Eurorack system:

### 1. **Dynamic Percussion Textures With CV Sequencers**
- **Module Suggestions:** Make Noise René, Intellijel Metropolix, or any CV/gate sequencer.
- **Patch Idea:** Use a sequencer to modulate the SURFACE parameter or the SPREAD. This can create evolving percussive palettes where Fracture cycles between percussive types (e.g., claps, snaps, and switches) each step.
- **Bonus:** Use random stepped CV (e.g., Mutable Instruments Marbles) to randomize the SURFACE parameter for unexpected percussive combinations.

### 2. **Poly-Rhythmic Bursts With Clock Manipulation**
- **Module Suggestions:** 4ms Rotating Clock Divider, Pamela’s New Workout
- **Patch Idea:** Clock the TRIG and TICK inputs with different clock divisions or shuffled triggers. This creates overlapping percussive bursts and accents that mimic large crowds or complex rhythms.
- **Accent Tips:** Modulate the ACC input with velocity or random gates for dynamic, alive rhythm swells.

### 3. **Spectral Sculpting Using Filters & Effects**
- **Module Suggestions:** Mutable Instruments Ripples, QPAS by Make Noise, or Erica Synths Black Hole DSP2
- **Patch Idea:** Take the stereo output from Fracture into a stereo filter or multi-FX. Bandpass filtering can emphasize the “clap” or “snap” range, while heavy resonance turns it into textured snare hits.
- **Reverb:** Turn REVERB fully wet on Fracture or send to an external reverb for lush audience effects; modulate decay/reverb for crowd-in-a-cave sounds.

### 4. **Granular Chord Clouds**
- **Module Suggestions:** Quantizer (Intellijel uScale, Tiptop Quantizer), Polyphonic sequencers
- **Patch Idea:** Patch a CV sequence to PITCH and SPREAD, then mult these to a quantizer for harmonic bursts. The result: percussive, pitched “clap chords” perfect for IDM or ambient music.

### 5. **Probability & Chaos With Random Modulation**
- **Module Suggestions:** Mutable Instruments Marbles, Wogglebug, SSF Ultra-Random
- **Patch Idea:** Modulate DENSITY and SPREAD with random or semi-random voltages, controlling how dense and how wide the stereo/pitch field is on every burst. For generative patches, tie this to slow, evolving random CV.

### 6. **Feedback & Resonance Loops**
- **Module Suggestions:** Send Fracture output back into effects or resonators (Mutable Instruments Rings, or physical modeling FX).
- **Patch Idea:** Send Fracture’s output into Rings or another resonator in “external input” mode, creating percussive textures with a unique, metallic or string-like quality—especially effective with short DECAY and low DENSITY.

### 7. **Live Performance Macros**
- **Module Suggestions:** Intellijel Planar, Make Noise Pressure Points, or a manual CV controller.
- **Patch Idea:** Use macro controls to sweep multiple parameters—e.g., fade from tight claps to granular crowd applause by sweeping DENSITY, DECAY, SPREAD, and SURFACE simultaneously with a single fader or joystick. Great for performance transitions.

### 8. **Dynamic Sound Design For Film/Game Audio**
- **Patch Structure:** Use Fracture TAIL and PUNCH settings to generate risers, impacts, and foley-like textures. Modulate TAIL and FREQ with LFOs or envelopes for evolving texture beds.

### 9. **Stereo Space Experiments**
- **Patch Structure:** Use Fracture’s stereo outputs for main percussion while supporting with tightly-panned mono percussion (from a DrumBrute, Basimilus Iteritas Alter, etc.) for a wide percussive field.

### 10. **Eurorack Drum Machine Integration**
- **Module Suggestions:** Trigger sequencers like Elektron Analog Four (CV outs), Trigger Riot, or Endorphin.es BLCK_Noir (as accompaniment)
- **Patch Idea:** Use Fracture’s versatile surfaces and grains as the main ‘clap’ or ‘crowd’ in a Eurorack drum set, and apply accent/gated bursts to break up standard patterns.

---

## Pro Tips

- **CV Modulation:** All major parameters can be CV’d. Use slow LFOs or random S&H for “humanization” of your percussive bursts.
- **Tail Modes:** Experiment with the TAIL switch for subtle differences in burst behavior—utilize in micro-sound design or when layering multiple Fracture modules.
- **INF (Infinite Mode):** For ambient sound beds, set Fracture to INF, and use slow sweeping CV, modulating DENSITY for immersive, shifting noise textures.

---

For deeper integration, consider using preset/cv recallers (e.g. ADDAC206) or audio manipulators (Loopers, Grain Delays) for evolving, set-and-forget sound structures.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)