# ADDAC Systems — ADDAC-506 SignalFlow

- [Manual PDF](../../manuals/ADDAC506_SignalFlow.pdf)

---

[ADDAC506 VC Stochastic Function Generator & Expansion Manual (PDF)](https://addacsystem.com/sites/default/files/files/ADDAC506_manual_0.pdf)

---

# Using the ADDAC506 VC Stochastic Function Generator to Create Full-Length Songs in Eurorack

## Overview

The [ADDAC506 VC Stochastic Function Generator](https://addacsystem.com/en/products/modules/complex-random/ADDAC506) is an advanced envelope generator with stochastic/random timing, voltage controllable per-stage parameters, curve shaping, and highly flexible logic outputs. Its design is ideal for bringing generative, evolving, and compositionally-rich behavior to modular setups—key for moving beyond static sequences to dynamic, full-length arrangements.

Below are several approaches to using the ADDAC506 in a typical Eurorack environment to help you bridge the gap between great short patterns and fully fleshed-out tracks.

---

## Key Features for Song Structure

- **Four Independent Envelopes**: Can act as modulation sources, function generators, or pseudo-sequencers.
- **Stochastic RISE/FALL Times**: Each stage (rise/fall) can randomize its duration within a defined range, making sequences less repetitive over time.
- **CV Control of All Stages**: Modulate every parameter with external LFOs, sequencers, or automation, enabling macro changes for different song sections.
- **Lock Control**: Lock the settings of some channels while changing others, enabling section-based modulation or transitions.
- **Gate/Trigger and EOR/EOF Outputs**: Perfect for triggering events, modulating rhythms, or clocking sequencers in a generative way.
- **Mix and Sum Outputs**: Use average or sum of envelopes for macro-modulation across your patch.

---

## Song Structure Techniques

### 1. Macro Arrangement with Envelopes

- **Verse/Chorus/Bridge Transitions**: Assign each channel to modulate a key parameter (filter cutoff, reverb mix, groove intensity, VCA amplitude, etc.) per section of your song. Use the lock function to keep settings stable during one part, unlock and re-randomize or morph them for the next.
- **Stochastic Variation**: The randomization features can subtly or dramatically alter your patterns on each retrigger, ensuring each section feels "composed" but evolving.

### 2. Dynamic Pattern Generation

- **Stochastic Clocking**: Patch EOR/EOF outputs to clock sequencers, rhythm generators, or sample players. This creates unpredictable yet musical timing—ideal for breakdowns, drops, and build-ups.
- **Looping vs. One-Shot**: Use one envelope in one-shot mode to orchestrate an “event” or fill, with others looping for ongoing modulation. Change modes per section to distinguish between verses and choruses.

### 3. Automated Transitions

- **Randomized Transitions**: Use the expansion’s random triggers to force new rise/fall times mid-cycle, resulting in “scene changes.”
- **CV-Controlled Macro Changes**: Sequence the min/max CVs from another module (a sequencer, voltage memory, or even keyboard) to script big changes at measure or part boundaries.

### 4. Texture and Structure

- **Layered Modulation**: Use envelope sums and averages to control reverb size, delay times, or effects sends—create swelling or receding soundscapes to mark intros, outros, or climaxes.
- **Envelope-Gating**: Use GATE OUTs for sidechaining other envelopes or triggering additional voices/effects only at specific moments, resulting in tightly-structured arrangements.

### 5. Continuous, Generative Development

- **Evolving Melodies/Beats**: Send random/stochastic CV from the expansion outputs to pitch quantizers or switch addresses, auto-generating non-repetitive but related melodies/rhythms over time.
- **Controllable Randomness**: Use the lock/unlock and external CV features to dial in or freeze desirable states—capture happy accidents for musical consistency as needed.

---

## Example Patch Ideas

1. **Section Morphing**
   * ENV 1 modulates VCF cutoff (chorus brightness)
   * ENV 2 modulates FX send (verse dry, chorus wet)
   * ENV 3's EOR clocks a melody sequencer (melody only in chorus)
   * ENV 4 opens up a noise crash (triggered on fill)

2. **Beat/Fill Automation**
   * Normally looping ENV triggers drum pattern
   * At each transition, a random trigger retriggers RISE/FALL times, making every fill unique

3. **Generative Structure**
   * Send ENV sum out to modulate main VCA to fade the song in/out automatically
   * Use average mix to slowly change the tonality (e.g., modulate chord quantizer root)

---

## Best Practices for Song Creation

- **Combine Stochastic and Deterministic**: Use randomness for variation, but use lock/one-shot modes or external CV for structure.
- **Automate/Sequence Module Controls**: Use sequencers/voltage memories to control envelope min/max times and amplitudes to create distinct song sections.
- **Record and Edit**: Capture long generative performances, then edit sections for arrangement.

---

**Pro Tip:** Pair the ADDAC506 with clock dividers, sequential switches, and quantizers for highly musical generative arrangements that can still be steered live or via automation.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)