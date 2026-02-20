# Arcus Audio — Unity Mixer

- [Manual PDF](../../manuals/Unity Mixer - Arcus Audio.pdf)

---

[Unity Mixer Manual PDF (Arcus Audio)](https://arcusaudio.com/product/unity_mixer/)

---

## Creative Eurorack Patch Ideas for Distortion, Basslines, and Pads Using the Arcus Audio Unity Mixer

The **Arcus Audio Unity Mixer** is a compact, 2hp Eurorack utility with some hidden creative potential due to its dual 3:1 (or single 6:1) summing capability, DC-coupled inputs, and bi-color signal-level LEDs. While it's technically a "utility" module, you can push it into sound design territory, especially when combining audio and CV in unconventional ways.

### Key Capabilities Reviewed

- **Unity gain summing:** No gain, but transparent blending of sources
- **Dual 3:1 or single 6:1 mixing modes**
- **DC-coupled:** Suitable for audio and control voltages (CV)
- **Bi-color LEDs:** Immediate feedback on polarity and signal strength

---

## **1. Distorted Percussive Sounds**

**Technique:**  
Use the Unity Mixer for aggressive CV and audio mixing to create clipping, transient attacks, and unusual summing distortions.

**Patch Ideas:**  
- **Drive the Mixer with Hot Sources:** Feed in multiple drum voices, oscillators, or even triggers/gates directly (some modules output "hot" levels that sum into mild distortion). The unity gain may cause internal soft-clipping when summing 3+ strong signals.
- **Percussive Transients Layering:** Mix a snappy envelope (e.g., Maths EOR out) into an audio-rate oscillator, along with a noise burst. Route the mixed signal straight to a VCA, then to a wavefolder or distortion for even gnarlier impact.
- **Sending Negative CV:** Flip the polarity on one input source (using an external inverter) and mix with audio – causing subtractive cancellation and asymmetric clipping for "broken" percussive artifacts.

---

## **2. Crazy Dubstep/Drum & Bass Basslines**

**Technique:**  
Combine multiple LFOs, envelopes, and audio-rate signals (oscillators, even wavetables) into the Unity Mixer, achieving wild, modulated bass movements.

**Patch Ideas:**  
- **Multiple LFO Summing for Wobble:** Take 3 LFOs at different sync rates, mix them in one group, and patch that output to modulate a filter or VCA opening your bass oscillator. This gives highly complex, rhythmic bass wobbles.
- **CV+Audio Modulation:** Patch a sub-oscillator, a detuned oscillator, and a negative envelope into the Unity Mixer; this new complex bass audio source can be routed through wave-shaping for those DnB growls or dubstep snarls.
- **Bicolor LEDs as Feedback:** Use the LEDs to watch for clipping or polarity reversals—push signals into the red for that broken, glitchy sound characteristic of harder genres.

---

## **3. Haunting Atmospheric Pads**

**Technique:**  
Sum multiple slow, undulating LFOs and envelopes (e.g., from Batumi, Zadar, or Maths) to modulate filters, resonators (like Rings or Clouds), or even CV-controlled FX.

**Patch Ideas:**  
- **Complex Filter Sweeps:** Mix an envelope, a slow sine LFO, and a randomly modulated S&H into one channel. Use this output to sweep a lowpass or bandpass filter on a pad voice—movement becomes rich and unpredictable.
- **Ambient Layer Blending:** Combine outputs of two or three different drone oscillator voices (e.g., sine, triangle, wavetable pad), shaping their combined amplitude for lush, blurred soundscapes.
- **CV Overlap:** Modulate two separate effect parameters (e.g., reverb size + filter cutoff) with one summed, evolving CV, creating an organic, spectral shift in the pad textures.

---

### **Bonus Tips**

- Because the **Unity Mixer is DC-coupled**, try feeding it a blend of audio-rate, LFO, triggers/gates, and even random voltages for unpredictable audio/CV cross-pollination.
- Experiment with patching the mixer’s output into distortion, wavefolders, or even back into itself (feedback loop with attenuation!) for more chaos and textures.
- Using those **bi-color LEDs**, push your patches until you see strong color changes, then dial back for subtlety.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)