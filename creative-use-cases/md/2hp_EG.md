# 2hp — EG

- [Manual PDF](../../manuals/EG_Manual-7ja4.pdf)

---

[Download the 2hp EG Eurorack Envelope Generator Manual (PDF)](https://2hp.com/uploads/1/0/1/3/101370584/eg_manual.pdf)

---

# Creative Patch Ideas with the 2hp EG Envelope Generator

The **2hp EG** is a compact and versatile two-stage envelope generator with some unique capabilities. Here are several creative ways to utilize it in your Eurorack system, referencing its features as described in the manual:

---

## 1. Dynamic Percussive Voice

**Modules Needed:**  
- Drum module (e.g., Erica Synths Pico Drums, Mutable Instruments Peaks)
- VCA (e.g., Intellijel Quad VCA)

**Patch Idea:** Use EG to shape percussive drum hits by patching its envelope output to the VCA that controls the amplitude of your drum sound. Try experimenting with linear vs. exponential curves for punchy vs. snappy drum envelopes. Use the ATTACK CV input with another envelope or LFO to morph from a tight to a slightly softer drum transient, simulating acoustic drum dynamics.

---

## 2. Snappy Basslines with Modulated Decay

**Modules Needed:**  
- Analog oscillator (e.g., Doepfer A-110)
- Filter (e.g., Mutable Instruments Ripples)
- VCA

**Patch Idea:** Use EG to open your VCA or filter. Patch a sequencer or trigger source (e.g., Arturia BeatStep, Pamela’s New Workout) to EG’s TRIG. Use an LFO into DECAY CV to shift envelope length for varying note articulation. Use the module’s attenuator to dial the desired envelope depth/impact.

---

## 3. Envelope-Controlled Modulation Source

**Modules Needed:**  
- Anything with a CV input (filters, waveshapers, effects modules; e.g., Xaoc Belgrad, Happy Nerding FX Aid)

**Patch Idea:** Use EG not only for amplitude but also as a modulation source. Patch OUT to modulate a filter cutoff or FX parameter. Flip between linear and exponential shapes for vastly different modulation feels: linear for steady sweeps, exponential for quick attacks and gentle tails. The wide time range (3ms to 11 minutes!) lets you go from percussive to extremely slow modulations.

---

## 4. Generative Dynamics in Ambient Patches

**Modules Needed:**  
- Random generator (e.g., Mutable Instruments Marbles)
- Sound source
- Reverb/delay (e.g., Make Noise Mimeophon)

**Patch Idea:** Connect a random trigger generator to TRIG. Use additional random or slowly modulating voltages into ATTACK and DECAY CV to create evolving, organic amplitude envelopes. Great for pads or drones. Attenuate the envelope or increase the length of stages for lush, morphing textures.

---

## 5. Envelope Shaping for Modular FX

**Modules Needed:**  
- Effect module with CV (e.g., delay/reverb)
- VCA

**Patch Idea:** Use EG to duck reverb or delay returns (sidechaining) by patching OUT to modulate a VCA in the FX return path. Trigger it from your kick drum triggers for a classic "pumping" effect. Use the exponential mode for a punchy effect.

---

## 6. Transient Shaping for External Audio

**Modules Needed:**  
- External audio input module (e.g., ALM S.B.G or Intellijel Audio Interface)
- VCA

**Patch Idea:** Use your EG to create a *pseudo-compressor* effect. Patch an envelope follower into TRIG and use it to gate or shape external drum loops or vocals through a VCA, letting you impart modular envelopes onto any sound source.

---

## 7. CV-Controllable Envelope Slicing

**Modules Needed:**  
- Sequential switch or logic module (e.g., Doepfer A-151)
- Multiple EGs (chained or combined with other envelopes)

**Patch Idea:** Use CV control over ATTACK and DECAY to create evolving envelopes. Use a switch/logic module to alternate between different EG settings for complex modulation and per-step envelope variety.

---

## Generic Module Pairing Recommendations

- **Sequencers:** For rhythmic or melodic gating/triggering (e.g., Make Noise René, Arturia Keystep)
- **LFOs or Random CV:** For dynamic ATTACK/DECAY CV modulation (e.g., ALM Pam’s New Workout, Mutable Instruments Tides)
- **VCAs:** For traditional amplitude shaping or voltage-controlled modulation routing
- **Utilities (attenuverters, mixers):** For combining EG with other mod sources, complex modulation generation

---

Explore the **EG’s** ultra-wide envelope ranges, CV control, and compact footprint in both basic and advanced patches!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)