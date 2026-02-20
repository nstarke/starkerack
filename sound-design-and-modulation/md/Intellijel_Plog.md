# Intellijel — Plog

- [Manual PDF](../../manuals/plog_manual.pdf)

---

[**Intellijel Plog rev 1.0 Manual (PDF)**](https://cdn.modulargrid.net/documents/manuals/2738/Plog_Manual.pdf)

---

# Creative Modulation Techniques with the Intellijel Plog

The **Intellijel Plog** offers deep voltage-controlled logic manipulation, ideal for pushing boundaries in percussive, bass, and atmospheric sound design. Let’s break down advanced creative uses, matching your stylistic goals:

---

## 1. Distorted Percussive Sounds

### Approach 1: Logic-Gated Ringing & Crunch

- **Source**: Route multiple drum trigger/gate patterns (e.g., from sequencers or random clocks) into the X and Y inputs of Logic Block A.
- **Logic Setting**: Use **AND** or **XOR**; they create “missing” hits and rhythmic holes.
- **Modulation**:  
  - CV-modulate the logic TYPE (with fast random or audio-rate CV for glitchy artifacts).
  - Use an LFO or envelope into the TYPE A CV input, and attenuate with the front panel knob.
- **Output**: Take OUT A to a VCA or directly to a distortion effect.
- **Variation**: Feed OUT A to a wavefolder or bitcrusher; the choppy logic-gated pulses will produce aggressive, crunchy textures.

### Approach 2: Flip-Flop Gating and Clipping

- Use TOGGLE flip-flop as a clock divider for micro-rhythms.
- Feed fast divided outputs (OUT T and OUT D) into percussive CV destinations or trigger short-sharp envelopes that control sound sources with distortion downstream.

---

## 2. Crazy Dubstep/Drum & Bass Basslines

### Approach 1: Rhythmic Logic on Bass Oscillators

- **Sources**: Take two or three synced or unsynced oscillators (audio-rate or LFOs) and patch them to X, Y, and Z of Logic Block A/B.
- **Logic Setting**: Set to **XOR** or **XNOR**. These generate complex, harmonically rich, and sometimes “digital” square waves—great for harsh basses.
- **Modulation**:
  - Use sequencer or random voltages to CV-modulate TYPE A/B, morphing between logic types in real time.
  - Apply envelopes or stepped/chaotic LFOs so the logic switching syncs with the beat or is tempo-randomized.
- **Output**: Feed OUT A through a wavefolder, filter, and distortion. The constantly morphing logic outputs make for dynamic, tearing basses.
- **Patch Flip-flops**: Use the flip-flop output as a sub-oscillator or to generate re-triggers for envelopes applied to the main bass signal.

### Approach 2: Abrupt Gating & Clock Skipping

- Clock a sequencer with OUT T or OUT D for “missing” or doubled bass steps—great for unpredictable drop patterns.
- Use data flip-flop (DFF) as a gated switch to sync movement between two bass elements (e.g., squelch and sub), toggling their roles based on clock pulses or logic events.

---

## 3. Haunting Atmospheric Pads

### Approach 1: Randomized Logic Envelopes

- **Inputs**: Send evolving/random LFOs or slow “environmental” generative gates into X, Y, Z of Logic A/B.
- **Logic Setting**: Use **OR** or **NOR** for layered, ghostly triggers. These create complex patterns as the inputs subtly drift in and out of logic highs.
- **Modulation**:
  - Slowly sweep the logic TYPE via modulation (using S&H, slow LFOs, or looping envelopes) for evolving, unpredictable pad articulation.
  - Feed the resulting OUT A/B to long, slowly-decaying envelope generators, which in turn drive spectral processors, reverb, or granular modules.
- **Flip-Flop**: Use as clock dividers for ultra-slow envelopes, so layers fade in and out at glacial rates.

### Approach 2: Logic-Driven Layered Chording

- Use OUT A/B to enable/disable polyphonic voice chains or switch harmonizer paths, creating pad textures that are constantly “switching” layers in and out based on evolving logic rules.
- The results can feel both random and intentional—perfect for organic, shifting ambiences.

---

## Additional Tips

- **Audio-Rate Modulation**: Plog handles signals up to 5V, but the comparators mean you can “abuse” it with audio-range signals for freezer, S&H, or harsh digital audio mangling.
- **Normalling**: Take advantage of the Plog’s normalization to quickly create “clock divider chains” for polyrhythms without heavy patching.
- **Saving/Recalling**: Use the STORE/LOAD button combos to quickly A/B complex logic states during performance.
- **Preset Performance**: Modulate logic selection via hands-on performance (button presses) mid-jam for “button mash” glitch.

---

## Quick Patch Example Recipes

### "Agitated Kick Gate"
- Drum seq gate → X
- Random LFO gate → Y
- AND logic, CV modulate TYPE A with audio-range triangle LFO for rapid stutter.
- OUT A → LPG or digital VCA + hard clipping/distortion

### "Glitchstep Bass Ripper"
- Two VCO squares (octave apart) → X and Y
- XOR logic, CV mod TYPE A with stepped random S&H
- OUT A → LPF → distortion/saturator

### "Shifting Phantom Pads"
- Slow random gates (from Turing Machine or Marbles) → X, Y
- NOR logic, TYPE A CVed by slow LFO
- OUT A → Slow AD envelope → FM amount on reverb or delay diffusion
- OUT T → occassional very slow gate to trigger granular re-freeze

---

**Reference Manual:**  
[https://cdn.modulargrid.net/documents/manuals/2738/Plog_Manual.pdf](https://cdn.modulargrid.net/documents/manuals/2738/Plog_Manual.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)