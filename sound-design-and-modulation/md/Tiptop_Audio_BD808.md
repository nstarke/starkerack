# Tiptop Audio — BD808

- [Manual PDF](../../manuals/Tiptop_Audio_BD808_ns.pdf)

---

[BD808 Tiptop Audio Manual PDF](https://tiptopaudio.com/manuals/BD808_Manual.pdf)

---

## Creative BD808 Patching & Modulation Strategies
As a fellow eurorack enthusiast, getting the most out of the Tiptop Audio BD808 means exploring its analog roots and pushing it with your modular environment. Based on the manual you uploaded, here are tailored approaches for producing **distorted drums, seismic basslines, and haunting pads**:

---

## 1. Distorted Percussion: Pushing the BD808 Into Mayhem

**The BD808 features a hotter-than-normal output stage**, designed specifically so you can push the module into wild distortion without external gear.

### Techniques:
- **Max Out the LEVEL & ACCENT**:  
  - Set the LEVEL and ACCENT knobs to their maximum and DECAY to midway. This will slam the output up to 20Vp-p, causing heavy clipping/distortion in most downstream modules or mixers.
- **Overdrive External Modules**:  
  - Patch the output of the BD808 into a wavefolder, distortion, or bit crusher module. The already-hot signal will multiply the harmonic content and crunchy character.
- **Accent “Pumping”**:  
  - Use an external gate/trigger sequencer for the ACCENT IN, programming accents on off-beats or randomly. Crank the ACCENT level for huge volume spikes and punchy transients.

---

## 2. Dubstep/Drum & Bass Basslines: 808 Bass Reimagined

The classic 808 boom is the bedrock of modern bass genres—but with eurorack, you can re-shape it far beyond its original intent.

### Techniques:
- **Long Decay Sine “Bassline”**:  
  - Crank DECAY nearly to max (back off just before self-oscillation starts to avoid constant drone). Use sequenced triggers to play very long bass notes.
- **Modulate Tone for Wobble**:  
  - Use an LFO or envelope generator patched to a CV-controlled filter (post-BD808) to create a *wobble* effect on the low-pass filtering.
- **Pitch Trick (External Processing)**:  
  - Route BD OUT into a pitch-shifter or frequency shifter module. This can create evolving, sliding tonal effects suitable for DnB basslines.
- **Amplitude Modulation (AM)**:  
  - Patch BD OUT and another percussive source into a VCA or ring modulator. This generates metallic or synthetic bass textures when two sounds interact.
- **Audio-Rate Processing**:  
  - Use the hot output from BD808 to FM another oscillator or CV input on a filter—you'll get gnarly, aggressive additional bass harmonics.

---

## 3. Haunting Pads & Atmospheric Tones: Eerie 808

It might sound wild, but BD808’s resonant circuit can be a surprisingly rich textural source.

### Techniques:
- **Induce Self-Oscillation**:  
  - Turn the DECAY almost all the way up. If your unit starts self-oscillating, you’ll get a steady low sine—a haunting drone.
- **Filter & Reverb Wash**:  
  - Send BD OUT through a slowly moving bandpass or resonant low-pass filter with modulated cutoff, then bloom it out with a long reverb or delay (such as the Z-DSP).
- **Layered Triggers**:  
  - Use random or clock-divided triggers for both the GATE IN and ACCENT IN. This creates unpredictable surges and dynamic shifts.
- **CV Cross-Patching**:  
  - Consider patching the BD808 into modules with audio-rate CV inputs (e.g. modulate wavefolder symmetry or filter resonance) to get evolving pad-like textures.
- **Ambient Feedback**:  
  - Run the BD OUT through an external delay or looper, re-injecting subtle signal back into your FX chain to build dense, atmospheric swells.

---

## Additional Modular Tips

- Always experiment with feedback loops: try routing BD OUT into itself via external FX/VCAs.
- Try clocking the BD808 at weird intervals or with Euclidean/trigger sequencers.
- Recall from the manual: “Send the audio out into CV inputs of just about any module.” This bestows pseudo-random, audio-coupled modulation to your system!

---

## Patch Example: Distorted DNB Bassline

```
[DRUM SEQUENCER] → [BD808 GATE IN]
[HIGH VOLT LEVEL + ACCENT] → [BD OUT] → [DISTORTION/WAVEFOLDER] → [VCF] → [DELAY/REVERB] → [OUTPUT]
[ENV/LFO] → [VCF CUTOFF]
```
- Max out BD808 LEVEL/ACCENT, patch the output through a distortion for rip, follow with VCF for tone control, and animate the filter. Add delay/reverb for space.

---

## References
- [BD808 Manual (PDF)](https://tiptopaudio.com/manuals/BD808_Manual.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)