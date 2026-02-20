# 2hp — Kick

- [Manual PDF](../../manuals/2hp_Kick.pdf)

---

[Kick Module Manual (PDF)](https://intellijel.com/downloads/manuals/kick_manual.pdf)  
*(Note: If this is not the exact module/brand, please adapt to your module's manufacturer as needed.)*

---

# Using the Kick Module for Full Length Eurorack Songs

Your **Kick** module is a versatile 2HP analog bass drum synthesizer with powerful control voltage (CV) capabilities. While it excels at creating punchy, reactive, and varied kick drum sounds, its real musical power comes through when combined thoughtfully with other Eurorack modules and performance strategies. Below are approaches, patch ideas, and compositional concepts for turning the Kick into a foundation for engaging, evolving, full-length songs.

## 1. Dynamic Rhythm Structures

**Challenge:** Static, "looped" beats can quickly become monotonous in long-form works.  
**Solutions with Kick:**
- **Vary Triggers:** Use a sequencer with multiple patterns, or employ logic modules (AND, OR, XOR) to combine rhythmic sources for the **TRIG** input. This enables you to switch up the rhythm, add skip steps, create fills, or introduce polyrhythms.
- **Accent Variation:** Patch velocity or accent CVs from your rhythm sequencer to **Tone** or **Pitch** CV for dynamically accented kicks (e.g., "harder" on beats 1 & 3).
- **Euclidean & Probability:** Use modules like Pamela’s New Workout or Euclidean Circles to create evolving, generative kick patterns that can change over the course of a song.

## 2. Tonal Variation and Transitions

**Challenge:** Many techno, electro, and ambient tracks benefit from timbral variation in drum sounds to signal transitions, breakdowns, or building energy.  
**Solutions with Kick:**
- **Automate Tone and Decay:** Use CV sequencers, LFOs, or Random sources to subtly (or dramatically) morph the **Tone** and **Decay** over time. Longer decay in breakdowns, sharper attack in drops.
- **Pitch as Bassline:** With 1V/Oct CV tracking, sequence the Kick’s **Pitch** input from a bassline sequencer. This lets you tune the kick as part of your bassline, or even morph it into sub bass in breakdowns.
- **Distortion for Climaxes:** Push the **Tone** CV into the overdriven (left) region for noisy/distorted climaxes, then return to clean for verses or breaks.

## 3. Arrangement and Song Structure

**Challenge:** Crafting a "narrative arc" in modular music.  
**Solutions with Kick:**
- **Event-based Mutes:** Use clock dividers, switch modules, or manual muting (via VCAs or sequential switches) to drop the Kick in and out for breakdowns, fills, and drops.
- **Scene Morphing:** Patch macro CV sources (Pressure Points, Planar, or a performance controller) to multiple parameters at once, allowing you to sweep the intensity and characteristics of the beat as you move from intro to chorus to outro.
- **CV Morphing:** Commit to long, evolving automation curves (using an envelope follower or slow LFO) on **Decay** or **Pitch** for organic, non-looping movement.

## 4. Layering and Sound Design

**Challenge:** A single Kick voice can lack presence.  
**Solutions with Kick:**
- **Layered Kicks:** Mult your trigger and send to another kick or percussion module tuned to complementary pitch. Blend with VCAs and crossfaders.
- **Add Sub Harmonics:** Use sub oscillator modules or pitch shifters to create tuned low end beneath the Kick’s output, especially in breakdowns or intros.

## 5. Integration with Melodic and Harmonic Content

**Challenge:** Cohesion between drums and melodic elements.  
**Solutions with Kick:**
- **Track Key Changes:** Use a global transpose CV source (from a master sequencer or quantizer) split to both bassline/pads and the Kick’s 1V/Oct input so kick pitches relate musically throughout.
- **CV-Driven Timbre Sync:** Modulate Kick’s Tone/Decay with the same LFOs or envelopes used on leads or chords for unified movement.

## 6. Live Performance Tips

- **Manual Overrides:** Use attenuverters or performance-oriented CV sources to “play” the parameters live.
- **Real-time Pattern Changes:** Switch trigger/gate patterns on-the-fly via manual or CV control to realign the Kick’s groove as your song develops.

## Example Patch: Full Song Structure

1. **Intro:** Minimal triggers, long decay, Tone swept by slow LFO for a reverb-y, atmospheric kick.
2. **Verse:** Regular rhythm, medium decay, “clean” Tone, pitch locked to bassline (1V/Oct from melodic sequencer).
3. **Chorus/Drop:** Increase trigger density, saturate Tone for distortion, max decay, high energy.
4. **Breakdown:** Remove triggers, let last kick decay; slowly modulate Pitch down for a dubby echo.
5. **Finale:** Bring elements back in, automate Pitch and Decay for “build” effect.

---

## Additional Resources

- For even more generative control and custom patching, see: [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---
*Ready to turn your beats into full tracks? Think modular: every patch can be a song in itself.*