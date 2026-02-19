# 2hp — Switch

- [Manual PDF](../../manuals/2hp_Switch.pdf)

---

[Switch Manual PDF](https://2hp.com/wp-content/uploads/2018/10/2hp_Manual_Switch.pdf)

---

# Using 2hp Switch for Dense, Hyper-Complex Percussion Sequences

The **2hp Switch** is a voltage-controlled signal router, not a voice or an effect, but an incredibly powerful utility for creating intricate, evolving rhythmic patterns in your Eurorack system. With four inputs, one output, CV control over channel selection, and fast/quiet switching, it lets you dynamically select and combine modulation, triggers, gates, or audio—perfect for intense, polyrhythmic percussion setups.

---

## Strategies for Complex/Rhythmic Patching

### 1. Polyrhythmic Trigger Routing
- **Patch multiple distinct trigger or gate patterns** (from different sequencers, clock dividers, or logic modules) into the four Switch inputs.
- **Sequence the SEL CV input** (using stepped or random CV, or a sequencer set to a non-divisible step length relative to your primary clock) to select between rhythmic trigger/gate streams.
- Run the **Switch output into percussion voices, drum modules, or a quad VCA**: this instantly re-wires your beat structure on the fly, creating micro-polyrhythms and complex time signatures.

### 2. Multisource Percussion Layering
- Send four different drum/percussion audio sources to the module’s inputs.
- Use SEL CV and/or the SEL knob to dynamically shift which drum sound is audible, or AB between complex percussive audio passages through rhythmic CV.
- **Map an LFO, random generator, or Euclidean sequencer** to the SEL CV for pattern mutations that are too intricate for standard step sequencing.

### 3. Glitchy, Percussive Audio Splicing
- Route chopped loops, single-cycle percussive waveforms, or granular “grit” samples to each input.
- Clock the SEL CV input with a high-speed pattern or audio-rate modulation for drum loop “glitching,” fast retriggering, or audio-rate wave splicing on the output for digital, hyper-complex percussion.

### 4. Gate Distribution for Modulation Switching
- Use Switch as a quick modulation router: patch four envelope or LFO shapes in, and use sequenced SEL events to “cut up” and mutate the modulation driving your percussion voices (VCAs, filters, LPGs, etc.).
- This produces animated, erratic transients and percussive qualities far beyond static envelopes or LFOs alone.

---

## Tips for Maximizing Uniqueness & Percussive Punch

- **Stack/mix triggers for flam effects**: Patch simultaneous gate/trigger bursts into adjacent inputs for close, superhuman drum bursts.
- **Insert accents**: Use SEL CV to briefly select an input with an accent trigger or longer gate, into a voice’s accent input, making irregular but punchy hits.
- **Switch fast**: Audio-rate SEL CV creates “bit crushed” or glitch percussion, suitable for IDM, glitch, or hyperpop beatmaking.
- **Pattern crossfading**: Sequence the SEL knob at slow speed with a voltage-block or precision adder for “drifting” pattern shifts over the course of your track.

---

## Integration Suggestions
- **Pair with clocked sequencers (e.g., Pam's New Workout, Euclidean Circles, Trigger Riot) for deep rhythmic complexity.**
- **Combine with random generators (e.g., Wogglebug, Turing Machine) for evolving, unpredictable patterns.**
- **Add slew limiters or stepped quantizers before the SEL CV for unique channel-hopping timings and feel.**

---

Dive into creative switching and routing with Switch—extract maximum mileage from limited channels and simple rhythms by recombining and permuting them on the fly for hyper-dense, evolving percussion!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)