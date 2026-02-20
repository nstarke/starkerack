# ALM — ALM005 - Dinky's Taiko

- [Manual PDF](../../manuals/alm005-manual.pdf)

---

[ALM-005 'Dinky’s Taiko' Operation Manual (PDF)](https://busycircuits.com/docs/alm005-manual.pdf)

---

# Creative Modulation Techniques for ALM-005 ‘Dinky’s Taiko’

The ALM-005 ‘Dinky’s Taiko’ is an exceptionally flexible 12-bit digital drum voice with full voltage control over almost every parameter (excluding the tone control), making it a powerhouse for innovative percussion, basslines, and atmospheric sounds. Below are detailed strategies for modulating Dinky’s Taiko to generate **distorted percussion**, **crazy basslines**, and **haunting pads** within a Eurorack setup.

---

## 1. Distorted Percussive Sounds

### Key Parameters to Modulate:
- **Noise Spectrum & Release**
- **Oscillator Start/End Frequency, Speed, Release, Wave**
- **Mix (Noise vs Oscillator)**
- **EQ (Tilt Filter)**
- **Accent & Choke trigger inputs**

### Modulation Ideas:

- **Overdriven Tones:**  
  - Set the Mix fully CW for mostly oscillator output; patch in a hot CV source (sequencer, looping envelope, or an LFO with lots of amplitude) to the frequency controls (Start/End Freq).
  - Push the output into +10V territory (“signals can get HOT”) and further clip/distort with external modules (wavefolders, analog distortion, or even the input of a VCA at high gain).
- **Crushed Metallic Hits:**  
  - Use fast random LFO or S&H CV on the Wave control to jump between the table's digital and noisy waveforms per hit.
  - Modulate the Noise Spectrum with fast pitch envelopes or stepped random voltages.
  - The Choke input can slice off the tails of heavily-decaying sounds, creating glitchy, cut-off sounds.
- **Sharpen via EQ:**  
  - Automate the EQ control (with a slow LFO or envelope) to alternate harsh treble or deep bass prominence.
- **Accent Torture:**  
  - Send varied gates to Accent—either from sequencer accent rows, Euclidean patterns, or probability triggers. Combine with noise-heavy settings for aggressive attack transients.

---

## 2. Crazy Bassline Sounds (Dubstep/Drum & Bass Style)

### Key Parameters to Modulate:
- **Oscillator Start/End Frequency**
- **Speed (FM-like, metallic sweeps)**
- **Oscillator Wave (Wavetable scan)**
- **Mix**
- **EQ**

### Modulation Ideas:

- **Tearing Bass Wubs:**
  - Modulate Start and End Frequencies with synchronized LFOs or envelopes, sweeping ranges rapidly for “talking” bass tones typical in modern bass music.
  - Use a sequencer CV track to pitch Oscillator Start Freq per note.
- **Formant-like Movements:**
  - Modulate the Wave parameter rhythmically for morphing timbres. Combine stepped and smooth CV for glitchy or vocal-like transitions.
  - Modulate Mix back and forth with a punched-in envelope for dynamic “talking” bass effects.
- **Resonant Edge:**
  - EQ control towards a treble tilt accentuates harmonic buzz; automate for vowel-like sweeps.
- **Choke for Micro-stabs:**
  - Use a trigger sequencer to punch in quick Choke triggers just after each note to create micro-length, percussive “pluck” basses.

---

## 3. Haunting Atmospheric Pads

### Key Parameters to Modulate:
- **Long Noise & Oscillator Release**
- **Low Speed and subtle Start/End Freq sweeps**
- **Wave (slow or smooth CV)**
- **Mix (for evolving blends)**
- **EQ (tilt for spectral movement)**

### Modulation Ideas:

- **Evolving Textures:**
  - Use long, free-running random LFOs or S&H on Oscillator Wave, Noise Spectrum, and Mix for morphing, shimmering textures.
  - Slow slewed pitch modulation on Start/End Freq gives drifting, unstable pitch—great for spooky pads.
- **Swelling & Fading:**
  - Use the Noise and Oscillator Release controls at higher values, so triggered hits overlap and create smooth washes.
  - Patch gentle envelopes or LFOs to EQ for subtle emphasis/fading between dark and airy moods.
- **Pad Sequencing:**
  - Sequence the Accent input with probability gates for softly shimmering attack variations.
  - Try chaining multiple short triggers for clustered, granular atmospherics.

---

## General Techniques

- **External VCA and FX:**  
  Dinky’s Taiko output can get very hot and digital—patch into a VCA for further amplitude sculpting, or into reverb for cinematic effects.
- **Pamela’s Workout Pair:**  
  The manual suggests ALM-001 ‘Pamela’s Workout’ for advanced rhythmic modulation: use it to send divided, shuffled, or random triggers/CV to every CV input on Dinky’s and accentuate the creative chaos!

---

> **Reference:**  
> [ALM-005 'Dinky’s Taiko' Operation Manual (PDF)](https://busycircuits.com/docs/alm005-manual.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
