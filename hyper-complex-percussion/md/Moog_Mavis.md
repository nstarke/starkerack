# Moog — Mavis

- [Manual PDF](../../manuals/MAVIS_MANUAL_V2_06.27.2022.pdf)

---

[Moog Mavis User Manual PDF](https://www.moogmusic.com/sites/default/files/2022-06/Mavis_Manual_1.4_Web.pdf)

---

# Using Moog Mavis for Densely Rhythmic, Complex Percussion in Eurorack

The **Moog Mavis** is a powerful analog synth voice and utility module that, when integrated with Eurorack, can deliver unique, punchy, and percussive sounds for hyper-complex rhythmic explorations. Here’s how to unlock its potential for polyrhythmic, polymetric, and rhythmically dense percussion patterns:

---

## 1. Mavis as a Percussive Voice

### a. Short Envelopes for Percussion
- **Patch**: Set the Envelope Generator’s Attack and Release to minimum. Keep the Decay low and Sustain at zero, or low for snappy triggers.
  - **Use**: Patch external triggers/random gates to the **GATE** input. Every trigger generates a sharp percussive blip—good for short analog kicks, blips, snaps, or hats.

### b. Self-Oscillating Filter “Ping” Percussion
- **Technique**: Turn the Filter **Resonance** to maximum or near maximum. Patch an envelope or sharp CV pulse into the **CUTOFF** input to "ping" the filter into self-oscillation.
  - **Result**: Generates analog “conga”, “bongo”, or woodblock style percussion sounds, especially when modulated at audio rate.

### c. VCO Hard/Soft Edges for Noise
- **Noise Percussion**: Use the pulse or saw waveform and modulate the Pulse Width for more noise-like, metallic percussive attacks.
- **Patch**: Route the VCO output through the **Wave Folder** for aggressive, harmonically rich percussion.

---

## 2. Modulation for Complex Rhythms

### a. Sample & Hold: Rhythmic Modulation Source
- Patch random/stepped CV from the **S+H OUT** to any mod destination (VCO pitch, VCF cutoff, or VCA level).
- Trigger S+H with a non-square clock or irregular gate sequence (from external clock dividers, logic, or sequencers) for **nonlinear, or polyrhythmic patterns**.
- Route S+H output to VCF CUTOFF or VCO PITCH for glitchy, percussive pitch/filter jumps.

### b. LFO Audio Rate & Cross-Modulation
- The LFO can run at audio rates (up to 550Hz). For *FM drum* effects, patch the LFO out to the VCO’s pitch, or the VCF’s cutoff.
- Use the LFO RATE CV input and fire it from erratic clocks, random gates, or complex clock multipliers for unpredictable or polyrhythmic movement.

---

## 3. External Sequencing and Polyrhythmic Gate Sources

- **GATE input**: Accepts external rhythmic triggers; sequence Mavis from a clock divider, logic module, or a polyrhythmic gate generator.
- Layer patterns by sending multiple independent clocks/gates through a logic module that merges them, then patch to Mavis GATE.

---

## 4. Layered and Stacked Percussion (Mix & Mult)

- Use the onboard **Mixer** and **MULT** to:
  - Combine Mavis’s output with other voices (or itself via feedback patches).
  - Duplicate a random/unusual modulation source (from S+H or LFO) and send to both pitch and filter for “macro” percussion changes.
  - Feedback the **Wave Folded** output or filtered output back into the Mixer for drone/percussion hybrids or “FM percussion”.

---

## 5. Unique FX—Wave Folding and Feedback

- **Wave Folder**: Not usually present in analog monosynths. Patch any percussive signal (from Mavis or external) into **FOLD IN** and modulate the FOLD depth (manually or by CV) for snappy, complex, and harmonically saturated electronic percussion.
- Combine with high resonance, tight envelopes, and modulated pitch for full-spectrum digital-esque percussion.

---

## 6. Patch Ideas for Advanced Rhythmic Percussion

### Polyrhythmic Filter Ping
- Patch two (or more) clocks/gates (with different divisions/lengths) into logic, sum to GATE IN.
- Modulate filter cutoff by fast S+H or LFO, set resonance high.

### Pseudo-Granular Percussion
- Use S+H or LFO, set to irregular triggers, and patch to VCA CV.
- Fire GATE with clock dividers on different timebases (e.g., /5 against /7).

### Harmonic “Metallic” Percussion
- Use VCO saw → Wave Folder → VCF high resonance, pinged by envelope.
- LFO and S+H mixed (via Mixer) to modulate both cut and pitch—creates atonal, metallic textures.

### External CV and Sequencing
- Use external Eurorack sequencers to send *non-standard* gate and cv voltage sequences (Euclidean rhythms, probability-based steppers, function generators).

---

## General Tips for Punch & Uniqueness

- Use the **Envelope’s Attack/Decay/Release in the sub-10ms range** for super-punchy enclaves.
- Use the **Attenuator** to shape modulation amounts, making motion more or less extreme.
- Exploit **unusual waveforms (combined saw/pulse, folded, FM)** for nonstandard percussion timbres.
- Sync multiple Mavis with other Eurorack voices or percussion modules for polymetric layers.

---

**[Full Moog Mavis User Manual PDF](https://www.moogmusic.com/sites/default/files/2022-06/Mavis_Manual_1.4_Web.pdf)**

---
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)