# Intellijel — Plonk

- [Manual PDF](../../manuals/plonk_manual_v1.16_2020.11.08.pdf)

---

[Download the Plonk Manual PDF](https://intellijel.com/downloads/manuals/plonk_manual_1.16.pdf)

---

# Modulating Plonk for Unique Sounds

As a eurorack modular synthesizer musician, Plonk is a powerhouse for creative percussive, bass, and atmospheric sound design. Here’s how you can push it into wild, textured, and expressive sonic territory by leveraging its modulation capabilities.

## Key Plonk Modulation Possibilities

Plonk features dedicated CV inputs and assignable modulation destinations for X, Y, and MOD inputs, each with attenuverters and flexible routing. Each input can hit a wide parameter range, and the combination with morphing, randomizing, and FX (saturation/bitcrushing) makes for unlimited possibilities.

---

## 1. **Distorted Percussive Sounds**

**Core Techniques:**

- **Saturation & Bitcrusher:**  
  Plonk has built-in saturation (distortion) and bitcrusher effects, assignable to X, Y, or MOD. Use these to roughen up percussive timbres.
- **Noise Parameters:**  
  Manipulate Noise Attack, Decay, Density, and filter settings, especially with high Noise Density, to get grainy, digital-harsh noise—a drum machine “breaking.”
- **Randomization:**  
  Set MOD destination to Randomize and trigger it rhythmically for each hit: you’ll get a load of janky, evolving drum sounds.

**Patch Example:**

- Assign **X** or **Y** to `Saturation` and crank an LFO or envelope into the input, *also* add CV to `Bitcrusher` for sample rate reduction “crunch.”
- Layer percussive noise by increasing both Mallet and Noise in the exciter Mix—modulate between them using the X or Y input.
- Use external gates on MOD input assigned to `Choke Both` or `Choke Noise` for gated, truncated “machine gun” textures.

**Extra Tips:**

- Try quick envelopes on MOD input routed to `Randomize` for constantly changing hats or snares.
- Assign X or Y CV to Exciter parameters for shifting between soft and harsh mallet sounds in real time.

---

## 2. **Crazy Basslines (Dubstep, Drum & Bass)**

**Core Techniques:**

- **Pitch Modulation (FM):**  
  Assign MOD, X, or Y to `R Pitch` (Resonator Pitch) for fast, audio-rate or wobbly pitch movement (FM basses).
- **Morph:**  
  Use MOD input set to `Morph`, interpolate between two heavily-distorted, bitcrushed bass patches, controlled by an LFO, envelope, or sequencer CV.
- **Resonator Inharmonicity:**  
  Modulate `R Inharmonic` deeply for metallic or bell-like wubs and extra “growl.”
- **Velocity to Dynamics:**  
  Set VEL Mode to `dynamics` so how hard you trigger influences percussiveness and growl.

**Patch Example:**

- Assign MOD to `Morph`, select two very different bass sounds (e.g., pure sine + noise distorted), then put a slow triangle LFO or stepped random CV into MOD.
- Assign X and Y to `Saturation` and `R Inharmonic` and sweep while sequencing pitch from a keyboard or sequencer.
- Use a fast envelope on MOD assigned to `Bitcrusher` for aggressive digital attack on each bass note.

**Extra Tips:**

- Assign X/Y CV to `Resonator Decay` and `Resonator Tone` for movement from plucky to sustained, and warm to cold metallic.
- Route VEL input to a stepped/random source for unpredictable note accents.

---

## 3. **Haunting Atmospheric Pads**

**Core Techniques:**

- **Long Decays:**  
  Turn up the DECAY knob and modulate `Resonator Decay` and `Noise Decay` for wash and breath.
- **Polyphony:**  
  Enable 2-voice polyphony to allow overlapping, echoing pad layers.
- **Morphing:**  
  MOD input to `Morph`—sweep between two subtle pad timbres for evolving textures.
- **Resonator Position & Tone:**  
  Slowly modulate `Position` (X) to move the excitation point, great for organic swells.
- **Filter Movements:**  
  Assign Y to `Noise Lowpass Cutoff` or Envelope, sending slow LFO or manual sweeps.

**Patch Example:**

- Assign X to `R Position`, MOD to `Morph` (between two ethereal pads), Y to `Noise LP Cutoff`. Feed all three with ultra-slow LFOs or slowly changing voltages.
- Engage high polyphony, set VEL mode to `volume` and modulate VEL with a slowly-varying CV for dynamic fade in and out.
- Keep `Saturation` and `Bitcrusher` low for clarity, or add a touch for ghostly artifacts.

**Extra Tips:**

- Try external random/chaos sources into MOD input for unpredictable, living atmospheres.
- Use high `Noise Density` with modulated filters for wind/rain/noise-like beds.

---

## **Further Creative Patch Notes**

- **Preset Step Sequencing:** Chain multiple percussion/instrument sounds by MOD input set to `Preset Step`, and scan through kits using a sequencer or S&H/random source.
- **Choke Tricks:** Use external gates to the MOD input (set to `Choke` options) to build dynamic hi-hat open/close, or to cut off long atmospheric tails abruptly for tension.

---

Plonk’s open modulation routing—with any knob assignable to X, Y, or MOD, plus CV summing and deep menu options—makes it an ultra-flexible hub for everything from analog drums to digital weirdness, deep bass wubs to spectral pads. The real magic comes from combining unique parameter mappings per patch, using the MOD input for performance automation, and blending physical modeling with digital destruction!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)