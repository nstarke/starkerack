# Bubblesound — HexVCA

- [Manual PDF](../../manuals/bubblesound.pdf)

---

[HEXvca Manual PDF](https://www.bubblesound-instruments.com)

---

## Bubblesound HEXvca: Creative Modular Patch Ideas

The Bubblesound HEXvca is a 6-channel voltage-controlled amplifier, highly flexible for both audio and CV processing in a Eurorack setup. Here’s how you can leverage its unique features for creative patching:

---

### 1. **Voltage Controlled Mixer**
- **How:** Use the MIX outputs (channels 1-3, 4-6, or all 1-6) as a VC-mixer.
- **Creative Patch:** Send six different sound sources (oscillators, drum modules, field recordings) into the channel inputs, modulate each channel with different CV sources (e.g., envelopes or LFOs from Make Noise Maths or Intellijel Quadra). The mixed output can create complex, evolving soundscapes or rhythmic textures.

### 2. **Envelope Sharing (Normalized CV)**
- **How:** Use the CV normalization jumpers to control several VCAs with the same envelope/gate.
- **Creative Patch:** Send a single envelope from an Intellijel Quadra to control multiple VCAs (e.g., gating multiple drum voices simultaneously or creating coordinated amplitude movement across several melodic voices).

### 3. **Polyphonic Voice Amplitude Control**
- **How:** Set up six individual voices (such as different oscillators and filters) and use each VCA as the final output for each voice.
- **Creative Patch:** Pair with a CV/gate sequencer like the Arturia Keystep Pro or Winter Modular Eloquencer. Mix and match envelopes to modulate each voice’s VCA for dynamic polyphonic composition.

### 4. **Modulated Voltage-Controlled Attenuator for CV**
- **How:** The HEXvca is DC-coupled, meaning you can run LFOs, sequencer CVs, and other modulation signals through it.
- **Creative Patch:** Send random voltages or LFOs into the VCAs, then use stepped CV (from Mutable Instruments Marbles or a Turing Machine) to modulate the amplitude of those LFOs. Use these dynamic CV signals to control filters, oscillators, or effects elsewhere in the rack.

### 5. **Amplitude and Stereo Pan Effects**
- **How:** Pair two or three VCAs in parallel for stereo or multichannel spatialization.
- **Creative Patch:** Route pairs of voices through VCAs controlled by quadrature LFOs (e.g., from Doepfer A-143-9), then out to the left and right channels of your output module for automated panning or spatial movement.

### 6. **Connection with HEXar**
- **How:** Use the rear header to connect with Bubblesound HEXar sequencer for cable-free triggering.
- **Creative Patch:** Sequence gates and triggers to HEXvca’s VCAs via HEXar, allowing per-step gates to open/close different channels—perfect for creative gating or rhythmically complex drone textures.

### 7. **Parallel Processing and Layering**
- **How:** Use the three mix outputs (1-3, 4-6, 1-6) to process selected groups of channels.
- **Creative Patch:** Route channels 1–3 through delay/reverb (like Mutable Instruments Clouds), and channels 4–6 through distortion (like Intellijel Tube VCA) for processed parallel blends, then sum everything via the 1–6 mix output.

---

#### **Recommended Modules for Pairing**
- **Envelopes/LFOs**: Intellijel Quadrax, ALM Pamela’s New Workout, Mutable Instruments Stages
- **Sequencers**: Winter Modular Eloquencer, Arturia Keystep Pro
- **Random/Stepped CV**: Mutable Instruments Marbles, Music Thing Turing Machine
- **Stereo/Spatial Control**: Doepfer A-143-9, Happy Nerding PanMix
- **Audio Sources**: Mutable Instruments Plaits, Noise Engineering Basimilus, Erica Synths Pico Drum
- **Effects**: Mutable Instruments Clouds, Make Noise Mimeophon, Erica Synths Stereo Delay

---

## Tips:
- **Experiment with exponential vs. linear CV for different envelope shapes and dynamics.**
- **Use VCAs for ducking effects: modulate one channel’s amplitude in opposition to another for rhythmic animation.**
- **Chain VCAs for complex amplitude modulation or sidechain effects (e.g., one VCA controlling the CV signal to another VCA).**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)