# 2hp — Kick

- [Manual PDF](../../manuals/2hp_Kick.pdf)

---

[Kick Module Manual (PDF)](https://github.com/nstarke/eurorack-processor/blob/main/docs/kick-manual.pdf)

---

# Creative Modulation Techniques for the Kick Module

Based on the supplied information and images from the manual, here are specific ways to modulate this 2HP Kick drum module for a variety of unique and powerful sounds:

---

## 1. **Distorted Percussive Sounds**

- **Tone CV Modulation:**  
  - Send a fast, stepped random voltage or sequenced LFO to the **TONE** CV input (-5V to +5V).  
  - Modulating this control leftward overdrives the internal sine, producing crunchy, distorted kicks and variable saturation character.  
  - Apply sharp envelopes (e.g. from Maths or Function), with a fast attack and decay, to sweep the Tone at trigger hit, creating organic, ever-changing distortion with each hit.

- **Extreme Decay Settings:**  
  - Set the DECAY control fairly short, but use CV from a tempo-synced LFO or envelope to modulate it for occasional long, blasting decays.  
  - Using a negative offset will snap the decay even shorter, creating tight claps or “zap” perc.

- **Wavefolding & External FX:**  
  - Patch the output to external wavefolders, distortions, or feedback paths to further accentuate the Kick's overdriven character.

---

## 2. **Dubstep/Drum & Bass Basslines**

- **1V/Oct Sequencing:**  
  - Use a sequencer or arpeggiator to send 1V/Oct cv to the **V/OCT** input for melodic, playable basslines.
  - Pair with fast gating (TRIG) and adjust DECAY for staccato or “wobble”-style notes.

- **Pitch Envelope “Punch”:**  
  - Patch an envelope generator to the **V/OCT** input and dial in a very fast attack/decay envelope.  
  - This will provide an “80s bass drum drop” or contemporary pitch-bent attack to each note—perfect for “donk” kicks, DnB hits, and grimey jumps.

- **Rhythmic Modulation:**  
  - Clocked LFOs to TONE or DECAY, synced with your breakbeats, will morph the timbre and smear the attacks for more movement.
  - Use sample & hold to create unpredictable stuttering bass textures.

---

## 3. **Haunting Atmospheric Pads**

...yes, you can make pads with a kick module!
- **Long Decay and Gentle Modulation:**  
  - Set DECAY at its maximum (knob and +5V CV). This pushes the envelope to ~15 seconds.
  - Slowly modulate TONE using a long, slow LFO or random smooth voltage (e.g. from Wogglebug or Tides). Drift between clean and distorted regimes.
  - Sequence or glide the V/OCT input using a keyboard, CV processor, or slow LFO for ambiguous, shifting pitch—a detuned/unstable feel that aids in eerie drones and pads.

- **Layering & Reverb:**  
  - Run OUT through a lush reverb (Supercell, FX Aid, etc.) and blend multiple kick pitches for evolving, spectral washes.
  - Gate TRIG at irregular intervals for haunted, echoing hits.

---

## **Patch Example: "Crunchy Machine Drummer"**

| Jack        | Source                         |
|-------------|-------------------------------|
| TRIG        | Fast Euclidean trigger         |
| TONE (CV)   | Stepped random from S&H       |
| DECAY (CV)  | Envelope with modulated decay |
| V/OCT       | Bassline sequencer            |
| OUT         | Into distortion FX + mixer    |

---

**General Pro Tips:**
- Try using attenuators or CV processors to scale CV depth—especially into TONE and DECAY—for more nuanced modulation.
- Audio-rate modulation of TONE and V/OCT can produce FM-like clangs and unpredictable artifacts, great for experimental sound design.
- Remember: all CV ranges are -5V to +5V, so bipolar LFOs and random sources can take full advantage of the tone shaping!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)