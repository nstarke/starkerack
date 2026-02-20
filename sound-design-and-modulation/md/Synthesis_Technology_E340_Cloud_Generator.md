# Synthesis Technology — E340 Cloud Generator

- [Manual PDF](../../manuals/E340_manual.pdf)

---

[**E340 Cloud Generator Manual (PDF)**](https://synthtech.com/docs/E340manual.pdf)

---

## Modulating the E340 Cloud Generator for Unique Sounds

The E340 Cloud Generator is an 8-VCO super oscillator designed for producing thick, detuned, and modulated waveforms ideal for pads, leads, FX, and more. Here’s an analysis of how to leverage its controls and CV inputs for:

- **Distorted Percussive Sounds**
- **Crazy Dubstep/Drum & Bass Basslines**
- **Haunting Atmospheric Pads**

### Overview of Creative Modulation Points

| Control / Input      | Description & Modulation Tips                                                                             |
|----------------------|-----------------------------------------------------------------------------------------------------------|
| **SPREAD / CV**      | Detunes VCOs exponentially; modulate via envelopes or LFOs for comb-filter, swarm, or pulsing effects.    |
| **CHAOS / CV**       | Adds filtered noise FM to VCOs; modulate with fast CV for animated, unstable timbres.                     |
| **CHAOS BW / CV**    | Sets speed of chaotic motion; CV control lets you sweep from slow drift to rapid "shredding" movement.    |
| **DENSITY Switch**   | Select between 2/4/8 oscillators – lower for punch, higher for huge/fuzzy walls.                          |
| **FM / CV**          | Pitch FM input; use at audio-rate for metallic, clangorous distortion or at audio-LFO rates for wobble.   |
| **SYNC Input**       | Reset the phase for hard sync; sync’ing with sharp transients creates aggressive, percussive attack.       |

---

### Sound Design Recipes

#### 1. **Distorted Percussive Sounds**

- **Kick/Drum Voice:**  
  - Patch a short, sharp envelope (e.g., from Maths/function generator) to the FM input for rapid pitch drop "thwacks".
  - Patch the same or another envelope into SPREAD CV for oscillator detune sweeps during the attack phase.
  - Increase CHAOS for complex clicks/texture, and sweep CHAOS BW for glitch/bitcrush-style percussion.
  - Sync E340 to rimshot, drum trigger, or clock pulse for "sync pop" artifacts.
- **Distortion Tips:**  
  - Patch the SAW OUT into a wavefolder or external distortion module for extra aggression.
  - Increase FM depth or feed in an audio-rate modulator (other VCO) into FM for metallic clang and noise attack.

#### 2. **Crazy Dubstep/Drum & Bass Basslines**

- **Wobble Bass:**  
  - Use a slow LFO or synced envelope into SPREAD CV to morph harmonic content—great for rhythmic movement.
  - Mult a fast, stepped random CV into CHAOS and CHAOS BW for unpredictable movement and animated vowel-like shapes.
  - Use DENSITY at 4 or 8 for a thick, gnarly sound; switch to 2 for sharper, more cutting bass plucks.
  - Patch a sequencer or keyboard CV to 1V/OCT for bassline melodics.
- **Dirty Growl:**  
  - Audio-rate modulate FM with another VCO (try a saw or square) for "talking", "formant", or growling dubstep tones.
  - Sync to a drum part for tearing, rhythmic sync’d bass FX.

#### 3. **Haunting Atmospheric Pad Sounds**

- **Evolving Pads:**  
  - Set DENSITY to 8, open the SPREAD and slowly modulate with a slow LFO or slow random CV for a shifting "cloud" effect.
  - Gradually increase CHAOS via an envelope or random LFO for evolving textures.
  - Modulate CHAOS BW for background shimmer or turbulence.
  - Mix SINE OUT (for body) with SAW OUT (for brightness) for complex timbres.
- **Drone Variance:**  
  - Use two slow LFOs with different shapes into SPREAD and CHAOS CVs for overlapping, psychoacoustic motion.
  - Add a hint of FM from another VCO for subtle inharmonicity and richness.
  - Use a reverb or delay after the E340 to enhance the “haunted” vibe.

---

### Extra Mod Tips

- **Stack multiple modulation sources (LFOs/envelopes/random) using a CV mixer to create evolving, non-repetitive movements.**
- **Experiment with extreme values:** Pushing SPREAD, CHAOS, and FM to max for total mayhem or pulling them back for subtler nuance.
- **Use muted or voltage-controlled attenuators preceding E340 CV inputs for more nuanced, hands-on control.**

---

> Find more Eurorack processing resources at  
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
