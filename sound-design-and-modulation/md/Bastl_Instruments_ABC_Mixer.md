# Bastl Instruments — ABC Mixer

- [Manual PDF](../../manuals/manual-abc-web.pdf)

---

[**Bastl Instruments ABC Mixer Manual PDF**](https://bastl-instruments.com/content/manuals/abc_manual.pdf)

---

# Creative Modulation Techniques with the Bastl Instruments ABC Mixer

The Bastl ABC is more than just a 6–channel mixer. With clever patching and a few of its internal modification options, you can turn it into a gnarly processor for percussion, bass, and evolving pads. Below is an analysis focused on wild sound design, drawing on details from the manual and modular techniques.

---

## Key Module Features for Sound Design

- **6 Inputs (A-F)**: Each with its own level control.
- **2 Main Outputs**: A+B+C and D+E+F. If nothing is inserted in A+B+C, it is combined with D+E+F for a 6-channel mixer.
- **Normalisation Jumpers**: Internally connect A to D, B to E, and C to F for interesting stereo or parallel routines.
- **AC/DC Coupling Mods**: Solder jumpers enable mixing control voltage (CV) instead of just audio.
- **Handy for Audio and CV**: Compact and flexible in small systems.

---

## Approaches for Unique Sound Creation

### 1. Distorted Percussive Sounds

- **Overdriving Inputs**: Feed several percussion voices or sharp transients (e.g., kicks, snares, hats) into the channels and push their level knobs to maximum. Though the gain is unity (1x), stacking multiple sources can produce **internal clipping**, especially if your sources are hot.
- **Feedback Routing**: Patch the output (A+B+C or D+E+F) back into one or more free inputs at low levels. This can create brutal digital–style distortion and flanging, perfect for shattered percussion in industrial or IDM genres.
- **Post-Processing FX Loop**: Patch the mix output into analog distortion, a wavefolder, or a filter, then return the post-effect signal into another input. Mix raw and processed sounds for smack and bite.

#### Patch Example:
```
KICK → A
SNARE → B
HIHAT → C
A+B+C OUTPUT → DISTORTION → E
```
Twist the E channel knob to blend dry+wet for distorted slaps.

---

### 2. Crazy Basslines (Dubstep/Drum & Bass)

- **Cross-Modulation with CV (DC Coupling)**: Solder the jumpers on the back to enable DC coupling. You can then mix audio and LFOs/envelopes into the same output! For example, add an envelope or stepped random CV into a channel along with a bass VCO. Their sum will modulate the bassline in unexpected ways, introducing "wobble" and irregular modulations.
- **Stereo Split/Layered Bass**: With the normalization jumpers, patch the same bass source to A and use D as a parallel chain—apply different effects (e.g., distortion vs. clean) on each output, then pan A+B+C left and D+E+F right. This helps in creating wide, complex bass.
- **FM/AM Stack**: Mix envelope or rapid LFO signals into your bass channel for amplitude or frequency-modulation–like textures (when the destination supports it).

#### Patch Example:
```
BASS VCO → A
MULTISTAGE ENVELOPE → D (with DC mod active)
PAN: A+B+C Left, D+E+F Right
```
Sweep envelope to modulate bass in stereo for animated growls.

---

### 3. Haunting Atmospheric Pads

- **Layered Slow-Modulation**: Use the DC mod to mix multiple, slow LFOs with pad VCOs or samples. Summing multiple sources with subtle drifts can create evolving wash and timbral complexity.
- **Stereo Spread With Jumpers**: Use the normalization jumpers to send the same pad source to both A+B+C and D+E+F, but with different filter or effect sends per group. Pan for stereo motion.
- **Ambient Feedback Network**: Send an output to a delay or reverb and return its tail to another channel. Gentle feedback can yield unearthly textures.

#### Patch Example:
```
PAD VCO → A
SLOW LFO → B
NOISE/SPRINKLE SAMPLES → E
A+B+C → REVERB → F
```
Mix all for lush, morphing space.

---

## Pro Tips

- **Patch Unused Channels with Subtle Modulations**: Even sub-audio LFOs at <1Hz mixed with audio can induce "movement" and subtle tremolo or vibration.
- **Exploit Non-linear Summing**: Pushing lots of audio into the sum outs can create soft saturation—combine with feedback for dirty lo-fi sound.
- **Jumpers are Easy Mods**: If you have a soldering iron, try enabling the DC coupling and input normalizations for a much greater sound palette.

---

[**Bastl Instruments ABC Mixer Manual PDF**](https://bastl-instruments.com/content/manuals/abc_manual.pdf)

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
