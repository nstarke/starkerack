# Schlappi Engineering — Three Body

- [Manual PDF](../../manuals/three_body_manual_01302023a.pdf)

---

[Three Body Manual (Schlappi Engineering, PDF)](https://schlappiengineering.com/wp-content/uploads/2023/12/schlappi-three-body-manual-2023.pdf)

---

# Using Schlappi Three Body for Hyper-Complex Percussion & Rhythmic Music

The **Schlappi Engineering Three Body** is exceptionally powerful for driving complex, evolving rhythmic and percussive material, thanks to its trio of deeply-interconnected digital oscillators, flexible normalization, and highly configurable modulation. Here’s how to leverage its architecture in the context of hyper-rhythmic, polyrhythmic, and advanced percussive music.

## Approaching Percussion with Three Body

### **Module Roles**

- **Voice:** Each of the three oscillators can act as an individual percussion voice—kick, tom, snare, metallic clang, noisy hit, etc.
- **Effect**: Use the internal cross modulation to process other voices, creating pseudo-coordinated “sidechain” or unexpected percussive artifacts.

---

## Key Techniques for Dense, Complex Rhythm

### 1. **Polyrhythms & Polymetric Structures**

- **Ratio Tracking**: Set oscillators to **RATIO** mode and use integer/non-integer ratios between carriers. Try tracking the inner oscillator (master “clock") with outer oscillators as polyrhythmic “subdividers.” 
    - *Example*: Center at “free” (master clocked oscillator), left and right at **ratio** with divisions/multiplies set to 3 and 5 for a 3:5 polyrhythm.
- **External SYNC**: Patch different rhythmic impulses (clock dividers, triggers, LFOs) into the **SYNC** inputs. Each oscillator can then lock to independent time bases or odd rhythmic clocks, furthering polyrhythmic complexity.

### 2. **Complex Patterns**

- **FM/PM Modulation**: Cross-modulate oscillators with audio-rate or sub-audio oscillators, making patterns with spectral/transient complexity that can “mimic” layered percussion ensembles.
    - Patch sine output of one into phase or FM input of another, then tweak the **index** and polarity for pseudo-chaotic percussive bursts and metallic artifacts.

### 3. **Time Signature Adventures**

- Use odd or evolving division/multiplication ratios on the outer oscillators for signatures like 5/4, 7/8, 11/16.
- Modulate these with random voltages or sequenced CV sources to automate pattern switching or evolving metric feel.

---

## Patch Concepts

### > **A: Polyrhythmic Percussion Triplets and Fives**

1. Set **Center** osc to **FREE, HIGH** (base frequency = clock/root note).
2. **Left** osc: RATIO, DIV: 3 (triplets), **MULT** as 1 (standard).
3. **Right** osc: RATIO, DIV: 5 (quintuplets).
4. Take **Sine**, **Triangle** or **Saw** from each out to separate LPGs or VCAs—trigger each with similarly divided external gates or let the phase interaction itself “illusion” hits (especially with envelope followers/comparators after).

### > **B: Algorithmic "Drum Machine" with Shifting Ratios**

- Use **step sequencer** or **random CV** into V/OCT RATIO on outer oscillators. Modulation can create live-shifting subdivision, blurring the line between precise and chaotic patterns.
- Use modulation attenuators to restrict the CV range so that only certain divisions/multiplies are accessible at a given time—morphing between 1, 2, 3, 5, 7, etc.
- This results in arpeggiating or grid-shifting patterns, like a generative rhythm engine.

### > **C: Metallic, Punchy Percussion With Phase Modulation**

- Self-patch the left and right oscillator’s sines to each other's **PHASE CV** inputs (**with index attenuators!**).
- Use center oscillator for a deep base, or patch outer oscillator waveforms to LPGs with fast envelopes.
- Turn up **PHASE INDEX** or **FM INDEX** just to the point before noise—this yields complex, biting metallic transients like cymbals, snares, or bells with naturalistic tails.
- For even more character, experiment with the **External Filter** header (16H) for noisier/cleaner modulation.

### > **D: Trigger-Gated Percussive Bursts**

- Use fast external triggers/gates into SYNC for hard resets.
- Patch audio-rate modulation between FM/Phase inputs for “ring mod” and atonal percussive pops.

---

## Manipulations For “Punch” and Uniqueness

- **Use Wavefolding Effects:** Push phase modulation hard for sharp wavefolded attacks that read “percussive.”
- **Dynamic Indexing:** CV control over *PHASE/FM INDEX* allows envelopes per hit for snappy/decaying timbral movement.
- **Multilayer With Outputs:** Simultaneously mix SINE, SAW, TRI out for rich transient “impacts” with high-frequency detail.
- **Stereo Field:** SINE/COSINE and SAW/COSAW pairs, with strong phase/frequency modulation, create wide, spatially animated percussive events.
- **Square Wave Phase Mod:** Use the **square output** with phase mod disengaged (header 14G) for suboctave “thump” or to layer fundamental body beneath noisy or metallic upper harmonics.

---

## Additional Tips

- Use comparators or envelope followers on outputs to convert wild waveforms into new gates/triggers for (meta-)sequencing drums.
- Run outputs through fast VCAs or LPGs to get that “clicky,” punch-in-the-face percussion transient, using envelopes synced to other oscillators’ cycles for layered, interlocking grooves.
- Don’t overlook: cross-pollinate Three Body’s outs as modulation sources elsewhere in your rack for system-wide chaos/groove.

---

### Recommended External Utilities

- **Sequencers** (step, random, or burst): Drive V/OCT RATIO for evolving pattern signatures.
- **Fast Envelope Generators/LPGs**: For sculpting output into drum-like envelopes.
- **Comparators/Logic**: For extracting triggers from complex waveforms.

---

**For additional ideas and inspiration, see the [Schlappi Three Body Manual PDF](https://schlappiengineering.com/wp-content/uploads/2023/12/schlappi-three-body-manual-2023.pdf).**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)