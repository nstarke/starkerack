# Omnitone — Beatsi

- [Manual PDF](../../manuals/Beatsi_Information_Package.pdf)

---

[Beatsi Module Manual (PDF)](attachment://Beatsi_Information_Package.pdf)  

---

# Creative Modulation with Beatsi: Advanced Sound Design for Eurorack

As a Eurorack synthesist, Beatsi offers extensive CV modulation and deep digital drum synthesis possibilities—ideal for everything from distorted beats to experimental atmospheres. Here’s how you can harness its features for unique sound design:

---

## 1. Distorted Percussive Sounds

**Key Parameters:**  
- Timbre (especially in the blue "lo-fi" kit)  
- Decay  
- Pitch  
- Level

**Modulation Techniques:**  
- **Assign External Distorted CV Sources:** Route external LFOs, envelopes, or random voltages into CV1 or CV2. Map these to the **Timbre** and **Pitch** of your drums (e.g., kick or snare) for metallic, glitchy artifacts.
- **Bit-Crushing and Downsampling:** The blue (lo-fi) kit is already processed with digital degradation. Modulate the **Timbre** across its range at audio or sub-audio rates for real-time morphing distortion.
- **Attenuvert for Aggression:** Use negative attenuverting (invert the CV) for squashed, aggressive parameter movements.  
- **Hard-Sync Percussion:** Trigger the drum voices with extremely tight or overlapping gate signals from a clock divider or even audio-rate oscillators, then modulate **Decay** and **Level** for glitchy, broken textures.

**Patch Example:**
1. Use a distortion or wavefolding module’s CV out patched to Beatsi’s CV1.
2. Assign CV1 to the snare’s timbre and pitch.
3. Heavily invert (attenuvert) CV1 for extreme effects.
4. Modulate at audio rates for digital aliasing and wild artifacts.

---

## 2. Crazy Basslines (Dubstep/Drum & Bass)

**Key Parameters:**  
- Tom’s **Pitch** (V/Oct input or CV assign), **Timbre**, and **Decay**
- Kick’s **Pitch** and **Decay**

**Modulation Techniques:**  
- **Sequence the Tom Pitch:** Use an external sequencer or random stepped voltage into TOM CV (V/Oct input).  
- **Fast Envelope Mod on Decay & Timbre:** Route fast LFOs or complex envelopes to modulate both **Pitch** and **Timbre** at the same time for basslines that “wobble” in character.
- **Kit Morphing:** Automate scrolling the **Timbre** beyond its limits to switch between the orange, blue, and green kits mid-sequence. This yields wild changes in texture, especially with green (alien) kit.
- **Layer with FM:** Use the CV assignments to have a bass drum’s **Pitch** modulated by an audio-rate oscillator signal, creating FM bass tones reminiscent of Reso or early Noisia basses.

**Patch Example:**
1. Patch a sequencer to TOM CV input.  
2. Assign CV1 (envelope/LFO) to Tom’s Timbre and Decay.  
3. Use fast, heavy modulation on Decay; attenuvert for negative or positive sweeps.  
4. Manually scroll Timbre to switch kits in realtime, or use CV if your external controller can handle quantized voltages.

---

## 3. Haunting Atmospheric Pads

**Key Parameters:**  
- Crash/Hi-Hat **Decay**
- Cymbal-based voices’ **Timbre**  
- Any voice’s **Level** for fade-in textures

**Modulation Techniques:**  
- **Slow LFOs or S&H:** Modulate Decay and Timbre slowly to create evolving, drifting textures.  
- **Multiple Assignments:** Map both CV1 and CV2 to different voice parameters for a lush, animated sound.
- **Crossfade Kits for Texture:** Slowly sweep Timbre over its full range, crossing from one kit to another for seamless morphing—especially eerie when moving into the green (alien) kit.
- **External FX:** Pair Beatsi with reverb, delay, or granular modules, using CV outputs from those modules (if available) to cross-modulate Beatsi parameters for internal “pad” movement.

**Patch Example:**
1. Patch a slow triangle LFO to CV1 and assign it to the Crash and Hi-Hat Decay.
2. Use CV2 for Level modulation on the snare or tom; sweep the value for gentle fade-ins and fade-outs.
3. Use attenuverting to find sweet spots: less than full scale for subtlety, inverted for ghostly decay tails.
4. Rout the output through a long-tail reverb and wide stereo delay.

---

## Pro Tips

- **Multiple Parameter Assignments:** You can assign a single CV input to multiple parameters, which helps create complex, coupled modulations (e.g., sweeping Pitch and Timbre together).
- **Safe State:** Wait 5 seconds after editing for parameter save—great for keeping your explorations intact.
- **Reset Experimentally:** Power up while holding HIT, PARAMETER, and VALUE to start fresh for every session.

---

Experimentation is at the heart of modular—and with Beatsi’s digital DNA, creative modulation possibilities are almost limitless.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)