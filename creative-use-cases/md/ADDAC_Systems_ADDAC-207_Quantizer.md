# ADDAC Systems — ADDAC-207 Quantizer

- [Manual PDF](../../manuals/ADDAC_207_Quantizer_REV05.pdf)

---

[ADDAC207 INTUITIVE QUANTIZER USER’S GUIDE PDF](https://www.addacsystem.com/sites/default/files/files/products/manuals/ADDAC207_MANUAL.pdf)

---

# Creative Uses for the ADDAC207 Intuitive Quantizer in Your Eurorack Setup

## 1. Chord Automation & Polyphonic Textures

**Combine with:**
- Multiple VCOs (ex: Mutable Instruments Plaits, Make Noise STO, Intellijel Dixie II+)

**Patch Idea:**
- Patch four independent VCOs to the four CV outputs of the ADDAC207. Use the NOTE 2/3/4 interval menu to set each output to intervals forming a custom chord (triads, 7ths, suspended/diminished, etc.). Quantize a single CV (from a sequencer, random source, or keyboard) and the module will generate harmonically-coherent chord outputs. Use independent gate outs to trigger different envelope stages for each voice for evolving polyphonic textures.

---

## 2. Algorithmic Harmonies With Sequenced Intervals

**Combine with:**
- Modulation sources (LFOs, Envelopes), Advanced sequencers (ALM Pamela’s New Workout, Make Noise René)

**Patch Idea:**
- Use CV modulation (LFO or random source) into the ASSIGN input, set to control NOTE 2/3/4 Intervals and Quantization type. Sequence or randomize these assignments, resulting in generative chords or harmonies that continuously drift and refreshtheir internal interval structure. This works especially well in generative ambient or experimental contexts.

---

## 3. Advanced Trigger & Gate Manipulation

**Combine with:**
- Trigger/gate sequencers (Malekko Varigate 4+, Tiptop Audio Circadian Rhythms), Envelope generators (Intellijel Quadra, Maths)

**Patch Idea:**
- Use the independent GATE IN for each channel to define when quantization should occur—this enables polyphonic arpeggios with complex or offbeat gate patterns. Each voice’s quantized note change is “permitted” only when a gate/trigger happens, allowing for polyrhythmic, structured, or randomized note patterning from a single CV sequence.

---

## 4. Keyboard/Performance Interface for Live Playing

**Combine with:**
- External CV keyboard interface (Arturia Keystep, Doepfer A-190 series), Manual gate sources, Sensors

**Patch Idea:**
- Use Keyboard Mode for monophonic playing with static chords assigned to the other three voices. While performing the melody from a keyboard, the additional voices fill in harmonies based on preselected intervals and quantized to scale, creating a “one-finger-chord” instant harmony mechanism for live improvisation.

---

## 5. Microtonal & Non-Western Tuning Experiments

**Combine with:**
- Oscillators with wide tuning range & fine adjustment, microtonal sequencers (Zetaohm FLXS1, Tiptop Audio Microtonal tuning cards for Quantizer modules)

**Patch Idea:**
- Engage the tuning fine adjustment and alternate temperaments (Pure, Bohlen-Pierce, Just, Exotic). Use the fine-tune menu (Ex. VII), and assign odd interval patterns, then integrate with microtonal sequences or random CV to explore Bohlen-Pierce or Just Intonation in generative or drone patches. The ADDAC207's microtonal support makes it ideal for exploring "non-standard" musical systems and creating unique sonic worlds.
- For even deeper results, mix this with complex function generators (e.g., Make Noise Maths) for evolving modulation in microtonal space.

---

## 6. Evolving Harmonic Modulations With External CV

**Combine with:**
- Voltage-controlled sequencers (Analog Solutions Generator, Malekko Voltage Block), CV-mappable effects (mutable instruments Rings, Clouds)

**Patch Idea:**
- Use the ASSIGN CV Input to switch between scales, transpose keys, or automate preset changes in real time. Animate the scale or root note via modulation, so an evolving bassline or melody always conforms emphatically to a dynamically shifting harmonic structure – think modal jazz on autopilot.

---

## 7. Dual Standard Integration: Moog/Buchla Conversion

**Combine with:**
- Buchla-format modules, CV scalers/converters (Tiptop Audio/Buchla 200 series, Synovatron CV Tools)

**Patch Idea:**
- Switch between Moog 1V/oct and Buchla 1.2V/oct using the quantizer’s menu. This can bridge disparate systems or allow you to use Buchla and Moog-style gear in the same patch, offering a consistent interface for melody and harmony across your studio.

---

## 8. Intelligent Randomization & Algorithmic Music

**Combine with:**
- Random/chaos modules (Mutable Instruments Marbles, Verbos Random Sampling, SSF Ultra-Random Analog)

**Patch Idea:**
- Feed random voltages (smooth or stepped) into the quantizer input, perhaps with unique scale/preset/temperament selections per channel. Use the GATE L condition and trigger repeat to control how frequently new notes are quantized, resulting in controlled generative melodic material—useful for ambient, scoring, or evolving soundscapes.

---

## 9. Preset Morphing and Live Set "Scenes"

**Combine with:**
- Multichannel performance controllers (Expert Sleepers ES-8/9 via Max/MSP/VCV Rack, MIDI-to-CV converters)

**Patch Idea:**
- Use the PRESETS menu along with assigned CV preset switching to instantly recall new “scenes” of scale, tuning, and quantization settings in a performance—morphing from one musical context to another live. Assign preset changes to an LFO or a performance controller for dramatic harmonic changes, or to accompany visual/multimedia cues in an AV set.

---

## 10. Layered Multi-Sourcing

**Combine with:**
- Multiple independent modulation sources (manual controllers, sequencers, random, LFOs)

**Patch Idea:**
- Patch four different CV sources (e.g., sequencer, random, envelope follower, pedal) to the four quantizer inputs, each set to different intervals, scales, or tunings—inventing “virtual instruments” that interlock and harmonize in real-time, producing intricate harmonic counterpoint.

---

## Bonus: Detailed Scale Control for Physical Modeling & Resonator Modules

**Combine with:**
- Modules like Mutable Instruments Rings, Intellijel Plonk, 2hp Bell

**Patch Idea:**
- Use highly specific or microtonal scales in the ADDAC207 to feed a melodic or harmonic source into a resonator or physical modeling voice—yielding unique bell, percussion, or modal string harmonics not attainable with standard quantizers.

---

For additional patching techniques, refer to the full [ADDAC207 Manual PDF](https://www.addacsystem.com/sites/default/files/files/products/manuals/ADDAC207_MANUAL.pdf).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)