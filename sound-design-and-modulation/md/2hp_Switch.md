# 2hp — Switch

- [Manual PDF](../../manuals/2hp_Switch.pdf)

---

[2hp Switch Official Manual PDF](https://2hp.com/docs/2hp_Switch_manual.pdf)

---

## Creative Modulation Techniques with the 2hp Switch

The **2hp Switch** is a compact, voltage-controlled signal router with four inputs and one output—an excellent utility for experimental signal processing in Eurorack setups. Below are detailed strategies for using this module to achieve:

- Distorted percussive sounds  
- Crazy, modulated basslines (dubstep/DnB style)  
- Haunting, evolving atmospheric pads  

---

### 1. Distorted Percussive Sounds

**Patch Idea:** Channel-Hop Drum Layering

- **Inputs:** Patch 4 different percussive sources (e.g., Kick, Snare, Hi-Hat, Digitally-distorted Noise Burst) to the four Switch inputs.
- **SEL CV Input:** Send a fast, stepped random voltage (e.g., from a Turing Machine, Sample & Hold, or sequencer set to gate mode) into the SEL CV input.
- **SEL Knob:** Use this to offset or "window" which drum types are being accessed in each phrase.
- **Processing:** Route Switch’s output through a distortion, wavefolder, bitcrusher, or even just heavy VCA gain for further smash-and-glitch artifacts.

**Outcome:**  
The Switch will instantly jump between percussive sounds on each step, creating highly unpredictable, glitchy drum lines perfect for breakcore or industrial genres.

**Variation:**  
- Patch only *varied* distorted sources, and CV-sequence the selection for unpredictable, ever-morphing percussion.
- Use audio-rate CVs (fast LFOs or oscillators) into SEL CV for rapid aliasing/granular chopping, creating digital artifacts.

---

### 2. Crazy Dubstep/Drum & Bass Basslines

**Patch Idea:** Bassline Chopper

- **Inputs:** Patch four different bass sound generators (e.g., classic sub, FM bass, formant oscillator, filtered noise bass) into the Switch.
- **SEL CV Input:** Use a complex modulation source, such as:
  - A quantized random sequence synced to your clock
  - An LFO multiplied and phase-shifted for wobbles
  - Envelope follower from a drum track to "key" bass selection to drum hits
- **SEL Knob:** Manually sweep during recording/jamming for live glitch effects.

**Outcome:**  
Generate "mutating" bass lines that rapidly morph character, reminiscent of chopped, re-sampled modern DnB/Dubstep bass sound. Audio-rate SEL CV modulation transforms the Switch into a digital waveshaper, causing wild, stuttering, bit-crushed edges!

**Variation:**  
- Use the SEL CV input with stepped voltages that align with your musical phrases for rhythmic precision.
- Modulate SEL CV with sidechained pumping for creative movement.

---

### 3. Haunting, Atmospheric Pads

**Patch Idea:** Textural Morphing

- **Inputs:** Patch four evolving drones or pad textures (sample playback, slowly modulated oscillators, granular clouds, etc.) to Switch inputs.
- **SEL CV Input:** Slowly modulate with an LFO, envelope, or manually-played voltage source (e.g., joystick, ribbon controller), or a super-slow random source.
- **SEL Knob:** Set the offset to bias certain textures.

**Outcome:**  
As the SEL CV sweeps, the module cross-switches between different pad sources abruptly (as opposed to crossfading), resulting in a textural, cinematic soundscape with haunting jumps—great for ambient, experimental, or horror sound design.

**Variation:**  
- Use the input LEDs for visual feedback, syncing texture changes to stage lighting/visuals.
- Modulate SEL CV with envelopes triggered alongside filter sweeps for synchronized movement.

---

### Additional Creative Tips

- Use gates or triggers to the SEL CV for instant, precise switching: great for live fills or breakdowns.
- Run CV signals themselves through the Switch (as opposed to audio). Use separate CV sequences for each input—modulate the selection for complex, algorithmic, generative modulation sources.
- Stack the output with a VCA and reverb for further dynamic and spatial manipulation.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)