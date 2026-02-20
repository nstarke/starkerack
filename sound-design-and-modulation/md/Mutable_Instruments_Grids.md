# Mutable Instruments — Grids

- [Manual PDF](../../manuals/Manual - Mutable Instruments Grids Documentation.pdf)

---

[Link to Grids Manual PDF](https://mutable-instruments.net/modules/grids/manual.pdf)

---

# Creative Modulation Techniques for Mutable Instruments Grids

As a eurorack modular synthesist, you can leverage Grids’ powerful pattern generation—and extensive CV (control voltage) modulation options—to go far beyond standard drum beats. Here’s how to coax distorted percussion, neurofunk bass, and eerie pads from your system using Grids as a rhythmic brain. Below, I’ll outline patching strategies and modulation tips, focusing on your stated goals.

---

## Grids Inputs—Your Modulation Targets

- **MAP X & MAP Y**: Morphs between pre-learned drum skeletons. Great for evolving, hybrid patterns.
- **FILL 1/2/3**: Control the complexity/sparseness of each percussion voice.
- **CHAOS**: Randomizes density, adds rolls/ghost notes.
- **CLOCK**: Feed unusual timing sources for evolving rhythms.
- **RESET**: Can force resets for chopped or repeating patterns.

All (except RESET, which is a trigger) can be voltage controlled (0 to +5V). Map X/Y/FILL/CHAOS also sum their knob and CV values.

---

## 1. **Distorted Percussive Sounds**

### Patch Idea: Gritty Industrial Groove

1. **Patch Grids' BD, SD, or HH triggers** into modules like wavefolders, distortion FX, or aggressive VCAs rather than vanilla drum modules.
2. **Modulate MAP X/Y** with random or sequenced LFOs to continuously morph basic drum skeletons—great for never-repeating rhythms.
3. **Modulate FILL CVs** (E1/E2/E3) with stepped random voltages or synced LFOs for shifting density. This creates rhythmic textures, syncopation, and chaotic fills.
4. **Crank CHAOS** with another LFO or a noise source—more random rolls and accents, perfect for breakcore or weird IDM beats.
5. **Apply Feedback/Distortion** (external modules): Mult a trigger output and use it to retrigger envelopes on an overdriven wavefolder or characterful filter.
6. **Use Gates Instead of Triggers**: Enable gate mode (see Options) and patch into VCAs with slow attack for slappy, pseudo-acoustic hits. Play with gate lengths via funky clock sources.

**Pro Tip:** Patch the ACCENT outputs into drum modules with accent or velocity inputs, or use them as envelopes for distortion amount!

---

## 2. **Crazy Basslines (Dubstep, DnB, Neuro, etc.)**

### Patch Idea: Rhythmic Bass Mayhem

1. **Assign a Grids Channel** (e.g. BD channel) to trigger a complex bassline synth voice—patch into the envelope or VCA that gates your bass.
2. **Feed MAP X/Y** with slow random modulation (Sample & Hold, chaotic LFOs, or even sequencer CV lanes) to create non-repetitive pattern morphs. This leads to evolving note rhythms.
3. **Modulate FILL** channels with fast synced LFOs or envelopes. More fill = more bass notes—awesome for sudden “rattles” and switch-ups.
4. **Clocking Tricks**:
   - **Unusual clock division/multiplication**: Use a clock divider/multiplier before Grids to create polyrhythms.
   - **Feed an audio-rate oscillator into the clock input**: This will generate glitched, audio-frequency rhythms for growly bass textures (especially with heavy processing downstream).
5. **CHAOS to Max**: Extreme randomness causes trap-like rolls and neuro-funk stutters.
6. **Accent Out to Bass Modulator**: Patch an accent output to the filter cutoff or wavefolder depth of your bass voice for nerve-jangling motion.

---

## 3. **Haunting, Evolving Atmospheric Pads**

### Patch Idea: Ghostly Grids Ambience

1. **Use Grids as a spatial texture generator** rather than a beat machine.
2. **Patch all three trigger outputs to envelope generators**, then to separate VCA-processed spectral drones or long-decay synth voices.
3. **Feed slow LFOs, joysticks, or aftertouch** into MAP X/Y for evolving, crossfaded, semi-predictable complexity.
4. **Set low density on the FILL knobs**; modulate them slowly to allow pads or ambient hits to swim in and out of the texture.
5. **Activate SWING**: For off-kilter, more ‘human’ ghost rhythms—when using the internal clock.
6. **CHAOS as a Texture Control**: Add a little for subtle, organic unpredictability.
7. **Accent Outs to Reverb/Delay Sends**: Patch accent triggers to gate smooth reverbs, spectral delays, or tape echo inputs to shadow only important transient events.

---

## Bonus Tips

- **External Audio as Clock**: Sync Grids to incoming audio—complex, reactive rhythms.
- **Voltage Controlled Option Tweaks**: Use the option settings (e.g., switch to Euclidean mode) for algorithmic, pattern-based rhythmic layering.
- **Combine with Logic and Switches**: Merge Grids outputs with other clock/logic modules to further mess with timing and trigger routing.
- **Manual Performance**: Ride the FILL and CHAOS knobs in real-time for wild live manipulation.

---

### [Grids Manual (Official PDF)](https://mutable-instruments.net/modules/grids/manual.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)