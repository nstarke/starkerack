# Tiptop Audio — SD909

- [Manual PDF](../../manuals/Tiptop_Audio_SD909_ns.pdf)

---

[SD909 Manual PDF](https://tiptopaudio.com/manuals/SD909_manual.pdf)

---

# Creative Sound Design with the Tiptop Audio SD909 Eurorack Module

The Tiptop Audio SD909 is designed to authentically reproduce the snare sound of the legendary Roland TR-909, but as a modular instrument, it invites much deeper creative exploration. Here’s how you can push it into wild territory for distorted drums, aggressive basslines, and eerie pads.

---

## Core Features for Modulation

- **CV Inputs:** The SD909 offers CV control over **Tune** (VCO pitch) and **Noise** (noise clock frequency), as well as external Accent.
- **Manual Controls:** TONE, TUNE, SNAPPY, NOISE, LEVEL, ACCENT
- **Audio Outputs:** SD OUT (full voice), NOISE OUT (raw, voltage-controlled noise)
- **Manual Trigger**: Also CV/gate triggerable
- **Accent Input:** Gate/trigger or CV for dynamic response

---

## Techniques

### 1. **Distorted Percussive Sounds**

- **Overdrive Internal Mix:**
    - Crank the **NOISE** and **SNAPPY** controls past the “909” region for an extra-aggressive blend of VCOs and noise.
    - Drive a hot CV sequence into **ACCENT IN**—use an envelope or random CV for dynamic amplitude distortion.
    - Patch the **SD OUT** through a wavefolder, distortion, or overdrive module after the SD909 for extra grit.

- **Noise Clock Modulation (Metallic Snares & Distortion):**
    - Modulate the **NOISE** CV with an LFO or random stepped CV. At low frequencies the snare becomes metallic or glitchy, and clocking noise becomes part of the sound—perfect for industrial distortion.

- **Brutal Amplitude Dynamics:**
    - Use a fast, high-voltage gate for TRIGGER and an independent sharp envelope for **ACCENT IN**: this allows "punchy" transients and deep timbral change.

---

### 2. **Dubstep / Drum & Bass-Style Basslines**

- **Tune as Bass Oscillator:**
    - Use the **TUNE** knob and send sequenced 1V/oct CV to **VC-TUNE** to "play" the snare body like a bass oscillator.
    - Turn down **NOISE** and **SNAPPY** for a clean VCO body, or keep some noise for a reedy edge.

- **Waveform Shaping with Noise:**
    - Modulate **NOISE** and **SNAPPY** with a slow LFO or envelope to add evolving texture to the bass note.
    - Take the **NOISE OUT**, run it through a VCF or waveshaper, and mix back with **SD OUT** for layered, complex bass.

- **Extreme FM:**
    - Self-patch: Take **NOISE OUT** and use as CV into **VC-TUNE** or **VC-NOISE** (beware voltage scaling). This creates feedback FM effects and wild bass growls.

---

### 3. **Haunting Atmospheric Pads**

- **Noise Source as Pad Base:**
    - Patch **NOISE OUT** to a VCA/Envelope, then through heavy reverb or delay modules for lush atmospheric noise beds.
    - Use an LFO or sequencer to modulate the **NOISE** frequency for drifting, morphing character.

- **Drifting Harmonics:**
    - Send slow LFOs or random stepping CV to **TUNE** and **NOISE** CV inputs simultaneously, diffusing the percussive snare into evolving textures.
    - Set **TONE** to lengthen the decay (as much as possible).

- **Drone Techniques:**
    - Sustain trigger with looping gates; increase **SNAPPY** to blend more noise for shimmer.
    - Parallel process **SD OUT** and **NOISE OUT** separately (filters, resonators, reverbs) and recombine for deep pads.

---

## Pro Tips

- **Patching External Signal to ACCENT IN:** Use audio-rate or chaotic CV for AM-like effects and brutal timbral shifts.
- **Layering:** Stack multiple gates/triggers, modulate all CV inputs—layer SD909 with other drum modules for unpredictability.
- **Noise Clock Artifacts:** Intentionally clock the noise generator down to metallic/bitcrushed territory—especially with the snare, this is an amazing “broken circuit” flavor.

---

## Additional Resources

- Manual: [SD909 Manual PDF](https://tiptopaudio.com/manuals/SD909_manual.pdf)
- Official Page: [Tiptop Audio SD909](https://tiptopaudio.com/909-2)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)