# Access Virus — TI Snow

- [Manual PDF](../../manuals/Virus_TI_Snow_Quickstart.pdf)

---

Sure! Here’s an analysis focused on modulation techniques for the [Access Virus TI Snow](https://www.virus.info/api/download/ti2/ti2_quickstart_manual.pdf) (manual PDF), adapted for a **eurorack modular mindset** with an ear toward **distorted percussive hits**, **monstrous basslines**, and **atmospheric pads**.

---

# Modulating the Virus TI Snow for Unique Sonic Results

[Access Virus TI Snow Quickstart Manual (PDF)](https://www.virus.info/api/download/ti2/ti2_quickstart_manual.pdf)

The Virus TI Snow isn’t a Eurorack module per se, but as a powerful digital synth with deep modulations, the same principles apply to modular patching. Below is a translation of the manual’s modulation and sound design tips into eurorack-style language and patches.

---

## 1. Creating Distorted Percussive Sounds

**a. Oscillator Selection & Filtering**
- Use the **Classic oscillator** for snappy, digital percussive elements, or the **HyperSaw** for a buzzier attack. For the most aggressive tones, try the **Grain** or **Formant Complex** oscillators (these double DSP usage, so keep it simple if you want polyphony).
- **Filter Section:** Crank the **Resonance** with a fast LFO modulating the Cutoff. This creates sharp, zappy "ping" sounds reminiscent of modular percussive modules.

**b. Modulation Tricks**
- Patch an envelope with a fast attack/decay to Filter Cutoff and Oscillator Pitch.
- Set the **Filter Saturation** to a digital or overdrive type and increase **Osc Volume** into saturation (>0) for distortion.
- Use the **Mod Matrix** to route velocity, aftertouch, or a random LFO to filter cutoff or oscillator pitch for variable intensity.

**c. Layering & Routings**
- In **Multi Mode**, trigger different sounds (kick, snare, clap) on different parts, each with unique envelope and saturation settings.

**Example Patch:**
```
Oscillator: Classic/Grain/HyperSaw
Envelope 1: Short Decay > Amp
Envelope 2: Short Decay > Filter Cutoff/Resonance
LFO 1 (Pitch) or Random Mod > Subtle Pitch Mod
Filter: Analog 1-4pole, High resonance, Saturation ON, Osc Mix High
Output: Use delay at extreme settings for metallic snare/hat sounds
```

---

## 2. Crazy Dubstep/Drum & Bass Basslines

**a. Oscillator Manipulation**
- Use **Wavetable** or **Formant Complex** oscillator for vowel/formant sweeping bass.
- Modulate **Wavetable Index** or **Formant Shift** with a synced LFO for classic dubstep vowel movement.

**b. Macro Modulations**
- **Mod Matrix**: Assign LFOs or Envelopes to:
    - Filter Cutoff (wobble)
    - Oscillator Pitch
    - Wavetable/Index/Formant Shift

**c. Distortion/Drive**
- **Saturate** post-filter using Filter Saturation or external analog drive pedal/folder.
- Stack two oscillators slightly detuned (Osc Balance knob to center), and use large amounts of FM from Osc 2.

**d. Automation & Live Control**
- Snap parameter changes between different filter types or oscillator models in Multi Mode for glitched sequences.
- Assign the Mod Wheel to a deep parameter (like filter cutoff or formant) for live bass morphing.

**Example Patch:**
```
Oscillator: Wavetable or Formant
Osc2: FM Amount High, Detune Slightly
Envelope: Fast attack, varying decay for rhythm
Filter: LP24 or Analog 1-4pole for growl, full resonance, cutoff swept by LFO
Saturation: Digital Overdrive or LoFi
Mod Matrix: LFO 1 (1/4 sync) > Wavetable Index, LFO 2 (1/8 sync) > Filter Cutoff
External: Optional modular bitcrusher/folder inline
```

---

## 3. Haunting/Atmospheric Pads

**a. Oscillator Tricks**
- **HyperSaw with high Density and moderate Detune** for lush, haunting pads.
- **Wavetable or Formant Complex** with slow LFO on Index or Formant Shift for evolving texture.

**b. Filter Movement**
- Use two filters in parallel; blend them to taste for nuanced tone.
- Slow, multi-stage envelope or LFOs modulating both Filter 1 and 2 cutoff and resonance.

**c. Modulation Routing**
- Crossfade LFO assignments so one controls index, another modulates pan, a third modulates vibrato depth.
- Use MIDI or velocity for real-time expressive control, or automate via DAW/sequencer.

**d. FX Layering**
- Layer **Delay** and **Reverb**. Set Delay Send and Reverb Send high, but be aware of polyphony hit.
- Phaser lightly for ghostly motion.

**Example Patch:**
```
Oscillator: HyperSaw - Density 7-9, Detune 20-40
Osc2: Detuned Sine, balance set for width
LFO 1: Slow ramp > Filter Cutoff for sweep
LFO 2: Very slow triangle > Wavetable Index or Formant Shift
Filter: Parallel dual LPF, gentle saturation
Envelope: Long attack/release (>60), moderate decay
FX: Max Reverb, Light Delay, Subtle Phaser
Mod Matrix: Random LFO > Slight Pitch/Index for analog drift
```

---

## Extra Eurorack-style Modulation Ideas

- **External Clock Sync:** Use tap tempo or clock sync parameters for modular/DAW integration of LFOs/arp.
- **"Patch Matrix":** Treat the Mod Matrix like a macro patchbay—assign multiple sources to the same destination for richer complexity.
- **Parameter Morphing:** Use automation (DAW, MIDI, CV out from euro sequencer->MIDI) to sweep macros over time, as you would with morphing-waveshapers or fading between effect busses in modular.

---

> [Access Virus TI Snow Quickstart Manual (PDF)](https://www.virus.info/api/download/ti2/ti2_quickstart_manual.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)