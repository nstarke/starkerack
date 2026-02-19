# 2hp — Swarm

- [Manual PDF](../../manuals/2hp_Swarm_v1-0.pdf)

---

[**2hp Swarm Manual PDF**](https://cdn.shopify.com/s/files/1/0256/9638/6176/files/swarm_instructions_4.0.pdf)

---

# Generating Hyper-Complex Percussion with 2hp Swarm

The **2hp Swarm** is a hyper oscillator module, ideal as a richly-dimensional sound source for percussive experimentation in eurorack modular setups. Here’s how you can leverage Swarm’s capabilities for complex, dense, and polyrhythmic percussion:

---

## 1. **Multioscillator Percussive Synthesis**

- **Dense Voicing for Claps/Snares/Hats:**  
  With Swarm, you can dial up multiple oscillators (up to 88 saws or 55 pulses) to form thick, noise-like, or metallic textures by maxing out the **VOICES** knob.
  - *Percussive Technique:* Use envelope generators (EG) with fast attack and decay to sculpt “clap,” “snare,” and “hat” sounds. Patch the Swarm through a VCA controlled by a snappy envelope.

---

## 2. **Detune for Metallic/Chaotic Percussion**

- **Unique Timbres via Detune:**  
  Manipulate the **DETUNE** knob for subtle or chaotic detuning per oscillator.
  - *Soft to Harsh Transients:* For metallic clangs, turn the Detune beyond 12-o'clock. For marimba or vibraphone-like attacks, keep detune subtle.
  - *Animate with CV:* Use a stepped or random clocked modulation source into the Detune CV input (-5V to +5V). Sequence or randomize the amount of detune in sync with your rhythms for unpredictable, stuttering cymbals or digital clap sounds.
  
---

## 3. **Rhythmic Complexity via Triggered Pitch Shifts**

- **Pitch as Percussion:**  
  Use polyrhythmic or euclidean sequencers to send voltage to the **1V/OCT** (Freq) input.  
  - With irregular, clock-divided, or probability/skipping patterns, the pitch of Swarm can be modulated in syncopated or complex cycles.
  - *Example Pattern:* Assign each subdivision (e.g., 5/8, 7/16) a pitch voltage. The oscillators shift in complex patterns, resulting in tuned “bongos” or “tom” voices cycling through odd rhythms.

---

## 4. **CV-Controlled Waveform Changes**

- **Saw/Pulse Morphing:**  
  Manually or via trigger/modulation, switch between pulse (clicky, more percussive) and saw (richer, denser) waveforms.  
  - *Performance Tip:* Patch a rhythmic gate or clock into a voltage-controlled switch or sequential switch to change Swarm’s waveform at different steps in your polyrhythms.

---

## 5. **Patch Processing for Rhythmic Emphasis**

- **Filter Animation (with MMF):**  
  Route Swarm’s output into the 2hp MMF filter, modulate cutoff/resonance with rhythmic LFOs/envelopes based on your polyrhythmic clocks.  
  - *Create filter “punch” by routing fast, per-step envelopes to the filter frequency for pseudo-acoustic drum articulation.*

- **Lo-Fi and Saturation:**  
  Send Swarm through the 2hp Lo-Fi to degrade, bitcrush, or add digital artifacts, accentuating attack transients.

- **Dual VCA Dynamics:**  
  Use a dual VCA for envelope shaping and amplitude modulation. Sidechain or crossfade two Swarm voices with opposing percussive envelopes for moving, ducking rhythms.

---

## 6. **Tips for Polyrhythmic/Complex Use**

- **Clocking and Modulation:**  
  - Use clock dividers/multipliers and polyrhythmic gates to trigger VCAs, envelopes, and CV sources for Swarm.  
  - Drive the Detune and Voices CV with patterns created by sequencer channels running at independent odd time divisions (e.g., 3-against-4, 5-against-7).

- **Rotation and Shuffling:**  
  - Experiment with sample-and-hold or sequential switches to shuffle between modulation sources or patterns sent to Swarm.

---

## 7. **Make It Punchy**

- **Accent Envelopes:**  
  Use accent envelopes—longer, higher peaks on certain steps—to punch specific oscillators or filtrations harder for groove accents.
- **Transient Shaping:**  
  Patch Swarm’s output into a transient shaper or wavefolder for sharp attack blips.

---

### [More on the 2hp Swarm Module](https://www.twohp.com/modules/swarm)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)