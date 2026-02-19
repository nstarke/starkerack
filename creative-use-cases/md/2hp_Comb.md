# 2hp — Comb

- [Manual PDF](../../manuals/Comb_Manual.pdf)

---

[**Comb Module Manual (PDF)**](sandbox:/mnt/data/Comb%20Module%20Manual.pdf)

---

# Creative Uses for the Comb (2hp) Eurorack Module

The 2hp Comb module is a compact and versatile IIR peaking comb filter capable of self-oscillation and creative timbral shaping. Below are several approaches—ranging from classic to experimental—to inspire your patching adventures with Comb:

---

## 1. **Fattening and Thickening Mono Signals**

- **Use case:** Make simple waveforms (saw, square, triangle) from a VCO richer and more “alive.”
- **How:** 
    - Patch the VCO output into **Comb IN**.
    - Adjust **FREQ** to suit your base pitch and tune the combing effect to harmonize with the VCO pitch.
    - Set **RES** for desired resonance/thickness.
    - Modulate **DAMP** with a snappy envelope for dynamic bright/dark sweeps.
- **Recommended modules:** Any VCO (Mutable Instruments Plaits, Make Noise STO), envelope generator (ALM Pip Slope), oscillator with FM.

---

## 2. **Physical Modeling (String and Plucked Sounds)**

- **Use case:** Decay noise bursts or triggers to generate Karplus-Strong string or percussion sounds.
- **How:** 
    - Generate short bursts using a noise source (Mutable Instruments Kinks, 2hp Noise) and a fast envelope into a VCA.
    - Feed noise burst into **Comb**, crank up **RES** to near self-oscillation.
    - Tune **FREQ** to pitch; modulate with sequencer for melodies.
    - Use **DAMP** to shape string/pluck brightness.
- **Extra tip:** Sequence **FREQ** for melodic “bouncing ball” or tonal pluck patterns.
- **Recommended modules:** Trigger sequencer (Pamela’s PRO Workout, Deluge), Noise Source, Envelope, VCA.

---

## 3. **Self-Oscillation Drone and FX**

- **Use case:** Turn Comb into a tunable oscillator or noise drone generator.
- **How:** 
    - Set **RES** high enough for self-oscillation.
    - Do not patch audio into IN, or feed a minimal signal for wave-warped results.
    - Modulate **FREQ** and **DAMP** with slow LFOs for “drifting” drones.
    - Try FM’ing **FREQ** with audio-rate oscillators for metallic “DX7” FM textures.
- **Recommended modules:** LFO (Batumi, Befaco Rampage), audio-rate modulator (Disting, Dixie II+).

---

## 4. **Pseudo-Phasing, Flanging, and Chorus-Like Effects**

- **Use case:** Animate dull pads or drones with moving peaks and notches.
- **How:** 
    - Patch audio (pads, chords, drones) to Comb.
    - Slowly modulate **FREQ** with an LFO, or use S&H for stepped movements.
    - Layer dry and wet signals using a mixer for parallel processing.
    - Modulate **DAMP** for subtle wet/dry shimmer.
- **Recommended modules:** LFO, mixer or crossfader module (Doepfer A-138, WMD Overseer).

---

## 5. **Percussive and Glitch FX**

- **Use case:** Rhythmically destroy or warp drum hits, breaks, or external sounds.
- **How:** 
    - Send drum loops or hits (via sampler/looper module or external input) to Comb.
    - Use clocked random voltages and stepped modulation for **FREQ** and **RES** (“digital artifacts,” “shredded” percussives).
    - Add a VCA or a gate to “chop” Comb’s output for circuit bent/game music style textures.
- **Recommended modules:** Sampler (Morphagene, BitBox), random CV source (Wogglebug, SSF Ultra-Random).

---

## 6. **Live Performance/Expressive Control**

- **Use case:** Make Comb’s settings playable in real time.
- **How:** 
    - Assign pressure sensor, joystick (Intellijel Tetrapad/Planar), or manual CV sources to modulate **FREQ**, **RES**, and **DAMP**.
    - Use foot controllers to control feedback/dampening for live builds/breaks in a jam.
- **Recommended modules:** Intellijel Planar/Tetrapad, Synthwerks FSR, DIY expression pedal interface.

---

## 7. **Multi-Comb Chaining for Resonant Clouds**

- **Use case:** Process sound through more than one Comb (or other resonant modules) in series for dense, moving peaks—a “comb cloud.”
- **How:** 
    - Chain multiple Comb modules or use a combination of Comb and resonant filters (Doepfer A-127).
    - Spread **FREQ** settings for each unique harmonic focus.
    - Experiment with cross-modulating their CVs for interdependent modulations.
- **Recommended modules:** More Comb modules, resonant filter banks (A-127, Frap Tools Fumana).

---

## Bonus Tips

- **Clocked Comb:** Use clock division/multiplication to “sync” FREQ modulation to your patch’s tempo for rhythmically coherent comb artifacts.
- **CV Automation:** Use sequencers or random sources to automate all three parameters—great for morphing textures in generative or evolving patches.
- **Stereo Processing:** Use two Comb modules for left and right channels, modulate FREQ slightly differently for wide, animated stereo fields.

---

> For reference, here is the [**Comb Module Manual (PDF)**](sandbox:/mnt/data/Comb%20Module%20Manual.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)