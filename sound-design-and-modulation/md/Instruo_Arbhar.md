# Instruo — Arbhar

- [Manual PDF](../../manuals/Arbhar-Manual-Firmware-2.0-A5.pdf)

---

[Download the Instruō arbhar v2 User Manual PDF](https://www.instruomodular.com/wp-content/uploads/arbhar_manual_firmware2.pdf)

---

# Instruō arbhar v2 — Modulation Strategies for Unique Sounds

The Instruō **arbhar** is a deep, versatile granular audio processor for Eurorack. By exploiting its modulation options, you can create an incredible range of sounds including gritty percussion, wild dubstep/DnB basslines, and spooky pads. Below is a practical, performance-oriented guide based on your goals and the information in the manual.

---

## 1. **Distorted Percussive Sounds**

**Goal:** Chopped/rhythmic, noisy, and dynamically morphing hits.

### Key Parameters to Modulate
- **Strike Input:** Use fast triggers/gates for rapid grain generation/accents.
- **Grain Window:** Square or sawtooth shapes make sharp, clicky grains.
- **Intensity:** Modulate intensity to rapidly gate between dense and sparse (percussive burst effects).
- **Spray:** Increase for micro-looper FX; decreasing tightens up transients.
- **Dub Knob:** Fully CCW for destructive, noisy overdubs.
- **Pitch & Deviation:** Sweep or randomize for metallic, digital artifacts.

### Patch Ideas
- **Rhythmic Distortion:** 
  - Patch sequencer triggers to the Strike Input.
  - Set **Grain Window** to saw or square.
  - Modulate **Length** quickly (short grains = sharp, long grains = smeared).
  - Send envelopes/LFOs to **Spray** or **Grain Direction** CV for scanning through recorded material at each hit.
- **Destructive Overdub:** 
  - While looping percussion, set **Dub Knob** fully CCW and overdub new material—old audio gets harshly cut or glitched.
-

## 2. **Crazy Basslines (Dubstep/Drum & Bass)**

**Goal:** Growling, re-pitched, moving bass with unpredictable movement.

### Key Parameters to Modulate
- **Pitch, Pitch Deviation (CV):** Use sequencer or random stepped CV.
- **Intensity:** Density of overlapping grains—modulating for acid-style movement.
- **Scan:** Use LFOs/audio-rate signals for position-scanning within a bass sample.
- **Spray:** High values = granular jitter/glitch.
- **Dub/Layer Cycling:** Rapid overdubbing or switching layers yields evolving timbres.
- **Mod CV - Feedback/Delay:** Twisted resonant echoes/Karplus-Strong effects with high negative voltage, for metallic bass “wobble”.

### Patch Ideas
- **Moving Wub Bass:**
  - Record or load a simple bass note/oscillator hit.
  - Set **Pitch** to track 1V/Oct; modulate **Pitch Deviation** with a stepped random or sequencer for extra “talk” modulation.
  - Send LFO or envelope to **Spray** or **Scan** CV for movement.
  - Set **Mod CV** in feedback/delay mode (per preset file) and sweep negative voltages for Karplus-Strong–like effects.
- **Layer Switching Growl:**
  - Automate **Layer CV** with a stepped random or gate sequence, switching between different bass samples in rhythmic patterns.

---

## 3. **Haunting Atmospheric Pads**

**Goal:** Ethereal, evolving, wide, and subtly moving textures.

### Key Parameters to Modulate
- **Scan:** Slow LFOs to move through capture/sample.
- **Spray:** Moderate to high for motion without losing smoothness.
- **Grain Window:** Centered for Gaussian envelope (smooth drones).
- **Length:** Long grains for smeared ambience.
- **Grain Direction:** Modulate for reversed/swirling effects.
- **Reverb (Mod CV):** Fade up for infinite, ghostly tails.
- **Layer Blending:** Use omega mode to scan all layers at once.
- **Pitch Deviation:** Gentle, random modulation for detuned/unsettled pad sounds.

### Patch Ideas
- **Frozen Ghost Pad:**
  - Record a sustained sound (voice, instrument, chord).
  - Set grains long, **Intensity** at center for a thick chorus.
  - Slow LFO on **Scan** for evolving movement.
  - Use **Spray** for random micro-movements.
  - Patch Mod CV to **Reverb** (preset.txt set to Reverb) and automate with slow envelopes or manual sweeps for swelling tails.
- **Polyphonic Texture:**
  - Use **Omega Layer** (all layers mode), automate **Scan** and **Layer CV** together for dense, layered pads.

---

## **Further Tips**

- For more modulation destinations, use the CV Expansion module—nearly every major control (Scan, Spray, Layer, Grain Direction, etc) can be voltage-controlled.
- Use the **preset.txt** file to:
    - Set different operating modes (Mono/Stereo, feedback model, panning, etc)
    - Assign **Mod CV** to your preferred effect
    - Tailor randomization/quantization behaviors for even more chaos or stability where desired.

---

## Quick Reference to Useful Pages

- **Granular Engine Modulation:** p.18–23
- **Pitch/Pitch Deviation:** p.24–25
- **Mod CV assignments:** p.43–46
- **Layer/Scan tricks:** p.16–17, 39–41
- **Preset system (advanced customisation):** p.56–68

---

## **Links**

- [Download the Instruō arbhar v2 User Manual PDF](https://www.instruomodular.com/wp-content/uploads/arbhar_manual_firmware2.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---

Happy patching—arbhar is extremely deep, so experimenting with live modulation and parameter combos will unlock continuously fresh new sounds!