# Noise Engineering — Basimilus Iteritas Alia

- [Manual PDF](../../manuals/Basimilus Iteritas Alia Manual - Noise Engineering Documentation.pdf)

---

[**Download the Basimilus Iteritas Alia Manual PDF**](https://manuals.noiseengineering.us/bia/)

---

# Using Basimilus Iteritas Alia for Hyper-Complex, Densely Rhythmic Percussion

The Noise Engineering Basimilus Iteritas Alia (BIA) is a highly flexible and performable percussion voice, perfectly suited for creating dense, intricate, and hyper-complex percussion patterns in Eurorack modular systems. It excels in stacking, modulating, and morphing synthetic drum sounds, making it ideal for polyrhythmic explorations and advanced pattern building.

Below, you’ll find strategies and patching ideas to maximize the BIA’s potential in complex rhythmic music:

---

## 1. Embrace CV Control for Pattern Complexity

Every important parameter of the BIA (Pitch, Morph, Decay, Attack, Fold, Harm, Spread) accepts CV, enabling you to animate and sequence each aspect of your drum sound:

- **Use Multiple Modulators:** Employ LFOs, random sources, envelopes, and step sequencers to independently control parameters. For example, modulate `Decay` and `Harm` with different Euclidean or random gates for shifting drum timbres within each bar.
- **Cross-modulate Patterns:** Modulate, say, the `Spread` parameter with one clock-division while the `Morph` is controlled by another — this generates evolving, non-repetitive textures.
- **Complex Rhythmic CV:** Use a clock divider/multiplier or probability skewed triggers (like Pam’s New Workout, Malekko Varigate, or Acid Rain Maestro) to input unusual timing into parameters, syncing the BIA’s tonal/texture evolution to complex polyrhythms.

---

## 2. Layering & Multitimbrality in a Single Voice

The BIA is exceptionally flexible as a drum synth — rapid manipulation of its sound via CV and manual controls allows you to use it as multiple percussive voices in a pattern:

- **High-speed Trigger Sequencing:** Trigger the BIA at audio rates, or fire triggers from multiple rhythmic sources (advanced sequencers or trigger combiners) to create densely layered, hyperactive percussion. Try combining several polyrhythmic trigger patterns into the Trig input.
- **Envelope Output as Mod Source:** Use the BIA’s Env Out to shape or modulate other modules, syncing amplitude envelopes or modulating effects in time with each drum hit for tight, interconnected rhythmic motifs.

---

## 3. Exploit the Three Synthesis Modes for Percussive Variety

- **Skin:** Tune for analog-like, tonal and punchy drums (snares, toms); great for underlying grid.
- **Liquid:** Use for punchy kicks and off-beat synthetic percussion, especially when modulating the pitch envelope for boomy, rolling effects.
- **Metal:** For metallic, inharmonic, and noisy percussion, perfect for filling complex patterns and accenting less obvious beats in a polymetric sequence.

Switch modes within a pattern (with sequential switches or “human” intervention) to re-map the BIA’s personality on the fly.

---

## 4. Advanced Techniques

- **Chaotic Accents & Flams:** Patch fast ratcheting or burst triggers (using modules like µBurst or a clocked random) to the Trig input, creating flams and rolls that cut across the rhythmic grid.
- **Accent With Parameter Triggers:** Gate the Decay, Fold, or Harm CVs with their own polyrhythmic trigger sequences to add texture and complexity. For instance, every third or kth hit gets increased Decay or more intense Fold, making each pattern cycle different.
- **Voltage-Addressed Kits:** Change the `Pitch` or mode switches via CV/sample & hold, building drum kits that morph fluidly across complex time signatures.

---

## 5. Patch Examples for Complex Patterns

### Polyrhythmic Hat Pattern

1. Patch Trig to a rhythm with a 5-step pattern.
2. Modulate `Spread` and `Fold` with alternating stepped random or another clocked LFO on a 7-step pattern.
3. Result: Each hat hit is slightly different, cycling over a long, non-repeating period.

### Morphing Percussive Textures

1. Send three CV modulators (e.g., random, sequenced, LFO) into `Pitch`, `Harm`, and `Morph`.
2. Create cascading gate/trigger patterns for `Attack` and `Decay`, accenting off-beats.
3. Output the `Env Out` to modulate a filter or effect downstream.

### Evolving Metallic Percussion

1. Set mode to Metal.
2. Clock sequencer triggering Trig on a Euclidean pattern (e.g., 13 steps over 16).
3. Modulate `Spread` and `Fold` with out-of-phase LFOs or clocked random values.
4. Use `Bass/Alto/Treble` switch or pitch CV for further octave jumps/cascades.

---

## 6. Further Tips

- **Firmware Swapping:** The BIA is part of the Alia platform—consider swapping firmware for even deeper rhythmic capabilities.
- **Autocalibration:** If using intricate pitch CVs, ensure the system is autocalibrated on startup for accurate tracking.
- **Extreme Folding:** Push the Fold control hard for unique, digital-sounding bites and buzzes—envelope compensation keeps hits punchy even at wild settings.

---

For full reference, see the [Basimilus Iteritas Alia Manual PDF](https://manuals.noiseengineering.us/bia/)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)