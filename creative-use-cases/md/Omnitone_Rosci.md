# Omnitone — Rosci

- [Manual PDF](../../manuals/Rosci-Manual.pdf)

---

[Rosci User Manual PDF](https://omnitone.ca/rosci/manual.pdf)

---

# Rosci Creative Integration Guide

As a fellow Eurorack musician, here are some inspiring and creative ways to combine the **Rosci** oscillator with other modules, based on its capabilities detailed above.

## 1. Complex CV Animation

**Rosci's Parameter CV Inputs (Complexity, Roundness, Harmonics, Formants, Detune)** cover a broad range (±10V), and the modulation is summed with onboard controls.  
**Try:**  
- Patching LFOs (like Make Noise Maths or Intellijel Quadrax) to modulate roundness or harmonics, automating spectral evolution.
- Use a random voltage source (Mutable Instruments Marbles, Wogglebug, Turing Machine) to “morph” between vowel-like formants for generative voice-esque timbres.

## 2. Audio Rate Modulation

Because Rosci accepts CVs up to audio rates, try feeding audio sources (oscillators, noise, or drum triggers) into its modulation inputs.  
**Ideas:**
- **FM Synthesis:** Send a VCO (e.g., Dixie II+) through an attenuator into the Detune input for audio-rate detuning/phase modulation.
- **Wavefolding:** Patch sharp envelopes or pulses into complexity/harmonics for dynamic “wave-shaping.”

## 3. Sequenced Timbre Animation

Use sequencers (like Make Noise René, Tiptop Z8000, or Erica Synths Black Sequencer) to send stepped voltages into the Roundness or Complexity input, making each note a discrete timbral snapshot.

## 4. LFO Mode: Unique Modulator

Switch Rosci to LFO mode and send its output to other module CV inputs:
- **Filter Cutoff/Resonance:** Modulate your favorite filter with a “voice-like” LFO for organic sweeps (e.g., Mutable Ripples, Doepfer SEM).
- **Wavefolder or VCA:** Animate a wavefolder’s symmetry or a VCA’s gain for FM/rhythmic stutter effects.
- With full CV-able waveform morphing in LFO mode, Rosci becomes a “meta-LFO,” changing shape as it modulates other parameters.

## 5. Harmonic Drone Machine

Set up multiple modulation sources (LFOs, sequencers) targeting each harmonic, roundness, and complexity input.  
- **Tip:** Mult output audio to a mixer; use crossfaders or VCAs (Doepfer A-135-2, Mutable Veils) to fade between Rosci and other oscillators.

## 6. Envelope-Driven SFX

Patch envelopes (e.g., Maths, Intellijel Quad Envelope) into Formant, Roundness, or Harmonics, synced to triggers from your sequencer or gate generator. This will make the timbre dynamically “talk” or shift with each note, ideal for expressive effects or percussion synthesis.

## 7. Experiment With Quantizers

After generating evolving or random voltages to modulate rosci’s pitch or parameters, use a quantizer (Intellijel Scales, Doepfer A-156) to keep things musical and in-scale, especially when using Rosci melodically.

## 8. Oscillator Sync and Cross-Patching

Use Rosci as the master or slave in an oscillator sync arrangement. The unique, morphing waveforms will provide unusual synced tones when paired with a classic analog VCO.  
- **Try:** Output from Rosci to the sync input of another oscillator, or vice versa.

## 9. Feedback Synthesis

Route Rosci’s output through effects (like Desmodus Versio reverb or Make Noise Mimeophon delay), then back into a modulation input for complex, evolving self-patched feedback textures.

---

## Recommended Module Types For Creative Pairing
- **Random Generators:** Marbles, Wogglebug, Turing Machine
- **LFOs/Function Generators:** Maths, Quadrax, Batumi
- **Sequencers:** René, Z8000, Black Sequencer
- **Envelopes:** Quadra, Contour, Function
- **VCAs/Mixers:** Veils, A-135-2, Blinds
- **Quantizers:** Scales, A-156
- **Classic VCOs:** Dixie II+, STO, A-110
- **Filters:** Ripples, Polaris, Three Sisters

---

## Manual & Resources
- [Rosci User Manual PDF](https://omnitone.ca/rosci/manual.pdf)  
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)