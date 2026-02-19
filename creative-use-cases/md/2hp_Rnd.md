# 2hp — Rnd

- [Manual PDF](../../manuals/2hp_Rnd.pdf)

---

[2hp Rnd Manual PDF](https://2hp.com/wp-content/uploads/2023/10/Rnd2023.pdf)

---

## Creative Patch Ideas for the 2hp Rnd Module

The **2hp Rnd** is a compact, flexible random voltage and gate generator, capable of smooth and quantized random voltages, with independent attenuators for each output. Here are several creative ways to exploit its features in a modular synthesizer setup:

---

### 1. **Randomized Sequencing/Note Generation**
**Modules Required:**  
- Quantizer (e.g., Intellijel μScale, Disting Mk4, or any pitch quantizer)  
- Oscillator

#### Patch:
- Patch the **Quant Output** of Rnd to a quantizer, then route the quantizer CV out to your oscillator's V/OCT input.
- Use the clock input to sync new random notes with your drum patterns or sequencer.

**Result:**  
You get musically locked random melodies or basslines. Control the voltage range with the **Quant Attenuator** for more melodic or restricted results.

---

### 2. **Organic Modulation and Movement**
**Modules Required:**  
- Filter or effect processor (with CV-able parameters)
- Envelope generator

#### Patch:
- Send **Smooth Output** from Rnd to the cutoff CV input on a filter or the 'rate' input on an LFO or envelope.
- Adjust the Rate Knob for glacial sweeps or frenetic motion.

**Result:**  
Your timbres morph over time in organically unpredictable ways, creating ambient or evolving sonic textures.

---

### 3. **Randomized Rhythmic Gates**
**Modules Required:**  
- Percussion synth, drum modules, or envelope/LPG (Low-pass gate)

#### Patch:
- Set Int/Ext switch to **External**, patch a master clock to the Clock Input, and patch **Gate Output** to trigger percussion hits or envelopes.

**Result:**  
Rhythmic, probabilistic gate bursts for evolving, semi-random drum patterns or stuttering effects, especially great for glitch or generative music.

---

### 4. **Synchronized Random Voltage Bursts**
**Modules Required:**  
- Sample & hold module (optional)
- Sequencer

#### Patch:
- Use the Gate Output to trigger a sample & hold (if available), sampling either the Smooth or Quant outputs (or another random or modulating source).
- Sync the Rnd clock externally to your main sequencer for coordinated randomness.

**Result:**  
Per-step controlled chaos, with locked timing but unpredictable voltages.

---

### 5. **Randomized Effect Control**
**Modules Required:**  
- Delay, reverb, or multi-effect pedal/module with CV input

#### Patch:
- Send Smooth or Quant Output to an effect's CV input (e.g., delay time, feedback, reverb decay).

**Result:**  
Spatial effects that mutate and morph, especially lush and warped with slow, smooth randomization.

---

### 6. **Probability Clock Divider/Mangler**
**Modules Required:**  
- Clock dividers/multipliers or logic modules (e.g., Mutable Instruments Kinks, 4ms Rotating Clock Divider)
- Sequencer

#### Patch:
- Use Rnd's random gates to mask or combine with sequencer or LFO gates through OR/AND logic modules.
- Alternatively, create a “chance” passage in a song where events only occur if Rnd’s gate is high.

**Result:**  
Dividers and sequencers that become less predictable, great for generative structures and aleatoric music.

---

### 7. **Ideas for Stereo/Polyphonic Movement**
**Modules Required:**  
- Two independent voices/channels  
- VCAs or panning modules

#### Patch:
- Use Smooth for left channel modulation, Quant for right, or vice-versa.
- Or, scan between two different filters or FX paths with each random output.

**Result:**  
Evolving, stereo-random textures that animate a mix or patch.

---

## Bonus Tips
- **Attenuators are key:** 2hp Rnd’s built-in attenuators help keep modulation ranges under control for finer, more musical gestures.
- **Sync to a DAW/tempo source:** For “controlled” randomness, clock Rnd from your main clock so everything stays in time—perfect for live/structured jams.
- **Double up:** Use two Rnd modules for even more intricate modulation webs!

---

#### [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)