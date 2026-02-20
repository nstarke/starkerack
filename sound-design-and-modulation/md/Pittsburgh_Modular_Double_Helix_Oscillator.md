# Pittsburgh Modular — Double Helix Oscillator

- [Manual PDF](../../manuals/Lifeforms Double Helix Oscillator - Pittsburgh Modular Synthesizers.pdf)

---

[**Double Helix Oscillator Manual (PDF)**](https://pittsburghmodular.com/_files/ugd/8c5a62_051cb80cceb24111b90c88a9214e48e0.pdf)

---

# **Creative Sound Design with the Lifeforms Double Helix Oscillator**

The Pittsburgh Modular Lifeforms Double Helix Oscillator is an exceptionally versatile **analog dual oscillator** voice with a built-in wavefolder, low pass gate, modulation sources, and voltage-controlled modulation matrix. Its architecture makes it perfect for exploring deep modulation, percussive timbres, complex bass sounds, and lush pads. Below are detailed patching and modulation strategies tailored to the sound categories you mentioned.

---

## **1. Distorted Percussive Sounds**

### **Key Techniques**
- **Wavefolder & Gate**: Use the contour section (wavefolder + LPG) for sharp, harmonically rich "plucks" and hits.
- **Impulse Input**: Use for striking the low pass gate to get a percussive decay.
- **FM/AM Modulation**: Increase harmonics/distortion with FM, and use modulation matrix for dynamic, rhythmic movement.

### **Example Patch**
- Send a trigger (from a sequencer or clock divider) into the **Impulse Input** of the **Contour Section** to “strike” the LPG for every hit.
- Patch the **Primary Oscillator’s Saw or Blade Wave** into the **In 1** of the contour.
- Increase the **Timbre** and modulate it using an LFO or stepped random from the modulation section for animated percussive transients.
- Set the **Dynamics Response** to taste for decay length.
- Add **FM from Oscillator 2** set as an LFO or in audio-rate; route this via the modulation matrix and vary the amount using CV for added distortion/texture.
- Patch **Noise Output** into a second input or use as a modulation source to add grit.

---

## **2. Crazy Dubstep/Drum & Bass Basslines**

### **Key Techniques**
- **Audio-rate FM**: Metallic, tearing bass sounds depend on modulating one oscillator with another at audio rates.
- **Wavefolder**: Further multiplies harmonics for that aggressive edge.
- **Voltage Controlled Routers**: Automate modulation amounts/crossfade between sources for rhythmic, evolving movement.

### **Example Patch**
- **Carrier**: Patch Primary Oscillator (Saw or Blade) through the contour section.
- **Modulator**: Set Secondary Oscillator to audio rates (octave(s) higher or lower), patch its sine output to **FM Input** of the Primary.
- Use the **FM CV Knob** and the **FM 1 Source Switch** to crossfade/modulate the amount via the VCR channels (A/B), using additional envelopes, LFOs, or random CV for movement ("wobble").
- **Route modulation**: Sequence the FM index, the wavefolder timbre, or the LPG dynamics simultaneously for layered, organic bass morphs.
- **Sub Bass**: Mix in or process the **Sub Output** (octave down square) for deep fundamentals.
- **LPG for punch**: Strike the LPG with a trigger, and modulate the **Dynamics** for each note hit, mimicking a bass pluck.

---

## **3. Haunting Atmospheric Pads**

### **Key Techniques**
- **Dual Oscillators Detuned**: Use both oscillators, slightly detuned for thick “chorus” effect.
- **Contour (Wavefolder + LPG)**: Morph between sine and complex harmonics for evolving timbres.
- **Slow Modulation**: Leverage built-in LFO, random, and mod matrix for slow-moving, evolving control of timbre, FM, and LPG.
- **Noise**: Subtle layering or mod source for texture.

### **Example Patch**
- Set both oscillators to similar pitches, detune slightly for movement, output both to the contour section’s mixer.
- Set **wavefolder timbre** low for initial purity, then slowly modulate via the **Timbre CV** (using slow LFO or random).
- Use the LPG’s **Dynamics Response** for a slow attack/decay shape; envelope the **Dynamics** with an external or internal source.
- Patch **Noise** (subtle!) to modulate **FM or Dynamics** for a hint of unpredictability.
- Routinely modulate all major CV-ins (FM, Timbre, Dynamics) via the voltage controlled routers, switching sources over time (A/B/Off) for organic drift.
- Layer external effects (reverb, delay), but the LPG already imparts some “natural” smoothing.

---

## **Modulation Matrix Tips**

- Both VCR channels can take any CV or audio signal, modulating all the main points (FM 1/2, Blade|Pulse, Timbre, Dynamics).
- Use the router source switches to automate switching between modulation sources (e.g., switch from LFO to random, or stack them).
- Use the **Random Output** for unpredictable, haunting or glitchy modulations.
- **Self-patch**: Use outputs from the oscillators or modulation section—aim for “West Coast” flavor with internal feedback, self-modulation, and routed CV.

---

### **General Pro Tips**
- **Dynamic Modulation**: Use external envelopes to modulate VCR A/B Level or patch those to LPG/Folder for synth voices with a sense of movement.
- **Try Feedback**: Out from contour back into modulator input, controlled via the router, for over-the-top chaos.
- **Mix**: Both oscillators/LPG outputs—layer them for hybrid textures.

---

> For deeper exploration, consult the full [Double Helix Oscillator Manual (PDF)](https://pittsburghmodular.com/_files/ugd/8c5a62_051cb80cceb24111b90c88a9214e48e0.pdf).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
