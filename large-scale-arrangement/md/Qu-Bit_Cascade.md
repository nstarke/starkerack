# Qu-Bit — Cascade

- [Manual PDF](../../manuals/Getting_Started_Cascade.pdf)

---

[Download the Cascade Manual PDF from Qu-Bit Electronix](https://www.qubitelectronix.com/_files/ugd/9efceb_16fa4f39eed349bbb880ceecd1d9842a.pdf)

---

# Using Qu-Bit Cascade to Create Full Length Songs in Eurorack

## Introduction

Turning cool patches into full songs is a classic challenge in modular. The [Qu-Bit Cascade](https://www.qubitelectronix.com/shop/cascade) is designed as a multi-function envelope generator, analog VCA, compressor, envelope follower, ratcheter, and even a basic sound source. Its depth opens a lot of possibilities for macro-musical ideas—arrangement, transitions, evolving parts, and dynamic changes—beyond just raw grooves.

Below is a guide to using Cascade in context, focused on techniques for song-length structure and interest.

---

## Cascade Capabilities, Recap

- **Multi-mode Envelope:** AD, ASR, ADSR, Ratcheting
- **VCA:** Internal 2164-based, high-fidelity
- **Internal Sound Sources:** White noise, 808 kick/hat, hi-frequency sine
- **Compressor/Envelope Follower:** Animation for dynamics and sidechain
- **Edit Functions:** Advanced control over gate modes and gravity (parameter evolution)

---

## Key Techniques for Song Arrangement

### 1. Macro Control & Dynamic Transitions

**How:**  
Use your sequencer, clock controller, or a dedicated modulation source to select Cascade modes and settings at different song sections.

- **Intro:** Start with compressed noise or sine drones using internal sound sources. Use the envelope follower to respond to other signals (e.g., a slow evolving pad or a field recording).
- **Drop:** Switch to ratcheting AD mode for rapid-fire percussive elements (snare rolls, hi-hat trills).
- **Breakdown:** Use the amplitude and time gravity settings to create evolving, decaying, or "bouncy" envelopes for more organic motion.
- **Outro:** Slowly extend attack/release for longer, swelling envelopes as the song fades.

**Practical Patch Example:**
- **Sequencer → Control Voltage → Mode or Decay**
- **LFO → Repeats/Input for evolving ratchets**
- **Manual/Remote Switching for live transitions**

### 2. Dynamic Envelope Automation

**How:**  
Cascade's CV controllable attack, decay, and repeats parameters mean a slowly changing voltage can morph the feel of your entire sequence.

- Use an LFO, random source, or macro controller to automate envelope stages for sections of your track (tight drums on verse, looser, larger on chorus, etc).
- Use the Mode and Curve to morph between exponential, linear, and log articulation per section for strong musical contrasts.

### 3. Polyphonic/Layers Control

**How:**  
Cascade’s envelope can be duplicated/multed and routed to layers—bass, lead, percussion.

- Use the Gate Output in "EOD" or "EOA" mode to coordinate other voices (e.g., a pad that swells while drums are in ratchet mode).
- Let Cascade function as a rhythmic modulator for multiple VCAs elsewhere, creating evolving grooves and fills synced to the song's section.

### 4. Sidechain Compression & Pumping Effects

**How:**  
The Compressor mode with virtual side chain works fantastically for arranging the "space" in your track—ducking elements out when a kick hits, for example.

- Route kick triggers (or simulated ones from Cascade’s own internals) to drive compression elsewhere.
- Use Envelope Out to modulate reverb send/return or filter cutoff for more animated, musical sidechaining.

### 5. Evolving Textures and Sound Source Layering

**How:**  
Leverage internal sources as beds or transitions—white noise swells, sine risers, percussive kicks for fills.

- Animate sound source selection throughout track (per section).
- Modulate sound source parameters (level, curve, gravity) for builds and breakdowns.

---

## Example Song Structure with Cascade

| Section   | Cascade Role                    | Modulated By                      | Other Modules                                  |
|-----------|---------------------------------|-----------------------------------|------------------------------------------------|
| Intro     | Envelope Follower, Noise Drone  | Slow LFO → Decay                  | Sample player, Reverb, Field Recorder          |
| Verse     | Classic AD Envelope, Sidechain  | Sequencer gates, CV to release    | Drum Module, Bass Voice                        |
| Pre-Chorus| Ratchet/Repeat Mode             | LFO/random on repeats             | Sequencer, Mixer, Filter                       |
| Chorus    | ADSR for thick pads/leads       | Macro CV to sustain/level         | Poly Synth Voice, VCA, Effects Loop            |
| Drop      | Compressor, EOD gate            | Kick trigger to compressor        | Bass, Lead, Effects, Clock Divider             |
| Bridge    | Gravity/Curve modulation        | Random voltage source             | Effects, Slicer/Looper                         |
| Outro     | Long envelopes, inverted mode   | Manual control / CV fade          | Sampler, FX Delay/Reverb                       |

### Patch Notes:
- **Envelope Out to multiple VCAs:** Animate several voices/drums at once.
- **Switching Modes Live:** Use Select Bus, MIDI, or manual for scene changes.
- **Gate Output in Edit Modes:** Sync fills, transitions, or FX events to envelope stages.

---

## Tips to Avoid "Loopitis"

- **Automate Everything:** Push controls and CV to evolve timbres and envelopes. Cascade’s gravity and repeats are great for slow, structural changes.
- **Use Gate Outputs Musically:** Drive FX, transitions, or trigger events elsewhere.
- **Layer Envelope Types:** Not just AD on drums, but also on textures, FX, and modulating parameters elsewhere (filters, wavefolders, etc).

---

## Final Thought

Cascade isn’t just a utility—it’s a performance and arrangement tool. When you treat envelope shape, amplitude, and groove as the heart of your composition, you can easily move from a static patch to a living, full-length musical performance.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
