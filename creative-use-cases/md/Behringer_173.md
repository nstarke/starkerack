# Behringer — 173

- [Manual PDF](../../manuals/QSG_BE_0720-AAL_173 QUAD GATE-MULTIPLES_WW.pdf)

---

[Behringer 173 Quad Gate/Multiples Manual PDF](https://mediadl.musictribe.com/media/PLM/data/docs/P0DOD/173_QUAD_GATE-MULTIPLES_QSG_WW_MULTI.pdf)

---

# Creative Uses for the Behringer 173 Quad Gate/Multiples

The Behringer 173 "Quad Gate / Multiples" is a versatile utility module featuring four voltage-controlled gates (and/or switches) and six sets of passive multiples (distributors/signal splitters). While it's easy to overlook utility modules compared to more glamorous voice or effect modules, the 173 can be a backbone and performance powerhouse in any Eurorack setup. Below you'll find techniques and patch ideas for integrating the 173 with a variety of other modules.

---

## Patch Ideas & Creative Recipes

### 1. Performance Muting & Rhythmic Variation

**Modules Needed:** Sequencer, Drum Modules, LFO, Clock Divider

- Use the 173's gate sections as manual mutes for drum or melodic sequences. Patch your sequencer’s gate outputs through the 173’s GATE IN, then take the GATE OUT to drum voices/sound-producing modules.
- Use an LFO, clock divider, or anything generating rhythmic gates into the GATE CV to create stuttering, polyrhythms, or random mute patterns.
- **Specific module suggestion:** Combine with [Mutable Instruments Grids](https://mutable-instruments.net/modules/grids/manual/) for probabilistic rhythm generation, using the 173 to further alter or re-route gate patterns dynamically.

### 2. Logic Processing & Gate Manipulation

**Modules Needed:** Logic Module (e.g., Intellijel Plog), Sequencers

- The non-inverting and inverting inputs are perfect for complex gate logic. Route two patterns or clocks into a logic module (AND/OR/XOR) and use the result to trigger the GATE CV of one channel, toggling sound sources on/off based on compound conditions (e.g., only play a snare when both your Euclidean rhythm and a chance generator fire).
- The 173 can even act as a simple signal-controlled switch for routing gates to different parts of your patch.

### 3. Voltage-Controlled Audio Switching

**Modules Needed:** Any Audio Source, Envelope Generator, LFO

- While the 173 is primarily designed for gates, you can treat the gate paths as simple voltage-controlled on/off switches for **audio** signals too.
- Route audio through the GATE IN (keeping levels within spec), and use envelopes, LFOs, or random sources to open/close the gate—creating rhythmic stutters or tremolo effects.
- **Trick:** Try audio-rate signals in the GATE CV for digital-style chopping/glitch effects (results can be lo-fi, but sometimes that’s what you want!).

### 4. Massive Live/Performance Signal Distribution

**Modules Needed:** Anything!

- Use the **Multiples** section to distribute clock signals, sequencer outputs, pitch CVs, triggers, etc., throughout your rack.
- For live improv: patch master clocks and key performance controls to the multiples, then patch out to any modules you want to affect together. Instantly re-patch your bay for new performance gestures.
- **Specific module suggestion:** Great when combined with something like the [Pamela’s PRO Workout](https://busycircuits.com/alm017/) for distributing complex clocks or modulation to multiple voices.

### 5. CV-Controlled Gate/Audio Matrix

- Chain several 173s or combine with other gate/switch modules (e.g., Doepfer A-150, Erica Synths Sequential Switches) for larger manually- or CV-controlled routing matrices. Perfect for generative music or live “crossfading” between multiple sources/voices.
- Use a voltage-addressable sequencer (e.g., Make Noise Pressure Points/Brains) to automate how signals flow through the matrix.

### 6. Advanced Sequencing & Fill Generation

**Modules Needed:** Gate Sequencer (e.g., Arturia Beatstep Pro), Clock Modifiers

- Use the 173 to inject/interrupt additional gates into a sequence chain. For example, route your regular hi-hat pattern through a channel, and then trigger the CV input with a clock divider for periodic fills.
- You can invert triggers (active low) with the inverting CV input—useful for creating “reversed” events based on incoming clock logic.

### 7. MIDI to Analog Control Expander

**Modules Needed:** MIDI-to-CV Interface, Multiple Drum or Voice Modules

- Use your MIDI-CV interface gates/triggers through the multiples to drive several voices at once (instant layered chords/arpeggios).
- Insert the gates through the 173 and use the gate CV inputs for global performance muting, EDM-style drops, or live glitching.

---

## Generic Module Type Combinations for Fun

- **Random Generators (e.g., Wogglebug, Turing Machine):** Route random gates to the GATE CV to create unpredictable switching patterns for evolving generative patches.
- **Envelope Followers:** Use the 173 to route gates based on live audio dynamics—great for interactive or reactive systems.
- **Sequential Switches:** Expand the 173’s functionality by using it as a pre-matrix for selectable inputs or outputs.

---

## Tips

- All 173 gate channels are independent—think in terms of parallel processing, not just serial.
- Patch a modulation source (LFO, S&H, random gates) into GATE CV to create “organic” muting and switching.
- Try using passive multiples to intentionally attenuate (slight passive voltage droop) in sensitive control voltage systems, for a touch of analog unpredictability.

---

> [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)