# 2hp — Slice

- [Manual PDF](../../manuals/2hp_Slice.pdf)

---

[2hp Slice Manual (PDF)](https://www.twohp.com/_files/ugd/2dae2a_d9bdc3a9d03d425f8141a639154a12ca.pdf)

---

# 2hp Slice: Advanced Modulation & Sound Design Tips

## Module Overview

The **2hp Slice** is a powerful beat repeat/glitch engine for Eurorack that is clock-driven, with flexible beat size, triplet toggles, and hands-on or CV activation. The key to unlocking unique sonic results is creative modulation and patching.

Below, I’ll break down methods for generating the specific types of sounds you mentioned:

---

## 1. Distorted Percussive Sounds

**Technique:**  
- **Input:** Route drum hits, sharp noise, or synthesized percussion into the Audio Input.
- **Size Modulation:** Patch a high-speed, jagged LFO or stepped random voltage (e.g. from a sample & hold like a Turing Machine or 2hp Rnd) into the **Size CV Input**. Abruptly changing the repeat size during playback can create stuttered, warped effects that verge on distortion.
- **Triplet Toggle:** Toggle this up to inject triplet divisions for more complex, off-grid burst patterns.
- **Gate Triggering:** Use a fast, irregular gate pattern to the **Trig Gate Input** (for example: from a clock divider/multiplier or probability gate module). Changing the **gate mode** (latching vs. momentary) with the Trig button at boot offers different activation “feel” for your glitches.
- **External Processing:** After the Slice, send audio through a wavefolder, distortion, or aggressive VCA to further mangle the repeated sound.

**Patch Example:**  
- Drum out → Slice Audio In  
- Turing Machine Random CV → Size CV In  
- Clock Divider Out → Trig Gate In  
- Enable triplets  
- Slice Out → VCA/Distortion → Mixer

---

## 2. Crazy Basslines (Dubstep/Drum & Bass Style)

**Technique:**  
- **Input:** Use a synth voice or dedicated bass oscillator with sharp attack modulation for your primary bassline, routed to Audio Input.
- **Clock Rate:** Modulate **Clock Input** with variable speed clocks for groove-swings, half-time/double-time rolls.
- **Size Knob & CV:** Manually tweak or automate via slow/random LFO or envelope follower, synced to your main groove, into **Size CV**—this will gate the “window” of the repeat and create those chopped, pitch-jumpy effects.
- **Trig/Gate Input:** Sequence activation in spots where you want “fills”, rhythmic breaks, or drop buildups.
- **Triplet Toggle:** Add or remove for rhythm complexity, but in dnb/dubstep, rapid 1/32 and 1/64 repeats are very effective for the “machine gun bass” feel.
- **Post-Slice FX:** Try running the output into a filter with heavy modulation and/or saturation to accentuate aggressive timbre changes.

**Patch Example:**  
- Synth Bass Out → Slice Audio In  
- Euclidean Rhythm Generator → Clock In  
- S&H or Wogglebug → Size CV In  
- Stepped Gate Seq → Trig Gate In

---

## 3. Haunting Atmospheric Pads

**Technique:**  
- **Input:** Long, evolving samples, slow pads, or granulated textures into Audio In.
- **Size Modulation:** Subtle slow LFOs (e.g. sine, triangle at <1Hz) or smooth random (wobbly) CVs into Size CV—changing repeat length gently to “smear” the pad sound and introduce a shifting, fractured haze.
- **Triplet Toggle:** Down (removed) for straight feel, up (included) for unstable, stuttering ghostliness.
- **Manual Trig:** Use the Trig button yourself at moments to freeze and repeat textures, or sequence it for timed “pad swells”.
- **External CV:** Modulate the input signal’s filter cutoff or waveshaper in sync with the repeat for evolving overtones.
- **Reverb:** Add heavy reverb/delay after Slice output to heighten the ethereal effect.

**Patch Example:**  
- Complex Pad/Field Recording → Slice Audio In  
- Slow LFO → Size CV In  
- Manual or slow gate → Trig Gate In  
- Slice Out → Lush Reverb  

---

## Experimental Tips

- **Buffer “Freeze” Exploitation:** Use latching mode for drone textures—trigger repeat and let it ride for static, looping fragments.
- **Clock at Audio Rate:** Input a VCO as Clock to produce digital audio-rate repeats—yields bit-crushed, granular textures.
- **CV Pairings:** Use the 2hp Play, Rnd, or Loop for further sample processing, as suggested in the manual; mult LFOs/random to both size (Slice) and pitch (Play).

---

## Key Creative Patch Points

- **Size CV Input** is your main modulation lane: fast changes = glitchy, slow = evolving/refracted.
- **Clock Input** lets you sync or destabilize groove: try odd rhythms, clock swings.
- **Manual vs. Sequenced Activation:** Use both for maximum organic variation.
- **Triplet Toggle:** Rhythmic “flavor” overlay—experiment liberally!

---

**For more ideas and patch inspiration:**  
[Full 2hp Slice Manual (PDF)](https://www.twohp.com/_files/ugd/2dae2a_d9bdc3a9d03d425f8141a639154a12ca.pdf)  
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
