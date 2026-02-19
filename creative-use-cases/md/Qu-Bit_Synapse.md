# Qu-Bit — Synapse

- [Manual PDF](../../manuals/Synapse.pdf)

---

[Qu-Bit Synapse Manual PDF](https://qubitelectronix.com/wp-content/uploads/2020/08/Synapse-Manual-Web.pdf)

---

# Creative Eurorack Patch Ideas Using Qu-Bit Synapse

Qu-Bit Synapse is a powerful crossfading sequential switch and dynamic routing module with internal modulation and memory. The following creative patch ideas combine Synapse with other modules for dynamic, generative, and performative Eurorack results.

---

## 1. **Animated Four-Voice Mixer/Crossfader**

**Combo:**  
- Synapse  
- 4 Oscillators (e.g., Mutable Instruments Plaits, Make Noise STO)  
- Modulation (Function generator/Envelope, e.g., Make Noise Maths or Intellijel Quadrax)

**Patch Idea:**  
- Patch four different oscillator voices into Synapse’s A inputs, then connect an envelope or LFO (from Maths/Quadrax) to Synapse’s CV ins for crossfading.
- Use the Terminal encoder and memory recall to quickly switch between preset mix/fade scenes for live set transitions or morphing textures.

**Why This Works:**  
- Synapse allows morphing between complex multi-oscillator blends and recalling them as scenes, making it a powerful performance mixer.

---

## 2. **Morphing Modulation Source and Stored DC Voltages**

**Combo:**  
- Synapse  
- Function Generators (e.g., Make Noise Maths, ALM Pamela’s New Workout)
- Sequential/Voltage-Controlled Switch (e.g., Doepfer A-151)

**Patch Idea:**  
- Enable +5V DC offset on Synapse B inputs, turning Synapse into a programmable/stage-able multichannel modulation bank.
- Use stored scenes to step through preset voltage levels for modulation targets (filters, oscillators, VCAs).
- Use the sum output as a custom, programmable modulation source for other modules.

**Why This Works:**  
- This approach gives you a morphable, storable, and recallable set of LFOs, envelopes, or stepped voltages for sequenced or generative music.

---

## 3. **Dynamic Effects Routing & Spatialization**

**Combo:**  
- Synapse  
- FX Modules (e.g., Magneto, Strymon Starlab, Mutable Instruments Clouds)
- VCAs and Panning (e.g., Intellijel Planar)

**Patch Idea:**  
- Route audio from Synapse through various effects chains by assigning Synapse outputs to different effect modules, then sum or pan.
- Use the Scatter/Advance features to create random or rotating effect chains for unpredictable, evolving textures.
- Sequence memory locations live to create song arrangements or live “remix” effects.

**Why This Works:**  
- Synapse’s switching and spatialization capabilities let you build evolving soundscapes with shifting effects paths, panning, and mix scenes.

---

## 4. **Generative Patch Matrix**

**Combo:**  
- Synapse  
- Random/Chaos Modules (e.g., Make Noise Wogglebug, Mutable Instruments Marbles)
- Sequencers or Manual Controls (e.g., Turing Machine, Pressure Points)

**Patch Idea:**  
- Send random gates from Marbles or Wogglebug to Synapse’s Advance/Scatter inputs, shuffling routing of CV or audio for generative composition.
- Use stored scenes (memory locations) to constrain generative states to “musical” or performable settings, ensuring controlled chaos.

**Why This Works:**  
- This enables controlled generative routing, suitable for live performance, ambience, or evolving generative pieces.

---

## 5. **Voltage-Controlled Crossfade Waveshaper**

**Combo:**  
- Synapse  
- Wavetable/Complex Oscillators (e.g., Mutable Instruments Braids, Make Noise DPO)
- Filters/VCAs

**Patch Idea:**  
- Crossfade between a complex oscillator’s different outputs (sine, triangle, saw, wavefolded) using Synapse’s per-channel crossfade and internal LFOs.
- Sequence or modulate Synapse for timbral morphing from smooth to harsh textures on the fly.

**Why This Works:**  
- You get a hands-on, voltage-controlled waveshaper and complex timbre-morphing without patching and repatching.

---

## 6. **Pseudo-Sequencer or Custom Step Sequencing**

**Combo:**  
- Synapse  
- Euclidean/Rhythm Generators (e.g., Euclidean Circles, Pam’s New Workout)
- Quantizers/Sample & Hold (e.g., TipTop Quantizer, Doepfer A-148)

**Patch Idea:**  
- Use Synapse as a 4-step sequencer by enabling DC offsets or storing voltage levels per crossfade bank. Advance steps with rhythm triggers.
- Route outputs to pitch quantizer for pseudo-sequenced melodies. Combine this with A/B crossfades to add melodic or modulation variety.

**Why This Works:**  
- It offers clocked, storable CV or pitch patterns, giving unique sequences not found in traditional sequencers.

---

## 7. **Customizable Performance Macro Controller**

**Combo:**  
- Synapse  
- Macro Controllers (Expert Sleepers Super Disting EX, Mutable Instruments Frames)
- Output to multiple system destinations (filter, effect send levels, VCA control)

**Patch Idea:**  
- Use Synapse memory banks and sum outputs as a macro controls for quick, sweeping system changes—like preset morphing or sudden scene changes.
- Assign output sums to multiple system targets for dramatic, coordinated changes.

---

## General Module Type Recommendations

- **Oscillators:** For crossfading and waveshaping.
- **Sequencers/Random Sources:** For dynamic routing and memory bank modulation.
- **VCAs/Panners:** For spatial audio uses.
- **Effect Modules:** For diverse routing and morphing effects.
- **Modulation Sources:** To animate crossfade, switch positions, or inertia.

---

> [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)