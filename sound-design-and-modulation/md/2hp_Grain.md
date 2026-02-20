# 2hp — Grain

- [Manual PDF](../../manuals/2hp_Grain_Manual.pdf)

---

[2hp Grain Manual PDF](https://2hp.com/docs/grain.pdf)

---

# 2hp Grain: Creative Modulation Tips for Unique Sounds

As a Eurorack modular synth musician, the 2hp Grain module gives you immense creative potential for everything from rude metallic percussion and dubstep basslines to haunting granular atmospheres. Below you'll find guidance on patching and modulating Grain for these styles, using the four key voltage-controlled parameters: Density, Mix, Frequency (pitch), and 1V/Oct.

---

## Module Overview & Key Modulation Points

**Key Inputs (modulatable):**
- Density CV (granular density & behavior)
- Mix CV (wet/dry blend)
- V/Oct (precise pitch)
- Freq (knob; pitch & speed; CV via V/Oct)

---

## 1. Distorted Percussive Sounds

To achieve hard hitting, distorted percussion:  
**Patch:** Fast envelope generators, stepped random sources, gates.

### Modulation Approaches:
- **Density CV:**  
  - Use a fast, sharp envelope, trigger, or stepped random voltage to Density CV.
  - When set left, grains are periodic—use sharp pulses for digital "hits."
  - Flick right for stochastic bursts and digital noise.

- **Freq Knob:**  
  - Turn left for sub-audio, crushed, metallic hits.
  - Try modulating Freq or the V/Oct input with sequences for "pitched" hits or with audio-rate signals for FM clang.

- **Mix CV:**  
  - Use envelopes to sweep from dry hit to fully wet/granularized sound.

- **Bonus:**  
  - Feed in drums or sharp transients, abuse the Density and Freq for glitchy, crushed percussive chaos.

---

## 2. Dubstep/Drum and Bass Basslines

For deep, moving basslines with grainy character:  
**Patch:** Sequencers, LFOs (slow to medium speed), audio-rate modulation.

### Modulation Approaches:
- **V/Oct & Freq:**  
  - Sequence V/Oct with pitch CV/gate for tuned melodies, basslines, or acid grooves.
  - Modulate Freq with a slow triangle LFO for growl and vowel shifts.

- **Density CV:**  
  - Use random or fast LFO for moving, jittery grain positions—“wubby” or talking bass effect.
  - Try audio-rate modulation for screaming/aliasing distortions.

- **Mix CV:**  
  - LFO sweep or envelope for movement between clean tone and full granular chaos.

- **Bonus:**  
  - Stack with a sub-oscillator at the input and saturate the output for huge, digital bass.

---

## 3. Atmospheric Pads & Haunting Textures

For eerie, slowly evolving pads:
**Patch:** Long, evolving samples/field recordings, slow LFOs, random CV.

### Modulation Approaches:
- **Density CV:**  
  - Modulate with very slow random/sample & hold for changing grain density/position, producing ghostly movement.
  - Try center position for sustained textures. Occasionally shift left/right for fades in/out of granular clouds.

- **Freq & V/Oct:**  
  - Sweep Freq manually or with slow LFO for spectral morphing.
  - Sequence V/Oct for evolving ambient melodies/transpositions.

- **Mix CV:**  
  - Fade between live and processed input for dreamy crossfades.

- **Bonus:**  
  - Stack multiple envelope followers or slow modulations to all CV points for generative, slowly shifting atmospheres.

---

### Socket Reference (for patching):
```
  [IN]    [DENS CV]
  [MIX CV] [V/OCT]
  [FREQ]  [OUT]
```
- All CV ranges are bipolar (-5V to +5V for Density & Mix; -1.5V to +5.5V for V/Oct).

---

## Quick Patching Recipes

**Perc Hit:**  
- Percussion audio → IN  
- Envelope (fast, snappy) → Density CV  
- ENV or random gate → Mix CV  
- Try: Audio-rate signal → V/Oct for wild metallics

**Dubstep Bass:**  
- Oscillator (saw/triangle) → IN  
- Sequencer → V/Oct  
- Slow LFO → Density CV, Mix CV  
- Try: FM into Freq or V/Oct for "scream"

**Atmospheres:**  
- Field recording/slow pad → IN  
- Slow random (S&H) → Density CV  
- Smooth LFO → Freq  
- ENV or LFO → Mix CV

---

**For further exploration, see the [2hp Grain Manual PDF](https://2hp.com/docs/grain.pdf)**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)