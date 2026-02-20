# Black Noise — Cosmos

- [Manual PDF](../../manuals/BLACK-NOISE_COSMOS_User-Manual_V1.pdf)

---

[**Download the COSMOS User Manual (PDF)**](https://blacknoisemodular.com/BLACKNOISE_COSMOS_USER_MANUAL_V1.0.pdf)

---

# How to Use the Black Noise COSMOS to Create Full-Length Eurorack Songs

Creating a compelling full-length song in eurorack modular synthesis isn’t just about cool sounds—it’s about structure, flow, and the ability to manipulate your arrangement in a performative, expressive way. The [Black Noise COSMOS](https://blacknoisemodular.com/cosmos) module is unique: it's a 100% analog, logic and analog processor with deep utility as a "computer for your rack." Below I'll explain how you can leverage COSMOS, in combination with other modules, to turn jams into real performances and songs with evolving sections, transitions, and expressive nuances.

---

## COSMOS: The Overview

COSMOS combines logic, mixing, analog processing, touch control, and more—enabling you to:

- Generate/modify gates, triggers, CVs, and audio signals  
- Patch performative controls with touchpads  
- Process audio or CV in extremely flexible ways (AND/OR/XOR/NAND logic, envelope following, comparators, wave folding, half & full wave rectification, probabilistic gates, etc)

---

## Song Creation Strategies with COSMOS

### 1. **Evolving Song Sections: Logic-Based Transitions**

**Problem:** One patch can sound great but gets repetitive without structured changes.  
**Solution with COSMOS:** Use COSMOS's extensive logic and gate processing to create sections, transitions, and automations.

#### **Practical Approaches:**
- **Probabilistic Gate Routing:**  
  Use "Random Gates" (page 35) to randomly switch between drum sequences or melodic lines, creating fills, drops, or scene changes.
- **Logic Switches:**  
  Use combinations of AND, OR, XOR gates to activate or mute certain voices/effects (e.g., mute bassline while bringing in pads).  
- **Envelope/Gate Combiners:**  
  Merge envelopes with "Envelope Combiner" (page 33) for evolving shapes—great for transitioning from verse to chorus.

#### **Example Patch Idea:**
- Use the XOR logic to switch between melodic and percussive sequences based on another module’s gate or clock pattern:  
  - XOR Output: Triggers synth voice in chorus.
  - NAND Output: Triggers kick drum in verse.
  - Use touch pads for live gating/muting.

---

### 2. **Live Performance Automation & Expressiveness**

**Problem:** Static patches lack human/expressive feel.  
**Solution with COSMOS:** Utilize touchplates and complex comparator logic for hands-on dynamics.

#### **Approaches:**
- **Touch Pads:** Instant performative gate/CV for fills, drops, on-the-fly mutes, or filter sweeps.
- **Window Comparator:** Use window comparators to only allow modulation or melody at certain voltages (e.g., only allow high melody when a big pad is present).
- **Dynamic Rhythm:** Use "Clock Multiplier with Swing" (page 36) to introduce/off-beat swing or double triggers at different song sections.

---

### 3. **Song Structure Through Self-Generation and Feedback**

**Problem:** How to create bridges, breakdowns, or "build" sections.  
**COSMOS Solution:**  
- **Self-Oscillation and Feedback:** Use the oscillator example (page 24)—feedback XNOR to input, and modulate slew/LPF for evolving timbre or rhythm generators that change over time.
- **Phase-Locked Loop (PLL):** Create inter-locking rhythms or melodies that track each other, perfect for call-and-response or dynamic interplay between voices/instruments.

---

### 4. **Automated Fills, Drops, and Surprise Elements**

- **Envelope Follower (page 34):**  
  Extract CV from percussion or vocals to automatically trigger changes in other modules—auto sidechaining, or dynamic EQ sweeps during loud sections.
- **Random Gates:**  
  Route clock into "Random Gates" to trigger randomized fills or sample changes—make every repeat unique.

---

### 5. **Mixing, Distortion, and Final Touches**

- **Clamping VCA / Ring Modulation:**  
  Add dynamic audio processing (pumping, saturation, wave-shaping) that changes in different sections of the song using CV control.
- **Audio Rectification:**  
  Use half/full-wave rectification to send audio-derived modulation to other modules for subtle or dramatic transitions.

---

## Example: Song Structure Using COSMOS

| Section         | Function                                           | Patch Suggestion                                                    |
|-----------------|----------------------------------------------------|---------------------------------------------------------------------|
| **Intro**       | Gentle pad, melody, sparse drums                   | Use AND gate to only let pads through when touchpad is pressed      |
| **Build**       | Rhythms become more complex, snare fills appear    | Use clock multiplier and XOR logic to introduce extra hits          |
| **Drop**        | Main bass drops, drums loud                        | Comparator to open up VCA for full amplitude during key trigger     |
| **Breakdown**   | Drums mute, melody evolves                         | Touch pads mute drums (gate logic), envelope combiner for melody    |
| **Climax**      | Everything full, complex rhythm                    | All gates unmuted, random gates inject fills, phase-locked loop adds harmonics |
| **Outro**       | Fade out, sounds slowly die                        | Use slew/offset to gradually drop gate lengths and amplitude        |

---

## What You’ll Need With COSMOS

- **Sequencers, LFOs, random sources** – for driving logic and CV
- **Envelope generators** – for shaping dynamics and timing
- **VCA, mixers, slews/attenuverters** – for building control paths as in patch suggestions
- **Sampler/Looper, drum modules, effects** – for sonic variety

---

## Final Thoughts

COSMOS is a musical "hub" that allows you to orchestrate, arrange, and perform modular patches as living, evolving songs—rather than static jams. By patching logic gates, comparators, and its touch interface into the wider system, you gain tools to create structure, automate transitions, and keep listeners engaged over longer timescales. Use its logic and analog processing to "compose" in real time—bridging the gap between interesting patch and finished track.

---

[**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)
