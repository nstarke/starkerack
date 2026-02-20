# 2hp — Swarm

- [Manual PDF](../../manuals/2hp_Swarm_v1-0.pdf)

---

[2hp Swarm Manual PDF](https://www.twohp.com/_files/ugd/2b1d4a_3b100b48ed674d5abf5f0475a9595030.pdf)

---

## Using the 2hp Swarm in Full-Length Eurorack Song Composition

The **2hp Swarm** is a “Hyper Oscillator” module designed to deliver swarming super-saws or thick, detuned pulse waves, providing a dense, evolving oscillator bank (up to 88 oscillators). While Swarm excels at creating rich, alive textures, it can feel challenging to move from amazing “moments” to constructing full-length, dynamic songs. Let's break down how to leverage Swarm, in tandem with thoughtfully-chosen modules, to achieve evolving, structured tracks like those heard in electronic music genres such as trance, ambient, synthwave, IDM, techno, or even experimental pop.

---

### Key Features for Song Composition

- **Massive Unison Textures**: Up to 88 detuned oscillators for chords, leads, supersaws, pads.
- **Waveform Switching**: Saw and Pulse timbres for timbral evolution.
- **Manual and CV Control**: Dynamic control over number of voices and detune amount, opening up morphing, evolving textures.
- **Compact Size (2HP)**: Leaves space for companion modules to shape, process, and sequence the sound.

---

## Strategies for Full-Song Composition

### 1. **Evolving Pads, Leads & Chord Progressions**

- **Macro Melodic Movement**: Use sequencers (e.g., [Intellijel Metropolix](https://intellijel.com/shop/eurorack/metropolix/) or [Make Noise Rene](https://www.makenoisemusic.com/modules/rene)) to send changing pitch CV into Swarm’s 1V/Oct input for your chord/bass/lead lines. Add analog or digital effects (e.g., delay, reverb) downstream for atmosphere.
- **Timbral Automation**: Automate the *Voices* and *Detune* knobs (using LFOs, stepped random, or automation lanes from a DAW via CV-to-MIDI modules) to move from mono leads to thick evolving pads. For a song intro, start with a single oscillator and gradually increase Voices and Detune for a “riser” or breakdown/buildup.
- **Waveform Variation**: Toggle between saw and pulse mid-song to add interest: e.g., use saw for the chorus/peak, pulse for verse/bridge.

### 2. **Rhythmic & Structural Variation**

- **Dynamic Filtering**: Pair with a filter module (e.g., 2hp MMF). Use multistage envelopes, VCAs, or sequenced modulation to open/close the filter for drops, swells, or transitions. Automation can help segment the song into intro, build, breakdown, drop, outro.
- **VCA Automation**: Use EG and VCA to sculpt the amplitude envelope of Swarm's output. Automate gating for rhythmic stabs, tremolos, or sidechain-like effects, or even silence for transitions/breaks.
- **Chopped Melodies/Basslines**: Run Swarm through a VCA modulated by a clocked envelope, trigger sequencer, or manual gates to chop the output into rhythmic pulses, evolving the song’s “groove” over time.

### 3. **Layering & Texture Morphing**

- **Stacking Voices**: With multitracking or multiple Swarms/oscillators, layer different settings (e.g., slow-evolving pad, tight, quick lead, noisy detuned effect) and fade them in/out across the song sections.
- **External Modulation**: Modulate Swarm's *Detune* or *Voices* with slow LFOs for evolving textures, or with stepped voltages for glitchy transitions.
- **Lo-Fi Degradation**: Pairing with [2hp Lo-Fi](https://www.twohp.com/modules/lofi) can decimate, bit-crush, or filter the supersaw, ideal for breakdowns, contrast sections, or experimental parts.

### 4. **Synchronization & Song Form**

- **Sequence and Gate Control**: Use clock dividers/multipliers to segment control (e.g., during a verse, keep Swarm subtle; bring in detuned mayhem at the drop). Song progressions can be mapped by scene in sequencers, or via performance switching.
- **Manual Performance**: Perform live tweaks on *Voices*, *Detune*, *Waveform*, or filter cutoff to “play the arrangement” of the song.
- **CV Scene Recall**: Advanced setups using preset selectors (like Select 2, or programmable switches) allow instant reconfiguration during a song, emulating verse-chorus-bridge structures.

### 5. **Other Techniques & Tips**

- **Evolving Drones**: Very slow modulation of *Detune* and *Voices* creates huge, morphing drones for ambient or cinematic passages.
- **SuperSaw Basslines**: Use Swarm with only a few oscillators and heavy detune to make moving, alive basslines and morph them into gigantic supersaw drops.
- **Polyrhythmic Textures**: Use clocked modulation or stepped random to introduce unexpected movement, keeping longer songs from feeling static.

---

## Example Patch Ideas

1. **Intro-Build-Drop Arrangement**  
  - *Intro*: Single voice, low detune, saw up high-pass filter, minimal decay.
  - *Build*: Gradually increase Voices, Detune, and filter resonance. Add LFO motion on Detune for intensity.
  - *Drop*: Max Voices, max Detune, sustain envelope, filter open, punchy rhythm via VCA gating.

2. **Ambient/Evolving Pad**  
  - *Swarm*: Many voices, gentle detune, slow modulation on Detune CV from LFO.  
  - *Filter*: MMF set to lowpass, modulated cutoff.  
  - *VCA*: EG in slow attack/sustain mode, automated via sequencer or performed manually.

---

## Conclusion

The **2hp Swarm**, when combined with dynamic modulation, filtering, and amplitude shaping, excels as a “centerpiece” oscillator for modern, evolving song structures. By approaching arrangement as a process of morphing, filtering, chopping, and modulating the Swarm’s output, you can transform great-sounding riffs into rich, full-length performances. Its strengths come alive when its controls are automated or performed—make those super-saws dance with modulation and sequencing!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)