# Expert Sleepers — ES-9

- [Manual PDF](../../manuals/es9_user_manual_1.3.pdf)

---

[Expert Sleepers ES-9 Firmware v1.3 User Manual PDF](https://expert-sleepers.co.uk/es9usermanual.html)

---

# Creative Modulation Techniques for the Expert Sleepers ES-9  
*Distorted Percussion, Dubstep/Drum & Bass Basslines, and Haunting Atmospheric Pads*

The Expert Sleepers ES-9 isn’t just an audio interface—its advanced routing, mixing, and signal processing features make it a deep playground for transforming and modulating Eurorack signals in real time. Here’s how to creatively manipulate it for modern electronic styles:

---

## 1. **Distorted Percussive Sounds**

### **Approach:**
- **Eurorack Inputs**: Patch raw drum modules, noise, or struck envelopes directly into several of the 14 ES-9 inputs.
- **Drive the Input**: Push higher amplitude percussive CV signals (+/-10V) for digital clipping at 0dBFS, creating crunch and digital distortion.
- **Mixing & EQ**: In the Mixer section, combine multiple percussive elements, and use the 4-band per-channel EQ to sharply boost/cut frequencies for tone sculpting (e.g., exaggerated transient attack or metallic overtones).
- **DC Coupling for CV/Modulation**: Patch LFOs or envelopes into other channels, and in the config tool, turn **OFF DC Blocking** on input pairs to allow pure CV shapes.
- **Macro & Raw Mix**: Set up parallel mix busses—one clean, one heavily EQ’d/distorted, and sum them at the outputs for parallel processing.
- **MIDI Macro Mix Control**: Perform live morphing of drum sound density using a MIDI controller to automate macro mix or pan (e.g., from snappy to obliterated).

### **Extra Tip:**  
Sum several sharp envelopes in the mixer and route to the same output with massive gain/EQ boost to create digital 'clicks' and spikes.

---

## 2. **Dubstep/Drum & Bass Basslines**

### **Approach:**
- **Analog Oscillator > ES-9 Input**: Route aggressive/sub oscillators into the ES-9. Use the optional DC coupling to bring in unfiltered CV for wild PWM or FM bass tones.
- **MIDI CC Mixer Automation**: Set MIDI control for mixer levels/pans. Automate with DAW or physical controls for 'wobble' effects (think LFO mapped to mixer gain/panning or quick filter enable toggles).
- **Hot EQ Settings**: Use Peak and Shelf EQ bands to create resonant peaks, exaggerated subs, or mid boost for growls. Try inverting the phase of one layer for “hollow” basses.
- **Layer & Route**: With 8x8 mixer and extensive routing, layer clean and processed bass signals. Route one signal path through Mixer 1 (for clean sub) and another through Mixer 2 or the S/PDIF loop with heavy EQ or intentionally clipped gain staging.
- **Dual/Linked Stereo**: Use Stereo Links for wider basslines that jump across the stereo image, further modulating pan via MIDI controllers.

### **Extra Tip:**  
Pass control-voltage derived LFO via DC-coupled input into mixer, then use that in routing as 'Amplitude Modulation' of the main bass lane, for robotic/driven tones.

---

## 3. **Haunting Atmospheric Pads**

### **Approach:**
- **Multi-Layer Input**: Feed multiple outboard synth voices, slow LFOs, noise, and drones into multiple ES-9 inputs.
- **Mixer Macro Automation**: Assign MIDI faders to control mix volumes and panning, dynamically weaving pads in and out (automatable in DAW or with MIDI controller for morphing textures).
- **Heavy EQ Sculpts**: Apply multiple band EQs—e.g., narrow high-pass to make “whispery” tops, or strong low-pass for murk. Combine phase inversion for ghostly cancellations.
- **Mix Smoothing**: **Turn on mix smoothing** to interpolate morphs between settings, creating slow, undulating pad evolutions (*DSP load permitting*).
- **Stereoizing & Bussing**: Use Stereo Links to create wide stereo pad movement; use the internal busses for parallel processing chains—e.g., layer a filtered pad and an unfiltered one.
- **S/PDIF/Second Mixer**: Use S/PDIF to send/return to outboard effects (big reverbs, shimmers), or, if running 2 mixers, set up one chain for the dry pad and another for the effected pad—blend via the ES-9.

### **Extra Tip:**  
Route a sidechain-modulated gate/envelope through CV inputs (with DC coupling) and use the mixer to duck pads in time with your drums for a “haunted pumping” atmosphere.

---

### **General Power Moves**

- **Live Performance**: Use the push-button knob to instantly switch between 'hosted' and 'standalone' configurations for dramatic mix/processing scene changes mid-set.
- **Extreme DSP FX**: Approach the 100% DSP limit by stacking filters and smoothing for digital mutants and over-processed oddities.
- **DAW+Modular Interplay**: With simultaneous DAW routing and modulation, treat the ES-9 as a hybrid programmable-effects-and-mixing brain.

---

## Manual Reference  
Be sure to check the [official ES-9 manual PDF](https://expert-sleepers.co.uk/es9usermanual.html) for detailed setup instructions and the full capabilities of the mixer, routing, and SysEx options.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)