# Qu-Bit — Mojave

- [Manual PDF](../../manuals/mojave_getting_started.pdf)

---

[Qu-Bit Mojave Quickstart Manual PDF](https://qubitelectronix.com/static/media/Mojave_Quickstart_2024-01-11.e457147….pdf)

---

# Qu-Bit Mojave: Modulation Strategies for Distorted Percussion, Dubstep Bass, and Haunting Pads

The Mojave by Qu-Bit is a live granular processor designed for deep, creative audio mangling. Its CV-controllable architecture and innovative grain-centric parameters make it an excellent playground for experimental sound design. Here’s how you can exploit its features for **distorted percussion**, **crazy basslines**, and **atmospheric pads**.

---

## **General Modulation Concepts**
Mojave accepts -5V to +5V CV on nearly all major parameters, allowing you to automate and shape its behavior radically. Use sequenced CV, random sources, LFOs, envelopes, or external audio as modulation sources patched into these CV inputs for complex, evolving soundscapes.

---

## **1. Distorted Percussive Sounds**
**Approach:** Utilize Mojave’s granular nature to turn audio or noise bursts into gritty, glitched, percussive hits.

### **Key Modulation Points**
- **Distribute:** Patch in a stepped random (sample & hold) or clocked random CV for unpredictable “ratcheting”, glitchy trigger timing. Try fast triggers for metallic textures.
- **Size:** Modulate with a sharp envelope (from a snappy AD envelope) so grains start short and decayed, mimicking drum transients.
- **Zone:** Steer with random voltage or LFO for rapid buffer position jumps, adding stutter and digital artifacts.
- **Rate:** Clock to an external trigger/gate sequencer for precise rhythmic alignment. Modulate between glacial and audio rates via sequencer or stepped CV.
- **Gust:** Map velocity or audio-rate LFOs to Gust for dynamic shifting between distortion (feedback) and reverb, saturating the output for aggressive tones.
- **Structure:** Patch melodic CV from a sequencer for tuned percussion (arpeggios, metallic melodies).

---
#### **Example Patch**

1. Feed audio (or noise burst) to input.
2. Patch a gate/trigger sequencer to Gen for rhythmic grain generation (Chisel Mode).
3. CV control Distribute and Size with percussive envelopes and random sources.
4. Crank Gust towards feedback for distortion.
5. Apply occasional Freeze or Lock for abrupt “glitch” stutters.

---

## **2. Dubstep/Drum&Bass Basslines**
**Approach:** Craft morphing bass textures with fast-modulated filters, grain size, and pitch. Let granular playback and feedback-driven distortion grind the sound.

### **Key Modulation Points**
- **Speed:** Use a sequencer with 1V/Oct CV for pitch tracking melodic basslines.
- **Gust:** Modulate between dry/feedback for “growl” and filter-like movement.
- **Size:** Envelope-follow the bass line for evolving, “wobble” effects—short, punchy grains for transients, longer for sustain.
- **Zone:** S&H random for buffer “jumping,” creating glitchy fill FX.
- **Structure:** Add melodic CV—use for harmonically rich/fuzzy basses.
- **Whirl:** Use LFO for spatial movement; subtle for stereo width, fast for chorus/flange-like sounds.

---
#### **Example Patch**

1. Send a saw or square wave from an analog VCO into Mojave input.
2. Clock Mojave with a fast division (e.g., drum rhythm pattern).
3. Sequence Speed with basslines.
4. Trigger Gen for staccato and rhythm-synced movement.
5. Modulate Gust/Size with envelopes/LFO for growl and rhythmic pulse.
6. Dial in Distribute/Structure for extra complexity.

---

## **3. Haunting Atmospheric Pads**
**Approach:** Use long grains, lush reverb, and evolving modulation to create eerie, shifting textures.

### **Key Modulation Points**
- **Zone:** Slowly modulate with LFO, morphing sample position for bloomy, evolving movement.
- **Window:** Morph with slow, random LFO or envelope for shifting grain envelopes.
- **Freeze:** Engage for infinite drones. Use Zone/Drift modulation to “scrub” through the buffer without new audio.
- **Gust:** Glide right for maximum reverb, left for feedback and haze.
- **Speed:** Use slow rising/falling envelopes or LFO for subtle pitch movement (detune effects).
- **Drift:** Add slow random to get gentle movement within the buffer for dreamy instability.
- **Whirl:** LFO for stereo motion or modulate with random voltages for spooky phase-wandering.

---
#### **Example Patch**

1. Sample voice, acoustic, or wide synth pad into input or mic.
2. Engage Freeze after capturing a chord/note.
3. Slowly modulate Zone, Drift, and Window for evolving timbre.
4. Keep Gust to reverb-heavy, sweep Size for shifting pad width.
5. Subtly nudge Speed/Whirl for haunting pitch/spatial drift.

---

## **Bonus Tips**

- **Mic Input:** Experiment with live input—strike objects, whisper, or record environmental sounds for organic percussive or pad layers.
- **Sky Mode:** Use Dusk or Twilight for atonal, chromatic, and non-synchronous granular rhythms—great for dark, cinematic atmospheres.
- **Narwhal App:** Deeply customize internal scales/behavior for unique musical rules.

---

[Qu-Bit Mojave Quickstart Manual PDF](https://qubitelectronix.com/static/media/Mojave_Quickstart_2024-01-11.e457147….pdf)

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
