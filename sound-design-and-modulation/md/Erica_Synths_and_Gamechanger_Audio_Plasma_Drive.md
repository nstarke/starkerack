# Erica Synths and Gamechanger Audio — Plasma Drive

- [Manual PDF](../../manuals/Plasma_Module_Manual.pdf)

---

[**Erica Synths Fusion Plasma Drive Manual (PDF)**](https://www.ericasynths.lv/media/PLASMA_DRIVE_1_manual.pdf)

---

# Using the Erica Fusion Plasma Drive for Percussive, Bass, and Atmospheric Sounds

The **Erica Synths Fusion Plasma Drive** is a unique eurorack distortion module based on high-voltage xenon tube technology. It features voltage-controlled distortion, dry/wet mix, switchable EQ, and octave-tracking oscillators for harmonic enhancement. Below are some creative patching and modulation ideas tailored for:

- Distorted percussive sounds
- Complex basslines
- Atmospheric pads

---

## 1. Fundamentals of Modulation

**Key modulation inputs:**
- **Voltage CV Input**: Controls distortion depth.
- **Dry/Wet CV Input**: Blends original and processed signals.
- **Octave Trigger Inputs (OCT TRIG / SUB TRIG)**: Dynamically activate harmonic oscillators (octave up, down, subs).
- **EQ Switch (CV-free but manual switch)**: Choose EQ pre or post-distortion for different coloration.

---

## 2. Distorted Percussive Sounds

**Goal:** Create punchy, rhythmic, and gnarly percussion (e.g., kicks, snares, hats).

**Patch Example:**
1. **Input Source**: Use a short envelope generator (EG) or trigger-driven percussion module to supply sharp, high-level transients to the Plasma Drive input.
2. **Voltage CV Input**: Patch the same/related envelope to the VOLTAGE CV. This will dynamically crank up the distortion at transient peaks, making attacks more explosive.
3. **Dry/Wet CV Input**: Modulate with a slow triangle or stepped random voltage for variable texture on each hit.
4. **Octave Triggers**: Send rhythmic gates to OCT TRIG and/or SUB TRIG from a sequencer or clock divider. This introduces harmonic accents or glitches at chosen moments.
5. **EQ Switch**: Try both ON and OFF positions. EQ ON (pre-distortion) makes frequency boosting more aggressive/distinct.

**Tips:**
- Overdrive may need to be turned up quite high for classic aggressive industrial hits.
- Experiment with output EQ to shape post-distortion thump (boost lows for kicks, highs for snares/hats).

---

## 3. Crazy Basslines (Dubstep/Drum & Bass)

**Goal:** Achieve tearing, modulated, formant-rich bass.

**Patch Example:**
1. **Input Source**: Fat analog VCOs, FM, or wavetable oscillators, ideally with lots of sub content.
2. **Voltage CV Input**: Use complex LFOs, envelopes, or sequenced modulation for wild distortion movement (e.g., fast LFO synced to tempo for "wub" patterns).
3. **Dry/Wet CV Input**: Modulate with gates, random voltage, or a second LFO (out of phase) for dynamic clean/dirty blends within the groove.
4. **Octave Triggers**: Send rhythmic or randomized gates to Octave triggers to activate the “+1” or “-1/2/3” sub oscillators in sync with your bass riff, generating growls and artifacts.
5. **EQ**: Set EQ ON with boosted lows and cut highs for classic dark, woolly bass; or cut lows and boost highs for metallic snarl.

**Tips:**
- Sub octave tracking is essential for dubstep "growl" – automate with trigger patterns closely tied to your groove.
- Drive the input hard for maximum harmonic content.

---

## 4. Haunting Atmospheric Pads

**Goal:** Dense, shifting, spooky textures.

**Patch Example:**
1. **Input Source**: Slowly evolving pads, granular, or spectral sources.
2. **Voltage CV Input**: Very slow random or sample & hold CV to create evolving timbral “drift” in distortion flavor.
3. **Dry/Wet CV Input**: Crossfade between states with an LFO or dynamic envelope follower to respond to pad intensity.
4. **Octave Triggers**: Use clock dividers, burst generators, or generative gates to bring +1/-1 tracking oscillators in and out in slow, unpredictable patterns.
5. **EQ**: ON for extra pre-distortion swirl; off for more faithful input texture. Boost highs subtly for air, or cut for gloom.

**Tips:**
- Combining octave triggers with reverb, delay, and VCAs downstream can produce spectral “ghost tones” and eerie, evolving beds.
- Moderate drive settings retain more pad detail; extreme drive makes for haunting, noisy, tape-distressed vibes.

---

## Additional Patching Ideas

- **Rhythmic Distortion Patterns:** Use clocked trigger sequences into Oct Trig/Sub Trig for "beats" within the distortion itself.
- **Dynamic Expressivity:** Patch velocity from a MIDI-to-CV or sensor module to the Voltage or Dry/Wet CV for real-time performance morphing.
- **Layer With Clean Signal:** Multi the input to another path, then blend dry and Plasma outputs in a mixer for complex depth.

---

[**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)