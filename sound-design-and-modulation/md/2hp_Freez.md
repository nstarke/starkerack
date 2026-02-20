# 2hp — Freez

- [Manual PDF](../../manuals/Freez_Manual.pdf)

---

[Freez Manual PDF (images above)](#)  
*(Note: Link to the actual PDF is not available since images are attached, not an online PDF. Reference screenshots above.)*  

---

# Creative Modulation Techniques for the Freez Module

As a Eurorack modular synth musician, the **Freez** module offers powerful real-time sound-sculpting abilities, especially for distorted percussive hits, gnarly dubstep bass, and spooky pads. Below are some tips for each sonic category, leveraging the features described in the manual:

---

## Distorted Percussive Sounds

1. **Short Buffer Sizes (Glitch Percussion)**
   - **Patch**: Feed sharp transients (e.g. drum hits, plucked VCO, or noise bursts) to **IN**.
   - **Set SIZE**: Fully clockwise (smallest buffer), for microcopic sample segments.
   - **Modulation**: Patch a fast envelope or random stepped CV to *SIZE CV INPUT* (2) so each hit records and locks at different, tiny durations—ideal for glitch and granular effects.
   - **Sample Rate Crunch**: Set **S. RATE** (9) to minimum for severe bitcrushing, digital distortion, and aliasing. Modulate *S. RATE CV INPUT* (8) at audio rates for a "metallic" gated feel.
   - **Freeze Mode**: Use momentary mode (toggle up) and pulse the **TRIG** to rapidly lock/unlock audio, for stuttering or "tape stop/restart" textures.

2. **Bitcrusher Snare/Hi-hats**
   - Use the combination of very short buffer and low sample rate for transformed clicks, claps, or hats that are both crushed and chopped.

---

## Crazy Dubstep/Drum & Bass Basslines

1. **Ripping, Animated Bass**
   - **Feed**: Aggressive, harmonically rich bass (complex oscillator, FM, or even a basic saw/pulse) into **IN**.
   - **Modulate Buffer Size**: Patch a slow LFO, envelope follower, or complex stepped CV to *SIZE CV INPUT* (2). This introduces erratic pitch jumps and formant changes (since size = buffer length = pitch/timbre).
   - **Wobble Sample Rate**: Simultaneously run another LFO (possibly synced to the beat) into *S. RATE CV INPUT* (8), alternating between hi-fi and downsampled digital filth. Slowly sweeping between 2–30kHz often yields thick, modulated grit.
   - **Beat Repeat/Gated Patterns**: Use momentary mode and trigger via gate/clock for precise repeat stutters and glitch bass FX—as the buffer refreezes, it “repeats” with wild spectral changes.
   - **Combine with Sequencer/Controller**: Use sequencer or touch controller voltage outs for real-time hands-on radical bass changes.
   
---

## Haunting Atmospheric Pad Textures

1. **Granular Freezes & Shifts**
   - **Feed**: Slow, lush pad or evolving texture.
   - **Freeze Large Buffers**: Set **SIZE** towards counterclockwise (long buffer up to 3s), freeze a chord or drone.
   - **Sweep Buffer Size**: Apply a looping envelope or smooth LFO to *SIZE CV INPUT* (2) for wavering, shifting textures—this will cause subtle pitch and formant morphs.
   - **Ghostly Sample-Rate Swims**: Gently modulate *S. RATE CV INPUT* (8) with a slow triangle LFO (or mod-wheel, aftertouch), introducing lo-fi warmth or cold digital haze.
   - **Freeze/Unfreeze Live Audio**: Occasionally freeze and unfreeze in latch mode with manual or random triggers for evolving ambient beds, layering real-time input with locked buffer content.

---

### **Patch Tips**

- **External Effects & Feedback**: Route Freez output through reverb, delay, or even back into itself for wild, evolving chaos.
- **CV Stacking**: Sum multiple control sources for unpredictable but musical textures (e.g. LFO+Envelope, or Random+Sequencer).
- **Audio-Rate Modulation**: For experimental noise, drive the CV inputs with oscillator audio for harsh AM/FM-like buffer/timbre manipulation.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
