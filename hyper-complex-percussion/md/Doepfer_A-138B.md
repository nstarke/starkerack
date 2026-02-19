# Doepfer — A-138B

- [Manual PDF](../../manuals/A138_man.pdf)

---

[Doepfer A-138 Mixer Manual (PDF)](https://www.doepfer.de/a100man/A138_Manual.pdf)

---

## Using the Doepfer A-138 Mixer for Dense, Hyper-Complex Percussion in Eurorack

The Doepfer A-138 is **not a voice or effects module**; it is a **utility module**, namely a four-channel mixer. However, utility modules are essential tools for sophisticated rhythmic music—especially when chasing densely layered, intricate, or polyrhythmic percussion. Below are creative ways to exploit this module in your pursuit of wildly complex drum and percussion architectures.

### 1. Creative CV Mixing for Rhythmic Complexity

#### Use: **A-138a (Linear response)**
- **Mix multiple rhythmic CV sources** (e.g., LFOs, gate/trigger sequencers, random sequencers) before routing to drum voices or modulation destinations.
- Example: Combine two varied and phase-shifted clock/gate signals to create polymetric trigger patterns. A slow LFO + a fast burst generator, for instance, will produce evolving, irregular triggers.
- **Result**: Percussion hits trigger in unique, shifting time relationships, yielding instant polyrhythm.

#### Advanced:
- **CV mixing with manual control**—Use the attenuators (input level controls) to “fade in” polymetric influences in real time, creating performances where the density and rhythm evolve dynamically.

---

### 2. Parallel Drum Voice Processing

#### Use: **A-138b (Logarithmic, for audio)**
- **Layer drum/percussion voices**: Send different drum modules or percussive EOs through each channel. Mix them to taste at the A-138’s output.
- **Manipulate punch and presence**: The output attenuator allows shaping final output gain, especially useful if sending out to effects or external mixers.
- Trick: If your voices share a common accent CV, use the A-138 to add/subtract CV from each channel, so layering a sharp accent onto one and a subtle offset onto another—ideal for punchy, complex grooves.

---

### 3. CV and Audio Feedback Tricks

- **Self-patching**: Mult a drum or percussion audio out, route to a channel of the A-138, then feed the mixer output *back* into a voice’s CV input or LPG. Attenuators let you sculpt the feedback amount for glitchy, self-evolving rhythms.
- With a multed clock signal, use A-138 to combine it with triggers, accents, or random gates—creating truly unpredictable percussive patterns.

---

### 4. Audio/CV Crossfading and Morphing

- Morph between entirely different rhythmic layers or drum voices by assigning them to different channels and sweeping levels by hand (or via external CV’d VCAs pre-mixer).
- By slightly detuning/swinging clocks that trigger voices mixed on the A-138, outputting the sum will produce shifting phase relationships—a recipe for polyrhythmic mayhem.

---

### 5. Offset Function (For unique timbres)

- If using a module built **mid-2004 or later**: The offset jumper for input 1 lets you add fixed positive or negative DC voltage when input is unplugged—a quick hack for adding “bias” to a CV stream, or generating percussive modulation when mixing DC offsets with LFOs/triggers.

---

#### More tips for “Punch” and Uniqueness:

- **Post-mixer processing**: Send the summed output into distortion, wavefolders, or resonant filters for extra bite.
- **Dynamic Leveling**: Use performance real-time knob tweaks on individual inputs to accentuate syncopation or ghost notes.
- **Overdrive**: Take advantage of the mixer’s headroom (or lack thereof) for saturating drum mixes before effects.

---

**Summary Table**

| Patch Type | Mixer Version | Typical Sources | Result |
|:----------:|:-------------:|:---------------|:-------|
| CV Polyrhythm | A-138a | LFOs, Triggers, Sequencer Gates | Evolving, complex triggers/accent patterns |
| Layered Percussion | A-138b | Drum voice outs | Fused/custom percussive textures |
| Feedback Glitch | Either | Audio/CV, feedback loops | Glitchy, generative patterns |
| Offset/Bias | A-138a (with jumper mod) | DC offset + rhythmic CV | Non-standard CV modulation patterns |

---

#### Patching Example for Polyrhythm:

```
[LFO1] -----> [In 1]  
[Clock/Trigger A] -----> [In 2]  
[Random Gates] -----> [In 3]  
[Nothing (use jumper for Offset)] -----> [In 4]  
[A-138 Output] -----> [Percussion Envelope In]  
```
Sweep input levels to morph between rhythms, accent patterns, and unpredictably phase-shifted grooves.

---

**Pro Tip**: Utility modules like A-138 are powerful when used creatively. In highly rhythmic, complex setups, the difference between “routine” and “next level” is often how fluently you can sculpt, layer, and interact with both audio and modulation signals—especially in real time!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)