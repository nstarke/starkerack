# Kaona Instruments — Stereo Weaver

- [Manual PDF](../../manuals/stereoweaver.pdf)

---

[Download the Kaona Stereoweaver Manual (PDF)](https://www.kaona.fr/uploads/manuals/Stereoweaver_Manual_EN.pdf)

---

# Creative Patch Ideas with Stereoweaver

Kaona’s Stereoweaver is more than just a “stereo widener.” It can transform mono sources into lush, animated, and characterful stereo images through psychoacoustics, phase modulation, movement, and micro-delay. Here are creative ways you can patch Stereoweaver within your eurorack system:

## 1. Animated Stereo Percussion

**Modules needed:** Drum module (e.g. Mutable Instruments Peaks, Tiptop Audio ONE), modulation source (e.g. LFO/Envelope—Make Noise Maths, XAOC Batumi)

- **Patch:** Route your mono drum output into Stereoweaver’s input. Use a slow, cyclic LFO to modulate the *Motion* and/or *Phase* CV inputs. This will create organic spatial animation, making each hit “move” across the stereo field, perfect for giving a static drum groove new life.
- **Tip:** Crank *Depth* and experiment with *Motion* in “rotary” mode for rotating, Leslie-like amplitude/phase shifting.

## 2. Swirling Lead or Pad Textures

**Modules needed:** Mono oscillator + filter/voice (e.g. Intellijel Atlantis, Mutable Instruments Plaits), random CV source (e.g. Wogglebug, MI Marbles)

- **Patch:** Send your lead or pad to Stereoweaver. Animate the *Haas* and *Width* with different rates of random CV. Subtle modulations yield evolving width and space; more aggressive modulations can result in swirling, unpredictable textures.
- **Tip:** Post-process stereo output with a stereo reverb (e.g. Mutable Instruments Clouds, FX Aid) for even deeper stereo immersion.

## 3. Metallic/Robotic FX & Sound Design

**Modules needed:** Digital noise or glitch source (e.g. Noise Engineering Basimilus, Erica Synths Pico Drums), envelope generator or sequencer, random CV

- **Patch:** Drive Stereoweaver’s input until the input LED blinks for deliberate analog “coloration” or distortion. Modulate *Phase* with stepped random or clocked envelopes for choppy, metallic phase artifacts.
- **Tip:** Use a sequencer to step through *Width* or *Motion* for abrupt spatial changes in sync with your sequence.

## 4. Stereoizing Vintage Mono Synths

**Modules needed:** Any vintage mono synth (external input via audio interface module), MIDI-to-CV converter

- **Patch:** Route external mono synth through Stereoweaver. Use DAW-generated LFOs or envelopes via MIDI-to-CV to animate *Width* and/or *Motion* for a modern, lively stereo sound.
- **Tip:** The *Haas* setting can add natural stereo space without introducing reverb—the result can sound like double-tracking or ensemble recording.

## 5. CV-interactive Performance Tool

**Modules needed:** Manual controller (e.g. Intellijel Tetrapad, Planar2 joystick), sequencer or clock divider

- **Patch:** Assign Planar2 joystick axes or Tetrapad faders to Stereoweaver’s *Phase* and *Width* CV inputs. Morph and animate the stereo field in real-time during performance—widen, pan, or destabilize leads, pads, or rhythms for dramatic live effects.
- **Tip:** Clocked triggers to *Motion* or *Haas* CV at specific points in your set can add dynamic contrast.

## 6. Experimental Feedback Network

**Modules needed:** Stereo mixer module (e.g. Befaco STMix), feedback send/return, stereo filter

- **Patch:** Take Stereoweaver’s stereo out into a stereo filter, then back to the mixer, and create a feedback loop (careful with levels)—modulate Stereoweaver parameters for evolving, unpredictable stereo feedback textures.
- **Tip:** Use cross-modulation between Stereoweaver’s CV inputs and filter parameters for complex spatial/timbre evolution.

---

**General Module Recommendations:**
- **LFO/Envelope Generators:** Animate spatial parameters for evolving stereo scenes.
- **Random CV/Stepped Modulation:** For non-repetitive, organic stereo motion.
- **Sequencers/Clock Dividers:** For rhythmic stereo modulations in sync with your patterns.
- **Stereo Mixers/VCAs:** To further process and mix Stereoweaver’s outputs.
- **External Effects (Reverb/Delay):** Extend the stereo space even further in post-processing.
- **Manual CV Controllers:** For tactile, live control over Stereoweaver’s spatial effects.

---

For more Eurorack patching inspiration and tools:  
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)