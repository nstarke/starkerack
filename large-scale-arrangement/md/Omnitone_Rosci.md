# Omnitone — Rosci

- [Manual PDF](../../manuals/Rosci-Manual.pdf)

---

[**Rosci User Manual (PDF)**](https://omnitone.ca/wp-content/uploads/2023/11/Rosci-Rev3-Manual.pdf)

---

## Using the Omnitone Rosci Module for Full-Length Song Creation in Eurorack

Transitioning from catchy grooves or riffs to a full-length, dynamic song is a challenge in modular synthesis. The Omnitone Rosci, as described in your manual, is a **deep wavetable oscillator with morphing, harmonic, formant, and detune capabilities**—a sonic chameleon designed for texture and motion. Here’s how you can use Rosci, alongside your other modules, to build evolving, arranged compositions:

---

### 1. **Morphing Soundscapes and Progression**

**Use Manual/Automated Knob Modulation:**
- The ability to morph between different waveforms (via the **generate** and **complexity** controls) lets you create evolving timbres. Automate these controls using LFOs/envelopes or sequence them via CV from a sequencer to have your lead or pad change character over time.
- **Scene building:** Start your track with a simple two-point waveform and gradually increase the complexity (number of points & harmonics) to add density as your song progresses.

---

### 2. **Formant/Vocal Transitions for Sections**

**Mimic Verse/Chorus/Bridge:**
- The formant parameter can make your synth voice resemble human vowel sounds. Assign different CV settings or automation to mimic verses (mellow formants), choruses (forward/aggressive formants), and bridges (unusual vowels or "compressed" waveforms).
- Change **formant settings with scene or part changes** for a clearly defined song structure.

---

### 3. **Creating Builds, Drops, and Transitions**

**Detune for Drama:**
- Gradually increase the detune parameter (or modulate via envelope) to introduce tension leading into a new section (drop/chorus), then snap it back to “in tune” for impact.
- Automate **harmonics** to add brightness for a build-up, then cut them back for a breakdown or verse.

---

### 4. **Polyphony and Layering**

**Layer Multiple Voices with Unique Roscis:**
- Use multiple Rosci modules or layers (possibly with a sampler or multitrack recorder) to assign different instances to bass, melody, and pads. Each can be uniquely modulated for its own evolution in the song.
- In a single-voice patch: Use the morphing capabilities to go from bass tones (simple wave) in verse to leads (complex, harmonic-rich) in chorus.

---

### 5. **Sequencing Song Structure**

**Combine with:**
- **Step Sequencers:** One can control progression of pitch, the other can send CV to Rosci's modulation inputs (complexity, formant, harmonics) for timbral shifts per song section.
- **Scenes/Presets:** If your case allows using a preset manager (like Frap Tools USTA, Erica Black Sequencer, or Malekko Voltage Block), you can store and re-call modulation states for verse/chorus/bridge.
- **Gate Sequencers:** Use gates to trigger waveform regeneration or changes at key moments in the song (e.g., chorus entry: trigger a new waveform with the generate input).

---

### 6. **Ambient & Textural Fills**

- **LFO Mode:** Set Rosci to LFO mode for slow, evolving modulation signals—modulate filters, effects, or even itself for continuously shifting backdrops between sections.
- **Manual Tweaks:** The full parameter range is available to tweak for live improvisation over your basic structure.

---

### 7. **Automation via External Controllers**

- Connect via MIDI-to-CV converters or use pressure pads, joysticks, or foot pedals to make real-time adjustments in performance—ideal for improvising fills, solos, or new song sections.

---

### 8. **Integration and Effects Chaining**

- **Processing the Output:** Pass Rosci through filters, delays, reverb, and distortion to change its character between parts of your song.
- **CV Feedback Loops:** Use utilities (attenuverters, VCAs) to create feedback between Rosci’s outputs and your modulation sources for self-evolving patches.

---

### Example Song Flow Using Rosci

1. **Intro:** Slow LFO modulates complexity, formants stay mellow. Minimal harmonics.
2. **Build/Verse:** Gradually increase harmonics and complexity, subtly detune for tension.
3. **Chorus:** Snap complexity and harmonics to higher values; morph to a new waveform. Change formant to a brighter tone. More modulation on all parameters.
4. **Breakdown:** Reduce all modulations. Strip back to a simple waveform. Use LFO mode for S&H random voltages or wobbly pads.
5. **Outro:** Slowly fade complexity/harmonics to zero or modulate detune for a drifting, dissolving ending.

---

### Useful Patch Example

- **Melody:** Sequencer pitch → V/OCT, modulation lanes to harmonics & formants.
- **Bass:** Simpler Rosci patch, filter after Rosci for depth.
- **Pads/Ambience:** Rosci in LFO mode, slow modulation to FX parameters or VCA amplitude.

---

**In summary:** Treat Rosci as a *timbral arranger* as much as an oscillator. By patching its modulation parameters and associating timbre shifts with song structure, you can easily craft pieces that evolve far beyond loops. Combine with sequencers, logic modules, effects, and manual performance for full-length, structured songs.

---  

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)