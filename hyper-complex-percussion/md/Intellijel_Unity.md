# Intellijel — Unity

- [Manual PDF](../../manuals/unity-mixer_manual_2020.04.15.pdf)

---

[**Unity Mixer Manual (PDF)**](https://intellijel.com/downloads/manuals/unity-mixer/unity-mixer_manual_2020.04.15.pdf)

---

## Using the Intellijel Unity Mixer for Hyper-Complex Rhythmic Percussion

The **Intellijel Unity Mixer** is a utility module, not a voice or effect module. While it does not *generate* sound on its own, it is incredibly powerful as a summing utility for **CV (control voltage)** and **audio signals**, making it an essential tool for dense, polyrhythmic, and complex percussion synthesis. Below you'll find creative strategies for leveraging the Unity Mixer in this context:

### 1. **Complex Gate/Trigger Summing for Polyrhythms**

- **Patch multiple rhythmic gate/trigger sources** (e.g. clock dividers/multipliers, sequencers like Pamela’s NEW Workout, Euclidean ratchets, or step sequencers set to different time signatures) into the input channels of the Unity Mixer.
- The summed mix at the output can feed an **envelope, percussive voice, or drum module**. This creates layered gate streams: e.g. sum a 5-step pattern and a 7-step pattern for a repeating 35-step cycle (polyrhythm), resulting in intricate rhythmic triggers.
- Since the Unity Mixer is phase correct and doesn’t invert or attenuate signals (unless you set the jumper), your complex grooves will come through cleanly.

### 2. **Percussion Layering via Audio Summing**

- Combine the audio outputs of multiple percussion voices (e.g. kick + snare + clicky percussion) as a summed bus to a single channel. This lets you build composite drum sounds that snap, punch, and evolve.
- For maximal punch, layer **raw VCO outputs or noise bursts** alongside your main hits. Use fast envelopes or vactrol/decay modules beforehand for percussive shapes.

**Tips:**
- Beware of clipping (max output 10.5V). If building aggressive, dense stacks, use the -6dB attenuation jumper to avoid distortion unless that's what you want.
- The dual 3:1 or single 6:1 functionality makes it possible to group sub-mixes (hats & clicks in one, kicks & toms in the other) and then re-combine or re-route them live.

### 3. **Creating Evolving Percussive Patterns (Mixing CV Sources)**

- Feed **uneven, evolving LFOs or random stepped modulators** (like S&H circuits) into a Unity Mixer, then route the sum as modulation to drum decay, pitch, or filter cutoff.
- This can automate subtle (or extreme) shifts in your percussion timbre, rhythm, or even panning — especially when the summed CV traverses different modular destinations per section.

### 4. **Driving Complex Modulation for Percussive Voices**

- Combine clocked/envelope CVs, LFOs, and noise as a control source for a synth voice’s VCA, making every hit have unpredictable dynamics but remain “locked” to a polyrhythmic cycle.
- Use the mixed output to control LPGs, VCAs, or other percussive sound shapers.

### 5. **Percussive FX Chaining and Parallel Processing**

- Split your percussion audio through various effects (distortion, reverb, comb filters) and mix them back together with the Unity Mixer for **parallel FX processing**.
- With careful gain staging (using the attenuation jumpers if needed), you can achieve anything from subtly enhanced grooves to wild, glitchy, multi-layered percussion bursts.

### 6. **Dynamic Re-Patching for Performance**

- Use the Unity Mixer’s simple, straightforward normalization to quickly re-route sub-mixes during live performance, evolving your polyrhythmic arrangement on the fly without repatching multiple cables.

---

### **Advanced Pro Tips**

- **Combine sequencer accumulators or burst generators** for layered fills and complicated pattern changes at specific points in your sequence.
- **Use with manual switches or mutes** before the mixer to selectively enable/disable rhythmic parts mid-performance, maximizing live playability.

---

> While the Unity Mixer doesn’t process voices directly, it is a secret weapon for constructing, layering, and routing complex percussion. Its role as a CV & audio summing matrix is foundational for hyper-complex modular rhythms!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)