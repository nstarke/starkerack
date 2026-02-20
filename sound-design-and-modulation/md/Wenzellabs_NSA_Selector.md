# Wenzellabs — NSA Selector

- [Manual PDF](../../manuals/wenzellabs_the_NSA_selector_ the NSA selector eurorack module.pdf)

---

[NSA Selector Eurorack Module Manual (PDF)](https://github.com/wenzellabs/the_NSA_selector/blob/main/README.md)

---

# Modulation Techniques for the NSA Selector Eurorack Module

The **NSA Selector** is one of the most unconventional Eurorack modules available, acting as a hardware network packet sniffer that converts raw Fast Ethernet network traffic data into audio signals. By patching it into your modular system, you can literally "listen to the internet" and use this strange data stream as a sound source. Here’s how you can harness the NSA Selector for unique sonic exploration, particularly for **distorted percussion, aggressive basslines, and haunting pads**.

---

## Key Features Relevant for Sound Design

- **Ethernet to Audio**: Directly outputs network bitstreams as audio via a 4-bit R2R DAC and low-pass-filtered output.
- **Network Activity as Modulation Source**: Acts as a translator of network events (pings, browsing, image transfers) into audible signals.
- **Extremely High Sample Rate**: Native 4-bit audio at 25MS/s (MegaSamples per second!).

---

## Techniques for Unique Modulation and Sound Design

### 1. **Distorted Percussive Sounds**

- **Method**: Use the module’s network-triggered transients.
    - Generate percussive events by pinging devices on your LAN at various packet sizes and rates. The included `sequencer/` shell script can automate this.
    - Percussive sounds can be shaped by creating regular or irregular packet bursts, translating to sharp clicks, pops, and noise hits at the audio output.

- **Distortion**:
    - Route the NSA Selector output into a wavefolder, bitcrusher, or analog distortion module after the initial conversion. The dense, noisy bitstream is perfect for hard digital distortion.
    - Adjust your network's traffic volume to control the “density” and intensity of the percussive artifacts.

---

### 2. **Dubstep/Drum & Bass Basslines**

- **Method**: Modulate network activity with rhythmic patterns corresponding to desired bass rhythms.
    - Use the upconverter utility to encode a 16-bit/48kHz WAV file (your own synthesized bass waveform, for example) into the module’s native 4-bit/25MHz format. Send this data over your network via the included fileserver scripts and listen out of the module.
    - Manipulate image or data transfer rates to “wobble” the output: Changing packet size or frequency in time with your drum patterns can impart stepped, stuttered, or vibrato-like movement.

- **Bass Enhancement**:
    - Filter the output with a strong low-pass filter (VCF) to emphasize sub-frequencies and eliminate harsh top-end.
    - Process with envelope followers or dynamic modulation to make the digital artifacts respond organically to your patch's amplitude or CV, introducing movement typical of electronic bass genres.

---

### 3. **Haunting Atmospheric Pads**

- **Method**: Stream large, uncompressed images or slow, steady, predictable data streams to generate consistent yet modulated noise beds.
    - The module responds in detail to raw .BMP or similar uncompressed image transfers via the network, producing evolving, swirling digital textures.
    - Stack multiple image transfers or overlapping slow network activities for a layered drone.

- **Atmosphere Processing**:
    - Patch the output through granular, reverb, or spectral processors to smear and stretch the digital noise into haunting pads.
    - Use slow-moving voltage-controlled amplifiers or panners to animate the sound spatially in your mix.
    - Experiment with disabling network encryption to let more nuanced “payload” evolve; with encryption off, more of the actual data can be made audible, adding texture.

---

## Advanced Tips

- **Analog Feedback**: Route the module’s output back into your LAN’s audio input (with careful level management) to create network-driven audio feedback loops—watch for wild, self-oscillating digital chaos!
- **Live Modulation**: Hook up MIDI-CV converters to software controlling your network streams. This allows sequencer/CV or even manual controller manipulation over what data (and thus what sound) is sent.

---

## Example Signal Flow
```
[Network Source: pings, file transfer, sequencer script]
         ↓
[NSA Selector] 
         ↓
[VCF/Distortion/Wavefolder/Granular/Reverb]
         ↓
[Mixer/Effects]
         ↓
[Speakers]
```

---

## Useful Links
- [NSA Selector Github repo (Manual and converters/tools)](https://github.com/wenzellabs/the_NSA_selector)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---

**Go wild—there’s nothing else quite like it in the rack. With the NSA Selector, your music can literally be powered by the pulse of the net!**