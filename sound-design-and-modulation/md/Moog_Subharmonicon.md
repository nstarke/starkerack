# Moog — Subharmonicon

- [Manual PDF](../../manuals/Subharmonicon_Manual.pdf)

---

[Moog Subharmonicon User Manual (PDF)](https://www.moogmusic.com/sites/default/files/2020-05/Subharmonicon_Manual_v1.pdf)

---

# Moog Subharmonicon: Eurorack Modulation Techniques  
*For Distorted Percussion, Dubstep/Drum & Bass Basses, and Atmospheric Pads*

This guide leverages the Subharmonicon’s semi-modular patchbay, sequencers, and unique architecture to achieve a range of experimental and contemporary sounds. Each section refers to specific functionality in the Moog Subharmonicon User Manual ([PDF link above](https://www.moogmusic.com/sites/default/files/2020-05/Subharmonicon_Manual_v1.pdf)), as well as general eurorack modulation concepts.

---

## Distorted Percussive Sounds

### Patchbay Techniques
- **Mixer Overdrive**: Push the sound sources (VCOs and SUBs) to near-maximum on the mixer. (Manual p.21-22, "MIXER") This will create warm analog distortion as the filter overdrives.
- **VCF Self-Oscillation**: Turn up the filter "Resonance" until it self-oscillates. Modulate the "CUTOFF" with fast stepped voltages from one of the sequencers or an external envelope to create kick or tom-like percussive sounds. (Manual p.23, "THE FILTER")
- **Envelope Triggers**: Use the patchbay "TRIGGER" or "RESET" input to inject external gates or rhythmic triggers, allowing precise control over percussive envelopes. (Manual p.35, "TRIGGER INPUT")

### Modulation Ideas
- **Clocked Filter Modulation**: Patch a sequencer clock or rhythmic generator output into the "CUTOFF INPUT" to create sharp, rhythmic filter envelopes.
- **Clock Out to VCA In**: As suggested (Manual p.49), patching the CLOCK OUT to VCA IN produces a choppy, gated effect, ideal for glitch percussion or artificial hi-hats.
- **Fast Decay**: Set both VCF and VCA envelopes to sharp attack and very quick decay for punchy, snappy sounds (Manual p.24-25, "THE ENVELOPE GENERATORS").

---

## Aggressive Dubstep/Drum & Bass Basses

### Subharmonics & Polyrhythms
- **Deep Subharmonics**: Use SUB 1/2 FREQ dials (on both VCOs) to divide the fundamental for massive, perfectly tuned undertones (Manual p.18-20, "THE OSCILLATORS").
- **Sequencer Modulation**: Assign sequencer rows to modulate both main VCO and SUBs independently, generating morphing wobbles or growls every step (Manual p.26-27, "THE SEQUENCERS").

### Modulation Tricks
- **External Modulation**: Use the “VCO 1/2 SUB INPUT” jacks to sweep the undertone divisions dynamically with LFOs, random CV, or envelopes, for basslines that morph or “talk.”
- **PWM Smash**: Select square waves and patch audio-rate sources, or envelopes/LFOs into "VCO PWM" jacks—produces brutal timbral variation, ideal for dubstep basses (Manual p.32-33).
- **Filter Dub-wobble**: Patch rhythmic outputs (RHYTHM 1-4) or sequencer clocks, possibly from another eurorack source, into "CUTOFF INPUT" and sweep cutoff for classic dubstep filter movement. High resonance coupled with deep subharmonics sounds huge.

#### Advanced Combinations
- **Cross-Modulation**: Send SEQ 1 OUT to VCO 2 FREQ IN and SEQ 2 OUT to VCO 1 FREQ IN for evolving FM-like movement.
- **Distorted Bass**: Max out the mixer, self-oscillate the filter, slap with envelope modulation—distorted, screaming, or broken-bass tones.

---

## Haunting Atmospheric Pad Sounds

### Slow, Evolving Modulation
- **Drifting Subharmonics**: Use slow, external LFOs/voltage sources patched to VCO 1/2 SUB INPUT or VCO FREQ INPUTS for freq drift and evolving chord clusters.
- **Gentle Quantization**: Try JI (just intonation) modes for consonant pads (Manual p.21), then slowly crossfade to ET or adjust underlying pitches to introduce subtle, complex beating/phase movement.

### Layering and Spatialization
- **VCO Mixer Fades**: Slowly animate the VCO/SUB levels with external VCAs and LFOs (patch VCA EG OUT to VCA IN, mod usefully elsewhere to create swells and fades).
- **Filter Resonance Drone**: Set filter to the edge of self-oscillation and modulate cutoff very slowly for whistling, airy resonance overtones. Apply small positive and negative amounts on "VCF EG AMT" for movement (Manual p.24).

### Rhythmic Ambience
- **Polyrhythmic Sequencing**: Tie multiple rhythm generators at slow clock divisions to sequencer steps, creating unpredictable, non-repeating cycles suitable for evolving ambient patterns.
- **Patchbay Trick**: Send mild random or sample & hold voltages to cutoff, VCO frequencies or subharmonics, for subtle, ghostly pitch/filter shifts.

---

## Further Expansion

- Integrate with other eurorack modules for more envelopes, LFOs, effects, or CV processing via the extensive patchbay (Manual p.31-37).
- Use MIDI or external sequencers for precise or generative modulation control (Manual p.41-44).

---

Explore the **patch sheet overlays** and blank sheets at the end of the manual (Manual p.45-55) to write down and recall your favorite discoveries.

---

**Reference: [Moog Subharmonicon User Manual (PDF)](https://www.moogmusic.com/sites/default/files/2020-05/Subharmonicon_Manual_v1.pdf)**  
**Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)**