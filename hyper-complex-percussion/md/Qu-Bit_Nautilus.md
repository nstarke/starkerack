# Qu-Bit — Nautilus

- [Manual PDF](../../manuals/Nautilus_v1.1.3.pdf)

---

[Download Nautilus Manual (PDF)](https://www.qubitelectronix.com/files/manuals/Nautilus_Manual_FW_1.1.3.pdf)

---

# Qu-Bit Nautilus: Dense, Hyper-Complex Percussion & Polyrhythms

The Qu-Bit Nautilus is a highly innovative, aquatic-inspired complex delay module ideal for generating extremely dense, polyrhythmic, and percussive textures. Here’s how you can leverage its features specifically for hyper complex, intricate rhythmic music—whether as an effect or an unconventional percussion voice:

## Key Features for Percussive, Rhythmic Complexity

### 1. **Multi-Delay Structure & Clocking**
- **8 Configurable Delay Lines**  
  Each sensor adds more delay lines, letting you create intricate echoes and multi-layered patterns that can overlap and interact in unpredictable ways.
- **Div/Mult with the Resolution Knob**  
  Experiment with the various clock divisions and multiplications (e.g., triplets, dotted notes, 64ths, 512ths), then modulate this via CV for evolving time structures.
- **Internal/External Clock Sync**  
  Use odd, wonky, or variable clock sources. Send in clocks with polyrhythmic gate patterns from sequencers (or modulation sources like Pam’s New Workout, Tempi, etc.) to create irregular, complex, and syncopated repeats.

### 2. **Sensors & Dispersal: Polyrhythm Generation**
- **Sensors Knob** – Controls how many delay taps are active. Turn this up to "stack" multiple delays, each a potential percussive repeat.
- **Dispersal Knob** – Controls spacing between those taps. At low values: tight flams and quick clusters; at high: wide, unpredictable delay spacing (= polyrhythms).
    - Try modulating Dispersal for live “strums”, stutters, or pseudo-random grid shifts.
    - Combine both at mid/high settings to create ratcheting stutters, canonic textures, or rhythmic cascades.

### 3. **Reversal: Rhythmic Reversals and Sound Chops**
- Assign Reversal to specific or all delays, flipping some taps backward for chaotic, chopped, “reverse snare” or “reverse hat” energy. Automate via CV for constantly shifting texture.

### 4. **Chroma & Depth: Character and Punch**
- **Variable Bitcrusher, Saturation, Wavefolding, Distortion**: 
    - Use these for hyper-digital “grain” or snap; bitcrushing and wavefolding impart punch and compute-percussion grit.
    - Depth CV lets you put these effects under sequencer/LFO control for “percussive effect hits” or rhythmically modulated character.
- **Highpass/Lowpass Filtering:**  
    - Can make space in the mix and "tighten" repeats for percussive clarity.

### 5. **Freeze, Purge, Feedback**
- Use Freeze to chop out rhythmic buffers, essentially turning sections of your mix, drums, or noise source into repeating “locked” loops—with polyrhythmic Resolution clocking.
- Purge = instant “stutter-stop”; combine with clocked modulation for live-performance fills or rolls.
- Feedback cranked = Karplus-style metallic percs, or digital snare/bell artifacts. Feed in short triggers/impulses to accentuate.

### 6. **Feedback Modes: Routing Patterns**
- **Ping Pong**: Wide, shifting rhythmic echoes (great for stereo panning percs).
- **Cascade**: Delays feed into each other for ultra-long, canonic/rhythmic washes, almost like a polyrhythmic multi-tap "ratchet".
- **Adrift**: Each delay line moves to the next on the opposite channel, generating “shifting” stereo patterns that land off the main beats.

### 7. **Self-Modulation & Sonar Output**
- **Sonar Output** provides evolving stepped CV (or gates) derived from Nautilus’s internal calculations; can be used to modulate Nautilus itself or something else—great for making the module “self-generative”.
- Patch Sonar into Dispersal, Chroma, or Depth CV for evolving, self-oscillating patterns—never the same twice!
- Use a splitter (“The Octopus” patch) to distribute Sonar CV across multiple parameters for madcap complexity.

---

## Practical Patch Example: "HyperPoly Perc Drum Lab"

**Source:** Short percussion/hat/snare/stab sample or impulse  
**Routing:** Sound source → Nautilus L input (R normalized)  
**Clock:** Irregular/polyrhythmic gate from a clock divider, clock generator, or crazily programmed sequencer.

### *Nautilus Settings*
- **Sensors**: 3–4 (multiple delays for density)
- **Dispersal**: Modulate via LFO/random CV, slow/medium speed, keep somewhere mid-high for polyrhythms.
- **Resolution**: 16th or 32nd, but try automated, stepped modulation for variety.
- **Reversal**: Modulate by a slow random for unpredictable glitch fills.
- **Chroma**: Set to bitcrusher or wavefolder, Depth at 60–100% for crisp, digital attack.
- **Feedback**: Just under infinite for “machine gun” repeats that fade slowly.
- **Freeze**: Patch a gate pattern (or trigger by hand) on fills/breaks.
- **Output**: Stereo out into mixer or reverb—for “bouncing” polyrhythms.

**Optional**: 
- Route Sonar out to modulate Chroma, or even feedback something else (e.g. trigger stereo panning in a VCA).

---

## Additional Tactics

- **Clock modulation**—clock-in does not have to be regular or perfectly quantized. Use clock-bursts, Euclidean patterns, or gates from generative sequencers.
- **Use external CV sources** to randomize parameters every bar, or every few steps, for even more chaotic percussion.
- **Process traditional drum voices** through Nautilus for “hyper-layered” grooves—each hit will generate new percussive overlaps.
- **Patch in audio-rate triggers** or chopped audio, and use high Sensors + Dispersal to create percussive drones or metallic percussion beds.

---

## End Result

With careful parameter modulation and creative use of the multi-tap, modulated delays, Nautilus can serve as both a dense "delay percussion" generator and a rhythmic texturizer/effect, capable of producing constantly shifting, organic polyrhythmic grids. You’re not limited to the "grid" of your sequencer or DAW; the delay network becomes a living, percussive instrument!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)