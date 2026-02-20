# Bubblesound — HexVCA

- [Manual PDF](../../manuals/bubblesound.pdf)

---

[**PDF Manual: Bubblesound HEXvca**](https://www.bubblesound-instruments.com)

---

# Using the HEXvca for Composing Full Length Eurorack Songs

The **Bubblesound HEXvca** is a versatile, six-channel voltage-controlled amplifier (VCA) module for eurorack systems, designed to be the backbone for dynamic signal control, mixing, and modulation. While VCAs are crucial for shaping amplitude envelopes and dynamics in patches, the HEXvca stands out due to its mix outputs, linear/exponential modes, and normalization features. Below, I’ll discuss how to creatively use this module to move beyond loops and build evolving full-length songs in eurorack systems.

---

## 1. **Macro-level Mixing and Muting**

- **Voltage-Controlled Gain**: Use CV sources (envelopes, LFOs, sequencers) to modulate amplitude on each channel, bringing parts in or out, or fading between them for song dynamics.
- **Submixing**: Dedicated mix outputs for channels 1-3, 4-6, and all 6 mean you can treat this module as a VCA mixer, grouping and routing voices or submixes to different destinations (e.g., FX sends, external mixers, or recording interfaces).
- **Manual Playability**: Use the CV normalization (by patching the same gate or envelope to multiple VCAs) for hands-on control, e.g., triggering several voices together for chorus/drop sections.

## 2. **Song Structure Automation**

- **Scene Arrangement**: Use separate CV sources (sequencers, function generators like Maths, automation lanes from MIDI-to-CV interfaces) to automate which voices are active in different song sections – intros, verses, choruses, bridges, etc.
- **CV Normalization for Group Transitions**: Set jumpers to normalize CV inputs — this allows you to change multiple parts at once (for instance, muting drums while introducing lead + bass).
- **Envelope Shaping for Drama**: Exponential/linear switching lets you fine-tune the punch/smoothness of transitions.

## 3. **Dynamic Modulation and Evolving Textures**

- **Crossfade and Layer**: Assign different modulation sources to each VCA (random LFOs, stepped CV from sequencers, synced envelopes) for evolving textures and dynamic crossfades.
- **CV Mix Output Processing**: Output a grouped mix to modulators, compressors, or spatial processors, then modulate that return with another HEXvca channel for evolving space/dynamics.
- **Audio & CV Paths**: The DC-coupled design means VCAs can be used to process CV as well as audio, so you can automate modulation depth, not just amplitude. For example — fade in vibrato intensity, or crossfade between sequencer patterns.

## 4. **Automation of Effects Sends and Returns**

- Use HEXvca channels to control the amount of signal sent to outboard effects (verb, delay, distortion), changing them over time via scenes or modulations.
- Switch effects routing per section, e.g., dry for verse, wet for chorus or breakdown.

## 5. **Integration with Sequencers and Switches**

- Many sequencers or function generators (Intellijel Tetrapad, Make Noise Pressure Points, etc.) can output modulation envelopes/gates; feed them to HEXvca for complex scene switching.
- Chaining with the Bubblesound HEXar enables cable-free triggering, tidying up performance setups and enabling tight, clean arrangement shifts.

## 6. **Recording Stems, Layered Arrangements, and Live Performance**

- Record separate submixes from the HEXvca outputs for post-production flexibility, or to overdub new song sections.
- In live sets, assign each VCA to a different section/track/sample/loop for on-the-fly improvisation and arrangement.

---

## Example Song Structure Implementation

1. **Intro**: Slowly fade in ambient noise with exponential response; bring in hi-hats with a linear envelope.
2. **Verse**: Gates from a sequencer open VCA channels for kick, snare, and bass; use grouped mixed output for quick mute/unmute of entire drum section.
3. **Build/Bridge**: Use a single CV source normalized to several VCAs to gradually introduce layered melodies + effects.
4. **Chorus/Drop**: Open all VCAs for full intensity; modulate auxiliary FX sends.
5. **Outro**: Use slow LFOs/envelopes to fade out sections by reducing VCA levels, perhaps crossfade to an evolving drone.

---

## **Tips for Full Song Arrangements in Eurorack with HEXvca**

- **Pre-patch voice and effects groups into the 6 VCAs**
- Set CV normalization jumpers for unified control
- Use external/sequenced CV for scene changes
- Route mix outputs to multitrack recorders or DAW for arranging post-performance
- Leverage DC coupling for morphing both audio and CV elements across the song

By carefully planning what goes through each VCA, and by leveraging the HEXvca’s mixing and normalization capabilities, you can introduce structured dynamics and compositional flow typical of full songs, rather than static loops.

---

[**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)