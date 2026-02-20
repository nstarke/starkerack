# Intellijel — Atlantix

- [Manual PDF](../../manuals/atlantix_manual_2024.09.12.pdf)

---

[Atlantix Manual PDF (2024.09.12)](https://intellijel.com/downloads/manuals/Atlantix_Manual_2024.09.12.pdf)

---

# Using the Intellijel Atlantix for Full-Length Songs in Eurorack

Creating a cohesive, evolving full-length song in modular synthesis—beyond simple loops or jams—requires careful patching, modulation, and planning. The **Intellijel Atlantix** (an analog dual-oscillator synthesizer voice with internal and external modulation depth) offers a powerful toolkit for this, but song-length structure emerges when Atlantix is thoughtfully combined with sequencers, modulation sources, utilities, and effects. Here's an analysis of how the Atlantix can anchor a complex composition, and tips for leveraging its features to arrange and animate full pieces.

---

## Challenges for Song-Length Structure in Eurorack

- **Repetition:** Modular synths excel at short loops/patterns. Songwriting needs section changes: intro, verse, chorus, bridge, breakdown.
- **Automation:** 'Set and forget' sounds static. Manual tweaking for minutes is exhausting.
- **Transitions & Variation:** You want dramatic changes, subtle evolution, and coordinated transitions across multiple voices.
- **Recallability:** How to perform/sequence a structure—hands-on live, or semi-automated?

---

## How Atlantix Supports Song Structure

### 1. **Multi-Source Synthesis in One Voice**

Atlantix is not a simple oscillator—it is a complete synth voice:  
- **VCO A / VCO B**: Dual oscillators with sync, FM (exp and thru-zero), PWM.
- **Flexible Mixer**: Pulse, saw, sub (-1, -2, OR), noise (white/pink), and two aux in, routable pre/post VCF.
- **VCF**: Multi-mode (LP/BP/HP/phaser; switchable poles), extensive modulation.
- **Envelope/VCA**: ADSR with rate ranges/drive, gated/organelle switching, manual gate.
- **MODs**: Internal sample & hold, multiroute LFO/S&H/noise/VCOB mix, normalled to VCO/FM and VCF FM.

### 2. **Built-in Modulation & Macro Controls**

- **Sample & Hold / Track & Hold**: Random or stepped modulation for generative movement.
- **Flexible MOD X/Y routing & inversion**: Multiply the modulation palette for evolving timbre.
- **PWM, Sync, FM, etc.**: Routable to almost any part of the voice—create self-patched feedback or modulation chaos.

### 3. **Expandable Outputs (ATLX Expander)**
- **Multiple outputs**: Tap all Osc shapes, ring mod, filter outs, etc.
- **Ring Modulator**: Add metallic, inharmonic timbres or percussive sounds.
  
---

## Songwriting Techniques with Atlantix

### 1. **Sectional Control with External Sequencers**

Use sequencers or voltage presets (like Intellijel Metropolix, Erica Black Sequencer, NerdSeq, or vector-based sequencers):
- Multitrack melodic/rhythmic lines: Sequence Atlantix pitch (1V/oct), triggers/gates, CV for filter or modulation depth.
- Program 'scenes' or 'pattern chains' for multisection arrangement (verse—chorus—breakdown, etc.).

*Patch Example*: Use a sequencer with multiple gate/CV tracks to:
  - Control Atlantix’s pitch and gate,
  - Automate the modulation sources/amount (via multiple CV ins or addressing MOD X/Y).

### 2. **Modulated Variation & EvoIution**
- Route S&H/T&H to FM, PWM, filter, envelope times for evolving or generative patches.
- Use MOD X/Y for slow/fast LFOs affecting timbre, panning (if patched out to stereo VCA), or even envelope times (via CV ins).
- Internally patch VIDA/B outputs (with AUX sends to VCA/filter directly or via expander) to create layered/complex voices.

*Patch Example*:  
- Use a slow random S&H from Atlantix MOD as ENV sustain or filter cutoff mod; use sequencer CV to alter which MOD X/Y source is chosen per section.

### 3. **Live Performance: Manual Transitions + External Utilities**
- Program macros: Use hands/on/off switches (filter pole, drive, sync type, envelope speed) for dramatic or subtle section transitions.
- Use sequential switches (e.g., Doepfer A-151, WMD Sequential Switch Matrix) or matrix mixers to route different Atlantix outputs or modulations per section, creating new combos.
- Manual Gate button: Immediate drops, accents—triggered by hand or patched to foot switch for performance.

### 4. **Layering/Polyphony with Expanders and Other Voices**
- Employ the ATLX expander’s extra outs to layer different timbres/oscillators for bass, lead, and pad lines.
- Pair Atlantix with drum modules and other voices; use multiple Atlantix outputs for stacked lines or cross-modulation for wide/epic textures.

### 5. **Coordinated Transitions with Utilities/Effects**
- Use voltage-controlled switches (e.g., Mutable Branches) to mute/unmute Atlantix lines.
- Patch Atlantix into effects (delays, reverbs, wavefolders) and sequence their bypass or CV parameters for scene-based changes.

---

## Example Patch Structure for a Full Song

1. **Intro**:  
   - Atlantix in LFO mode, VCO B running S&H noise, filter in PHZ mode, slow envelope, sparse notes manually triggered or sequenced.
2. **Verse**:  
    - Switch filter to LP4, up envelope speed, increase sub amount and noise for foundation groove; sequence main melody.
3. **Chorus**:  
    - Open filter, drive VCA, sync VCOs, automate FM index for brighter, harmonically rich sound; add reverb/delay send.
4. **Bridge/Breakdown**:  
    - Switch to HP filter, randomize pitch or filter with S&H, drop sub/noise, use ring mod out for percussive FX.
5. **Finale/Outro**:  
    - Slow envelope, crossfade OSC A/B, bring in phaser/FX, fade-out using VCA with long release.

Swap section transitions using sequencer patterns, switches, or by modulating routings/sliders by CV.

---

## Patch Utilities to Combine With Atlantix

- **Sequencers**: Complex multitrack and pattern-chaining capability
- **Voltage Preset/Address Modules**: Harvestman/Industrial Music Electronics, Malekko Voltage Block, Frap Tools USTA, etc.
- **Utility/LFO/Random Modules**: Mutable Stages, Pamela’s New Workout, Zadar, etc.
- **Attenuverter/Mixers**: For dynamic manual or CV control of modulation depths/routings.
- **Effect Processors**: Mimeophon, Magneto, FX Aid, Data Bender, for post-Atlantix drama.

---

## General Tips

- **Plan macro CV lanes**: Use a performance controller or sequencer to automate key parameters per song section (e.g., filter cutoff, MOD amount, ENV rate, AUX sources).
- **Self-patch Atlantix**: Exploit MOD outputs, internal S&H/random, and expander outs.
- **Scene/CV Preset Changers**: The more programmable control you have over Atlantix’s settings, the more “songlike” evolution you can achieve.
- **Manual Play + Automation**: Combine performance switches/sliders with pre-programmed CV for an organic but structured feel.

---

## Final Thoughts

**Atlantix** provides an exceptionally deep synthesis engine in a single module, and with intelligent patching and a focus on modulation routing—especially when paired with a structured sequencer, switches, and CV utilities—you can build not just beautiful loops, but entire songs with dynamic transitions, melodies, basslines, and evolving timbres.

**[Download the manual PDF](https://intellijel.com/downloads/manuals/Atlantix_Manual_2024.09.12.pdf) for detailed reference to all controls and patch points.**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)