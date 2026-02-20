# 2hp — Unity

- [Manual PDF](../../manuals/2hp_Unity.pdf)

---

[2hp Unity Manual (PDF)](https://2hp.com/wp-content/uploads/Unity_Manual.pdf)

---

# Using the 2hp Unity Module in Full Length Eurorack Songs

The 2hp **Unity** module is a dual unity mixer with flexible summing, normalling, and gain modes for both audio and control signals (CV). While it’s a relatively simple utility, its careful integration into your system can be key for bringing musical development and performability to your modular compositions. Here’s how you can use Unity—paired with other modules—to structure and perform full songs in Eurorack format.

---

## Key Features for Song Development

- **6-to-1 or Dual 3-to-1 Mixer**: Mix more sources than usual in tight skiffs.
- **Averaging/Unity/Split Modes**: Gain staging for audio (preserves loudness) or control voltage (summation), even simultaneously.
- **Normalling**: Cascade the two mixers for more complex routing and functional patching.

---

## Techniques for Full Song Construction

### 1. **Performance Control: Dynamic Mixing and Section Mutes**
- Use Unity to combine multiple rhythm voices (e.g. multiple percussion modules).
- Patch drums to Mixer 1 and melodic voices to Mixer 2.
- Use manual patch cable insert/removal, mute switches, or sequential switchers (e.g., Mutable Instruments Branches or sequential switch modules) in tandem with Unity's OUT jacks to bring elements in/out—great for musical transitions, breakdowns, or drops.

### 2. **Automated Section Changes with CV**
- Unity in CV mode (Unity Mode) allows you to sum multiple sequencers or modulation sources into a single destination:
    - Mix several LFOs or envelopes to create evolving modulations for timbre, filter, or effects sends. Turn a static part into a dynamic one over the course of your song.
    - Sum two sequencer outputs to add melodic variation—a simple way to generate "verse" and "chorus" pattern changes.

### 3. **Creating Macro Controls**
- Use Unity to sum macro controls (knob, CV slider, or pedal input) with other automation sources. E.g., sum a slow LFO (overall filter sweep) and envelope (note accenting) into a filter cutoff, letting you "open up" a section live.

### 4. **Transition Building & Breakdown Techniques**
- Mix pre-set modulations or entire voices ready to be faded/blended in:
    - In **Split Mode**, blend control signals into a melody voice for modulated transitions, while mixing percussive voices at averaged gain for big drum drops.
    - Cascade the two mixers for a long multi-track buildup, slowly adding voices or modulated layers via the normalling feature.

### 5. **Song-Endings, Drops, and Climaxes**
- Use Unity to sum multiple effect returns (e.g., reverb, delay tails, or feedback loops) for dramatic climaxes.
- Patch Unity into a voltage-controlled amplifier (VCA). Use Unity to sum all voices for a sudden stop, drop, or sweeping fade-out controlled by a single CV or envelope.

---

## Example Song Structure Using Unity

1. **Intro**: Mix only atmospheric sounds and simple percussion in Unity Mixer 1; keep main melody sources unpatched or muted from Mixer 2.
2. **Build-Up**: Gradually add melodic voices via Mixer 2, begin to sum modulated envelopes to open up filters slowly.
3. **Chorus/Drop**: Patch the OUT of Mixer 1 (percussion) into Mixer 2 to combine full beat and melody, possibly summing in extra modulation for added energy.
4. **Breakdown**: Remove OUT cable from Mixer 1, bringing the energy back down to melodic components only.
5. **Outro**: Gradually reduce elements, fade out through VCAs or mixer, sum all voices into a reverb/delay feedback loop for a trailing end.

---

## Combine Unity with Other Essentials

- Pair with clock dividers/multipliers (e.g., Pamela’s New Workout) for timed changes, making transitions at musical intervals.
- Use mute/solo switches downstream for hands-on control.
- Combine with sequencers, CV/audio sources, performance mixers, and effect modules for max flexibility.

---

Unity may seem basic, but in Eurorack, simple utilities become the connective tissue of complex, performable music. Use it to seamlessly blend, automate, control, and evolve your patches over time. That’s the essence of modular songcraft!

---

## More Tools

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
