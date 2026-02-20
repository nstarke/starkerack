# Quanalog Instruments — Boubou

- [Manual PDF](../../manuals/Boubou – Quanalog Instruments.pdf)

---

[**Quanalog Boubou Manual (web)**](https://quanalog.com/boubou/)  
*(Note: PDF download not directly available at time of writing)*

---

## Creative Modulation Techniques for Quanalog Boubou

As an experienced Eurorack modular synthesist, here's how you can push the Quanalog Boubou into uniquely experimental territory, especially for distorted percussion, heavy bass, and spooky pads.

---

### 1. Distorted Percussive Sounds

#### **Kick Drum Drive & Waveshaping**
- **Overdrive Knob**: Crank this for heavier distortion—full CW approaches self-oscillation for acid or Vermona/909-style kicks.
- **Click Tone & Blend**: Dial in aggressive click frequencies and blend with bottom sine for sharp, digital-sounding transients.
- **Compression Modes**: Cycle through the three for different punch/character. The hardest mode will be most distorted.
- **Audio Input Abuse**: Instead of just sending triggers, feed in audio or complex waveforms to the Kick's trigger input—this "wavefolds" or bit-crushes, mangling incoming signals into percussion with extreme digital edge.

#### **Velocity & Accent Tricks**
- **Dynamic Triggering**: Use step CV from a sequencer into the trigger input (instead of a gate or trigger) for velocity-sensitive drum hits. This massively increases expressive range and can result in louder & softer, dynamically saturated drum sounds.

---

### 2. Monster Basslines (Dubstep, Drum & Bass)

#### **Kick as Bass Oscillator**
- **Self-Resonance**: Push the overdrive until the kick self-resonates. Now, this is a sine bass oscillator.
- **Pitch CV**: Patch sequencer, LFO, or envelope to the Kick's "Tune CV" for rolling, thumping, or wub-wub movement. Fast LFOs and envelopes will twist the bass for EDM/sub genres.
- **Decay CV Modulation**: For wobble or rhythmic gating, send stepped or synced LFO/CV to the Decay CV to create short-plucked to long-droning bass notes.
- **Audio Rate FM**: For tearout/fuzzy bass, patch an audio-rate VCO to the Kick's CV inputs or the trigger—this will frequency-modulate or hard-sync the kick oscillator for metallic, aggressive textures.

#### **Layer with Dual Tom**
- **Lo Tom as Notch Filter**: Without a trig in, use it to process kick or bass channels, sweeping the notch CV to accentuate or carve the low-mids like a formant.
- **Retrig Knob**: Dial in noise/flam for "growling" or rhythmic fluttering on bass.

---

### 3. Haunting, Atmospheric Pad Sounds

#### **Atmospheric Processing**
- **Signal Processing**: Any of the Boubou voices can act as a filter/VCA processor. Feed complex drones, vocal samples, or slow-moving waveforms into Trig or Ext Ins. Their filter cores impart analog color or can turn white noise into windy, distant atmospheres.
- **Snare/Hi Tom Layering for Texture**: With snare triggered and hi tom open (no trig), snare becomes thicker and more resonant—perfect for ghostly, metallic pads. Sweep RES (resonance) CV for morphing, otherworldly formants.
- **Hat CV "Pedal"**: Use slow LFOs or smooth envelopes into the hat’s decay CV to create swelling, shimmering noise beds, processed through bandpass or fed with your own VCOs for spectral pads.

#### **Noise Sources for Soft Textures**
- **Blending**: Feed external oscillators into the Hat engine’s Mixer. With noise level low, use your own VCO or sample as a base, filtered/VCAd by the Boubou, to sculpt vast, shimmery pads.
- **Slow Modulation**: Use multiple slow LFOs/envelopes to modulate decay, resonance, and pitch across toms, snare, and hats, creating constantly evolving soundscapes.

---

### 4. Cross-Module Patching Strategies

- **Feedback Loops**: Route the audio from one voice (say, a resonating tom or hat) into another’s trig/ext in and modulate their CVs—unique intermodulations, erratic rhythms, or organic pads result.
- **Gate Length Tricks**: Use sequencers with variable gate length into the tom’s retrig—longer gates give you stuttering, rolling, or trilling percussion. Combine this with distortion/overdrive on the Kick for breakcore or DnB-style grooves.
- **Accent/Envelope via CV**: Patch envelopes or stepped random sources into decay/pitch/tune CVs for humanized or chaotic movement.

---

## Summary Table

| Sound Goal            | Key Modulation Techniques                                                         |
|-----------------------|-----------------------------------------------------------------------------------|
| Distorted Drums       | Overdrive, click blend, audio as trig, velocity/step CV to triggers, compression  |
| Wobbly Monster Bass   | Kick self-resonance, sequencer to pitch CV, audio-rate FM, CV decay, notch filter |
| Haunted Pads          | Slow modulate decay/resonance, noise blending, ext in processing, envelope hats   |
| Organic Cross-Mod     | Feed one section’s out to another’s in, retrig for rolls, gate lengths, feedback  |

---

**REMEMBER:** The Boubou is designed for experimentation. Patch unconventionally—try everything from FM overdrive to using linear LFOs as triggers, and process signals through multiple voices’ filtering circuits.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)