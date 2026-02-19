# Noise Engineering — Terci Ruina

- [Manual PDF](../../manuals/Terci Ruina - Noise Engineering Documentation.pdf)

---

[Terci Ruina Manual (PDF)](https://manuals.noiseengineering.us/tr/)

---

# Creative Patch Ideas for Terci Ruina — Noise Engineering

Terci Ruina is a triple-distortion module offering three distinct analog topologies, each with a unique character. Its compact size, normalization, and individual I/O make it an excellent candidate for wild sound design. Here are some creative ways to integrate it with other modules:

---

## 1. **Parallel Distortion & Layering**

- **Concept:** Use a mult or stackcable to split your sound (e.g. oscillator, drums) into Terci Ruina and a clean path.
- **Patch:** 
    - Oscillator → [Passive mult] → (1) Terci Ruina input FB / (2) Clean path
    - Terci Ruina output FZ + Clean path → [Mixer] (eg: Mutable Instruments Shades, or Doepfer A-138)
    - Result: Blend clean and distorted versions for increased punch while retaining clarity.
- **Advanced:** Add reverb (e.g. Mutable Instruments Clouds) post-mixer to create huge, cinematic textures.

---

## 2. **Feedback Mayhem**

- **Concept:** Patch the last output (FZ) back into the first input (FB) with attenuation/VCAs or a mixer in between.
- **Patch:** 
    - FZ Out → [VCA / Attenuator] → FB In
    - Add modulation to the VCA via LFO (eg: Make Noise Maths)
    - Input your main sound to FB In as usual, or leave external input unpatched for chaotic feedback oscillation.
- **Result:** Escalating, self-oscillating feedback textures. Modulate feedback amount for evolving noise beds.

---

## 3. **Distorted Percussion Madness**

- **Concept:** Run drum modules through the Terci Ruina and sequence the drive amounts with CV.
- **Patch:** 
    - Drum voice (e.g. Noise Engineering Basimilus Iteritas Alter, or Tiptop Audio 808 hats) → FB In
    - Patch through all three stages for brutal drum mangling.
    - Use a CV pedal like Befaco CV Thing or Intellijel Tetrapad to sequence/automate input levels or run post-TR into a VCA for gated/clocked noise bursts.
- **Result:** Full-on industrial/rave/techno drums with ever-changing grit.

---

## 4. **Routed Filter-Distortion Hybrids**

- **Concept:** Change the order of classic filters (lowpass, bandpass, etc.) and the Terci Ruina for new timbres.
- **Patch A:** VCO → Filter (e.g. Erica Synths Polivoks, Doepfer A-124 Wasp) → Terci Ruina (try only FF for smooth saturation or FB for asymmetry)
- **Patch B:** VCO → Terci Ruina → Filter
    - Envelope (e.g. ALM Pip Slope II) modulates filter cutoff for acid lines.
- **Result:** Acidic leads, modulated bass, and unreal textures—each order provides distinct coloration.

---

## 5. **Voltage-Controlled Distortion FX**

- **Concept:** Use the normalization breakpoints and insert VCAs or crossfaders (e.g. XAOC Devices Tallin, Happy Nerding 3x VCA) between stages, or use an envelope follower (Mutable Instruments Ears, Intellijel Dual EnvF) to dynamically process the distortion stages based on incoming audio.
- **Result:** Responsive, touch-sensitive, or envelope-driven distortion that reacts to your playing or the audio dynamics.

---

## 6. **Stereo/Spatial Destruction**

- **Concept:** Use two Terci Ruinas for stereo processing, one per channel, but patch their internal routing differently (e.g. L channel: FB→FF→FZ, R channel: FZ→FB→FF).
- **Patch:** 
    - Mix processed stereo signals with a stereo field mixer (e.g. Befaco STMix).
    - Optional: Cross-patch L-to-R feedback for utter spatial chaos.
- **Result:** Asymmetrical stereo distortion with dramatic imaging.

---

## 7. **CV-Modulated Automated Destruction**

- **Concept:** Use stepped/random voltages (e.g. Make Noise Wogglebug, Mutable Instruments Marbles) to control drive levels via external VCAs and offset mixers.
- **Result:** Glitchy, morphing distortion that constantly evolves.

---

## 8. **Post-Processing: Reverb, Delay, Granular**

- **Concept:** After Terci Ruina, route into modules like:
    - Make Noise Mimeophon (delay)
    - Mutable Instruments Clouds (granular)
    - Noise Engineering Desmodus Versio (reverb)
- **Result:** Epic, textural soundscapes — huge, washy terror drones, or shredded ambient pads.

---

## 9. **Terci Ruina as a Chaotic CV Shaper**

- **Concept:** Feed LFOs, envelopes, or stepped random voltages through the distortion circuits, then use the output to modulate other parameters (filter cutoff, oscillator waveshape, etc.).
- **Result:** Create modulations with aggressive and nonlinear shapes — ideal for complex, organic-sounding movement.

---

## Module Pairing Suggestions

- Filters: **Erica Synths Polivoks**, **Doepfer A-124 Wasp**, **Mutable Ripples**
- VCAs: **Happy Nerding 3xVCA**, **Intellijel Quad VCA**
- Mixers: **Mutable Shades**, **Doepfer A-138**
- Utilities: **Make Noise Maths**, **Intellijel Quadratt 1U**
- Effects: **Desmodus Versio**, **Mimeophon**, **Clouds**
- Drum Modules: **BIA**, **Tiptop Audio One**
- Random/Chaos: **Wogglebug**, **Marbles**

---

Take advantage of the per-stage inputs/outputs and normalization to experiment with non-standard routing. The chaos-eager nature of Terci Ruina means creative "abuse" will often lead to the wildest results!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)