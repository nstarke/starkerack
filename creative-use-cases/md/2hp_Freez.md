# 2hp — Freez

- [Manual PDF](../../manuals/Freez_Manual.pdf)

---

[**Freez Manual PDF**](https://nstarke.github.io/freez-manual.pdf)

---

## Creative Patch Ideas for 2hp Freez

The **2hp Freez** is a compact, voltage-controllable locked looper for Eurorack, with sample rate reduction and buffer manipulation capabilities. With these tools, you can turn any incoming audio into granular textures, glitchy loops, or time-warped fragments.

Below are some creative ways to integrate Freez with other modules:

---

### 1. **Granular Textures with Random CV**

**Combine with:** Random voltage generators (e.g. *Mutable Instruments Marbles*, *ALM Pamela’s New Workout*), LFOs, or stepped CV sequencers (e.g. *Make Noise Tempi*).

- **How:** Patch random or slowly evolving CV to the **SIZE** and **S. RATE** CV inputs.
- **Result:** The buffer length and sample rate change in unpredictable ways, creating constantly morphing granular sounds and shifty digital artifacts.

---

### 2. **Rhythmic Glitches and Beat Repeat**

**Combine with:** Sequencers or clock sources (e.g. *Intellijel Metropolis*, *Arturia Keystep Pro*).

- **How:** Send gate or clock signals into the **TRIG** input, synced to your drum machine or sequencer patterns.
- **Result:** Locks audio snippets in time with your rhythm, creating stutter or beat-repeat effects on command.

---

### 3. **Live Audio Dicing and Stutter FX**

**Combine with:** Drum modules, sampled voices, or any rhythmic audio source (*Mutable Instruments Plaits*, classic drum modules).

- **How:** Route audio through Freez, and use a footswitch, manual button, or controller for instant freezes.
- **Result:** Stutter or cut-up effects on live audio (great for live electronic improvisation or experimental performances).

---

### 4. **Voltage-Controlled Bit Crusher**

**Combine with:** Fast LFOs, audio-rate modulation sources (*Make Noise Maths*, *ALM Busy Circuits Pip Slope*).

- **How:** Modulate **S. RATE** with CV at fast or even audio rates.
- **Result:** Real-time destruction of incoming audio, with wild sample-rate modulation and gritty timbre.

---

### 5. **Dual-Buffer FX with Stereo or Parallel Audio**

**Combine with:** An additional looping/freezer module (*4ms Dual Looping Delay*, *Qu-Bit Nebulae*), mixer, or splitter.

- **How:** Freeze one channel with Freez, and another with a different module; switch between, pan, or blend.
- **Result:** Create complex, layered textures, transitioning between two mangled buffers, suitable for immersive soundscapes.

---

### 6. **CV Looping/Processing**

**Combine with:** Envelope followers or CV-to-audio interfaces (*Doepfer A-119*, *ALM S.B.G*).

- **How:** Use Freez to lock and process CV signals converted to audio-rate, then re-convert them back to CV.
- **Result:** Highly experimental stepped or "sampled" CV sources for unpredictable pitch, filter, or VCA modulation.

---

### 7. **Karplus-Strong/Plucked Synthesis Modifier**

**Combine with:** String synthesis voices (*Mutable Instruments Rings*, *2hp Pluck*).

- **How:** Insert Freez after a physical modeling module and freeze very short snippets.
- **Result:** Generates metallic, atonal, or glitched variations of "plucked" sounds.

---

### 8. **Formant & Vocal FX**

**Combine with:** Microphone preamp module, vocal processor, or contact mic input (*Doepfer A-119*, *Eurorack mic preamp*).

- **How:** Use your voice or acoustic input as source material; freeze and manipulate size & rate.
- **Result:** Makes robotic, grainy vocal effects, especially interesting with external CV modulation of buffer size/rate for evolving textures.

---

### Module Recommendations

- **Random/Chaos CV:** Mutable Instruments Marbles, WMD Geiger Counter (*CV output*), Make Noise Maths.
- **LFO/Envelope:** Intellijel Quadra, ALM Pamela's New Workout, Doepfer A-145 LFO.
- **Sequencer/Gate Generator:** Make Noise Tempi, Arturia Beatstep Pro.
- **Mixer/Utilities:** Happy Nerding 3x MIA, Mutable Instruments Shades.

---

Experiment with placement in your signal chain: immediately after drum sources for glitchy beats, or after a rich pad for ambient textures. The small size of Freez means it easily fits into most racks and opens up a world of timbral and rhythmic manipulation. The CV and trigger options make it uniquely performable and responsive to your modular system.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
