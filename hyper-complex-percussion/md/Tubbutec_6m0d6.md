# Tubbutec — 6m0d6

- [Manual PDF](../../manuals/6m0d6-User-Manual-1.0.pdf)

---

[6m0d6 User Manual PDF](https://tubbutec.de/files/6m0d6/6m0d6_manual.pdf)

---

# Using the 6m0d6 for Densely Rhythmic & Hyper-Complex Percussion

The **6m0d6** by LPZW & Tubbutec is an extremely versatile Eurorack drum module, ideal for forward-thinking rhythmic exploration. With its CV, trigger, accent capabilities, digital noise/metal sources, and MIDI, it’s ready for generative, polyrhythmic, polymetric, and experimental sequencing.

Below are strategies to harness its features for intricate, complex percussion in modular setups:

---

## 1. **Multiple Trigger & Accent Inputs**

- **Individual Instrument Triggers:** Each of the 7 drum voices (BD, SD, LT, HT, CY, OH, CH) has its own trigger input. This allows you to use multiple complex or unrelated sequencers (E.g., Euclidean, burst generators, random gates, clock dividers/multipliers) to drive each sound independently, supporting true polymetric layering.
- **Dynamic Trigger Levels:** Input voltages (1V–15V accepted) affect both sound and volume. Modulating trigger amplitude per voice creates extra dynamic nuance, aiding in mechanical or ‘human’ feel during dense sequences.

## 2. **Accent CV & Gate Complexity**

- **Accent as Macro-Controller:** Use the Accent Gate and Accent Amount CV (including external attenuation) to introduce global accentuation, cross-voice stuttering, or velocity-based groove.
- **Discrete or Modulated Accents:** Patch probabilistic/conditional gates or clock-skipped gates (from, e.g., Pamela’s New Workout or Mutable Instruments Grids/Branches) into Accent inputs for per-pattern loudness emphasis, or sequence voltage changes for constantly-evolving phrasing.

## 3. **Noise, Metal & XOR Sources**

- **Sound Design Diversity:** With per-voice selection between white noise, metal (6 oscillator stack), and XOR ‘ringmod,’ each drum voice can sound unique or morph within a pattern. Automation of these via CV allows for evolving, morphing textures; essential in dense/complex genres.
- **Bit-Crushed Noise:** Use the Noise Tune and CV input for lofi/industrial timbres, or automate transitions from clean TR-606 to gnarly, fractured bites within a single phrase.

## 4. **Flexible Decay, Tone, and Tuning**

- **Modulate Everything:** Snare, cymbal, and hihat decays; metal tune; metal spread; noise tune—all have direct CV input. This allows for:
  - Ratcheting effects by shrinking/increasing decay time per step.
  - Evolving cymbal/hihat/pitched percussion as you sequence or cycle spread and tune CVs over non-matching divisions.
  - Ping-ponging tunings, microtonal or otherwise, across polyrhythmic grids.

## 5. **MIDI as Meta-Percussion Engine**

- **Separate MIDI Control:** The 6m0d6 can be externally sequenced or CC-automated via MIDI (TRS), including instant paraphonic metal-oscillator synth mode—all over channel 1 (see manual pp. 12-13). Useful for layering with DAWs, key-stepping, or integrating sequencer-based odd-time signatures that are hard to patch.
- **Pulse Length Variability via Velocity:** MIDI velocity dynamically adjusts trigger length, creating ultra-dense, filterable FM/noise bursts within patterns.

## 6. **Mixer/Output Section for Live Layer Muting**

- **Patch Individual Outs:** By routing voices out individually and removing from the sum, you can use external VCAs to create crossfaded/automated/rhythmically gated mutes, which is key for managing density in chaos.
- **Sub Tom for Extra Layer:** Flip the Sub Tom for a sub-bass “shadow” on one Tom channel—great for doubling in alternate rhythms/meters.

## 7. **Config Menu—Performance Innovation**

- **Accent Normalisation:** Quickly switch accent normalisation (default ON/OFF) on the fly for radical performance changes.
- **Cymbal Pulse Shaping:** Bypass cymbal pulse shaping in config; enables drone or “string synth” behaviour under CV, ideal for noise breakdowns or melodic bridges in polyrhythmic tracks.

---

### **Example Patch Approaches**

- **Polymetered Drum Machine:**
  - Use several clock dividers or unconventional step-length sequencers for each voice.
  - E.g., BD every 7, SD every 4, HT every 11, etc.
- **Randomized Gate Streams:**
  - Use random gates/probabilistic sequencers for hi-hats/percussion for controlled chaos.
  - Accent can be triggered by rare/conditional events.
- **Morphing Techno Grid:**
  - Sequence changing noise/metal sources mid-pattern.
  - Modulate decay/tune per hit for cybernetic-sounding fills or breakdowns.
- **Hybrid MIDI & Modular:**
  - MIDI-in some sounds (using a DAW/electronic drum grid at 7/8, 9/8, or "irrational" signatures), patch others from modular logic for ultra-complex cross-patterns.

---

## **Further Reading**
- [6m0d6 Full Manual PDF](https://tubbutec.de/files/6m0d6/6m0d6_manual.pdf)  
- See [Tubbutec.de/6m0d6](https://tubbutec.de/6m0d6) for manual/further updates.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)