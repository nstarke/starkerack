# Intellijel — Unity

- [Manual PDF](../../manuals/unity-mixer_manual_2020.04.15.pdf)

---

[Unity Mixer Manual PDF](https://intellijel.com/downloads/manuals/unity-mixer-manual-2020.04.15.pdf)

---

# Creative Uses for the Intellijel Unity Mixer

The Intellijel Unity Mixer is a compact, dual 3:1 or single 6:1 unity-gain mixer for both CV and audio signals. While simple at first glance, its true power emerges in creative patching contexts. Below are several imaginative ways to put the Unity Mixer to work, drawing on key features outlined in the manual.

---

## 1. Mixing Multiple LFOs for Complex Modulation

**Combine several LFO outputs** (from modules like the [Mutable Instruments Tides](https://mutable-instruments.net/modules/) or [Doepfer A-145](https://doepfer.de/a145.htm)) into a single, composite modulation signal. This allows you to generate intricate, evolving CV for modulating parameters like filter cutoff, oscillator pitch, or wavefold depth.

- **Patch:** LFO A → In 1, LFO B → In 2, LFO C → In 3, Output → Filter cutoff.
- **Tip:** Use different LFO rates and waveforms for unexpected results.

---

## 2. Summing Triggers or Gates

Need to create complex rhythm patterns from several trigger/gate sources? **Combine triggers from multiple sequencers** (e.g., [ALM Pamela’s New Workout](https://busycircuits.com/alm017/) or [Make Noise Tempi](https://www.makenoisemusic.com/modules/tempi)) to build polyrhythmic gate streams for percussion, envelope firing, or logic gating.

- **Patch:** Three sequencer gates → Inputs 1, 2, 3. Output → Drum module gate input.
- **Result:** Drums play on any active gate; can also combine with simple diode logic for advanced patterns.

---

## 3. Summing Pitch CV: Performance Transposition

With accurate unity gain, the Unity Mixer lets you create **transpose buses** for pitch CV. For example:

- **Patch:** Sequencer pitch CV → In 1, Keyboard CV (manual pitch bend or transpose) → In 2, Offset voltage (from e.g., [Intellijel Quadratt](https://intellijel.com/shop/eurorack/quadratt-1u/)) → In 3, Output → Oscillator 1V/oct.
- **Result:** Live transpositions and octave switching; perfect for performative play.

---

## 4. Unified Mixer for Audio Layering

**Group up to six audio sources** (e.g., VCOs with different waveforms) to a single mixer for thick, layered basses or pads.

- **Tip:** Use the rear -6dB jumper when mixing raw VCO outputs to prevent clipping and produce a cleaner sound.

---

## 5. Control Voltage Blending for Morphing Envelopes

Mix outputs of multiple envelope generators (e.g., [Intellijel Dual ADSR](https://intellijel.com/shop/eurorack/dual-adsr/), or [Make Noise Maths](https://www.makenoisemusic.com/modules/maths)) to sculpt a more complex composite envelope.

- **Example Patch:** MATHS Ch. 1 → In 1, Dual ADSR A → In 2, Another EG → In 3, Output → VCA or filter.
- **Use:** Morph smoothly between sources for evolving drums, pads, or textures.

---

## 6. Feedback Mixing for Karplus-Strong Synthesis

Build a simple **Karplus-Strong voice** by routing the output of a short digital delay (e.g., [Doepfer A-188 series](https://doepfer.de/a188.htm) or [Mutable Instruments Beads](https://mutable-instruments.net/modules/beads/)) and the original pluck trigger through the Unity Mixer and back into the delay's input. 

- **Patch:** Delay output → In 1, Trigger pulse → In 2. Output → Delay input (via attenuation as needed).
- **Result:** "String" feedback, easily controlled/mixed.

---

## 7. Manual CV Summing for Live Tweaks

Use with hand-controlled offset/attenuators (like [Intellijel Quadratt](https://intellijel.com/shop/eurorack/quadratt-1u/) or [Doepfer A-138n](https://doepfer.de/a138n.htm)) to build a manual mixer for voltage control. Adjust up to three sources on the fly, sum, and send to any modulation destination.

---

## 8. Gate and CV Bus Creation for Polyphony

With polyphonic modules ([Mutable Instruments Plaits](https://mutable-instruments.net/modules/plaits/) in poly mode, or [Polyend Poly](https://polyend.com/eurorack/poly/)), build a bus host for distributing summed gate or modulation signals to multiple voices, either for layer blending or unified velocity/gate control.

---

## 9. Multing and Routing: Serial/Parallel Processing

Patch outputs from one set of sources into the top mixer, outputs from another set into the bottom, and send the summed outputs to separate effects or VCAs for easy A/B blending or serial effects routing (e.g., one sum to reverb, the other to delay).

---

## Notable Module Pairings

- **Intellijel Quadratt/Triatt:** For pre-attenuation and voltage generation.
- **Intellijel Dual ADSR / Maths:** For envelope and shape summing.
- **ALM Pamela’s New Workout, Tempi:** For creative clock/trigger summing.
- **Filter modules (e.g., Intellijel Polaris):** For summed LFO modulation or audio layering.
- **Function Generators (e.g., Malekko ADLFO):** For generative CV blends.

---

## Pro Tip

Use ModularGrid to visualize your setups and prevent accidental overloading of your case's power supply.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)