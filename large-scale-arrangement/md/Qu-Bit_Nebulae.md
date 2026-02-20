# Qu-Bit — Nebulae

- [Manual PDF](../../manuals/Nautilus_v1.1.3.pdf)

---

[**Nautilus Manual PDF** (Qu-Bit Electronix)](https://qubitelectronix.com/manuals/qu-bit_nautilus_manual.pdf)

---

# Using Nautilus to Structure Full-Length Eurorack Songs

As a modular performer, one of the biggest hurdles is moving beyond tightly-looped jams to fully realized song-length pieces with variation, movement, and narrative. The Qu-Bit Nautilus isn’t just another delay—it’s a novel “complex delay network” that can act as a song-structuring tool, inspiration generator, and performance hub when paired with other modules. Here’s how you can use it to build and play out long-form compositions.

---

## Key Functions for Song Development

### 1. **Sound Design Foundations**

Nautilus can create unique audio events from simple patterns due to:
- 8 independently addressable delay lines
- Switchable delay types (Fade, Doppler, Shimmer, De-Shimmer)
- Chroma (internal filter/effects per feedback loop)
- Reversal (incrementally reverse delays per line)

**Result:** You can turn simple rhythmic or melodic gestures into sprawling, evolving soundscapes with rich internal variation—essential for filling out song sections.

---

### 2. **Sectional Variation via Nautilus Controls**

#### **Manual or Automated Macros**
- **Morph Scenes:** Map Nautilus CV inputs to macro controllers (e.g., Planar, Tetrapad, CV sequencers) to automate or perform radical changes in delay lines (Sensors), dispersal, feedback, Chroma type, and reversal.  
- **Song Sections:** Assign different Nautilus Chroma and Feedback Modes to intro, verse, chorus, break, etc. Use the Freeze or Purge button to clearly delineate between sections (e.g., Frozen stutters for a breakdown).

#### **Sonar Output for System-Wide Modulation**
- **Structure via Modulation:** The Sonar output generates stepped CV or gates based on Nautilus’ internal delay network. Use this as a scene-change or "cue" for your other modules—patch to envelopers, filters, sequencer reset inputs, or sample selectors for arranger-style jumps.

---

### 3. **System Integration: Patch Strategies**

#### **A. Song Progression with Nautilus as Live Performance Hub**
1. **Drums** (separate channel, e.g. using a drum module like Erica Pico Drums, Tiptop, or BIA)
2. **Bassline** (independent voice, could employ a filter/distortion for variation)
3. **Lead/Pad** through Nautilus
   - Start with minimal delay, simple Chroma, and one delay line (Sensors CCW).
   - Gradually open up Sensors and Dispersal to “multitrack” your phrase into evolving counterpoint.
   - Bring in Reversal and higher feedback for breakdown/build sections.
   - Freeze buffer to create tension, then Purge for a drop.

#### **B. Self-Modulation and Feedback Networks**
- Patch Sonar output to modulation destinations on Nautilus itself or to external voices.
- Use long delay times on a slowly evolving sequence; modulate feedback/dispersal for movement.
- Key trick: Assign Attenuverters via USB app to re-route control easily during a live set (e.g., swap from external LFO to internally generated Sonar CV for impromptu changes).

#### **C. Song Endings and Transitions**
- Employ De-Shimmer/Shimmer modes for climactic moments (rising/falling pitch echos).
- Use the Purge function as a dramatic “drop”/reset or before a new song section, ensuring a clean slate.

---

### 4. **Live Looping and Performance Resampling**

- **Freeze** = instant buffer stutter, synchronized to the clock.
- **CV-control Freeze:** Patch dynamic gates from sequencers or logic to freeze for fills, transitions, or rhythmic slicing.
- **Resolution changes post-Freeze:** Dramatically alter rhythm for glitch breakdowns/ drops.

---

### 5. **Generative Arrangements**

- Use random/chaos CV generators (e.g., Wogglebug, Ornament & Crime, Turing Machine) to modulate Chroma, Dispersal, Feedback, or Resolution.
- Change delay modes or feedback types at musically meaningful points (with clocked logic, manual performance, or external events).

---

## Example Song Structure Using Nautilus

**Intro**
- Minimal voices, Nautilus in Fade/Normal feedback, single Sensor, no chroma.

**Build/Verse**
- Gradually increase Sensors and Dispersal for more echo complexity.
- Introduce Ping Pong/Cascade/Adrift feedback for stereo movement.
- Modulate Chroma/Depth for new harmonics/textures.

**Chorus**
- Engaged Freeze for rhythmic stutter on key hits.
- Chroma to Shimmer or De-Shimmer for pitch-lifted repeats.
- Bass lines and drums in parallel, relatively dry.

**Breakdown**
- Feedback/Reversal up, exploit infinite echo & reversing for ambient breakdown.
- Slowly Purge and reset.

**Outro**
- Return Feedback, Sensors, Dispersal to minimum, quiet wash to silence.

---

## Tips

- **Assign performance macros:** To morph multiple parameters for song sections.
- **Automate with CV:** Scene and section changes can be robotically precise or manually expressive.
- **Synchronize everything with master clock:** Ensures delay and freeze transitions lock to your arrangement.
- **Explore self-patching:** To extract new, generative melodies/structures from Nautilus’ internal logic.

---

## Conclusion

Nautilus is a performance instrument as much as an effect, capable of dividing, multiplying, and transforming your musical ideas across sections and full songs. Embrace its internal modulation, external patchability, and the creative re-sampling potential of its delay lines to keep any performance or composition varied, engaging, and narrative from the first second to the last.

---

**Manual:** [https://qubitelectronix.com/manuals/qu-bit_nautilus_manual.pdf](https://qubitelectronix.com/manuals/qu-bit_nautilus_manual.pdf)

**Generated With Eurorack Processor:**  
[https://github.com/nstarke/eurorack-processor](https://github.com/nstarke/eurorack-processor)