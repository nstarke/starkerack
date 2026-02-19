# Zlob — Triple Cap Chaos

- [Manual PDF](../../manuals/Zlob Modular - Triple Cap Chaos.pdf)

---

[Triple Cap Chaos Build Docs & Manual PDF](https://zlobmodular.com/wp-content/uploads/2023/09/TripleCapChaos_BuildDoc.pdf)

---

## Using the Zlob Modular Triple Cap Chaos for Dense, Hyper-Complex Percussion

The **Triple Cap Chaos** is a 2hp chaos-based analog oscillator and audio mangler. It's uniquely suited to generating unpredictable, rich audio textures and pseudo-rhythmic elements through its chaotic attractors, audio-rate oscillation, and audio/CV mangling capabilities. Let’s break down how you can exploit its features for generating dense, polyrhythmic, and highly percussive sequences in a Eurorack setup.

---

### Module Type:  
**Primarily an Audio Source & Mangler/Processor**  
- Not a traditional voice or effect, but chaotic oscillator with audio/CV processing abilities.

---

### Techniques for Hyper-Complex Percussion

#### 1. **Percussive Voice Creation Using Audio Outputs (X & Y)**
- **X Output**: Sinusoidal, noisy, “windy” textures—can form the basis of snare-like or metallic percussion.
- **Y Output**: More squared-off, harsh/aggressive—great for kicks, claps, or highly electronic percussive hits.

**How to use for punchy, unique percussion:**
- **Short EG or VCA**: Trigger the X or Y outputs with short envelopes through VCAs for sharply defined, punchy percussive hits.  
- **Randomized Triggers**: Use a clock divider/multiplier and trigger the EG/VCA at different rates for automatic polyrhythms.
- **Layering**: Combine both X and Y outputs to form composite drum sounds with organic top end/noise and a beefy fundamental.

#### 2. **Audio/CV Mangling for Evolving Patterns**
- **IN Jack**: Feed drum machine, oscillator, or existing modular percussion through the AC-coupled input.  
  - As the "IN" interacts with the chaotic core, it generates heavily modulated, shifting timbres and tones.
- **External Modulation**: Patch complex LFOs, stepped random voltages, or sequencer channels to "CV IN" (expects -5V to +5V). This disrupts the normal chaos and steers the resulting signal into even wilder, more unpredictable pulses and waveforms.

**Patch Ideas:**
- Send a simple drum loop or repeating synth line into the IN and modulate Width/Emanate with polyrhythmic/irregular CV sources (from a Pamela’s New Workout, Zadar, Maths, etc).
- Use rhythmic clocks or gates at different divisions or from Euclidean/sequencer modules to modulate the chaos parameters for complex, evolving syncopations.

#### 3. **Polyrhythm & Complex Time Signatures**
- **Voltage-Controlled Chaos**: Using the CV input, feed in rhythmic, stepped CV (from a melody sequencer or trigger-to-CV converter at different clock rates).
  - This makes the chaos evolve at unrelated time signatures from the main clock, overlaying random, rhythmic bursts on top of the expected meter.
- **Divide/Multiply Triggers**: Use the Triple Cap Chaos’ X or Y output as an audio-rate clock source (run through an envelope follower or comparator) to extract gates/triggers, then use these for triggering percussive voices in unusual rhythms.
- **Sync Your System to the Chaos**: Pass the X or Y output through a clock extractor module (e.g., Mutable Instruments Peaks, Pamela’s New Workout clock input) and sync sequencers or clock dividers to the chaotic output for organically evolving, non-repeating complex patterns.

#### 4. **Sound Shaping for Percussive Emphasis**
- **Emanate Knob (Spectrum/Activity)**:  
  - CCW = more chaos = more gnarly, noise-based percussion and wild sample & hold artifacts.
  - CW = more stable oscillation = tight, almost FSK/Buchla drum tones.
- **Width/CV Att**: Fine-tune the chaos/oscillation to sweep the sound into more tonal or sharper, more digital/bitcrushed realms—ideal for hats, claps, digital percussion splashes.
- **Fast Short Envelope Modulation**: Patch velocity or accent envelopes to the CV input to accentuate certain hits/passes, adding hyper-dynamic, punchy variation to the stream of sound.

---

### Creative Patch Example:  
**Chaotic Bongos with Polyrhythmic Modulation**  
- Patch X output through a VCA, envelope the VCA with different-length clocked triggers (e.g., 3-step and 5-step divisions for polyrhythm).
- Modulate Width with slow LFO or stepped sequencer at yet another unrelated division.
- Feed Y output through a wavefolder or lowpass gate for “woodier” percussion layers.
- (Optional) Feed a syncopated sequence or another random CV to IN for evolving chaos, bringing random grain or “flam” to the hits.

---

### Quick Summary Table

| Feature                | How to Exploit Percussively                            |
|------------------------|--------------------------------------------------------|
| X Output               | Windy/noisy metallic, hats/snare/percussion layers     |
| Y Output               | Aggressive, squared-off claps/kicks/electronic drums   |
| IN (Audio/CV)          | Chaotize loops/drums, impose chaos on incoming signal  |
| CV Input               | Modulate chaos for polyrhythm, time-shifted pulses     |
| Emanate & Width Knobs  | Sweep between unstable/chaotic and tone-like sounds    |

---

### Final Notes

- **Experiment with feedback**: Try patching audio or CV from Triple Cap outputs back into its IN or CV input for even more self-organizing complexity.
- **Non-repeating patterns**: The chaotic core ensures no two passes are identical—great for glitch and complex IDM, breakcore, experimental techno, etc.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)