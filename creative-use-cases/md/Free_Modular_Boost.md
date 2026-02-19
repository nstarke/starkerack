# Free Modular — Boost

- [Manual PDF](../../manuals/boost_manual.pdf)

---

[Boost Manual PDF](https://free-modular.com/manuals/boost_en.pdf)

---

# Creative Uses for Boost in Your Eurorack System

The Boost module by Free Modular is a flexible, all-analog preamp with gentle diode clipping and a tone circuit. Below are several ways to creatively integrate Boost into your Eurorack system and get the most from its unique character.

## 1. Add Harmonic Interest to Digital Oscillators
- **Why?** Digital oscillators (like the Mutable Instruments Plaits or Noise Engineering Basimilus Iteritas Alter) can sometimes sound sterile.
- **How?** Place Boost after the digital oscillator to inject analog warmth and subtle (or not-so-subtle) saturation. Use the Tone knob to shape the overtones for a richer or more aggressive sound.
- **Tip:** Modulate the VCA level pre-Boost for dynamic distortion.

## 2. External Gear Integration: Guitar Pedal Sounds, Line Level to Modular
- **Why?** Want to use guitar pedals or synths with your rack, or feed in audio from your DAW/interface?
- **How?** Use Boost to bring external line-level sources (drum machines, grooveboxes, audio interfaces, microphones) up to modular levels, with a dash of analog overdrive.
- **Combo Suggestion:** Pair with a send/return module (like Befaco's Instrument Interface) for extra routing/metering options.

## 3. Envelope-Controlled Saturation
- **Why?** Dynamic distortion = more expressive sound.
- **How?** Place a VCA (e.g., Intellijel VCA, Mutable Veils) before Boost, amplitude-modulated by an envelope (like Maths or an ADSR). Fast, snappy envelopes spike the distortion; slower envelopes give smooth saturation.

## 4. Feedback, Bitcrushing, and Glitch FX
- **Why?** Push Boost into extreme territory for clipped, crunchy artifacts.
- **How?** Feed the output of Boost back into itself, via a mixer with an attenuator (e.g., Doepfer A-138), and control input with a VCA. High feedback can yield "hard" distortion and noise textures.
- **Combo Suggestion:** Use with a bitcrusher module (e.g., Erica Synths Pico BitCrusher) post-Boost for wild digital grit.

## 5. Overdriven Percussion
- **Why?** Make your percussion knock!
- **How?** Route hats, snares, or kicks through Boost. Use the Tone control to emphasize sizzle (right) or tame it for rounder drum sounds (left).

## 6. Analog Fuzz Lead Sounds
- **How?** Send a simple waveform like a sine or triangle from an analog oscillator (e.g., Dreadbox Hysteria or Make Noise Dixie II+) through Boost. The gentle diode clipping creates fuzz or overdrive-like leads, unlike aggressive wavefolders.

## 7. Tame Harshness or Push Brilliance in Pads
- **Why?** Flexible tone shaping!
- **How?** Use Boost in an aux send return path on a mixer. Boost and brighten washed-out pads, or take off the edge to sit them comfortably in the mix.

## 8. Layered Coloration in Submixes
- **Tip:** Place Boost on a submix (e.g., grouping multiple voices, percussion, or FX returns) for glue and cohesion. Subtle clipping works as a bus compressor alternative to gel disparate sounds together.

## 9. Excite Vocals and Spoken Word
- **How?** With a dynamic mic and a preamp to bring levels up (or an interface module), send vocals through Boost for overdriven, radio-like punch—great for aggressive voice processing or lofi sampling.

---

## Example Patch

```
Oscillator → [VCA] → Boost → [Filter/Phaser/FX] → Mixer/Output
Envelope → CV In (VCA)
Modulation Source → Tone (if using external attenuverter or voltage-controlled tone circuit via DIY)
```
- Replace oscillator with any sound source (drums, field recordings, vocals)
- Try with FX after Boost (delay, reverb modules) for wild saturation trails

---

**Module Type Recommendations:**
- **VCA** with envelope/LFO modulation
- **External input interface** (Befaco Instrument Interface, ADDAC200)
- **Modulation source:** Envelope generators (Make Noise Maths), LFOs
- **Wave shaping modules:** Before or after Boost for aggressive tones
- **Filters:** To tame harmonics post-Boost
- **Delay/Reverb:** For ambient/smeared textures
- **Mixers:** To blend Boosted and clean signals

---

For more info and updates, check out the [Boost manual PDF](https://free-modular.com/manuals/boost_en.pdf).

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)