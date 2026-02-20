# Doepfer — A-138B

- [Manual PDF](../../manuals/A138_man.pdf)

---

[Doepfer A-138 Mixer Manual (PDF)](https://doepfer.de/a100man/A138_Manual.pdf)

---

# Doepfer A-138 Mixer - Strategies for Song Structure in Eurorack

The **Doepfer A-138 Mixer** (System A-100) is a simple but powerful 4-channel mixer for both audio and control voltage (CV) signals. While not inherently "musical" on its own, it can become a secret weapon in turning basic Eurorack patches into full-length, evolving songs when creatively patched with other modules.

Below, I’ll outline approaches for song structuring, modulation, and live performance using the A-138 Mixer in synergy with other modules.

---

## Key Features

- **4 Inputs with Attenuators** for blending audio/CV sources
- **Master Output Attenuator** for the final signal level
- **Linear (A-138a) / Logarithmic (A-138b) Response** for CV or audio mixing
- **Optional Offset Generator** on input 1 (apply DC offset when no plug is inserted)

---

## Creative Uses for Songbuilding

### 1. Dynamic Song Part Switching

- **Send Parts to Mixer Channels:** Patch different "parts" of your patch (for example: drum loop, bassline, melody, drone, FX) into the mixer’s inputs.
- **Manual or Automated Fades:** Use the A-138’s channel attenuators to bring voices in and out. For live sets, manually ride the faders. For more automation, send CV-controlled VCAs (pre-mixer) to enable, fade, or mute parts in sync with your song.
- **Master Volume/FX Send:** Use the master output attenuator to control the entire mix, or mult the signal for parallel processing (e.g. dry + reverb).

### 2. Morphing and Layering Textures

- **Layer Subtle Transitions:** Crossfade between two scenes (e.g. mixing between two drum patterns, bass styles, or melodic textures).
- **Interpolation:** Send CV/automation to the channels before the mixer for hands-free transitions.

### 3. CV Mixing for Macro Control

- **Macro Performance:** Use the module in linear (A-138a) mode to sum together different voltage sources (LFOs, envelopes, manual offsets, sequencer outputs). Send this macro CV to filter cutoff, oscillator pitch, etc., allowing you to control multiple parameters with a "composed" macro-lane— essential for verse/chorus breakdowns.

#### Example:
- Input 1: Slow LFO for movement
- Input 2: Step sequencer for melodic change
- Input 3: Manual offset for live tweaking
- Input 4: Envelope for section transitions

Summed CV out modulates filter cutoff, shaping your sound in evolving blocks corresponding to song sections.

### 4. Automated and Performed Transitions

- **Automate with Sequencers/Clocked Modulation:** Use clock dividers and sequential switches to route different pattern sources through the mixer inputs for song sections (intro, verse, fill, etc).
- **Offset for Section Jumps:** Use the offset feature to nudge a mod destination for distinct changes (e.g. instantly open up reverb or filter for a chorus).

### 5. Mute Groups and Quick Breakdowns

- Use A-138 as a mute hub: Patch several voices/drums through, leave attenuator at zero on unused channels for instant drop-outs— bring back for breakdowns/drops/returns.

---

## Example Patch for Song Structure

**Goal:** Evolving techno track with intro, breakdown, drop, and outro

- IN 1: Kick and bass (routed through pre-VCA for sidechain)
- IN 2: Percussion loop
- IN 3: Melodic sequence (sample & hold or quantized LFO)
- IN 4: Noise/FX (for risers and transitions)

**Master Out:** Goes to main mixer or audio interface

### Song Structure Workflow

1. **Intro:** Start with attenuator 4 (FX) and 3 (melody) up; Percussion and Bass down.
2. **Bring in Percussion:** Fade up IN 2 for energy build.
3. **Drop Kick/Bass:** Fade IN 1 up on the drop.
4. **Breakdown:** Fade bass/percussion down, ramp up FX riser (IN 4).
5. **Chorus:** All channels up or swap melodies via patch cables or external switches.

_Add sequenced VCAs or switch modules for automation, or perform these transitions by hand for a live feel._

---

## Tips for "Songifying" Eurorack Patches

- **Preset Morphing:** Use several mixers for A/B/C "states," crossfade sections for sonic development.
- **External Modulation Sources:** Patch gates/triggers/sequences to CV addressable switches pre-mixer to automate muting and transitions.
- **Manual Control:** Keep channel attenuators at hand for expressive mixing—like a mini performance console.

---

For further reading, download the official [Doepfer A-138 Manual (PDF)](https://doepfer.de/a100man/A138_Manual.pdf).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
