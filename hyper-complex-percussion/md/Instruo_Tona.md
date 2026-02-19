# Instruo — Tona

- [Manual PDF](../../manuals/Tona-Manual-A5.pdf)

---

[Instruō tòna Oscillator Manual (PDF)](https://www.instruomodular.com/wp-content/uploads/2022/02/tona_manual-compressed.pdf)

---

## Using Instruō tòna for Densely Rhythmic & Hyper-Complex Percussion

The Instruō tòna is a high-quality analog oscillator with classic and modern waveforms plus an integrated wavefolder, offering significant utility for complex percussive and rhythmic synthesis. Here’s how you can leverage its features to craft punchy, unique polyrhythmic percussion:

---

### Percussive Voice Generation

**1. Use tòna as a Percussive Voice Source**
- **Waveform Selection:** The sine and triangle outputs are ideal for classic kick, tom, or bell tones. The square and sawtooth outputs can create snare or clap-like timbres (further processed with filters/VCA).
- **Wavefold Output:** For metallic, noisy, or dynamically morphing percussion, use the folded waveform. Animate the Wavefold with CV for evolving, ‘West Coast’ style claps, snares, or hats.

**2. Sculpt Envelope Shapes**
- Feed short, snappy envelope CVs to a VCA after tòna for percussive decay. Use exponential envelopes for attack-heavy hits.

**3. Complex Modulation for Rhythm**
- Modulate the **Wavefold CV Input** with stepped random generators, clocked LFOs, or even trigger pulses, creating rhythmically morphing timbral changes within each hit.
- Trigger the hard **Sync Input** with polyrhythmic gates/clocks to ‘reset’ the oscillator cycle on each drum hit—very sharp, synthetic attack transient!

---

### Polyrhythms & Complex Patterns

**1. Advanced Oscillator Syncing**
- Use asynchronous (non-divisible) clocks or rhythmically-related trigger sequences into Sync Input for oscillator retriggering, producing polyrhythmic or irregular percussion hits with punchy shapes.
- Sequencer channels with different lengths/step counts can create complex patterns when used for sync/reset or envelope triggers.

**2. FM Techniques**
- Patch a second oscillator (with its own complex rhythm) into **Linear FM Input**. Use rapid, envelope-shaped, or per-step-tuned modulation for toms, metallic percussion, or pseudo-random blips.
- Animate **FM Depth** with a clocked CV (e.g., stepped random, or a sequencer track) for variable timbral complexity per hit.

**3. Audio-Rate Wavefolding Modulation**
- Use tòna’s own waveforms, or other VCO outputs, to modulate the **Wavefold CV Input** at audio rates, synced to rhythmic pulses. This can produce highly complex, 'granular' or metallic percussive overtones with each trigger.

---

### Unique, Punchy & Percussive Patch Ideas

- **Kick/Bass Perc:** Sine output → VCA with short envelope; add a touch of wavefold for punch; clocked sync/reset for tightness.
- **Snare/Clap:** Layer square with folded output, process through a noise source or folder, VCA envelope with fast/slow dual envelopes for snap and body.
- **Hat/Cymbal:** High Fold setting with triangle or folded sine; FM by random voltage+enveloope shaped VCO; rapid retriggers for buzzing hats.
- **Glitch/Ridiculous:** Polyrhythmic sequences to Linear FM, Wavefold CV and Sync inputs all at once; each ‘drum’ hit in the pattern is unique.

---

### Tips for Eurorack Integration

- Pair with clock dividers, gate sequencers (especially those supporting polyrhythms, e.g. Euclidean or logic functions).
- Use triggered LFOs or random sources for modulating tòna’s parameters on every hit for ever-changing drum timbres.
- Mult tòna’s waveform outputs to different VCAs/envelopes for layered percussion from a single oscillator.

---

#### More Resources
- [Instruō tòna User Manual PDF](https://www.instruomodular.com/wp-content/uploads/2022/02/tona_manual-compressed.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)