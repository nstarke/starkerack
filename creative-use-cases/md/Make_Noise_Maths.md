# Make Noise — Maths

- [Manual PDF](../../manuals/MATHSmanual2013.pdf)

---

[Make Noise Maths Manual PDF](http://makenoisemusic.com/manuals/Maths2013Manual.pdf)

---

# Creative Use of Make Noise Maths in Your Eurorack System

The Make Noise Maths module is an ultra-flexible analog function generator, function processor, and signal mod utility. Below are advanced and creative ideas for how to patch Maths in combination with other popular and general Eurorack modules. These techniques make use of the functionality outlined in the manual above and suggest some musical or sound-design directions you might pursue.

---

## 1. Rhythmic Skipping, Randomization & Probabilistic Pulses

**Interesting With:** Mutable Instruments Branches (gate randomizer), Wogglebug (random voltage source), or any clock divider/multiplier

- **Patch:** Use the EOR/EOC (End of Rise/Cycle) to gate a randomizing module (e.g. clock input of Branches or Wogglebug).
- **Why:** You’ll generate probabilistic rhythm triggers in sync (or out of sync) with your core Maths cycles, enabling generative drum or percussion lines.
- **Bonus:** CV-in the Rise/Fall times with a slow LFO or random voltage for evolving rhythms.

---

## 2. Slewed Envelope Following & Spectral Animation

**Interesting With:** Mutable Instruments Rings, MI Elements, or any filter/LPG (LxD, Optomix, etc.)

- **Patch:** Process external audio (from a tape loop, guitar, or mic input) through Maths as an envelope follower (manual p.23).
- **Then:** Use Maths’ OR out as an envelope to modulate the cutoff of a filter or LPG (e.g., DPLPG, LxD, Optomix), or control timbre on Rings’ structure/brightness.
- **Why:** This lets you dynamically sculpt tonal color or resonance based on real audio amplitude – great for live performance.

---

## 3. West Coast Complex Oscillator "Serge" Style Waveshaping

**Interesting With:** Make Noise DPO, Verbos Complex Oscillator, Instruo Cs-L, The Harvestman/Industrial Music Electronics oscillators

- **Patch:** Use Maths as both a CV processor and audio-rate function generator:
    - Send audio-rate modulation from Maths’ cycling channels into a complex osc’s FM input.
    - OR, process an external oscillator through Maths’ input for non-linear slew limiting, resulting in "wavefoldy" shapes.
- **Why:** Maths' shaping and curvature control provides unique, animated timbral variation.

---

## 4. Trigger Sequencer/Clock Manipulator

**Interesting With:** Pamela’s New Workout (clock module), Make Noise Tempi, Intellijel Steppy, or ANY simple step sequencer

- **Patch:** Take clock pulses or step triggers into Maths channels. Patch EOR/EOC to sequencer reset/input/step inputs.
- **Why:** You can skew/shift steps, trigger logic, or create complex polyrhythms easily by varying the Rise/Fall and cycle time. Maths can also manually delay or divide clocks.

---

## 5. Evolving LFOs and Dual-Mixed Modulation

**Interesting With:** Mutable Instruments Tides, Intellijel Quadrax, ALM Pamela’s New Workout, or any other modulation sources

- **Patch:** 
    - Self-patch EOR/EOC from Maths to cycle inputs for bouncing-ball, phase-shifted LFOs (manual p.21-22, 23).
    - Mix Maths' outputs with other LFO shapes in a CV mixer (e.g., Intellijel Triatt, Happy Nerding 3xMIA).
- **Why:** Great for evolving drones/cinematic modulation, or to create shifting CVs that subtly morph other parameters over time.

---

## 6. Audio Mangling & Pseudo-VCA

**Interesting With:** Mutable Instruments Clouds/Beads (granular), resonant filters, ring modulators

- **Patch:** Model the "pseudo-VCA" technique (manual p.24): run an audio signal through a Maths channel, and use offsets from Ch2/3 to push the level toward clipping or silence. Envelope-control the amplitude and clipping point.
- **Why:** Achieve highly driven, dynamically changing fuzz/distortion, waveshaping, or gating effects—especially striking when automated via Maths' own cycling or an external envelope.

---

## 7. Oscillator Sync and Complex Trigger Chaining

**Interesting With:** Any VCO (Dixie II+, DPO, STO), percussion synths, drum modules

- **Patch:** Use Maths’ EOR/EOC outputs as sync or trigger inputs for other oscillators, percussion voices, or envelope modules.
- **Why:** This enables creative chained envelopes, start/stop triggers, stepped modulation, or complex "gate choreography" beyond conventional sequencer capabilities.

---

## 8. Advanced Logic Functions—CV Level & Polarity Game

**Interesting With:** Any step sequencer, comparative logic module (Doepfer A-166, Livestock Electronics Maze)

- **Patch:** Use the SUM/OR and INV outputs for voltage thresholding, maximum/minimum voltage derivation, and sum/difference CV mixing.
- **Why:** Great for key-transposable sequences, dynamic CV mixing, or complex "CV math" in generative or evolving patches.

---

## 9. Generative & Self-Patching Ecosystem

**Interesting With:** Mutable Instruments Marbles (random), Make Noise René (touch controller sequencer), feedback loops

- **Patch:** Use Maths’ outputs to modulate its own cycle/gate/trigger inputs, possibly via feedback from processed audio or other modules. Combine with random sources or stepped voltages for unpredictable emergent patterns.
- **Why:** Maths makes an excellent CV "brain" for generative modular music, constantly creating new signals in unpredictable ways—especially when chained via logic with sequencers, random, or probability sources.

---

## 10. Crossfading and Log/Exp "Animation"

**Interesting With:** ANY VCA/Mixer (e.g., Intellijel Quad VCA, Mutable Veils), Make Noise Morphagene

- **Patch:** Use Maths channels as voltage-controllable crossfaders between LFOs, envelopes, audio, or modulate the curvature (log/lin/exp) via CV for time-evolving modulation depth.
- **Why:** Animate not just shape and timing, but also the character AND depth of every modulation in your system for extra vibrancy.

---

Experiment with patching Maths' functions in both audio and CV domains—sometimes it sounds great to just clock, modulate, and process everything through its highly-flexible architecture. The more you self-patch and chain it with modulation or utility modules, the more complex and musical your results will become.

---

**Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)**