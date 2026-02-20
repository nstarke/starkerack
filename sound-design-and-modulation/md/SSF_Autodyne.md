# SSF — Autodyne

- [Manual PDF](../../manuals/Autodyne - Steady State Fate.pdf)

---

[Steady State Fate Autodyne Manual (PDF)](https://steadystatefate.com/products/autodyne)

---

# Creative Modulation and Sound Design with SSF Autodyne

The **SSF Autodyne** is a 4hp analog auto-compressor/distortion module with CV-controllable sidechain, character-driven gain stages, and a blend for NY-style parallel compression. Because it fuses compression, distortion, and sidechain manipulation in a small package, it’s highly versatile—not just for mixing duties but as a driving force for fresh, animated modular tones.

Below you'll find some focused strategies for exploiting the Autodyne in three styles: **distorted percussion**, **aggressive basslines**, and **haunting atmospheric pads**.

---

## General Tips

- **COMP (Combo Ratio/Threshold/Gain) Control:** Main shaper. Left = mild, to right = heavy compression & saturation.
- **GAIN:** Output gain control—crank for hard clipping/distortion, or keep low for transparency.
- **Side Chain Input & Filter:** External or internal (normalled) sidechain; sculpt what triggers compression with HP slope filter.
- **BLEND:** Mixes unprocessed signal with compressed/distorted signal. Far left = dry, far right = wet.

---

## 1. Distorted Percussive Sounds

### *Patch Example*

1. **Audio Input:** Feed in drum hits, complex percussion, or a basic analog drum sound.
2. **BLEND:** Start around 75–100% wet for maximum compression/distortion impact.
3. **COMP:** Sweep right to get brutal squashing. Extreme settings for "smacky" transient attacks.
4. **GAIN:** Crank to taste for over-the-top distortion and drive.
5. **Sidechain Filter:** Turn on, set moderate HPF to allow sharp transients but tame subby body (prevents "flabby" low end from choking the compressor).
6. **CV Modulation:** Modulate COMP or GAIN with an envelope (synced to drum trigger) for per-hit intensity change, or apply stepped random CV for “broken tape machine” effects.

#### *Pro Tip:*  
For “all-buttons-in” type FET compression, push COMP to max, GAIN to max, BLEND to max—with sidechain HP engaged for punchy, techy drum busses.

---

## 2. Crazy Basslines (Dubstep, DnB, Electro)

### *Patch Example*

1. **Audio Input:** Use a wobbly VCO or sampled reese bass.
2. **COMP:** Center or just past for aggressive, pumping compression. Right past center = dirty, rowdy.
3. **GAIN:** Dial up for saturation. Full-up = gnarly bass growls.
4. **Sidechain Input:** Patch a kick or modulating CV (like an LFO) to the sidechain; this will "duck" or animate compression with the kick/LFO rhythm.
5. **Sidechain Filter:** Engage for tightness—turn up HPF so sidechain responds less to sub frequencies (avoids muddy compression).
6. **BLEND:** Start wet, then back off a bit to retain original transient snap.
7. **CV Modulate:** Modulate BLEND or COMP with sequencer-patterned LFOs or random voltages for basslines that “breathe” or glitch.

#### *Pro Tip:*  
Turn GAIN up to the edge of tearing and feed in pitch- or filter-modulated bass for classic neuro/dubstep stabs. Sidechain to drums for instant “pumping” effects.

---

## 3. Haunting Atmospheric Pads

### *Patch Example*

1. **Audio Input:** Long, evolving VCO wave, sample loop, or dense reverb wash.
2. **COMP:** Set low (left of center) for smooth, slow, transparent compression; higher for “ghostly” pumping.
3. **GAIN:** Low to medium for gentle grit & warmth. Higher for eerie, lo-fi sounds.
4. **BLEND:** Use about halfway; full wet can sound “withering” and otherworldly. Experiment for blend of clarity and fogginess.
5. **Sidechain Input:** Patch a slow LFO, noise, or random stepped voltages to modulate the sidechain—this creates undulating, spectral volume swells and spectral dips.
6. **Sidechain Filter:** Experiment with triple slope HPF to let low mids pass through, highlighting “hollow” or “chilly” upper mids.
7. **CV Modulate:** Automate BLEND or COMP with subtle slow CV for movement and depth.

#### *Pro Tip:*  
Feed the output into a big reverb or granular processor for endless, morphing atmospheres. Use random gates/envelopes to animate COMP or GAIN for evolving “whispers.”

---

## Bonus: Stereo Processing

- If using two Autodynes, match controls closely for stereo bus compression, or mismatch slightly for wide, animated stereo fields on pads, drums, or complex textures.

---

## More Modulation Ideas

- **Envelope Following:** Patch envelope followers to COMP or GAIN for dynamic, audio-reactive compression.
- **Audio-Rate:** Try modulating GAIN or COMP with audio-rate signals for FM-like amplitude distortion.
- **Random Gates:** Plug random clocks or gates into sidechain input for unpredictable stutter & glitch.

---

**Want to patch all this digitally, or auto-generate wild modular recipes? Browse the tools at:**  
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)