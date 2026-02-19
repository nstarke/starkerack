# Earthquaker Devices — Afterneath

- [Manual PDF](../../manuals/EQD-EU-Afterneath-Eurorack-R1.pdf)

---

[Afterneath Eurorack Module – Operation Manual PDF](https://www.earthquakerdevices.com/static/Afterneath_Eurorack_Manual.pdf)

---

# Using Afterneath for Densely Rhythmic, Hyper-Complex Percussion in Modular Synthesis

The **Afterneath** by EarthQuaker Devices, while designed as a reverb/effect, is an extraordinarily malleable module for rhythmic and percussive complexity—especially if you lean into its voltage-controllable, delay-line-based structure. Here’s how you can weaponize its parameters for generative drumming, complex polyrhythms, and outré percussion.

---

## Understanding Your Tool: Afterneath as a Rhythmic Engine

- **Not just a reverb:** The Afterneath is a cluster of short delay lines, not a standard reverb. This gives it a “smearing,” pingy or stuttering potential.
- **CV Control:** The Drag, Mode, Diffuse, and Length parameters are all voltage controllable with dedicated inverting attenuators—perfect for dynamic manipulation via external rhythmic, trigger, or sequencer sources.
- **Self-Oscillation:** At high Length and Reflect, it can self-oscillate—opening up pseudo-voice/oscillator duties driven by rhythmically-triggered CV.
- **External Feedback Loop:** Via Reflect Send/Return—process the feedback path with rhythmic VCA chopping, filtering, or even clocked effects for synced complexity.

---

## Strategies for Hyper-Complex & Percussive Rhythmic Exploration

### 1. **Rhythmic CV Modulation**
- **Drag CV Input:** The Drag control is where dense rhythm action happens. Patch fast/complex envelopes, random clocks, trigger sequencers, burst generators, or sharply rhythmic LFOs here—each change in Drag shifts the ‘delay tap’ times, creating pronounced stuttering, time-warped, and even pitched effects. Use a clock divider/multiplier for polyrhythms!
- **Mode Selection:** In quantized modes (4-9), Drag tracks 1V/oct for pitch-rhythmic relationships. In non-quantized modes, it's much more freeform—try both!

### 2. **Percussion Sound Design**
- **Self-Oscillation Percussion:** Crank Reflect and Length > 12 o'clock. Trigger the Drag CV input with fast envelopes, gates, or random step CV sources to “strike” the reverb buffer, generating tonal/atonal pings perfect for IDM, glitch, or experimental rhythms.
- **“Chopped” FX:** Use the Reflect Send to reroute the feedback path through a VCA sequenced with sharp rhythmic gates/triggers—this creates gated, isntrumental, or sliced-percussion effects.
- **Input Drive:** Input control at modular level ensures incoming drum sources are punchy and don’t get washed out. Overdrive the input for transient snap.

### 3. **Complex Patterns/Polyrhythms**
- **Asynchronous Drag CVs:** Patch two or more LFOs, each at an odd/even multiple (e.g., 5/7 against 4/8), through a CV mixer or sequential switch into Drag. This modulates delay density polyrhythmically.
- **Step Sequencer Per Mod Destination:** Send different sequenced voltages to Drag, Diffuse, Mode, and Length for evolving textures. Use odd-length sequences (e.g., 7-step, 13-step) for maximum temporal complexity.
- **Burst Gates:** Use burst generators or clock randomizers patched through logic modules for unpredictable, organic rhythm bursts—these will make the reverb “skip” unpredictably.

### 4. **Creating Perceptual “Punch” and Clarity**
- **Short Length, High Dampen, High Input:** For crisp, transient-rich percussive effects, keep Length and Diffuse low, Dampen higher (for brightness), and drive the input.
- **Reflect Feedback Abuse:** Inject noise, envelopes, or short triggers into Reflect Return to “re-strike” the input with feedback-tuned transient artifacts.
- **CV Attenuator Tuning:** The inverting attenuators allow for both normal and “reversed” CV directions—use this to invert the correlation between your CV and the resulting sound for more variety.

### 5. **Stereo and Spatial Play**
- **Pseudo-Stereo Outputs:** Mult output and Reflect Send to two mixer channels or main outputs. Use external processing on one branch (distortion, filtering) for a moving image, as the manual suggests—this makes complex patterns feel wider and less cluttered.

---

## Additional Tips
- Experiment with sequencers that offer probability or randomization for real “beyond-human” rhythm.
- Use Mode CV (with a stepped/trigger source) to rhythmically jump between quantization scales per bar/beat.
- Use chained VCAs or matrix mixers before the CV inputs to “draw” rhymic scenes or interpolate between beats with fine control.

---

## Inspirational Patch Example

```
Kick Drum → Afterneath Input
Trigger Sequencer (odd-length steps) → Drag CV (through attenuator)
Euclidean Burst Generator → Reflect Return (audio)
Maths/Envelope → Diffuse CV (inverted on alternate bars)
Reflect Send → Distortion → Right output
Dry Output → Left output
```

This patch will create polyrhythmic, stuttering, clap-like bursts with swirling, glitched reflections—making even a basic drum pattern hyper-complex and evolving.

---

**Manual Reference:**  
[Afterneath Eurorack Module – Operation Manual PDF](https://www.earthquakerdevices.com/static/Afterneath_Eurorack_Manual.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)