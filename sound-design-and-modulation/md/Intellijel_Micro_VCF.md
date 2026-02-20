# Intellijel — Micro VCF

- [Manual PDF](../../manuals/uvcf_manual_2021.08.15.pdf)

---

[Download µVCF Manual (PDF)](https://intellijel.com/downloads/manuals/uVCF/uVCF_Manual_2021.08.15.pdf)

---

# Using the Intellijel µVCF for Unique Sound Design

The Intellijel µVCF is a compact, high-quality state variable filter that lets you sculpt sound in creative ways. Below, I’ll walk you through advanced modulation techniques—as a fellow Eurorack artist—for achieving **distorted percussion**, **aggressive basslines for genres like dubstep/drum & bass**, and **haunting, evolving atmospheric pads**.

---

## General Modulation Approaches

### Key Controls & Patch Points
- **FREQ Knob**: Manually sets the cutoff. Also responds to voltage at FM1 (1V/oct) and FM2.
- **Q Knob**: Resonance. High values cause self-oscillation, which is key for distorted/percussive and “screamy” sounds.
- **FM1 (1V/oct, attenuated)**: Ideal for pitch or envelope modulation.
- **FM2 (bipolar, with dedicated attenuverter)**: Best for LFOs, complex CV, and sound animation.
- **LPF, HPF, BPF Outputs**: Simultaneous use offers parallel processing, layering, or unusual stereo effects.

---

## 1. Distorted Percussive Sounds

**Goal:** Sharp, aggressive, or metallic bursts, ideal for techno, industrial, or experimental beats.

**Suggested Patch:**
- **Input**: Patch a short envelope or drum sample (from a Disting, sample player, or clocked noise burst) to IN.
- **Q (Resonance)**: Turn Q up high (close to full for self-oscillation). This creates a snappy, ringing attack.
- **FM1**: Send a fast, snappy envelope to FM1 (e.g., Maths or Function), with the FM1 Attenuator close to maximum for precise cutoff tracking.
- **FM2**: Try modulating with an audio-rate square wave or a fast LFO for added grit. Setting FM2's attenuverter slightly negative or positive introduces unique pitch-dive or sweep artifacts.
- **Output**: Use BPF for “snare” like thwacks, or HPF for sharp “clap”/“rim” style transients.

**Pro Tip:** To add distortion without a dedicated distortion module, clip the filter output by running the module hot into a VCA, then overdrive the next stage, especially with high resonance settings.

---

## 2. Crazy Basslines (Dubstep/Drum & Bass)

**Goal:** Wobbly, tearing bass with pronounced filter movement, vocal/talking textures, and dynamic resonance.

**Suggested Patch:**
- **Input**: Saw, square, or digital wavetable oscillator (from a STO, Dixie, or digital source).
- **Q (Resonance)**: Set moderately high for vocal, squealing peaks. For more vowel-like movement, push Q higher.
- **FM1 (1V/oct)**: Patch your melody or sequencer line for cut-off pitch tracking, then tweak the FM1 Attenuator for tracking or pitch-bend FX.
- **FM2**: Use a slow, clocked LFO or envelope follower (from your bassline groove) to modulate. Set the FM2 knob for positive or negative polarity—try sweeping it as you play for formant morphs or classic “wobble.”
- **Output**: LPF for rounder subs; HPF for mid/high buzzing; BPF for vocal/talker “narrow” sound.
- **Bonus**: Dial the FM2 knob to invert LFOs for unique reverse movement. Stack FM1 (sequence) + FM2 (LFO) for complex rhythmic wobbles.

**Pro Tip:** Send the output *into another distortion or wavefolder* for even more growl. Parallel-process the HPF and LPF outputs for wide, gnarly stereo effects.

---

## 3. Haunting Atmospheric Pads

**Goal:** Shifting, ethereal drones with evolving overtones, subtle movement, and mysterious resonance blooms.

**Suggested Patch:**
- **Input**: Use a complex pad chord, or slowly modulate oscillator shape/timbre.
- **Q**: Set to mid or high—higher Q adds shimmering, singing resonance.
- **FM1**: Patch a very slow envelope or sample-and-hold for random drifts in cutoff. Slightly attenuate for subtle evolution.
- **FM2**: Use a slow LFO (e.g., sine/triangle, or a looping envelope) to FM2. Set the FM2 knob off-center for nuanced cutoff movement; sweep during performance for extra atmosphere.
- **Output**: Try BPF for ghostly, whispering sounds; LPF for warmth; HPF for icy, brittle highs.
- **Extra Depth**: Multi-track all three outputs, panning each differently and treating them with reverb/delay.

**Pro Tip:** No input? With high Q and no signal, µVCF self-oscillates—patch the output, introduce gentle FM1/FM2 modulation, and process the sine wave as an organic drone generator.

---

## Creative Tips

- **FM at Audio Rate**: For metallic, almost FM synthesis-like effects, patch an oscillator into FM2 and adjust the attenuverter. This creates inharmonic sidebands, great for abstract percussion and wild soundscapes.
- **Rhythmic Gating**: Put a sharp square LFO/envelope into FM1 or FM2, snapping the filter open/closed for rhythmic “chopping.”
- **Feedback**: Patch one output (e.g., HPF) back into the filter’s audio input with attenuation for wild, unstable feedback tones.

---

## Additional Resources

- [Intellijel µVCF Manual PDF](https://intellijel.com/downloads/manuals/uVCF/uVCF_Manual_2021.08.15.pdf)
- Experiment with patching based on your system, and always use your ears!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)