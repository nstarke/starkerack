# Frequency Central — Wonderland

- [Manual PDF](../../manuals/Wonderland-Build-Document.pdf)

---

[Frequency Central Wonderland Manual PDF](http://www.frequencycentral.co.uk/)

---

## Using Frequency Central Wonderland for Complex Rhythmic Percussion and Polyrhythms

The **Wonderland** is an 8x8 matrix mixer/switcher/patchbay for Eurorack—with both normal and inverted outputs and onboard micro-attenuators. It's neither a voice nor a direct effect; instead, it's a highly creative signal router, which lets you build complex permutations of triggers, gates, audio, and CV paths. This makes it a dream for advanced, algorithmic, and polyrhythmic percussion setups.

### Creative Approaches for Dense, Polyrhythmic Percussion

#### 1. **Rhythmic Routing and Pulse Logic**

- **Inputs:** Patch 8 unique rhythmic sources—clocks, LFOs, triggers, gates, random pulses, Euclidean sequencers, or polyrhythmic patterns (from modules like Pamela’s New Workout, Zularic Repetitor, etc.)—to Wonderland’s 8 inputs.
- **Outputs:** Connect 8 drum/voice/envelope/VCAs or percussion module trigger inputs to Wonderland’s outputs (A–H).
- Use the push-button switches to send any combination of inputs to any combination of outputs—inverting if needed. Route multiple clocks to a single output to create XOR'd, AND'd, or layered rhythmic patterns.
  - Example: Send a 5-step clock to output A, a 4-step clock to output B, and also patch both clocks to output C (now C fires on both, creating a rolling polyrhythm).

#### 2. **Live Pattern Manipulation**

- Wonderland’s buttons are manually playable and can re-route on the fly: manually mute triggers, swap patterns, or quickly rearrange routings to inject fills, breaks, or ‘illogical’ reversals in sequence.
- The ability to invert signals per output means you can generate "anti-rhythms"—triggers or gates that fire in the gaps of the main rhythm.

#### 3. **Matrixed CV Fusion for Modulation Sequences**

- Patch modulation sources (random LFOs, progressing sequencers) to the inputs. Send them, with selective attenuation (via the micro-attenuators), to multiple destinations—pitch, decay, filter cutoff, or other parameters on percussive voices.
- Combine multiple modulation sequences into a single output and control the blend for ever-evolving, hard-to-reproduce patterns.

#### 4. **Instant Polyrhythm/Polymeter Programming**

- Create polymeters by patching two uneven clocks (e.g., 7 and 5 pulses per bar) to different destinations, or even to the same—using the matrix, you can route as many as you want to a single drum trigger module. The result: impossible-to-patch-otherwise composite patterns.
- Use inverted outputs to drive envelopes or sidechain gates that only open on ‘missing’ pulses, filling the voids of your patterns.

#### 5. **Audio as Percussive Source**

- While primarily a CV/trigger matrix, Wonderland can also be used to route audio signals—use short one-shot percussive sounds, clicky envelope pops, or even metallic noise bursts.
- Run raw waveforms to multiple destinations and layer them with triggers; invert for phase-cancellation effects, short metallic percussive sounds, or stutter-style gating.

#### 6. **Creating Controlled Clipping Distortion**

- The manual mentions: *"If you add many inputs to one output you will of course cause clipping... the micro-attenuators are your on-board way around this."*
- Use this fact intentionally: Route multiple triggers or audio clicks to a single output and push the sum into mild or wild distortion, creating crunchy, noisy percussion layers or unpredictable stuttering effects. Attenuate to taste, or leave wide open for chaos.

#### 7. **Generative and Algorithmic Drumming**

- Set up a few logic-derived clock divisions on the inputs (even random gates/LFO resets).
- Use Wonderland to recombine them in shifting configurations—since you can re-route instantly, you can explore new generative/aleatoric patterns that would be much harder on a plain patch bay.

### General Eurorack Tips To Make Patterns Unique, Punchy, and Percussive

- Exploit the **attenuators** to "duck" certain voices, making them more percussive by controlling their loudness within a cluster of sounds.
- Use **phase-inverted outputs** to flip the polarity of modulation/envelopes, changing their attack/decay feel or accent timing for percussive voices.
- Rout signals for creative feedback via effects/filters, using multiple matrix points for hybrid drum voices.
- Combine rhythmic gates with short audio pulses for synthetic "click" percussion, reminiscent of modular drum synthesis.

---

### Summary

Wonderland’s true power in "hyper complex percussion" comes from its tactile, patchable matrix, letting you instantly combine, invert, and attenuate any combination of rhythmic, CV, audio, or modulation signals. Build evolving, convoluted, and tightly controlled polyrhythmic webs without re-patching, and keep your sequences fresh, odd, and uniquely modular.

---

**Reference:**
- [Frequency Central Wonderland Manual PDF](http://www.frequencycentral.co.uk/)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)