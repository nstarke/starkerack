# Buchla and Tiptop Audio — 266t Source of Uncertainty

- [Manual PDF](../../manuals/Buchla_&_Tiptop_Audio_266t.pdf)

---

[**Buchla 266t "Source of Uncertainty" Eurorack Manual (PDF)**](https://www.tiptopaudio.com/manuals/266t-manual.pdf)

---

# Creative Sound Design with the Buchla 266t "Source of Uncertainty"

With the wide variety of noise, random, and voltage processing sections in the 266t, you can craft wild percussive tones, aggressive basslines, and evolving pad textures that thrive in experimental or heavy electronic genres.

Below, you'll find modulation routing tips and patch ideas for distorted percussion, dubstep/DnB basslines, and haunting atmospheres.

---

## 1. **Distorted Percussive Sounds**

**Key Utilities:**  
- **Noise Source (White/Blue)**
- **Sample and Hold**  
- **Quantized/Stored Random Voltage**
- **Integrator**

### *Patch Techniques*

- **Kick & Snare Transients:**
  - Use the **White Noise Output** for the core audio signal—route through a VCA and envelope.
  - Heavily modulate pitch/frequency of your VCO (or filter cutoff) with the **Quantized Random Voltage** to create dirty, unstable percussive hits.
  - Run percussive envelopes through the **Integrator** with a **very low smoothing** for clicky attacks, or crank up smoothing for impulse "thumps."

- **Crunched Hats & Distorted Textures:**
  - Trigger the **Sample and Hold** with a fast clock (audio rate for digital-bit noise or ~16th notes for broken hats).
  - Sample the **Pink or White Noise** for each trigger—out --> highpass filter --> overdrive for instant industrial hats.
  - Feed CV from **Fluctuating Random Voltages** to modulate VCF cutoff or VCA amplitude on each hat/snare hit for variation.

---

## 2. **Crazy Basslines (Dubstep/Drum & Bass Style)**

**Key Utilities:**  
- **Fluctuating Random Voltages**
- **Stored Random** & **Quantized Random Voltage**  
- **Integrator**

### *Patch Techniques*

- **Wobble Bass Modulation:**
  - Use the **Quantized Random Voltage** or **Stored Random Voltage "n+1" mode** to generate voltage steps—patch to your bass oscillator's waveshaper/wavetable position, filter cutoff, or distortion amount.
  - Ping the random source with a rhythmic clock derived from your main groove.
  - Roll the "number of steps" knob to 2 or 3 for classic stepped bass movements, go up to 6 for glitchier lines.

- **Organic Step-Sequencing:**
  - Combine **Sample and Hold** outputting stepped voltages (sampled from Fluctuating Random) to modulate various bass synth parameters each time you trigger a note.
  - Smooth the random voltages with the **Integrator** for gliding, sick "portamento" style modulations.

- **Growl & Saturation:**
  - Use **Pink or Blue Noise** as an oscillator layer for aggressive texture or as a modulation source for FM-ing your main bass.
  - Modulate distortion unit CVs with the **Fluctuating Random Output,** creating unstable, unpredictable grit.

---

## 3. **Haunting Atmospheric Pad Sounds**

**Key Utilities:**  
- **Fluctuating Random Voltages**
- **Stored Random (Curved distribution)**
- **Integrator**

### *Patch Techniques*

- **Evolving Motion:**
  - Slowly modulate VCO pitch, filter cutoff, panning, or effect depths with the **Fluctuating Random Voltages** output; set the knob for slow rates (0.05–2 Hz).
  - Use the **Integrator** with a high smoothing setting; let the voltage morph gently for lush pads.

- **Otherworldly Harmonics:**
  - The **Stored Random Voltage (right output, skewed by knob and CV in)** can serve as a modulation source for harmonic CVs, reverb mix, vibrato amount, or delay time.
  - Try dialing in "low skew" for evolving sub drones, or "high skew" for shimmering top-end movement.

- **Ghostly Filter/EQ Automations:**
  - Modulate multi-mode filter resonance or bandpass position with the **Fluctuating Random CV** for spectral shifts.
  - Sample and hold slow random voltages to periodically shift patch characteristics without predictable looping.

---

## Expert Tips

- **Randomizing Everything:**  
  Use multiple S&H and random outs to hit every available modulation input for controlled chaos—tune ranges carefully for musicality.

- **Pinging the Integrator:**  
  For stepped proggy effects, feed clocked stepped sources into the **Integrator** and mess with smoothing live with CV.

- **LEDs = Visual Feedback:**  
  Watch the LEDs to get a sense of rate and voltage movement—it helps dial in the character you want.

---

**HAPPY PATCHING!**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)