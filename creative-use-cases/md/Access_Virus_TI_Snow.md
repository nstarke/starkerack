# Access Virus — TI Snow

- [Manual PDF](../../manuals/Virus_TI_Snow_Quickstart.pdf)

---

[Access Virus TI Snow Quickstart Manual (PDF)](https://medias.audiofanzine.com/files/virus-ti-snow-quickstart-475111.pdf)

---

# Creative Eurorack Integration Ideas for Access Virus TI Snow

## Introduction

Though technically not a Eurorack module, the Access Virus TI Snow is an immensely flexible and deep standalone digital synthesizer/sound module that integrates beautifully with Eurorack and other modular setups, given the right interfacing modules. By routing audio and MIDI/CV signals between the Virus TI Snow and your rack, you can take full advantage of its multi-timbral sound engine, effects, and Total Integration features. Below are creative patching and integration ideas for using the Virus TI Snow as part of your wider Eurorack ecosystem.

---

## 1. **Audio Processing: Virus TI as an Effects/Synth Voice**

**Patch Idea:**  
Send Eurorack audio into the Virus TI Snow’s audio inputs for processing with Virus filters, envelopes, and effects.

**How:**  
- Use a Eurorack Output/Attenuator module (e.g., [ALM HPO](https://busycircuits.com/alm019/), Intellijel **Audio Interface II**, or Befaco **Out v3**) to bring your modular-level signals down to line level.
- Route the attenuated signal to the Virus’s L/R input.
- On the Virus TI, tweak filter types, envelopes, and effects (chorus, phaser, reverb, delay).
- Use “Input Thru” for dry/wet blending.
- Return the Virus’s output back into your Eurorack system with an Input/Preamp module (e.g., **Intellijel Audio Interface II**, or Befaco **Inamp**).

**Creative Uses:**  
- Use Virus’ lush filters and effects to create "hybrid" analog/digital textures.
- Animate Virus effect parameters with internal LFOs synced to modular clock sources by sending clock via MIDI or USB from your modular system.

---

## 2. **Virus as a Multi-Timbral Sound Hub in a Modular Hybrid System**

**Patch Idea:**  
Use the Virus’s 4-part multi-timbrality as four independent synth voices triggered/sequenced via your modular.

**How:**  
- Convert Eurorack pitch/gate signals to MIDI using a MIDI-to-CV interface (e.g., **Expert Sleepers FH-2**, **Mutable Instruments Yarns**, or Endorphin.es **Shuttle Control**).
- Configure each part of the Virus TI Snow on different MIDI channels.
- Use multiple CV/Gate tracks from modular sequencers (e.g., **Intellijel Metropolix**, **Make Noise René**) through your MIDI-CV converter to play the different Virus voices in parallel.

**Creative Uses:**  
- Address each Virus part from separate modular sequencers for live polyphony, layered patches, or key splits.
- Use the Virus' internal arpeggiator and layer patterns over modular percussion.

---

## 3. **Hybrid Modulation — Virus LFOs > Modular and Vice Versa**

**Patch Idea:**  
Cross-modulate: Use Virus TI’s LFOs/envelopes to modulate parameters on modular gear, and use Eurorack LFOs to modulate Virus params.

**How:**  
- Use a MIDI CC-to-CV module (e.g., **Endorphin.es Shuttle Control**, **Polyend Poly 2**, or **Expert Sleepers FH-2**) to convert Virus' MIDI LFO/Envelope CC messages to analog CV.
- Patch modular LFOs or random CV sources (e.g., **Make Noise Maths**, **Mutable Instruments Marbles**, **Intellijel Quadrax**) through CV-to-MIDI modules (e.g., **Expert Sleepers FH-2**) to sweep Virus parameters via MIDI CC.

**Creative Uses:**  
- Animate the Virus TI’s filter cutoff or FX mix using modular LFOs or stepped random voltages.
- Use Virus envelopes/LFOs to influence modular parameters (e.g., VCA levels, filter resonance).

---

## 4. **Layered Percussion and Texture: Virus Percussive Sounds + Modular Drums**

**Patch Idea:**  
Use the Virus as a digital percussion source to complement analog percussive modules.

**How:**  
- Sequence fast-envelope Virus patches via a modular gate sequencer (e.g., **Tiptop Audio Circadian Rhythms**, **Malekko Varigate 8+**) with clock and gate converted to MIDI.
- Mix Virus drum sounds with modular drum modules (e.g., **Noise Engineering Basimilus Iteritas Alter**, **ALM Akemie’s Taiko**).
- Process all percussion through Virus’s multi-FX and / or return Virus processed signal into Eurorack for further mangling.

**Creative Uses:**  
- Use Virus percussion as "glue" for modular drum kits; route selected channels through Virus for digital enhancement or stereo imaging.

---

## 5. **Virus as a Modulated Ambient Drone Engine in a Modular Environment**

**Patch Idea:**  
Use the Virus as a multi-oscillator drone source, layered with modular drones (e.g., via Mutable Instruments Rings/Plaits).

**How:**  
- Hold/latch notes or chords on the Virus, and use slow modular LFOs or sample-and-hold modules to modulate Virus parameters via MIDI-CC (filter, wavetable index, FX depth).
- Layer Virus audio with modular drone voices, sum and apply shared reverbs/delays in either system.

**Creative Uses:**  
- Slowly morph the digital texture using Virus' internal modulation system, while cross-fading with evolving analog modular textures.
- Use Virus’ arpeggiator as a gated rhythmic element inside a cloud of modular drones.

---

## 6. **Virus FX Only: "Modular → Virus → Modular" Signal Path**

**Patch Idea:**  
Use the TI Snow as a dedicated multi-FX processor for modular synth voices or even an external drum machine.

**How:**  
- Patch the output of a Eurorack mixer or voice through a Eurorack output module into the Virus' inputs.
- Bypass Virus' oscillators, and set up effects chains (chorus, phaser, delay, reverb, distortion).
- Bring the processed line-level signal back up via an input module to further patch into your rack (e.g., send into a Make Noise Morphagene, or granular/sample modules for more mangling).

**Advanced Twist:**  
- Use Virus’ MIDI learn to control FX parameters with modular CV signals converted to MIDI CC.

---

## 7. **Generative Sequencing: Random/Algorithmic Modular → Virus**

**Patch Idea:**  
Create generative melody/sequence data in the modular using modules like **Mutable Instruments Marbles**, **Intellijel Scales**, or **Tiptop Audio Z8000**, and convert to MIDI for Virus TI control.

**How:**
- Output quantized CV and gate from random/sequencer modules into MIDI conversion.
- Assign different random sources to the Virus’ different synth parts or patch parameters (e.g., assign one Marbles output to Virus pitch, another to Virus filter cutoff).
- Let Virus internal effects smooth and enhance the generative textures.

**Creative Uses:**
- Hybrid digital/analog randomness, controlled from one domain, morphing into the other.

---

## 8. **Polyphonic Pads and Sampling**

**Patch Idea:**  
Sample lush Virus pad chords into granular/sample Eurorack modules for further textural processing (e.g., **4MS Stereo Triggered Sampler**, **Make Noise Morphagene**, or **1010music Bitbox**).

**How:**  
- Play, sequence, or chord-stab pads on Virus, record short or long samples into your modular sampler.
- Re-trigger, slice, or granulate the samples for rhythmic, glitchy, or evolving ambient results, blending Virus timbral quality with modular audio processing.

---

## Recommended Interface/Utility Modules for Integration

- **MIDI-to-CV/Gate**: Expert Sleepers FH-2, Mutable Instruments Yarns, Endorphin.es Shuttle Control
- **Audio Interface (Eurorack to Line Level/vice versa)**: Intellijel Audio Interface II, Befaco Out/Inamp, ALM HPO
- **CV-to-MIDI**: Expert Sleepers FH-2 (with expanders), Polyend Poly 2
- **Modulation/S/H/LFOs**: Make Noise Maths, Mutable Instruments Marbles, Quadrax
- **Sequencing/Random**: Tiptop Z8000, Intellijel Metropolix, MI Marbles

---

## Inspiration

- Think of the Virus TI Snow as a polyphonic digital "oscillator/EQ/FX bank" for your entire modular system.
- Use its Total Integration (USB audio/MIDI to DAW) to interface your DAW, Virus TI, and modular as a creative triangle — audio and MIDI/CV flowing all directions.

---

### [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)