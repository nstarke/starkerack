# Xaoc Devices — Batumi

- [Manual PDF](../../manuals/xaoc_batumi2_poti2_manual.pdf)

---

[**Xaoc Devices Batumi II & Poti II Operator's Manual (PDF)**](https://xaocdevices.com/manuals/xaoc_batumi_ii_manual.pdf)

---

# Using Batumi II & Poti II to Create Full Length Songs in Eurorack

As a modular synth musician, one of the most common creative hurdles is turning a solid loop—drum groove, bassline, melody—into a **composition that evolves over time**. The Xaoc Devices **Batumi II** quadruple LFO (and the optional Poti II expander) is designed to be more than just a “modulation source.” Its synchronization, phase manipulation, multiple outputs, assignable waveforms, and individual channel CV control make it a **powerful song-structuring instrument**. Below, I'll present concrete techniques and patching ideas to help you use Batumi II to turn creative fragments into **full length, dynamic tracks**.

---

## 1. **Master Modulation Clock and Transitions**

**Batumi II** can function as the "brain" of your patch, keeping various musical elements in sync or subtly shifting them to create evolving arrangements.

### Song Structure Macro-Modulation
- **Free/Phase/Divide/Mult Modes:** Set Batumi II to divide or multiply, then use its channels to distribute time-related CV to:
    - **VCA/LPGs** for fades, mutes, or evolving timbres.
    - **Filter cutoff** for gradual timbral shifts between sections.
    - **Sequencer reset or direction** (reset/sequencer stepping): Reset the start point of melodic/rhythmic phrases at big transitions.
- **Master Clocking:** In *mult* mode, one channel can advance a sequencer at standard tempo (e.g., 1/16th notes), another can send a signal every 32 steps to introduce fills, break sections, or transitions.
- **Global Transitions:** Use the **reset/sync inputs** on Batumi II to re-align all LFOs with a clock, trigger abrupt changes, or real-time "DJ-style" drops and returns.

### Morphing States (Dynamic Arrangement)
- Send Batumi II's **random or phase-shifted waves** to:
    - **Waveshaper or distortion CV** for phrases that rise in intensity over multiple bars.
    - **Reverb or delay wet/dry CV**, fading FX in/out over time.
    - **End-of-cycle gates** (from other slew or logic modules) to automate scene changes every few minutes.

---

## 2. **Polyrhythms and Evolving Rhythmic Structures**

One of the most powerful song-building techniques in modular is **polyrhythm and phase manipulation**.

- **Divide/Multiply Modes:** Have Batumi II produce different subdivisions/multiplications from a master clock:
    - Channel A: 1x (main rhythm)
    - Channel B: /3 (triplets or 3-bar pattern)
    - Channel C: /5 (odd meter or cross-rhythm)
    - Channel D: x4 (fast fills or ratchets)
- Use these outputs to trigger drum voices, envelope resets, or rhythmically mute/unmute voices for song sections that *push and pull* against each other, creating **textural variety over time**.

### Evolving Drum Patterns
- *Phase mode*: Use the phase offset per channel to subtly rotate rhythmic elements (e.g., analog-triggered percussion) across the stereo field or as rhythm "shifting" fills.
- *Reset inputs*: Re-synchronize polyrhythmic elements at key song moments for impactful transitions.

---

## 3. **Long-Form Timbral/Tonal Automation**

Batumi II's **slow rates (as slow as 0.00001 Hz!)** allow you to automate macro-level musical changes over several minutes, not just seconds.

- **Voices/OSC parameter drift**: Slowly modulate oscillator waveshape, FM amount, or pitch for evolving melodies or pads that never repeat exactly.
- **Tonal Evolution**: Morph filter resonance/cutoff, wavetable position (if using digital oscillators), or crossfader positions between sound sources for cinematic builds.
- **Random Waveform Output**: Use Batumi’s sample & hold or smooth random outputs to automate parameters literally for *hours* without obvious looping—great for ambient or generative pieces.

---

## 4. **Individual Song Sections Control with Poti II**

The **Poti II expander** adds **per-channel CV attenuation, waveform selection, and shape modulation**. This makes scene-based song structure easy:

- **Store different attenuation and wave settings per channel** as “states” for verse/chorus/bridge sections.
    - E.g., Verse: Channel B is slow triangle modulating filter. Chorus: Channel B switches to random stepped, modulating distortion or offering rhythmic variation.
- **CV Inputs for Shape**: Switch waveform shapes for each section, or have external envelopes/sequencers control which shape is heard, changing modulation flavor as the song progresses.
- **External Automation**: Use a sequencer or MIDI-to-CV module to automate Batumi’s mode/wave settings and Poti’s attenuators for recallable "scenes".

---

## 5. **Self-Generating/Generative Arrangements**

Combine **Batumi II**'s outputs with **sequencers**, **quantizers**, **S&H circuits**, **switches**:
- Use phase offset LFOs to clock *several* sequencers at different (yet musically-related) rates.
- Use **rectified outputs** as evolving gates for random drum fills, melodic retriggers, or effect sends/returns.
- CV control of waveform shape (with Poti II + Batumi II) slowly transforms modulation type—simple triangle growing more complex, morphing the flavor of your sequence over the length of the piece without manual intervention.

---

## 6. **Patching Examples**

- **Building Blocks:**
    - Ch. A (Batumi, sine, slow): Modulate master lowpass filter for global tone sweeps.
    - Ch. B (Batumi, step random, medium): CV into VCA for tremolo on melody.
    - Ch. C (Batumi, downward saw, divided): Clocking random S&H for evolving hats or percussion.
    - Ch. D (Batumi, rectangle, multiplied): Triggers for snare rolls or fill generator module.
- **Using Reset Inputs:**
    - Patch a performance controller or footswitch (or DAW clock) to reset all Batumi channels at “drop” points for coordinated scene changes in your arrangement.

---

## 7. **Expert Moves**

- **Audio-Rate "Utility" Oscillators**: Batumi has V/Oct tracking and audio-rate range—use as *FM operator*, audio-rate modulator, or even a sub-oscillator. Automate which channel is audio-rate during different song sections!
- **Interactive Live Performance:** Change Batumi’s mode mid-set (free → phase → divide → mult) to introduce dramatic changes in how all downstream modulations function.

---

## 8. **Tips for Integrating with Other Modules**

- **Sequencers (ALM Pamela’s Pro Workout, Intellijel Metropolix, etc.):** Sync Batumi’s resets to sequencer start/stop for bar-accurate modulation.
- **Logic/Random (Mutable Marbles, Doepfer A-160-2):** Combine Batumi gates and LFOs with logic to drive pseudo-random but bounded musical events.
- **Switches or Sequential Addressing (Doepfer A-151, Mutable Branches):** Have Batumi outputs crossfade or switch modulations between multiple destinations—a powerful tool for live arrangements.

---

## Conclusion

**Batumi II** (with **Poti II**) is an extraordinarily **powerful macro- and micro-arrangement tool**. By leveraging its multi-channel, syncable, phase-shifting LFO design, you can not only modulate simple parameters but construct full musical narratives—introducing true *song structure* and *evolution* to your modular performances.

---

#### [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)