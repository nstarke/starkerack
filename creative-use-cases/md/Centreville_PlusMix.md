# Centreville — PlusMix

- [Manual PDF](../../manuals/PlusMix _ centrevillage.pdf)

---

[Manual PDF](https://centrevillage.net/products/PlusMix.html)

---

# Creative Eurorack Patch Ideas with PlusMix

The **PlusMix** by centrevillage is a compact (2HP) unity mixer with gate-controlled switching, high-precision CV mixing, and manual mute/switching capability. Here’s how you can creatively integrate it into your Eurorack system:

## 1. **Pitch CV Remixing / Transposition Selector**
- **Modules to combine:** Sequencer (e.g. Arturia Keystep, Intellijel Metropolis), Quantizer (e.g. Intellijel uScale), Envelope Generator
- **Patch:** Send sequenced pitch CV to `BASE`, a second melodic CV to `PLS1`, and another transposition source (e.g., an LFO or slider) to `PLS2`.
- **Action:** Use the manual switches (`SW1PL`, `SW2PL`) as transposition toggle switches, or remotely control with triggers/gates from your sequencer to "activate" extra voices or modulations.
- **Result:** Perform live key changes, transpositions, or layered melodies on the fly—without drifting out of tune.

## 2. **Gate-Controlled CV Routing for Expressive Modulation**
- **Modules to combine:** Envelope generators, LFOs (Mutable Instruments Tides or Pamela’s New Workout), Random CV (e.g., Wogglebug), Step sequencer gates
- **Patch:** Mix several modulation sources (envelope to `BASE`, LFO to `PLS1`, random to `PLS2`). Then use rhythmic gates/triggers to the `SW1` and `SW2` inputs from your sequencer or drum machine.
- **Result:** Voltage-controlled, rhythmically gated modulation to a target parameter (e.g., filter cutoff), with certain LFOs/envelopes only mixed in for specific beats, fills, or groove changes.

## 3. **Instant Audio Ducking or Manual Muting**
- **Modules to combine:** Drum modules, percussion samplers, effect units (reverb, delay)
- **Patch:** Route dry drum audio to `BASE`, wet (reverb) signal to `PLS1`. Use SW1PL as a manual mute—or patch a gate from a kick drum trigger into SW1 to instantly "duck" or mute FX tails in sync.
- **Result:** Quick mute, ducking, or switching between dry/wet signals for percussive mix clarity with hands-on or automated (trigger) control.

## 4. **Performance Mixer with Footswitches**
- **Modules to combine:** Foot-operated gate switch (e.g., Erica Synths Pico Drum Programmer), Effects modules (Distortion, Chorus)
- **Patch:** Route clean guitar synth signal to `BASE`, overdriven/chorused version to `PLS1`, controlled by gate switches triggered via a foot pedal into `SW1`.
- **Result:** Live guitarists/synth players can use effect toggles hands-free for performance dynamics.

## 5. **Precision Logic Mixing**
- **Modules to combine:** Logic modules (Mutable Instruments Kinks, Doepfer A-166), gates and triggers
- **Patch:** Send AND/OR logic outputs to `PLS1` and `PLS2`, with manual/gate switches selecting which logic stream goes to a drum trigger input or effect.
- **Result:** Intelligently route and mix logic functions to create complex fills, drum rolls, or scene changes, with tight, precision-level voltage control.

## 6. **Multi-Layered CV Mixing for Polyphony**
- **Modules to combine:** Polyphonic CV sources (Polyend Poly, Expert Sleepers FH-2)
- **Patch:** Use each input for different voice control voltages, and gate-switch ramps between unison, duophonic, or layered results, especially useful for chord voices or harmonized lines.
- **Result:** Switch, combine, or layer voices for polyphonic or harmonic passages without repatching.

## Additional Tips
- **Vactrol or Light-Controlled Gates:** Insert a vactrol or opto-coupler for smooth voltage-controlled fades via SW1/SW2 gates.
- **Clocked Step Sequencing:** Sync stepping/mixing modulation to a master clock for polyrhythmic groove dynamics.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)