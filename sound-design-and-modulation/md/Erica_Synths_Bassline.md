# Erica Synths — Bassline

- [Manual PDF](../../manuals/BASSLINE_web.pdf)

---

[Erica Synths Bassline Module Manual (PDF)](https://www.ericasynths.lv/media/Bassline_manual_2.0.pdf)

---

## Creative Modulation Techniques with the Erica Synths Bassline

Based on the manual for the Erica Synths Bassline, here are several approaches you can use to create **unique and expressive sounds** with this analog synth Eurorack module. Techniques are tailored to build **distorted percussion**, **crazy basslines**, and **haunting pads/atmospheres**.

---

### Key Modulation Points

The Bassline module offers the following modulation options:
- **VCO FM In (1V/oct & FM)** – Frequency modulation
- **VCF CV In** – Voltage control of the filter cutoff
- **VCF Env In** – External modulation of the filter envelope
- **Accent In** – Accent dynamics/grooves
- **Gate In** – Trigger the envelope/VCA
- **VCO SUB/LEVEL, TUNE, DETUNE** – Add weight and detuned dirt

Below are targeted patches and ideas for each sound design goal:

---

## 1. Distorted Percussive Sounds

**Patch Tips:**
- Set the oscillator to pulse or saw for harmonic richness.
- Crank the **VCO Level** and use the **SUB Oscillator** for added punch.
- Use a very short **VCF Env Decay** for sharp, snappy transients.

**Modulation:**
- **Overdrive with Resonance**: Increase **VCF Resonance** to near self-oscillation. Modulate **Cutoff** via VCF CV for aggressive filter pops.
- **FM Percussion**: Patch envelopes, LFOs, or fast random CV into the **FM In** for pitch modulation at audio rates, creating metallic/distorted timbres.
- **Accent Input**: Use a sequencer or random gate source to accent alternate hits—crank up gain to push the VCA into saturation.
- Patch a noise module or another VCO into the **VCF CV**, slightly, for dirt and unpredictable snappy energy.

---

## 2. Crazy Basslines (Dubstep/Drum and Bass)

**Patch Tips:**
- Push the TUNE into lower registers for sub-bass power.
- Use **SUB Oscillator** for additional weight and movement.

**Modulation:**
- **Wobble Bass**: Sync an LFO (triangle/sine) or step-sequencer to the VCF CV for rhythmic filter sweeps (“wobble”) at musically synced rates.
- **Filter FM**: Use audio-rate FM into the **VCF CV In** for aggressive, vocal-like growls—route another oscillator or noise in here.
- **Envelope Shaping**: Adjust the VCF Envelope Decay for plucky or drawn-out shapes; modulate this decay time with external CV if possible.
- **Accent Input**: Sync to the ‘off-beats’ or drums for pumping/groove effects.

---

## 3. Atmospheric Pads/Haunting Textures

**Patch Tips:**
- **Detune** the oscillator for chorused width.
- Use **both the saw and pulse** waves plus SUB for dense harmonic content.
- Long VCF Decay for slow-moving filter morphs.

**Modulation:**
- **Slow LFO/Envelope to VCF CV**: Slowly move the filter cutoff for evolving ambient drones.
- **FM with slow LFO/random source**: Subtle FM (into FM In) for ghostly, shifting timbres.
- **Manual tweaking of Resonance & Cutoff**: Perform live sweeps for organic, haunting edges.
- **VCF Envelope Input**: Patch an external envelope (from another EG or complex modulator like Maths) for complex opening and closing of the VCF.
- **External Effects**: Run the output through long reverbs/delays, but pre-feed these by modulating the Bassline for constantly transforming pad soundscapes.

---

### Tips for Maximum Variation
- Stack modulation: Use a mult/attenuator to modulate both VCF and VCO FM with related but distinct LFOs.
- Experiment with self-patching: Route audio-rate square wave to FM In for circuit-bending textures.
- Use the **Accent** input to inject sequence/groove into any patch type.
- Slightly clip the **VCA output** or overdrive a following module for extra filth.

---

## Summary Table

| Mod Source        | Patch To      | For What Sound              | Result                             |
|-------------------|--------------|-----------------------------|------------------------------------|
| Fast Envelope     | FM In        | Percussion                  | Metallic, snappy attacks           |
| LFO/Seq           | VCF CV       | Dubstep, Pads               | Movement/Wobble, evolving sweeps   |
| Audio-rate Osc    | VCF CV / FM  | DnB Basses, Distorted Hits   | Vocal, growl, harsh textures       |
| External Envelope | VCF Env In   | Ambient                     | Evolving timbral changes           |
| Accent Gate/Pulse | Accent In    | Groove, Emphasis            | Accented notes, dynamics           |

---

## Additional Resources

- [Erica Synths Bassline Manual (PDF)](https://www.ericasynths.lv/media/Bassline_manual_2.0.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

Use these ideas as starting points for custom patches—let your modulation sources run wild!