# Moog — Subharmonicon

- [Manual PDF](../../manuals/Subharmonicon_Manual.pdf)

---

[Moog Subharmonicon User Manual (PDF)](https://www.moogmusic.com/sites/default/files/2022-01/Subharmonicon_Manual_v1.pdf)

---

# Creative Eurorack Patching Ideas  
## Using the Moog Subharmonicon with Modular Synthesizers

The **Moog Subharmonicon** is a unique analog polyrhythmic semi-modular synthesizer, excelling in generating subharmonic undertones and intricate polyrhythms. Its extensive patchbay (32 points: 17 ins/15 outs, CV/audio-compatible) opens broad creative potential in a Eurorack system. Below are ways to leverage its features with other modules—specific and generic—plus patch ideas for expanding its sonic territory.

---

## 1. Expand Subharmonic Voices
### *Patch Idea:*  
- Take VCO 1/2 or SUB 1/2 audio outputs and route them to external waveshapers (e.g., [Intellijel Bifold](https://intellijel.com/shop/eurorack/bifold/) or [WMD Geiger Counter](https://wmdevices.com/products/geiger-counter-eurorack)).
- Use the individual outs to feed external filters—parallel them with the Subharmonicon’s filter for “multi-filter” timbres (e.g., [Make Noise QPAS](https://www.makenoisemusic.com/modules/qpas)).

**Benefit:**  
Layer subharmonics with different textures, stereo positions, or process just subs for massive growls, percussive depths, or evolving spectral composites.

---

## 2. Polyrhythmic Control Over Other Modules
### *Patch Idea:*  
- Use SEQ 1 CLK and SEQ 2 CLK outputs to clock external sequencers ([Mutable Instruments Marbles](https://mutable-instruments.net/modules/marbles/manual/) or [Pamela’s Pro Workout](https://busycircuits.com/alm017/) for extra modulation/rhythm layers).
- Send CLOCK OUT (or polyrhythmic triggers) to drum modules (e.g., [2hp Kick/Snare](https://2hp.com/products/kick), [Jomox ModBase](https://jomox.de/modbase09.php?lang=en)) or sample players.

**Benefit:**  
Build layered, evolving polyrhythmic patterns—Subharmonicon can “drive” the pulse and/or complex groove logic of your whole system.

---

## 3. Intricate CV Cross-Patching & Logic
### *Patch Idea:*  
- Self-patch CV outs (e.g., SEQ, EG, or clock) to rhythm CV ins to create generative rhythmic movement.  
- Send VCA EG or VCF EG OUT to modulate parameters in other modules, such as Morphagene’s Morph CV or FX parameters in [Tiptop Z-DSP](https://tiptopaudio.com/z-dsp/).
- Take external gate logic (e.g., XOR from a [Doepfer A-166-2](https://doepfer.de/a1662.htm)) to the PLAY or RESET input—Subharmonicon as a polyrhythmic performer, modulated by evolving patch logic.

**Benefit:**  
Interconnective generative-patch techniques make your Subharmonicon a modular heart of an evolving composition or live system.

---

## 4. External Modulation & Randomness
### *Patch Idea:*  
- Patch LFOs/S&H/random CVs (e.g., [Make Noise Maths](https://makenoisemusic.com/modules/maths), [Mutable Tides](https://mutable-instruments.net/modules/tides/manual/)) to VCO or subharmonic CV ins for unconventional microtonal or fluctuating undertone divisions.
- Use complex envelopes or DAW-controlled CV sequencers (cv.OCD, Expert Sleepers modules) to “play” Subharmonicon’s parameters in sync with external systems.

**Benefit:**  
Infuse organic expressions—wobbly rhythms, generative tuning shifts, controlled chaos—blurring the line between “melody” and “modulation.”

---

## 5. Eurorack Integration as a Sequencer/Modulator
### *Patch Idea:*  
- Use SEQ outputs to modulate oscillator pitch, filter cutoff, or effect depth in entirely different modules (e.g., send SEQ 1 OUT to the DPO’s 1V/oct in and SEQ 2 OUT to a quantizer and then LPG).
- Use MIDI input (with a Type A 3.5mm adapter) to clock/gate Subharmonicon, synchronized with DAW or other MIDI hardware—expand Subharmonicon’s role as a part of a hybrid setup.

**Benefit:**  
Subharmonicon is not just a sound source but an expressive polyrhythmic CV/gate generator, integrating with broader modular or hybrid environments.

---

## 6. Stereo and Spatial Experimentation
### *Patch Idea:*  
- Process each oscillator output though stereo effect modules ([Happy Nerding FX Aid XL](https://happynerding.com/product/fx-aid-xl/), [Strymon Magneto](https://www.strymon.net/products/magneto/)), then send their returns to a stereo mixer ([Intellijel Mixup](https://intellijel.com/shop/eurorack/mixup/)).
- Pan separate VCO and Sub outputs, automate pans via external VCAs—add motion to your polyrhythms.

**Benefit:**  
Transform Subharmonicon’s rich harmonic output into huge, moving, spacious sound textures for immersive performances or recordings.

---

## 7. Feedback, Self-Patching & Harmonic Chaos
### *Patch Idea:*  
- Patch filter or envelope outs back into frequency/division/rhythm CV ins (carefully!), or externally loop audio through wavefolder, comp, or ring mod modules then back into Subharmonicon’s audio path.
- Use external fixed filter banks ([Doepfer A-128](https://doepfer.de/a128.htm)) to sculpt subharmonic content for unique spectral drones.

**Benefit:**  
Push the boundaries into chaos, rich noise, harmonics, and generative soundscapes—tap into the Subharmonicon’s semi-modular roots!

---

## Module Recommendations for Synergy
- **Effect Processing:** Strymon Magneto, Mimeophon, FX Aid, Clouds, Z-DSP
- **Rhythm & Logic:** Pamela’s Pro Workout, A-166-2, Mutable Grids or Marbles, Erica Pico Seq
- **Utility CV:** Maths, Quad VCA (Intellijel, Doepfer A-135-2), VCAs, Attenuverters
- **Randomness:** Turing Machine, Wogglebug, Marbles, Ornament & Crime (“CopierMaschine” mode)
- **Wave Shaping:** Serge Wave Multipliers, Bifold, Doepfer A-137-2

---

Let the Subharmonicon become a living, breathing part of your modular system—its rhythmic and harmonic "logic" as much a generator of melody as of evolving, multifaceted control voltages, audio textures, and system-wide interaction.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
