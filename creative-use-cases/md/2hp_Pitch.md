# 2hp — Pitch

- [Manual PDF](../../manuals/2hp_Pitch.pdf)

---

[2hp Pitch Manual PDF](https://twohp.com/resources/pitch/PITCH_manual.pdf)

---

# Creative Ways to Use 2hp Pitch in Your Modular System

The 2hp Pitch is a compact, time-domain pitch shifter with integrated wow & flutter for authentically “wobbly” tape and vinyl-like pitch modulation. Below are some inventive patch ideas and module combinations to maximize its potential in your Eurorack system:

## 1. Faux Dual Oscillator (VCO Pairing)

**Concept:**  
Use the Pitch module after a basic VCO (analog or digital) to easily achieve dual-oscillator timbres, stacked harmonies, or dense mono/poly textures without a second VCO.

**How:**  
- Patch your primary VCO into 2hp Pitch (audio in).
- Pitch-shift the output up/down by a set interval (fifth, octave, etc.) with CV or the pitch knob.
- Mix this with the VCO's dry output using a mixer, or blend the dry/wet on Pitch itself.
- Heavy wow & flutter can simulate “drift” in one oscillator—perfect for classic synth warmth.
- **Example Modules:** Make Noise STO, Intellijel Dixie II+, Mutable Instruments Plaits.

---

## 2. Harmonic & Timbral Processing (Waveshapers/Folders)

**Concept:**  
Send pitch-shifted audio into a waveshaper/wavefolder or filter for unique harmonic results. Pitch shifting introduces new intervals and overtones that react in dramatic and unexpected ways to further processing.

**How:**  
- Audio Source → 2hp Pitch (subtle or extreme shift) → Wavefolder (e.g., Befaco Chopping Kinky) or Filter (e.g., Ripples).
- Modulate the Pitch's wow & flutter for animated, organic sonic movement—especially good for drones or pads.

---

## 3. Creating Lush Textures (Reverb/Delay/Looper)

**Concept:**  
Add “tape machine” character to reverbs, delays, and loopers by pitching and fluttering the input or output. Great for generative ambient, lush sound beds, and pseudo-tape warble.

**How:**  
- Place 2hp Pitch before or after a looper (e.g., 2hp Loop, Mutable Instruments Clouds for granular looping).
- For shimmer-style effects, run reverberated audio back into 2hp Pitch and blend octaves.
- Modulate wow & flutter for deep tape echo feel (send short “tape” repeats to delay, e.g. Make Noise Mimeophon or Erica Synths Pico DSP).

---

## 4. Glitchy Percussion Reshaping

**Concept:**  
Transform drum loops or one-shots (from a sample player or drum module) with extreme pitch shifting or modulated wow & flutter, producing glitch, IDM, and experimental textures.

**How:**  
- Sample Source/Drum Machine → 2hp Pitch (modulate wildly with stepped random, sample & hold, or sequencer CV) → output.
- Combine with a drum filter or stutter module to accentuate lo-fi, chopped flavors.
- **Example:** Patch the W&F CV input with an LFO, S&H, or random source (e.g., Mutable Instruments Tides, Wogglebug).

---

## 5. Animated Sequences & Dynamic Melodies

**Concept:**  
Animate pitch shifts via sequencer or CV for evolving riffs and melodies, or create harmonic counterpoint with arpeggiated lines.

**How:**  
- Use a pitch CV/Gate sequencer (e.g., Arturia Keystep, Malekko Varigate) to modulate both your VCO and the Pitch's 1V/oct input. Offset or invert one of the sequences for rich counterpoint.
- Animate the Mix CV input for morphing between dry and wet signals in real time, using a synced envelope or LFO for dynamic movement.

---

## 6. Lo-Fi Freeze and Harmonic Freezing

**Concept:**  
Pair with 2hp Freez or another looper/stutter module for sound design. Freeze slices of heavily pitch-shifted and fluttered audio for evolving lo-fi pads and textures.

**How:**  
- Chain: VCO or Noise > Pitch (max wow/flutter) > Freez > Reverb/texture FX.
- Modulate both modules' parameters for a range from mild tape shimmer to total glitch meltdown.

---

## 7. Stereo Widening/Detune Techniques

**Concept:**  
Send a dry signal to one channel and the pitch-shifted, fluttered signal to another for instant stereo wideness and animation—excellent for thick basses, leads, or synth layers.

**How:**  
- Use a mult or buffered splitter.
- L ↔ dry, R ↔ wet (pitch up, wow/flutter modulated).
- Pan hard left/right for classic chorus, or modulate pitch for extra width.

---

## General Module Type Recommendations

- **VCOs** (any flavor) for harmonic stacking
- **Mixers/Crossfaders** for dry/wet blending (e.g., Happy Nerding PanMix, Doepfer A-138)
- **Loopers/Granular Samplers** (Mutable Clouds, 2hp Loop)
- **Envelope Generators/LFOs/Random** (modulate Pitch/W&F CV)
- **Delays/Reverbs** for ambient tails
- **Drum Machines/Samplers** for unpredictable percussion
- **Wavefolders/Filters/DISTORTION** for sculpting shifted tones

---

**Further Reading:**  
[2hp Pitch Manual PDF](https://twohp.com/resources/pitch/PITCH_manual.pdf) (official)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
