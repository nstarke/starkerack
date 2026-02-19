# Qu-Bit — Chord

- [Manual PDF](../../manuals/QB_Chord.pdf)

---

[Qu-Bit Chord v2 Manual PDF](https://manuals.qubitelectronix.com/chord-v2-manual.pdf)

---

# Using Qu-Bit Chord v2 For Hyper-Complex Percussive and Rhythmic Patching

The Qu-Bit Chord v2 is primarily a polyphonic oscillator/voice module designed for rich harmonic textures, but with creative patching, you can absolutely harness it for dense, punchy, and rhythmically complex percussion and polyrhythmic material.

Below are many strategies and patching tips for getting dense, rhythmic, polyrhythmic, and hyper-complex patterns out of Chord v2 in a Eurorack percussion context.

## 1. **Percussive Sound Design on Chord v2**

- **Envelope Control:** Route fast attack/decay envelopes to both the VCA(s) and FM inputs. Percussive hits require snappy envelopes for amplitude and timbral movement. Use external VCAs after each individual voice out (Root, Third, Fifth, Seventh) and modulate with rhythmically complex, possibly polyrhythmic, envelopes.
- **Waveform Selection:** Many internal banks include sharp/edgy digital waveforms (`Distorted`, `Video Game`, `FM`). These are ideal for synthetic drums and percussion.
- **User Wavetables:** Load percussive or non-harmonic waveforms into user banks for even more “drum-like” strike tones. (See manual: User Wavetable Creation; use e.g. [WaveEdit](https://waveeditonline.com/)).
- **Linear FM:** Use audio-rate FM from other oscillators for extremely metallic, clangorous, bell-like or noisy percussion hits.

## 2. **Polyrhythms & Patterns**

- **Independence of Voices:**
  - **Free Poly Mode:** Each oscillator has independent pitch control via separate CV ins (Root: V/Oct, Third: Fine, Fifth: Voicing, Seventh: Quality). Patch polyrhythmic gates/triggers and pitches to each independently. This lets you create four-part rhythmically independent sequences for layered or contrasting rhythms—a classic polyrhythm trick.
  - **Unison Poly Mode:** All four voices tune together but receive gate/pitch from separate CVs. This is great for creating "stacks" of related percussion hits, e.g., four voice drum machine.
- **Mix Output for “Drum Kit”:** Each individual output (Root, Third, Fifth, Seventh) can be used for a different drum voice, or you can mix them for dense composite percussive hits.
- **Utilizing Chord Inversions and Voicings for Variation:** Scan through chord types, voicings, and qualities *per step* in your rhythmic sequence to generate ever-shifting, non-repetitive drum timbres. Percussion sounds are deeply affected by microtonal and intervallic shifts.
- **CV Control for Parameter Morphing:** Send polyrhythmic LFOs, random, or complex sequenced modulation into Chord v2’s waveform, quality, voicing, and mode controls to move through very different percussion “instruments” or timbral textures mid-pattern.

## 3. **Rhythmic Complexity, Time Signatures, and Polymeters**

- **External Gate/Rhythm Sequencing:** Use polyrhythmic trigger sources like Euclidean sequencers, clock dividers, or probability-based triggers to control VCAs (for amplitude envelopes) or the chord’s CV ins.
- **Automating Bank or Waveform Changes:** Modulate the `bank` and `wave` parameters per rhythm step for dramatically changing timbre—a techique rarely used in drum synthesis but with huge payoffs for unpredictable, complex “drumline” flavors.
- **Chopping Chord Mix:** Gate or chop the summed mix output with ultra-fast envelopes or rhythmic VCAs controlled by polyrhythmic clocks/gates.
- **Layering with External FX:** Route one or more outs to external distortion/wavefolders for added punch, or into resonators/filters that are VCA-controlled by other polyrhythmic gates.

## 4. **Non-Standard Chord Types = Non-Standard Percussion**

- **Custom User Chords:** Program non-harmonic or microtonal intervals in the user chord slots via SD card (e.g., clusters, semitones fractions) for unpredictable, metallic, or bell-like hits. Percussion often works best with non-musical intervals!
- **Spread and Big Spread Voicings:** Use the “Spread” and “Big Spread Energy” voicing indexes for wide, non-overtone sets—ideal for digital “conga” or synthetic hand drum sounds.

## 5. **Advanced Techniques**

- **LFO Mode as Four-Phase Rhythm Generator:** Enable LFO_Mode in config.txt. Chord v2 becomes four related LFOs—use them to clock other percussion modules or modulate timbral parameters in polyrhythmic ways.
- **Velocity/Accent:** Use the amplitude of your triggers/envelopes to modulate the FM depth, quality, or waveform CV, giving you velocity-sensitive drum hits.
- **Glitch & Stutter:** Program rapid chord/voicing/waveform transitions (manual, sequencer, or random stepped CV) for “stuttery” glitch percussion.

---

## **Example Patch: Hyperactive Polyrhythmic Drum Machine**

**Modules Needed:**  
– Chord v2  
– 4 Envelope Generators  
– Polyrhythmic Gate/Trigger sequencer (Pamela’s New Workout, Intellijel Steppy, etc.)  
– 4 VCAs  
– Mixer

**Setup:**
1. Set Chord v2 to Free Poly Mode. Patch separate sequenced pitch and gate/envelope sources to each Root, Third, Fifth, Seventh input/VCA pair. Use very fast attack/decay settings.
2. Use a Euclidean, polyrhythm, or clock divider/multiplier to trigger each drum “part” at different rates/time signatures.
3. Modulate waveform, voicing, and quality with additional sequencers/LFOs for constantly shifting timbre.
4. Mix outs to a single bus for composite “hypercomplex” percussive output, or pan individual outs for a spatial drum ensemble.

---

## **Reference**
- [Qu-Bit Chord v2 Manual PDF](https://manuals.qubitelectronix.com/chord-v2-manual.pdf)
- [WaveEdit](https://waveeditonline.com/) for custom wavetables

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)