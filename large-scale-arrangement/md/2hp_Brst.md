# 2hp — Brst

- [Manual PDF](../../manuals/Brst_Manual.pdf)

---

[Brst Manual PDF](https://2hp.com/wp-content/uploads/2021/03/2hp-Brst-Manual.pdf)

---

# Creating Full-Length Songs with Brst in a Eurorack System

The 2hp Brst module is a powerful, compact voltage-controlled burst generator and trigger delay. Often, the challenge in Eurorack composition isn’t making inspiring short loops, but transforming those loops into compelling, full-length tracks. Below are ways Brst can help you introduce structure, variation, and movement in your songs.

---

## Key Functions Overview

- **Burst Generation**: Emit a programmable stream of triggers per incoming gate.
- **Voltage Control**: Modulate the number of pulses and rate via CV.
- **Trigger Delay**: Create time-shifted rhythmic elements, even omitting the initial hit for creative patterns.
- **Repeat Flexibility**: From 1 up to 32 triggers per burst for anything from fills to flurries.

---

## Strategies for Full-Length Song Arrangements

### 1. Dynamic Fills & Drum Accents

**How:** Patch Brst's OUT to a drum sound trigger input (e.g., snare or clap). Use sporadic, resettable gates from a sequencer at key moments (e.g., pre-chorus, chorus starts).

- Use CV to vary the pulse count for each fill.
- Automate the RATE with a sequencer, LFO, or random source for fills that change feel every time.
- Use the TRIG TOGGLE to include/omit the initial drum hit for call-and-response effect.

**What this adds:** Variety and excitement, unique fill each time, breaks monotony.

### 2. Humanizing Repetitive Sequences

Patch Brst between a master clock and some event triggers (e.g., hi-hats, plucks).

- Adjust RATE with subtle modulation (slow LFO, envelope) to introduce slight timing swings, randomization.
- Inject bursts at different pulse counts to “shuffle” percussion—great for IDM/experimental styles.

**What this adds:** Keeps robotic patterns feeling alive and unpredictable.

### 3. Transition FX and Risers

Route Brst’s bursts to trigger envelopes or function generators patched to modulate filters, VCAs, or effects.

- At moments of transition, a single gate could trigger 16 fast Brst pulses, creating a “ramp up” of modulation— for a whoosh, reverb build, or synth morph.
- Use external CV (from sequencer scenes, random sources, or manual changes) to shape each transition differently.

**What this adds:** Punctuates sections, smooths out stagnant song parts, heightens tension/releases.

### 4. Layering and Section Differentiation

Assign Brst to multiple drum voices, with different PULSES and RATE settings per song section.

- Verse: 1–3 bursts on toms.
- Chorus: Up to 8 pulses on claps.
- Bridge: Omitted initial triggers for off-grid, syncopated feel.

Scene or pattern-based sequencers can automate Brst’s role, turning a basic beat into evolving, sectioned drum arrangements.

**What this adds:** Clear section changes over time, a sense of movement and storytelling.

### 5. Triggering Melodic or Harmonic Events

Patch Brst bursts into a quantizer or melodic trigger path. For every gate from your main sequencer, you could get flurries of notes or arpeggios.

- Vary pulse numbers/rate with CV as above.
- Pair with random CV sources for ever-shifting melodic clusters.

**What this adds:** Richer, evolving melodies and harmonies, suitable for bridges, outros, or breakdowns.

---

## Workflow Tips

- **Automate Everything:** Use sequencers and modulation sources to change Brst panel settings over the course of your song.
- **Layer with Other Modules:** Pair Brst with logic, mixers, random modules, and sequential switches for maximal variety.
- **Integrate with Performance:** Manual bursts (tapped or gated from a controller) are amazing for live builds and breakdowns.

---

**In conclusion:**  
Brst transforms static, repetitive patterns into dynamic, humanized, and structurally varied music—ideal for turning short jams into complete tracks.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)