# Tiptop Audio — Fold Processor

- [Manual PDF](../../manuals/Tiptop_Audio_foldprocessor.pdf)

---

[Tiptop Audio Fold Processor Manual (PDF)](https://www.tiptopaudio.com/manuals/Fold-Processor-Manual.pdf)

---

# Creative Uses for the Tiptop Audio Fold Processor in Eurorack

The Fold Processor is a particularly flexible analog module, bringing Serge-inspired wavefolding and unique octave subdivision to your rack. Here are some advanced, creative, and fun ways to get the most out of it:

---

## 1. **Classic Wavefolding with VCOs**
- **Patch:** Sine or triangle output from a VCO (e.g., *Make Noise DPO*, *Tiptop Z3000*, *Intellijel Dixie II*) into the IN1.
- **Result:** Animate simple waveforms into complex, harmonically-rich timbres. Use the FOLD and INJECT CVs with modulating sources (envelopes, LFOs) to keep the sound evolving.
- **Suggestion:** Run the OUT to a low pass filter (*Mutable Instruments Ripples*, *Doepfer A-120*) to tame harmonics and sculpt the tone further.

---

## 2. **Analog Distortion for Drums or Sampling Modules**
- **Patch:** Audio out from a drum module or sample player (e.g., *ALM Squid Salmple*, *Tiptop ONE*, or *Noise Engineering Basimilus Iteritas*) into Fold IN1.
- **Result:** Use the module as an analog distortion, achieving characterful grit and crunch—analog "drive" inside your rack for percussive elements, similar to using guitar pedals with beats.
- **Tip:** CV-modulate the FOLD amount with a snappy envelope for punchy, distorted attacks.

---

## 3. **Sub-Oscillator Magic with SUBDIV Section**
- **Patch:** After folding, send OUT to SUBDIV OUT. The SUBDIV section generates four divisors, each an octave apart, mixed to taste.
- **Result:** Create fat, layered sub-basses or chord-like intervals from a single oscillator. Great for beefing up mono lines or adding pseudo-polyphony.
- **Suggestion:** Feed SUBDIV OUT through a wavefolder (such as *Intellijel uFold*) or frequency shifter (*Doepfer A-126*) for evolving bass textures.

---

## 4. **Wild Octave Pulse Processing**
- **Patch:** Feed a complex or noisy source—such as the output from *Mutable Instruments Plaits* or *Random Source Serge*—into the Fold Processor.
- **Result:** Extreme harmonics, drones, and unpredictable octave pulses, especially fun when sweeping FOLD and INJECT knobs, then modulating those with synchronized or cross-modulated LFOs.
- **Combo:** Send SUBDIV OUT to a clocked delay (e.g., *Make Noise Mimeophon*) to capture wild rhythmic artifacts.

---

## 5. **Harmonic Animation via Feedback Paths**
- **Patch:** Place the Fold OUT or SUBDIV OUT into the feedback path of a digital FX processor like *Tiptop Z-DSP* or *Mutable Instruments Clouds*.
- **Result:** Folding in the feedback loop adds dynamic harmonics and new timbres with every repeat, mutating delays and reverbs into lush textures.

---

## 6. **FM & Timbre Feedback**
- **Patch:** Patch OUT or SUBDIV OUT into the FM input of a second oscillator (or the same oscillator in a feedback patch).
- **Result:** Achieve FM sounds with more upper harmonics—great for metallic or bell-like tones, or pseudo-chaotic feedback networks for experimental music collaborations.

---

## 7. **Voltage-Controlled Harmonics (Automated Sound Design)**
- Use envelopes, LFOs, or sequencers (e.g., *Make Noise Maths*, *Intellijel Quadra*, *Malekko Voltage Block*) to modulate FOLD, INJECT, and their CV inputs for living, moving waveforms ideal for generative and self-playing patches.

---

## 8. **Cross-Processing with Other Analog Effects**
- Try running OUT > *Ring Modulator* (*Doepfer A-114*), *Wave Multiplier* (*STG .MIX* or *Serge Wave Multiplier*), or *Wavefolder* (*Intellijel uFold*).
- Double or triple up on folding/distorting for unstable, aggressive analog sounds perfect for industrial, noise, or glitch.

---

## 9. **Unusual Sidechaining and Ducking**
- Use the SUBDIV OUT for audio-rate amplitude-modulation or gating effects. Patch it into a VCA's CV input, and route a rhythmic element to the Fold Processor IN1 for musically reactive gating.

---

## 10. **Strange CV Generation**
- Feed CV-rate signals or LFOs into IN1 or modulate with audio-rate sources. Due to the analog wavefolding and subdivision, Fold Processor can transform or quantize CVs for unconventional modulation shapes.

---

**Bonus:**  
Try patching both OUT and SUBDIV OUT simultaneously into two channels of a stereo FX unit or mixer for wide, weird stereo images.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)