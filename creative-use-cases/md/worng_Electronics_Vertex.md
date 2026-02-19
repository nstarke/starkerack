# worng Electronics — Vertex

- [Manual PDF](../../manuals/Vertex manual v1.00.pdf)

---

[WORNG Electronics Vertex Manual (PDF)](https://static1.squarespace.com/static/5516ac7ae4b05a68d1cfb7c3/t/5cf02f1b6094e10001d9a572/1559238683852/WORNG+Vertex+Manual+WEB.pdf)

---

## Vertex: Creative Eurorack Patch Ideas & Combinations

The WORNG Electronics Vertex is a highly flexible stereo VCA module, with fascinating abilities for stereo automation, envelope shaping, and dynamic control in a Eurorack setup. Below you'll find some creative and advanced ways to patch it, in combination with other modules. Where possible, specific module suggestions are given (but any similar module will work). 

---

### 1. **Stereo Animation & Spatial Movement**

- **Patch:** Use a stereo signal source (e.g., [Make Noise X-PAN](https://makenoisemusic.com/products/x-pan), [ALM Jumble Henge](https://busycircuits.com/alm022)), routing its outputs to Vertex's L/R inputs.
- **Modulate:** Patch a complex, unsynced LFO (e.g., [Xaoc Batumi](https://xaocdevices.com/main/batumi/)) to the Skew CV input, and a second LFO/envelope to Gain CV.
- **Result:** The sound moves dynamically in stereo, but with the Vertex allowing you to sculpt asymmetrical envelope shapes for each channel, rather than just volume or pan.

### 2. **Dual Envelope Shaping for Percussion or Bass**

- **Patch:** Send a single envelope (e.g., [Intellijel Quadrax](https://intellijel.com/shop/eurorack/quadrax/), [Mutable Instruments Stages](https://mutable-instruments.net/modules/stages/)) to the Gain CV input. Feed two percussive audio sources (e.g., different drum channels or waveforms) to L/R inputs.
- **Skew:** By modulating Skew, each channel receives its own unique envelope shape, adding rhythmic or dynamic variations not possible with a single envelope alone.
- **Tip:** Try modulating Skew at audio rates for AM-like sidebands on percussive hits.

### 3. **Voltage-Controlled Crossfader**

- **Patch:** Patch two completely different mono signals (can be anything: VCO, drum, field recording) to L & R inputs.
- **Manual or CV Control:** Use Skew as a manual crossfader, or patch a modulation source (LFO, sequencer, envelope) into Skew CV for automated crossfading.
- **Advanced:** Clock-sync the Skew CV to your master clock for rhythmic crossfade patterns.

### 4. **Dynamic Stereo Distortion/EQ (in combo with waveshaper/distortion modules)**

- **Patch:** Run both Vertex outputs into two distortion modules (e.g., [VSL Vortices](https://www.vertxmodular.com/product-page/vortices-summation-mixer), [Bastl Cinnamon](https://bastl-instruments.com/products/cinnamon)), or EQ units, then back to your mixer.
- **Use:** Vertex shapes transient/sustain portions, and Skew imbalances the processing between L/R, so you can "spotlight" the effect (e.g., distorted left only on the attack, clean right only on the decay).
- **CV Animate:** Use envelopes/LFOs/sequencers for Gain and Skew CVs for morphing timbres.
  
### 5. **Stereo CV Processing (Control Modulation Routing)**

- **Patch:** Instead of audio, feed two modulation sources (e.g., one LFO and one random) into L/R inputs.
- **CV:** Use Vertex’s Gain and Skew controls to blend/CV-control the levels sent to downstream destination modules.
- **Application:** With e.g. a vector oscilloscope ([Zorg 3trins](https://zorgindustries.space/3trinsRGB1c/)), you can VCA-pilot two axes with real-time stereo*easing* and cross-modulation.

### 6. **Simulation of Dual Dynamic Stereo Sidechaining**

- **Patch:** Stereo audio in, patch a sidechain envelope (maybe from a kick drum or complex modulation) to Gain CV. Set Skew to preference for off-center ducking.
- **FX:** Insert reverb/delay after the Vertex to make side-chained swirling ambience.

### 7. **Creative Feedback Networks**

- **Patch:** Use Vertex's L & R outputs to feed separate effects (delay, distortion, phaser, etc.), then sum them and loop back into Vertex inputs for feedback.
- **Animate:** Use Skew CV to send the feedback more heavily to one side, or swap which effect dominates the feedback.
- **Warning:** Always monitor/keep feedback under control to avoid speaker damage!

### 8. **CV-Controlled XY Modulation for External Devices**

- **Patch:** Amplitude-control two control voltages (e.g., to a laser system, XY monitor, or 3D vector synth like [LZX Industries](https://lzxindustries.net/)), using Vertex as a stereo VC/attenuverter.
- **Animate:** Use audio/modulation at Skew CV for spinning or wobbling XY shapes.

---

### General Module Type Suggestions:
- **LFOs/Envelopes:** Anything with varied waveforms and/or modulation outputs (Batumi, Zadar, Maths, Quadrax, Stages).
- **Stereo Mixers/Panners:** For destination or routing before/after Vertex (X-PAN, A-138s, Planar2).
- **Audio FX (Stereo):** Reverb, delay, chorus, distortion for post-processing (Mimeophon, Erica Synths Black Hole DSP, FX Aid XL).
- **CV sequencing/generation:** Select random, stepped, or gated CV for intricate spare modulations (Pamela’s Pro Workout, Voltage Block, Ornament & Crime).

---

For more ideas, adapt these to your system and experiment with patch order, modulator speeds, and signal types.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)