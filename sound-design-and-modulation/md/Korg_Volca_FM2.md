# Korg — Volca FM2

- [Manual PDF](../../manuals/volca-fm2_OM_EFGSCJ3.pdf)

---

[**Korg Volca FM2 – Manual PDF**](https://cdn.korg.com/us/support/download/files/9863546a1d7b52332efbfc68870ea464.pdf)

---

# Korg Volca FM2: Creative Modulation Strategies for Eurorack Musicians

The Korg Volca FM2 is not a direct Eurorack module, but its highly flexible FM engine can be integrated into a modular setup for wild, unique sound design—especially via MIDI, clock/sync, and audio routing. Here’s how you can achieve distorted percussive sounds, basslines for genres like dubstep/DnB, and haunting atmospheric pads by modulating this FM synthesizer.

---

## Quick Reference: Modulation & Connectivity

- **Sync In/Out**: Sync the Volca FM2 to your modular clock or use its clock output to drive modular sequencers.
- **MIDI In/Out**: Extensive MIDI control over parameters (via external MIDI modules or eurorack-to-MIDI interfaces).
- **Motion Sequencing**: Record parameter movements for evolving sequences.
- **Multiple Voices & Operators**: Deep FM editing for modulation and complex textures.
- **CV to MIDI**: Use eurorack CV-to-MIDI modules to control FM parameters in real time.

---

## 1. **Distorted Percussive Sounds**

**Key Concepts:**
- Fast EG (Envelope Generator) attacks & decays
- Overdriven modulation indexes
- Sequenced operator modulation for rhythmic textures

**How-To:**
- **Sharp Envelope Settings:**  
  - Set MODULATOR and CARRIER **attack and decay** knobs to minimum for super-snappy transients.
  - Use the built-in sequencer or MIDI triggers to play short, percussive sequences.

- **Operator Feedback for Distortion:**  
  - Edit FM algorithms to maximize feedback. Algorithms with operator self-feedback create more harmonics and can sound distorted.
  - In EDIT mode, experiment with feedback parameters—crank them for harsh metallic or noisy percussion.

- **Motion Sequencing:**  
  - Record distortion-inducing movements on your operator envelopes and feedback during the sequence.
  - Use FUNC + MOTION SEQUENCE ON to capture real-time knob tweaks for glitchy, mangled rhythms.

- **External Distortion:**  
  - After output, route the Volca FM2 into a wavefolder, distortion, or bitcrusher eurorack module for even more aggressive drum hits.

---

## 2. **Crazy Basslines (Dubstep/Drum & Bass)**

**Key Concepts:**
- FM for growls and wobbles
- Quick, extreme MODULATOR/CARRIER parameter changes
- Real-time modulation (via MIDI or Motion Sequence)
- Velocity & envelope shaping

**How-To:**
- **Wobble Bass:**  
  - Assign LFO (RATE and P.DEPTH) to pitch or index modulation for classic wobble.
  - Use Motion Sequence to automate the movement of the LFO’s RATE while the sequence plays—this gives “talking” or formant bass FX.

- **Growling Bass:**  
  - Use complex FM algorithms (8, 21, 23, 27, etc.) with multi-stage operators feeding into each other.
  - Modulate FM index and carrier levels for “wet” bass dynamics.

- **MIDI/CV Control:**  
  - Use a CV-to-MIDI module (like Mutable Instruments Yarns, Expert Sleepers FH-2, etc.) to map Eurorack LFOs or envelopes to MIDI CC messages controlling LFO rate, feedback, velocity, or algorithm selection.
  - Map your modulation sources to the pitch or operator envelope parameters via MIDI Learn or DAW automation.

- **Transient Variation:**  
  - Use the internal sequencer to vary note velocities (VELOCITY slider), and record that motion for dynamic accents typical of DnB/dubstep.

---

## 3. **Haunting Atmospheric Pads**

**Key Concepts:**
- Slow attack/release on envelopes
- Subtle LFO modulation
- Motion Sequence for evolving timbres
- Layering internal FX (chorus, reverb)

**How-To:**
- **Envelope Settings:**  
  - Set MODULATOR and CARRIER ATTACK/DECAY to medium-high for slow, swelling pads.
  - Layer long-release times for pads to “bleed” into one another.

- **Chorus & Reverb:**  
  - Activate chorus (FUNC + CHORUS) and reverb (FUNC + REVERB) for rich stereo depth.
  - Adjust chorus/reverb levels with FUNC + ARP TYPE (Chorus) and FUNC + ARP DIV (Reverb).

- **Modulate Algorithms:**  
  - In EDIT mode, Motion Sequence slow sweeps of the algorithm or feedback parameters for constantly-shifting harmonic content.

- **Sync & Layering:**  
  - Sync Volca FM2 to a slow external clock. Sequence chords or drones with eurorack MIDI control.
  - Stack several motion-sequenced pad programs in a CHAIN to create sustained, evolving ambient soundscapes.

- **Atmospheric FX:**  
  - Use FUNC + PROGRAM RANDOM to occasionally randomize sound programs for weird, evolving backgrounds—in a controlled, sparing manner for “ghostly” layers.

---

## **Extra Patch Ideas/Integration**

- **Layering:**  
  Use the Volca FM2 as a voice in a multi-timbral setup with other Eurorack sound sources. Layer its digital FM with analog VCOs for hybrid textures.

- **Realtime Performance Tweaks:**  
  Exploit the Touch Keyboard to inject pitch runs, trills, or glissandos amidst modulated sequences for more humanized, expressive performance.

- **Sample and Reprocess:**  
  Record Volca FM2 output, slice up in a sampler, and trigger with percussive sequencers—or pipe back through resonant filters, granular FX, etc.

---

## **Tips When Integrating with Eurorack**

- You *must* convert your modular signals—use MIDI or clock interfaces, as the Volca FM2 does not have native CV inputs.
- To control program parameters from Eurorack, use a MIDI-to-CV converter capable of automation or CC transmission.
- Consider battery or isolated power to avoid ground loops when integrating with large Eurorack rigs.

---

For detailed MIDI CC mappings and parameter explanations, [download the full Korg Volca FM2 manual here (PDF)](https://cdn.korg.com/us/support/download/files/9863546a1d7b52332efbfc68870ea464.pdf).

---

[**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)
