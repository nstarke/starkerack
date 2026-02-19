# 2hp — Kick

- [Manual PDF](../../manuals/2hp_Kick.pdf)

---

[Download the Kick Module Manual (PDF)](https://intellijel.com/support/manuals/Manual_Kick.pdf)

---

# Using the Kick Module for Densely Rhythmic and Hyper-Complex Percussion

The **Kick** module is a versatile 2HP bass drum synthesizer perfect for any modular system aiming for advanced rhythmic complexity. Based on your interest in polyrhythms, complex time signatures, and intricate patterns, here’s how you can leverage every feature of the Kick module to build intensely percussive music:

---

## 1. Rhythmic Triggering: Trig

- **Input Complex Gates**: Use a trigger generator or sequencer capable of non-standard time signatures (e.g., 5/8, 7/8, 11/16) or a pattern generator like **Pamela’s New Workout**, **Euclidean Circles**, or **Westlicht Performer**.
- **Polyrhythms**: Patch multiple, unsynchronized clocks or LFOs into clock/trigger logic modules, then send the derived gates to **Trig** to generate polyrhythmic kicks.
- **Probability/Randomization**: Use a probability gate (e.g., **Branch**, or controlled logic from Marbles or Pamela’s New Workout) to sporadically trigger the kick for living, generative beats.

## 2. Tone Modulation: Tone

- **CV Animate Character**: Sequence or randomly modulate the Tone parameter using a fast, stepped random CV (e.g., using **Wogglebug** or **Turing Machine**) within the -5V to 5V range. This can turn each kick in a complex pattern into a uniquely colored hit—metallic, clean, or overdriven.
- **Dynamic Movement**: Map performance controls or envelopes to the CV in, so the timbre changes dynamically per hit or phrase, making dense rhythms more organic.
- **Stereo Imaging**: Use an external module to pan Tone-altered kicks within a wider stereo stage.

## 3. Decay Control: Decay

- **Variable Decay**: Modulate Decay with slow LFOs, envelopes, or stepped CV to alternate between short, snappy hits and long, booming tails within a single phrase.
- **CV Sequencing**: Use a sequencer with CV output to adjust decay per step; e.g., set short decays on quick runs, long decays on accent hits. 
- **Complex Patterns**: Pattern the Decay CV at rates relating to your drum triggers but offset for cross-rhythmic interplay.

## 4. Pitch Sequencing: V/Oct & Pitch

- **Tonality in Percussion**: Sequence V/Oct input from a melody, arpeggiator, or a quantized random voltage, turning your kick into a tuned percussive instrument—ideal for IDM or experimental polyrhythms.
- **Voice Layering**: Use fast changes in V/Oct to create "basslines" from just the kick.
- **Microtonal & Odd Tunings**: Use analog sequencers or quantizers capable of microtonal scales for even more unusual patterns.

## 5. Output Use: Out

- **Accent Processing**: Route output through further effects (distortion, compression, stereo processing) and modulate those effects in sync with the complex triggers for even more unique hits.
- **External Processing**: Layer the Kick with other drum voices, send to a VCA for amplitude shaping with funky envelopes, or resample into granular modules for even denser rhythmic layers.

---

## Patch Example: Polyrhythmic Kick Network

1. **Sequencer 1** (outputs in 5/8) ⟶ Trig 
2. **Sequencer 2** (outputs odd CV patterns) ⟶ Tone CV 
3. **LFO (slow, triangle)** ⟶ Decay CV 
4. **Random CV Source** (quantized scale) ⟶ V/Oct 
5. **Performance Macro** (manual offset, e.g., Planar or Pressure Points) ⟶ Pitch knob

Result: Each hit is different in tone, intensity, and pitch—organized by a matrix of rhythmic clocks and evolving CV modulations.

---

## Tips for Uniqueness and Punch

- **Double the Voice**: Mult the Trig and gate multiple kicks slightly out of phase with different settings for flams/drags.
- **Distortion Sweet Spot**: Use the left side of Tone heavily, push through soft clipping for punch.
- **CV Everything**: The more parameters you automate (even with slow LFOs), the more dynamic complexity you achieve.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)