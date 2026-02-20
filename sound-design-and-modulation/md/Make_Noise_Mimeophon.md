# Make Noise — Mimeophon

- [Manual PDF](../../manuals/mimeophon-manual.pdf)

---

[Make Noise Mimeophon Manual (PDF)](https://makenoisemusic.com/manuals/mimeophon-manual.pdf)

---

# Creative Modulation Strategies for the Make Noise Mimeophon  
**Focus:** Distorted Percussion, Basslines, and Haunting Pads

The Make Noise Mimeophon is more than a conventional delay or echo; it excels as a voltage-controllable sound mangler thanks to its unique approach to time, color, and spatialization. Here’s how you can harness its modulation points and architecture to craft distinctive percussive, bass, and atmospheric sounds for Eurorack.

---

## 1. Distorted Percussive Sounds

### **Zone 0/1 & Flip for Percussive Distortion**
- **Patch a short burst/noise/gate or plucky envelope to the Left input.**
- Set **Zone** to 0 or 1. These zones are optimized for microsound, Karplus-Strong, flanging, and distortion effects.
- **Set Repeats high** (2-3 o’clock or more) for resonant, metallic ringing.
- Modulate the **μRate** input with another envelope or stepped random voltage for metallic pitch sweeps (Zone 0 is 1V/oct!).
- **Engage Flip** (either manually or via clocked triggers): in Zone 0/1, Flip causes "total protonic reversal," i.e., brutal buffer flipping and distortion. For extra madness, modulate Flip with an audio-rate signal or a fast LFO.
- **Modulate Color and Halo** with an LFO or stepped random for additional spectral movement and “broken” timbres.

**Patch Example:**
```
Kick trigger → Maths Envelope → Mimeophon Left In
Kick pitch CV → Mimeophon μRate
Fast LFO → Flip
Wogglebug quick random → Color CV
Output: Super-crushed, metallic, distorting transients
```

---

## 2. Dubstep/Drum & Bass Basslines

### **Resonant, Movement-Filled Bass**
- **Zone 0 (Karplus), 1, or 2:** These are best for fast, pitch-controllable bass.
- **Patch a snappy envelope or oscillator “pluck” into Mimeophon input.**
- Use a **sequencer CV to μRate** for “wub” and pitch tracking (in Zone 0 μRate is 1V/oct).
- **Crank Repeats (Noon or higher)** for growling resonance; modulating Repeats introduces squelch and decay movement.
- **Color:** Route a synced LFO or envelope to Color CV for classic formant and filter sweeps (try ramp LFO synced to your bass riff).
- **Halo:** Adds stereo movement—tie it to a slow sine LFO for stereo bass widening.
- **Skew + Flip:** Engaging Skew (and Ping Pong) pans bass motion; modulating Flip with rhythmic gates gives unpredictable syncopation.

**Patch Example:**
```
Sequencer CV → Mult → Oscillator 1V/oct, Mimeophon μRate
Pluck Envelope → Mimeophon Left In
Steep Envelope → Color CV Input
Slow LFO → Halo CV
Gate/Clock → Flip
Run output through distortion or filter for even more filth.
```

---

## 3. Haunting Atmospheric Pads

### **Smearing, Evolving Space**
- **Input a harmonically rich pad or drone to Left (or both) inputs.**
- **Zone 5-7:** Use the longest zones for maximum temporal smear and spaciousness (41 seconds in Zone 7!).
- **Repeats near max**: Enter self-oscillation territory, creating long, decaying clouds.
- **Modulate Rate and Zone** slowly with LFOs or random voltages (attenuate for subtler movement). This sweeps pad textures through different time scales.
- **Color & Halo:** Slow LFOs (triangle or sine) to both CVs create constantly morphing spectral/detail shifts. Halo at high settings for maximum “smear” and stereo diffusion.
- **Flip ON:** Pads played into Zone 4–7 will reverse, creating ghostly, inverted textures.
- **Hold:** Use the Hold feature to “freeze” evolving textures, modulate color/halo/rate for frozen, but ever-mutating clouds.

**Patch Example:**
```
Pad/droning oscillator/polyphonic mix → Mimeophon Left In
Slow LFO/random -> Zone CV
Different slow LFOs -> Color, Halo CV
Gate button or clocked CV -> Hold (activates freeze for textural morphs)
Manual or LFO -> Flip
Stereo out → Reverb for even more atmosphere
```

---

## Advanced Tips from the Manual

- Modulate **Zone** with a sequencer clocked to your rhythm for rhythmic “windowing” of percussive or melodic patterns. When Repeats is up, shorter Zones will imprint percussive transients onto larger echo buffers.
- Skewed Rate plus modulation of **μRate** = wild stereo chorus/flange.
- For **drum & bass-style bass**, use **Zone 0/1 with Flip**; modulate μRate for signature “growl,” and crank Repeats for feedback.
- Input gain can be boosted or cut (hold FLIP+HOLD) for drive/saturation, but beware input clipping.
- Use **Ping Pong** (hold Skew) for rhythmic panning and stereo motion in atmospheric material or tails of percussion.

---

For the full manual with examples and diagrams, [click here (PDF)](https://makenoisemusic.com/manuals/mimeophon-manual.pdf).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)