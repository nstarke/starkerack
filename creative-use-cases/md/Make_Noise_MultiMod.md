# Make Noise — MultiMod

- [Manual PDF](../../manuals/multimod-manual.pdf)

---

[Download the MultiMod Manual (PDF)](https://cdn.modulargrid.net/p/files/620219/MultiMod-Manual.pdf)

# Creative MultiMod Patch Ideas & Module Pairings

The Make Noise MultiMod is a remarkably deep and flexible modulation workstation. Below you’ll find some creative ways to use MultiMod in your Eurorack system, both with specific modules and generic types. These ideas explore rhythm, generative, audio, and modulation domains to help you unlock the full potential of MultiMod.

---

## 1. Rhythmic & Polyrhythmic Modulation

**Use Case:** Polyphonic and evolving rhythms across multiple voices  
**Pair With:**  
- Trigger-based sequencers (e.g., **Pamela’s NEW Workout**, **MALEKKO Varigate 8+**)
- Drum modules (e.g., **ALM Squid Salmple**, **Noise Engineering Basimilus Iteritas Alter**)  
**Patch:**  
- Use MultiMod's internal LFO and different Spread/Phase settings to clock multiple drum voices or sequencer clock ins.  
- Patch the Tempo input of MultiMod to your master clock, then route the 8 outputs to trigger different drums or events.  
- Adjust Spread/Phase for polyrhythmic overlaps and evolving groove.

## 2. Polyphonic Voice Control & Harmonic Spreads

**Use Case:** Creating dynamic, related pitch or modulation lines for polyphonic textures  
**Pair With:**  
- Multiple analogue VCOs (e.g., **Doepfer A-110s**, **Mutable Instruments Plaits** in poly mode)
- Polyphonic envelopes (e.g., **XAOC Zadar**, **Intellijel Quadrax**)
- Quantizers (e.g., **Intellijel Scales**)
**Patch:**  
- Send a single sequencer CV or modulation source to MultiMod’s input.  
- Route 4–8 MultiMod outputs to VCO pitch CVs or to envelope or LPG modulation for polyphonic voices.
- Vary Time, Spread, and Phase to create canon-like or morphing polyphony and modulation offsets.

## 3. Audio Mangling & Pseudo-Tape Delay FX

**Use Case:** Multi-channel, interrelated audio delays, tape warble, or granular effects  
**Pair With:**  
- Audio rate sources (e.g., **Morphagene**, **Make Noise Mimeophon**, loopers)
- FX Chains (e.g., **Desmodus Versio**, **4MS Dual Looping Delay**)
**Patch:**  
- Run an audio signal (e.g., loops, field recordings) into MultiMod’s input.
- Use different Phase and Spread settings to output to several FX or mixers for multi-tap delay, evolving textures, or pitch-shifted spectra.
- Change Shapes to Random or Triangle for tape “wow & flutter” or granular-style unpredictability.

## 4. Controlled Chaos & Generative Self-Patching

**Use Case:** Generative, evolving modulation and random CV/gates  
**Pair With:**  
- Sample & hold/random modules (e.g., **Wogglebug**, **Turing Machine**)
- CV addressable switches & sequential selectors (e.g., **Doepfer A-150**, **Mutable Branches**)
- VCAs for modulation routing (e.g., **Intellijel Quad VCA**)
**Patch:**  
- Use internal LFO in a random Shape mode.
- Send MultiMod outputs to various attenuation and modulation destinations, including their own CV inputs for feedback.
- Use Channel Index output to automate VCAs or switches for shifting modulation.

## 5. Modulation Scene Morphing

**Use Case:** Dynamic preset-like changes and “scenes” for live performance  
**Pair With:**  
- Preset manager/cv recorder (e.g., **Expert Sleepers Disting mk4/cv recorder**)
- Macro controllers (e.g., **ALM Busy Circuits ALM032 Boss Bow Tie**)
**Patch:**  
- Create 8 variations of a modulation source, route to different modulators or sound parameters.
- Morph between “scenes” using synchronized Reset, Hold, or Phase changes.
- Use external CV (e.g., from a foot pedal, joystick, or MIDI-to-CV converter) to transition or morph between complex modulations.

## 6. Clocked Function & Envelope Derivation

**Use Case:** Creating time-synced, coordinated modulation shapes  
**Pair With:**  
- Function generators & envelopes (e.g., **Maths**, **Doepfer A-171-2**)
- Clock dividers/multipliers (e.g., **4MS Rotating Clock Divider**)
**Patch:**  
- Feed a clock or trigger into MultiMod’s input, set one channel to fire an envelope on each beat, and others at fractions or multiples for time-warped modulations.
- Use Triangle or Sine Shapes for per-step, LFO-like modulations in sync with beats or manual triggers.

## 7. Cross-Modulation & CV Chaos

**Use Case:** Creating intricate cross-mod feedback networks  
**Pair With:**  
- Any CV processor (e.g., **Happy Nerding 3xMIA**, **Tiptop Audio MISO**)
- Multiple complex oscillators or effects with CV-able parameters
**Patch:**  
- Route MultiMod outputs to modulation destinations, but also feed some outputs or processed feedback CV into MultiMod’s own Phase/Spread/Time CV inputs.
- This self-patching creates evolving, semi-autonomous feedback modulation chains.

---

## Additional Little Tricks:
- **Master Mod Source:** Use MultiMod’s 8 outputs as the “brainstem” for a whole patch’s modulation, ensuring organic relations between disparate elements.
- **Step Addressing:** Channel Index Out can serve as a step CV for sequential switch modules or other addressable devices, giving a “winner take all” high-voltage logic.

---

## Type-Based Module Synergy

- **Modulators:** Envelopes, LFOs, random sources, slew limiters
- **Audio sources:** VCOs, samplers, loopers, granular processors
- **Utilities:** VCAs, switches, addressable matrices, logic modules, mixers
- **Time-based:** Delays, clock generators/dividers, sample & hold

## Inspirational Module Combinations

- MultiMod + Maths = Evolving offset envelopes/LFOs
- MultiMod + Quad VCA = Dynamic morphing of volume/pan/mod
- MultiMod + Mimeophon/Desmodus Versio = Rhythmic multi-tap FX
- MultiMod + Wogglebug = “Intelligent Random” modulations
- MultiMod + Pam’s NEW Workout = Clock division & event-based resets for rhythmic invention

---

Experiment by abusing the MultiMod’s CV inputs, chaos modes, or feeding its outputs back into its own parameters for undiscovered modulation frontiers!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)