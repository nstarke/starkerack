# Erica Synths — Compressor

- [Manual PDF](../../manuals/compressor_manual_2023.04.04.pdf)

---

[Erica Synths Stereo Compressor Manual PDF](https://www.ericasynths.lv/media/StereoComp_manual_1.02.pdf)

---

# Using the Erica Synths Stereo Compressor for Creative Modulation

As a eurorack modular musician looking to push sonic boundaries, the **Erica Synths Stereo Compressor** offers far more than traditional utility compression. Its creative potential opens up unique directions for sound design, especially in genres like industrial percussion, dubstep, drum & bass, and atmospheric electronics. Here are some modulation strategies and patching techniques focused on distorted percussion, wild basslines, and haunting pads.

---

## 1. Distorted Percussive Sounds

### Signal Routing
- **Feed heavily saturated drum sounds** (claps, kicks, snares) into the `IN L` and `IN R` audio inputs.
- If using mono drums, try sending variations or other drum elements to the other input for creative parallel compression.

### Key Modulation Tricks
- **Dynamic Sidechain:** Use the `SIDEIN L/R` with transients from hi-hats or rimshots. A short, punchy sidechain input will cause the compressor to duck and recover quickly, increasing punch and rhythmic interest.
- **Extreme Compression:** Set a low `THRESHOLD`, turn `COMP AMT` (Ratio) high, and apply makeup gain (`GAIN`). This will squash dynamics and add harmonics for a gritty, pumping effect.
    - For **distortion**, push input levels past 0dB—modular levels (+5V) will hit the analog VCA hard, driving the chip into nonlinearity.
- **Bypass as a Performance Tool:** Flick the `BYPASS` switch rhythmically for instantly switching between raw and smashed versions of your drums.

### Bonus: Stereo Tricks
- Turn off `STEREO LINK` and send different signals left/right. Let one side compress hard, and the other stay more dynamic—this can create an unstable, swirling stereo image.

---

## 2. Crazy Dubstep/Drum & Bass Basslines

### Patching Tips
- Run your main bass (e.g., a modulated, wobbly oscillator stack) into one input. Sidechain with a kick or snare transient.
- For *growling* and *pumping* movement, connect a sequencer or stepped random LFO to the Sidechain, or even process the Sidechain signal externally with distortion/EQ before returning it to `SIDEIN L/R`.

### Modulation Strategies
- **Sculpt the Bass Envelope:** Set a medium `THRESHOLD` and a high `COMP AMT`. The sidechain will make the bass "duck" around drum hits, classic for liquid DnB or wobble bass.
- **Drive Into Compression:** Use the `GAIN` control, but also modulate the input level (prior VCA, envelope follower, burst generator) for a gated or sputtering bass effect.
- **Automate Compression Amount:** With a sequential switch or voltage-controlled attenuator upstream, swap between low and extreme compression for evolving, unpredictable bass movement.

---

## 3. Haunting Atmospheric Pads

### Signal Approach
- Process stereo pad sources or big reverbs through both `IN L/R`.
- For evolving textures, slowly modulate source amplitude or filter content with slow LFOs.

### Creative Sidechaining
- Use unrelated material as Sidechain—white noise, a granular sample, or even environmental field recordings.
- When the Sidechain input undulates, compressor movement will impart subtle timbral shifts or "breathing" effects over long, sustained chords.

### Gentle Settings
- Set `THRESHOLD` and `COMP AMT` lower, aiming for transparent, soft ducking rather than hard limiting.
- Use `STEREO LINK` ON for even compression, or OFF for distributed, ghostly stereo modulation.

---

## General Modulation Ideas

- **Feedback Patch:** Mult the output back into the `SIDEIN` input for experimental auto-wah or feedback-driven gating textures.
- **Envelope Followers:** Use the `SIDEOUT` jacks as buffered taps of your original signal to drive CV inputs elsewhere in your rack, reinforcing rhythmic or amplitude-based modulation.
- **VU Meter as Visual Performance:** Use the 8-segment VU meter to time manual adjustments for live performance, or to tune the amount of compression dynamically for dramatic builds/drops.

---

> **ALWAYS** start with low levels when experimenting with feedback and high compression; the module is DC-coupled and can create wild swings or saturate quickly.

## Additional Resources

- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---

Let your creativity lead—this module is built to bring modular compression *alive* in both subtle and extreme ways!