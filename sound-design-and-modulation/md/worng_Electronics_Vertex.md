# worng Electronics — Vertex

- [Manual PDF](../../manuals/Vertex manual v1.00.pdf)

---

[WORNG Electronics Vertex Manual (PDF)](https://www.worngelectronics.com/manuals/Vertex_Manual.pdf)

---

# Creative Modulation Techniques for the WORNG Electronics Vertex

The Vertex is a powerful and flexible stereo VCA that goes far beyond basic stereo amplitude control. Leveraging its unique architecture—featuring both linear and exponential VCAs, wide-ranging gain CV response, and voltage-controllable stereo skew—you can shape, mangle, and animate audio and CV signals in truly unique ways.

Below, I’ll outline techniques focused on three areas:  
- **Distorted Percussive Sounds**  
- **Aggressive Basslines (Dubstep/DnB style)**  
- **Haunting Atmospheric Pads**

---

## 1. Distorted Percussive Sounds

#### **Overdriven Envelope Shaping**
Vertex’s special 3320 VCA choice means that pushing the gain CV *over* unity produces *envelope clipping*—not audio distortion, but a pseudo-hard-limiting effect on your envelopes. This tweaks the envelope shape from an AD to something more like an AHD, great for punchy percussive attacks.

**Patch Idea:**
- Send a fast, snappy envelope (from a Maths, Quadrax, or similar) into the **Gain CV Input**.
- Crank the **Gain CV Amount** up *past* the point that fully opens the VCAs. The envelope peaks will clip, shortening the attack and adding an instantaneous “hold” stage—a pseudo-transient.
- Patch a mono drum (kick/snare) hit into the **L Input**.  
- Modulate **Skew** (manually or with a random/stepped CV) so the left and right channels clip at different points—producing asymmetric transients. This can make percussive hits sound wider and more aggressive.

#### **Stereo Crush and Fatten**
- Use two different envelopes into **Gain CV** and **Skew CV**, or patch the same envelope inverted to Skew CV Amount.  
- The result is each channel having a *different* clipped envelope shape—almost like two drums layered, but interleaved across the stereo spectrum.

---

## 2. Crazy Basslines (Dubstep/Drum & Bass)

#### **Voltage-Controlled Panning + Overdriven CV for Bass Distortion**
- Send a gnarly bass oscillator into the **L Input** (keep R unpatched for mono-to-stereo).
- Max out the **Gain** knob to ensure the signal is always passing.
- Use a rhythmic, fast envelope (from a sequencer or synchronized LFO) into the **Gain CV Input**, set Gain CV Amount to just over full (to ensure some clipping).
- Now patch an LFO or step sequence (sync’d to your drum groove) into **Skew CV**. As the bass follows your envelope, it dynamically “jumps” or warps across the stereo field.
- For extreme “talking” bass, modulate **Skew CV Amount** with audio-rate modulation (FM), low and deep for wobble or high and noisy for artifact-filled aggression.

**Bonus:**
- Run a CV from your pitch sequencer (transposed down an octave) into the **Gain CV** input. Now the amount of “clipping” follows the bass pitch, enhancing low notes and creating pseudo-dynamic distortion.

#### **Bitcrushed Stereo Movement**
- Use a stepped random or sample-and-hold signal patched to Skew CV at audio rate.
- This makes the Left and Right envelopes randomly clip, resulting in a chaotic, aliased stereo motion—great for DnB reese lines.

---

## 3. Haunting Atmospheric Pads

#### **Slow Stereo Animation**
- Patch a lush pad (complex chord or drone) into **L Input**.
- Use very slow, offset LFOs (or smooth random CV) into **Skew CV**—this causes the signal to drift dreamily between left and right.
- Run another LFO into **Gain CV**, with the **Gain CV Amount** lower, so only subtle overall swells occur.
- Subtle envelope overdrive (set Gain CV Amount so envelope peaks are *just* clipped) adds an unpredictable "hold" to one channel at a time, swelling the stereo field in ghostly, unnatural ways.

#### **Granular, Drifting Swells**
- Patch a granular synth or reverb tail into **Vertex**.
- Use *offset* and slowly modulated voltages for both Gain and Skew.  
- Invert and cross-modulate slow random voltages (use a VC Polarizer/Attenuverter) into **Gain CV Amount** and **Skew CV Amount**.  
- The stereo image will breathe and morph, with unpredictable “ghost” swells due to the unique clipping of the CVs.

---

## Pro-Tip: CV Processing

Vertex is **DC-coupled**, so you can use these same techniques on control voltages (LFOs/envelopes/sequences) as well as audio, creating complex, stereo, cross-modulated envelopes or modulation signals for downstream modules—making your stereo modulation as lively as your audio.

---

Explore these techniques and you’ll discover the Vertex is far more than a VCA: it’s a hands-on sculptor of envelopes, gates, amplitude, and stereo movement.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)