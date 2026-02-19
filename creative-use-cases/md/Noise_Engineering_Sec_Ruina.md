# Noise Engineering — Sec Ruina

- [Manual PDF](../../manuals/Seca Ruina - Noise Engineering Documentation.pdf)

---

[Seca Ruina Manual PDF](https://manuals.noiseengineering.us/sr/)

---

# Creative Patch Ideas for Seca Ruina

The **Noise Engineering Seca Ruina** is a compact (6HP) and versatile *multiband distortion/VCA* offering per-band and global drive control, with CV over both. Here are creative ways to integrate it with other Eurorack modules, leveraging both its multiband architecture and modulation possibilities.

---

## 1. **Dynamic Multiband Percussion Processing**

**Modules Needed:**
- Percussion source (e.g. Erica Synths Drum Modules, Tiptop Audio BD909)
- Envelope generator (e.g. Maths, Zadar)
- Seca Ruina

**Patch:**
- Route drums or percussion loops into Seca Ruina’s input.
- Patch separate envelopes to the individual band CV inputs (High, Mid, Low).
- Use the envelopes to dynamically modulate distortion per band, making kicks boomier, snares crunchier, and hats fizzier—independently.
- Take the Sum out to your mixer.

**Result:** Rhythmic, dynamically shifting multiband drum textures. Great for glitch, breakcore, experimental techno.

---

## 2. **Frequency-Selective Distortion Chains**

**Modules Needed:**
- Seca Ruina
- Three different effects modules (e.g. delay, phaser, reverb: Mimeophon, Warped Circuits Bend, FX Aid)
- Mixer (e.g. Intellijel Mixup, Befaco STMix)

**Patch:**
- Patch an instrument or field recording into Seca Ruina.
- Route each Seca Ruina individual band out to a different FX module.
- Mix processed bands back together.

**Result:** Drastically different FX chains sculpted tightly to frequency content—think low-end going through a phaser, mids through heavy delay, and highs washed in reverb. This creates a rich, spatially complex signal.

---

## 3. **Animated Multiband Distortion with LFOs/Sequencers**

**Modules Needed:**
- Modulation sources (LFOs: Batumi, Pam’s New Workout. Sequencers: René, Metropolix)
- Seca Ruina

**Patch:**
- Patch LFOs or stepped CV from sequencers into any or all band CV inputs (or the All CV input for global chaos).
- Slowly modulate drive settings, or use sequencer triggers for rhythmically pulsed distortion.

**Result:** Animated, evolving timbres. Hook up a random voltage source (Wogglebug, Marbles) for wild, pseudo-generative distortion movement.

---

## 4. **Additive Multiband “Vocoding”**

**Modules Needed:**
- Seca Ruina
- Vocoder or bandpass filter bank (Doepfer A-128, Mutable Instruments Vocoder)
- Voice signal and carrier (two audio sources)

**Patch:**
- Patch voice signal into Seca Ruina, split bands out, send to vocoder’s modulator band inputs.
- Send a synth sound to the carrier input.
- Use the Sum out for processed, intelligible distortion-vocode hybrid timbres.

**Result:** Choppy, hyper-articulated “vocal synth” textures, ideal for industrial and experimental pop.

---

## 5. **Multiband Envelope Following for CV Extraction**

**Modules Needed:**
- Seca Ruina
- Envelope followers (Doepfer A-119, Mutable Ears)
- Modulation destinations (VCA, filter cutoff, etc.)

**Patch:**
- Process a complex signal (drums, field recordings) through Seca Ruina.
- Patch individual outs to envelope followers.
- Use generated envelopes to control parameters elsewhere in your system—e.g. send the envelope from the High band to modulate reverb mix or pan, Mid band to bass synth cutoff.

**Result:** Eco-systemic, frequency-reactive modulation throughout your rack. Great for live sets and generative patches.

---

## 6. **Spectral Wavetable Distortion**

**Modules Needed:**
- Wavetable oscillator (Plaits, E352, Piston Honda)
- Seca Ruina
- Spectral or granular processor (MIMEOPHON, Morphagene)

**Patch:**
- Morph oscillator through Seca Ruina; patch the band outs to spectral processor inputs.
- CV sweep distortion per band (with LFOs or sequencer).
- Record or granularize the results.

**Result:** Animated spectra, with distortion “filling in” different parts of the frequency spectrum as you sweep. Great for music concrete or cinematic sound design.

---

## 7. **Voltage-Controlled Groovebox**

**Modules Needed:**
- Seca Ruina
- Envelope/VCA module
- Sequencer
- Drum and bass synth voices

**Patch:**
- Use Seca Ruina as a final bus for your stereo mix.
- Patch sequencer gates/envelopes to the All Drive CV input, “pumping” the entire mix’s harmonic content in time with your groove.

**Result:** Punchy, dynamically driven multiband bus distortion for entire groovebox/live techno setups.

---

These patch ideas should get you started; Seca Ruina’s multiband, CV-able architecture encourages experimentation—especially with modulation and routing. Pair it with stereo/frequency processors, complex modulators, or effects for endless sound design possibilities.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)