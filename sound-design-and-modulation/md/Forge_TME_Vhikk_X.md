# Forge TME — Vhikk X

- [Manual PDF](../../manuals/vhikk x.pdf)

---

[**Download the Vhikk X Manual (PDF)**](https://forge-tme.com/vhikk-x/)  

---

# Modulating Vhikk X for Eurorack: Sound Design Guide
*(Focus: Distorted Percussion, Dubstep/DnB Basses, Haunting Pads)*

The **Vhikk X** by Forge TME is a multi-algorithm stereo sound source and processor designed for hands-on exploration in modular synth setups. It offers 36 algorithms (9 per bank, 4 banks), extensive CV modulation, and stereo in/out for both creation and processing of wild, dense, or delicate sounds.

Below are recommended patching and modulation strategies tailored for **distorted percussion, crazy basslines, and haunting atmospheric pads**.

---

## 1. Key CV Inputs & Controls

- **MORPH, BASIS, FIELD, TIME, FORM** (CV with attenuverters): Modulate these for dynamic timbral shifts.
- **VCA**: Internal stereo VCA; CV control for amplitude/punch shaping.
- **SEED, SCAN** (Encoders, no CV): Manual/automation for algorithmic randomness & morphing.
- **Volume in/out**: Can be overdriven for distortion.
- **Two Toggles**: Algorithm selection.
- **Four Banks**: More options with future updates/firmware.

**CV Routing Tips:**
- Any CV in VCA is normalled to all other param CVs (if unpatched).
- MORPH CV normalled to remaining param CVs (if unpatched).
- Attenuverters = on-the-panel fine-tuning.

---

## 2. Distorted Percussive Sounds

**Setup:**
- Choose an algorithm with sharp transients, granulation, or aggressive processing (experiment with different toggle/bank combos).
- Feed short triggers, envelopes, or audio percussion samples into the stereo inputs.

**Modulation Moves:**
- Patch fast, snappy envelopes (from Maths, Quadrax, etc.) into the **VCA CV** for sharply gated, drum-like attacks.
- Modulate **MORPH** and **BASIS** with stepped/random voltages or fast LFOs — jump between different timbres, glitchy distortion, and pitch bursts.
- Drive the **Input Gain** and **Output Gain** using the encoders to add internal clipping/distortion (Vhikk X soft-clips at each gain stage for punchy grit).
- Patch a slow LFO into **FIELD** to create movement within the percussive shell, morphing the overtones or decay characteristics per hit.
- Use the **TIME** CV to vary granulation or internal delay/reverb times, for metallic, ringing, or decaying echoes.

**Creative Extreme:** Randomize **SEED/SCAN** via manual press (both buttons), causing algorithmic chaos between hits.

---

## 3. Dubstep/Neuro Drum & Bass Basslines

**Setup:**
- Select an algorithm that's synth-heavy—complex oscillators, wavefolders, or aggressive filters.

**Modulation Moves:**
- Use a quantized pitch sequence into **BASIS** (V/Oct calibrated) for note control.
- Route an audio-rate LFO or oscillator to **MORPH** or **FORM** for FM-style, gnarly transformer bass movement.
- Patch a sync'ed envelope or stepped random into **TIME**, **FIELD**, and **VCA** for 'wobble'—tight amplitude shaping, filter sweeps, and formant morphing.
- Push the **Input** and **Output Gain** encoders into saturation for crunchy, heavy distortion.
- Manually 'scan' with the **SCAN** encoder during a sequence to morph bass 'characters' in real time.
- Use stereo outputs to widen the bass via external mid-side, chorus, or direct patching for a massive effect.

**Creative Extreme:** Launch into extreme modulation depths, overdriving CV attenuverters for unpredictable, unstable timbres. Try flipping algorithms mid-bar ("toggle switch performance") for glitchy, aggressive phrases.

---

## 4. Haunting Atmospheric Pad Sounds

**Setup:**
- Pick an algorithm focused on granular, shimmering, or filter-resonant sounds—often in true stereo.

**Modulation Moves:**
- Feed slow, looping envelopes or random LFOs into **MORPH, FIELD, FORM, TIME** for continuous drifting soundscapes.
- Use low amplitude/no CV in **VCA** for swelling, evolving pads.
- Patch stereo field recordings, synth chords, or noise into **Stereo Inputs**; process these with Vhikk X's reverb, delay, or spectral algorithms.
- Keep the **Input/Output Gains** moderate for headroom; overdrive only for distant, haunted saturation.
- Slowly rotate **SEED** and **SCAN** encoders to drastically evolve algorithms, introducing spectral artifacts and spectral haloes.
- Automate switching through banks/algorithms for scene changes without patch rewiring.

**Creative Extreme:** Use the **internal randomisation (press both buttons)** to inject spontaneous ghostly mutations.

---

## 5. Power User Tips

- **Attenuverters as Manual Shapers:** When no CV is patched, these become precise manual 'morphers'—glide through sound worlds by hand.
- **Global vs. Per-Algorithm Save:** Store 'scene' settings for rapid recall—use per-algorithm storage for live sets/performance flexibility.
- **Calibration:** Ensure BASIS is calibrated for perfect 1V/oct tracking if playing melodies/basses.

---

## 6. Example Patching Summary

**Distorted Snare:**
- Envelope → VCA
- Fast S&H → TIME, MORPH
- Hot Input Signal + High Output Gain = Hard Digital Clipping
- Tap both buttons for SEED-ful chaos

**Wobble Bass:**
- Sequencer → BASIS (V/Oct)
- Audio-rate Osc → FORM
- S&H or Sequenced Envelope → FIELD, TIME
- MOD Wheel → MORPH (performance filter sweeps)
- Slow SCAN encoder movement for evolution

**Haunted Pad:**
- Stereo Input (tape hiss/field) → Inputs
- Two slow LFOs → FORM, FIELD
- Envelope → VCA for slow fade ins/outs
- Periodic manual SEED/SCAN movements or internal randomization

---

## Resources

- [Vhikk X Official Manual / Web Guide](https://forge-tme.com/vhikk-x/)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---

Let yourself get lost in the [tele]presence and dynamic algorithmic world of Vhikk X—the stranger and more interwoven your modulations, the more this module will reward creative exploration!