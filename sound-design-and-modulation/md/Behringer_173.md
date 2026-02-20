# Behringer — 173

- [Manual PDF](../../manuals/QSG_BE_0720-AAL_173 QUAD GATE-MULTIPLES_WW.pdf)

---

[Behringer 173 Quad Gate/Multiples - Official Manual (PDF)](https://mediadl.musictribe.com/media/PLM/data/docs/P0DZZ/173_QUAD_GATE_MULTIPLES_QSG_WW.pdf)

---

# Creative Sound Design with the Behringer 173 Quad Gate/Multiples

As a modular synth artist, the Behringer System 100 173 Quad Gate/Multiples module offers simple logic utility functions, but with a little creativity, you can make it a surprising powerhouse for wild modulation, percussive destruction, and spatial textures. Though the module itself doesn’t generate audio, its ability to process, route, and modify gates and control voltages makes it an essential ingredient for shaping dynamic, complex, and *unique* modular sounds.

Let’s break down how you can exploit the 173 for the styles you mentioned.

---

## Module Overview

- **Quad Gate**: Four independent gate processors, each with non-inverting (active high) and inverting (active low) CV inputs. Think of these as fast, voltage-controlled switches.
- **Multiples**: Six groups of four jacks (A–D) each, distributing a signal plugged into any "A" jack to the corresponding B, C, D jacks (passively).

---

## 1. Distorted Percussive Sounds

### Patch Concept:
*Chop, invert, and layer gates to trigger and process drum modules (or distortion FX) in unusual rhythmic ways.*

**Patch Example:**
- **Gate Generation**: Send a drum sequencer or random gate generator to GATE IN 1.
- **Gate Processing**:
  - Feed an LFO or envelope to GATE CV (non-inverting) of Gate 1. This allows the gate to "open" only when the CV is high—creating rhythmic skipping or syncopation.
- **Distorted Layering**:
  - Mult the processed gate using the multiples (Plug processed Gate OUT into A1, take B1, C1, D1 out to trigger different drum modules or distortion effect gates simultaneously).
  - Take inverted gates (using inverting GATE CV inputs on another channel) and use them to trigger bursts, glitch modules, or open/close distortion pedals at unpredictable times.
- **Advanced:**
  - Route acoustic percussion sounds through an envelope follower, then use its output as GATE CV—you’ll "gate" new sounds with the *articulation* of the acoustic drum.

**Result:** Chopped rhythms, polymetric trigger patterns, and gated distortion—great for mangled percussive sounds.

---

## 2. Aggressive, Wobbling Basslines (Dubstep/Drum & Bass)

### Patch Concept:
*Use the Quad Gate to rhythmically chop or duck basslines, and the Multiples to create multiple simultaneous modulations.*

**Patch Example:**
- **Wobble Sync**:
  - Patch a bass VCO or filtered oscillator to your audio mixer.
  - Run a rhythmic gate pattern (from sequencer or manually clocked gate generator) into GATE IN 2.
  - Feed a sync’d LFO or envelope to GATE CV; this controls when the bass is "open."
- **Gate as Mod Source**:
  - Send GATE OUT 2 to a VCA implementing sidechain ducking (classic DnB/Dubstep pump).
  - Alternatively, mult the gate to trigger rapid filter cutoff modulation or to gate distortion units only during certain rhythmic points.
- **Multiples for Parallelism**:
  - Plug one lively CV/LFO into A2. Spread the same LFO to multiple filter or effect modules in parallel, sync’ing several components for evolving timbre.

**Result:** Chopped/pumping basslines with pronounced, rhythmic "ducks" and wobbling architecture, evolving alongside your groove.

---

## 3. Haunting, Atmospheric Pads

### Patch Concept:
*Gating slow-moving envelopes, spreading eco-LFOs everywhere, introducing jittering drone cut-ups.*

**Patch Example:**
- **Chopped Textures**:
  - Send an evolving drone or pad (output from an oscillator-bank, granular, etc.) into a VCA.
  - Use a slow random gate from Quad Gate (GATE IN driven by a random rhythm, GATE CV shaped by another envelope/LFO) to open/close the VCA—ghostly, pulsing pads.
- **Distributed Modulation**:
  - Plug a complex, cyclical LFO into a multiples group (A3), and route B3, C3, D3 to slightly detune filters, reverbs, or phase shifters—slow movement makes the pad shimmer and swirl.
- **Inverted Gating**:
  - Use inverting GATE CV to selectively *close* something (like a high-cut EQ) only at specific moments, creating breathing "holes" in your pad’s spectral range.

**Result:** Evolving, haunted ambiences that pulse and sweep with life, gate controlled for extra unpredictability.

---

## Tips & Advanced Tricks

- **Create Polyrhythms:** Use separate channels of the Quad Gate for different time signatures or divisions. Mult and cross-patch gates to create evolving polyrhythmic textures.
- **CV Feedback Loops:** Mult a gate out back into a CV input (with attenuation/offset) for unpredictable gate bursts or "chaos" patterns.
- **Logic-Like Use:** Combine multiple gates in Mults and sum/OR them with external logic, for complex rhythmic patterns (great for IDM/experimental).
- **Distortion Control:** Gate the power or enable/disable function of a distortion/fuzz effect using wild gate/CV combos for glitchy, destructive artifacts.

---

## Extra Resources

- Official manual (multi-language): [PDF here](https://mediadl.musictribe.com/media/PLM/data/docs/P0DZZ/173_QUAD_GATE_MULTIPLES_QSG_WW.pdf)
- For more patching ideas and tools: [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---