# Schlappi Engineering — Angle Grinder

- [Manual PDF](../../manuals/angle_grinder_manual_20181022.pdf)

---

[**Angle Grinder Manual PDF**](https://www.schlappiengineering.com/manuals/AngleGrinderManual.pdf)

---

# Using the Schlappi Engineering Angle Grinder for Hyper-Complex Percussion & Dense Rhythmic Sequencing

## Overview

The **Angle Grinder** is a highly versatile quadrature sine wave oscillator, state-variable filter, and voltage-controlled waveshaper. Its unique spin and grind architecture—capable of both clean sine oscillation and distorted, dynamically morphing harmonics—makes it an ideal tool in your rack for inventive percussion and rhythm.

---

## Strategies for Dense Rhythms and Percussive Complexity

### 1. **Self-Oscillation for Layered Voices**
- **Patch:** Use the Angle Grinder's four SPIN outputs (0°, 90°, 180°, 270° sine phases) as the sources for individual percussion voices.
- **Technique:** Send each phase to different processing chains (VCAs, filters, or wavefolders). By triggering VCAs with staggered gates or random pulses, you can create interlocking polyrhythms and phase-shifted percussion.
- **Pro Tip:** Employ envelope followers or comparators on each sine output to extract rhythmic gates from the natural zero-crossings of the waveforms.

### 2. **Complex Polyrhythms via Phase-Shifting**
- **Patch:** Take advantage of the quadrature outputs by clocking logic/gate processors from the zero-crossings or peaks of the 0°, 90°, 180°, and 270° outputs.
- **Result:** This naturally produces phase-based polyrhythms (e.g., 4/4 cross-patterns and odd divisions if you frequency-modulate the core).
- **Twist:** Modulate frequency rapidly (FM1 or FM2) for shifting, "elastic" polyrhythms or complex swung rhythms.

### 3. **Grind Section as Percussive Waveshaper**
- **Patch:** Feed fast, sharp envelope or gate-based audio (clicks, pulses, sampled drums) to the main IN and manipulate the [GRIND] sliders.
- **How:** Mix the four GRIND slider controls, which introduce phase-compared, subtracted square waves, to create edgy, metallic, and noisy percussive transients.
- **Morph:** Sweep the GRIND->SPIN knob to move from tight, crunchy attacks to wild, unpredictable chaos.
- **Control:** Apply CV sequences or random voltages to the GRIND CV inputs to “play” percussive timbres rhythmically.

### 4. **Angle Grinder as Extreme Filter/Resonator**
- **Patch:** Send percussive sample or analog drum synth through the Angle Grinder’s INPUT; use the filter outputs (Low Pass, Band Pass, High Pass, Inverted) as four parallel voices.
- **Dynamic Response:** Modulate cutoff frequency (SPIN control/V-OCT or FM jacks) in tempo-synced patterns—a great route for evolving, dynamically morphing drum shapes.
- **Percussive Snap:** Use the DAMPING control to dial in resonance; short, high-resonance bursts mimic toms, metallic hits, or bells with a snapping attack.

### 5. **INJECT for Syncopated “Sync” Hits**
- **Patch:** Use the INJECT input (header-selectable AC/DC coupling) to send sync pulses or sharp tones into the oscillator core. Each “reset” creates a spike—a synthetic drum click or hat.
- **Sync Polyrhythm:** Sequence INJECT from odd divisions relative to a master clock for shifting, evolving percussion.

### 6. **Use Sinewaves for Envelope Generation or Trigger Extraction**
- **Patch:** Send a sinewave output to a comparator or slope detector to generate rhythmic gates or triggers locked to LFO-cycle rhythms.
- **Utilization:** Sequence drum module triggers using differently phased outputs for shifting polyrhythmic patterns.

---

## Patch Examples

### A. **Four-Voice Phase Percussion**
1. Set Angle Grinder to self-oscillate (SPIN, DAMPING, FM1 full CCW).
2. Patch each sine phase output to a VCA.
3. Trigger each VCA/gate from a different rhythm division or odd clock multiplier.
4. Shape with envelopes for kicks, toms, claps, and hats.

### B. **Metallic Polyrhythms with Grind Section**
1. Feed rhythmic pulse train to IN.
2. Bring up various GRIND sliders.
3. FM the core with audio or subaudio sources for clangorous, struck object sounds.
4. Crossfade between filter and grind outputs for evolving, metallic percussion.

### C. **Cross-Modulation for Hyper-Complex Grooves**
1. Use envelope or gate generator to hit INJECT at odd intervals.
2. Simultaneously modulate FM inputs with voltage-controlled patterns from a sequencer.
3. Sample & hold FM or GRIND CV inputs for “chaotic” yet repeatable rhythmic textures.

---

## Unique & Punchy Percussion Tips

- Use the **high output swing (22Vpp)** to overdrive downstream VCAs or filters for gritty saturation.
- Pair with complex modulation sequences (Euclidean, probability, random step, or algorithmic CV) on GRIND sliders and SPIN frequency.
- Sequence the **GRIND -> SPIN** control for patterns that “morph” from oscillatory to filtered percussion within a bar or phrase.
- Crossfade or alternate between the **sine, filtered, and grinded outputs** using CV switches or even fast, audio-rate modulation for highly dynamic, unique results.

---

## Further Inspiration

Angle Grinder excels as an unpredictable percussive voice *and* a rhythmically flexible harmonic processor. With creative patching and clever CV routing, you can generate everything from intricate IDM drum patterns to complex generative polyrhythms and brutalist metallic percussion.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)