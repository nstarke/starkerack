# Moog — Mavis

- [Manual PDF](../../manuals/MAVIS_MANUAL_V2_06.27.2022.pdf)

---

[Moog Mavis User Manual (PDF)](https://www.moogmusic.com/sites/default/files/2023-05/Mavis%20User%20Manual%20WEB_0.pdf)

---

# Using the Moog Mavis in Composing Full-Length Eurorack Songs

As a modular musician, you’ll quickly find that while the [Moog Mavis](https://www.moogmusic.com/products/mavis) is a powerful, self-contained analog voice, unlocking its true creative potential for full-length tracks means leveraging its flexibility as a patchable, semi-modular system within a larger eurorack environment. Below, I’ll discuss both the strengths and the limitations of the Mavis as a song-building tool, followed by **strategies and patch ideas** for integrating it into larger modular arrangements to produce evolving, structure-rich songs.

---

## 1. What Is Mavis Good At?

**Core strengths:**
- Classic analog monophonic voice (oscillator, ladder filter, envelope, VCA)
- Powerful patchbay for external CV/audio integration
- Unique features like wavefolding, built-in utility mixer, sample & hold (S+H), and attenuator

**Limitations** (to keep in mind for song construction):
- Single oscillator & single envelope generator
- No built-in sequencer, clock, or complex modulation sources
- No internal multi-channel mixing, effects, or sophistication for polyphony/complex layering

Thus, **Mavis alone is a great building block for individual voices and sounds**. To build *songs*, you’ll want to integrate it with:
- Sequencers
- Modulation sources/LFOs
- Clocks & dividers/multipliers
- Utilities (VCAs, mixers, switches)
- Effects modules (delay, reverb, distortion, etc.)
- Additional voices/instruments
- Performance controls (touch, MIDI–CV, etc.)

---

## 2. Strategies for Building Full Songs with Mavis

### A. Song Structure via Modulation & Control
**Problem:** Patches can be static; musical “moments” rather than songs.

**Solution:** Use **external CV modulation and sequencers** to achieve *macro* song structure, not just “looping” patterns.

#### **Ideas:**
- **Multiple Sequencers:** Use one sequencer for basic Mavis melodies/basslines and another for controlling filter cutoff or envelope shape to create verses, choruses, bridges, builds, etc.
- **Utilities:** Use voltage-controlled switches, sequenced muting, or sequential switches to activate/deactivate patches or modulation sources in a songlike arrangement.
- **Key Changes:** Use precision adders/quantizers to transpose the Mavis sequence in and out of key centers for different song sections.

### B. Layering/Voice Doubling
- Use Mavis as a bassline when layered with a second oscillator voice (another synth or sample) for leads or chords.
- Sequence different sections: e.g., have Mavis play intro and then “move” its sequence to another voice for development, or vice versa.

### C. Live Performance & Macro Controls
- Map all-important “macro” changes—filter sweeps, envelope settings, wavefolder amount, etc.—to external CV and perform or automate them.
- Use external clock dividers and mults to change rhythm/tempo between song sections.

### D. Dynamic Timbre and Texture
- Use Mavis’s **wavefolder and filter** as an effects processor on other voices (via patchbay).
- Insert S+H or LFO modulation for more generative, evolving patches (e.g. for song bridges or breakdowns).

### E. Thematic Variation and Transitions
- Patch S+H or random sources to create subtle variations (melody, timbre) in each song repetition/section.
- Automate switching between modulation sources (LFO, EG) via CV, so each section sounds distinct.

---

## 3. Example Patch Concepts for Full-Song Composition

### **A. Bassline to Lead Switch**
- **Intro/Verse:** Use Mavis as a bass voice via sequencer 1.
- **Chorus:** Via voltage-controlled switch, send sequencer 2 (with higher notes) to Mavis for lead duty, while another voice takes over bass.
- **Use sample & hold** or random modulation for breakdowns/transitional sections.

### **B. Filter/EQ and Macro Transitions**
- Patch the filter cutoff to be modulated by an external envelope/fader/automation for sweeps in/out of new sections.
- Use the attenuator to control the amount of external LFO/EG influence over long periods (slow builds).

### **C. Texture, FX, and Post-Processing**
- Send non-Mavis voices through the Mavis’s filter or wavefolder for creative breakdowns (e.g. use FOLD IN input to process drums with dramatic filter sweeps).

### **D. Randomization and Variation**
- Patch S+H output to VCO pitch or filter cutoff for subtle generative “fills” or breakdowns.
- Route random or stepped CV to attenuator for controlled signal “evolutions” during the track.

---

## 4. Sample Patch Integration (with Other Modules)

```markdown
[Sequencer] --1V/OCT--> [Mavis VCO]
               |              |
            [Clock]----> [Other Voice: Drums/Lead/FX]
                              |
         [Function Generator/ADSR] --CV--> [Mavis Filter/Envelope]
                              |
        [Sample & Hold] --------------> [Mavis PWM, cutoff, or VCA CV]
                              |
         [FX Send/Return] <-------------> [Mavis Wavefolder/VCF as processor]
```

---

## 5. Songwriting Mindset Tips

- **Perform patch changes, parameter sweeps, and voice switching live** to create sections distinct in both sound and rhythm.
- **Automate or script sequence changes, keys, and modulations**—use matrix switches, preset managers, or scenes if available.
- **Embrace utility/logic modules**—they can trigger, gate, mute, or morph between patterns and textures for "song mode."
- Remember: *Compositional structure comes from change and contrast!* Use Mavis as an expressive *element* in a broader performance system.

---

For more patching ideas and technical details, see the [Mavis Manual PDF](https://www.moogmusic.com/sites/default/files/2023-05/Mavis%20User%20Manual%20WEB_0.pdf).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)