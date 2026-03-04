# Cute Lab — Mom Jeans

- [Manual PDF](../../manuals/mom-jeans-manual-rev1-1.pdf)

---

[**Download the Mom Jeans Manual PDF**](sandbox:/mnt/data/manuals/MomJeans_Manual_Rev1.1.pdf)

---

# Creative Sound Design with Mom Jeans Oscillator

Based on the manual you provided, here's a sound design analysis and recommendations for using the Mom Jeans oscillator to craft **distorted percussion**, **aggressive basslines**, and **atmospheric pads**. I'll include modulation tips, CV patching strategies, and parameter combinations tailored for each sound type.

---

## **General Modulation Concepts**

Mom Jeans offers **CV modulation** over nearly every key parameter: Shape, Density, Cadence, Torque, FM Index, Pitch (V/Oct and Linear FM), plus toggles for Coupling and Quantization. This gives you a wide palette for animation and morphing:

- **Shape** — Crossfades between seven waveforms (from soft to stepped saw).
- **Density** — Grain/pulsaret width, affects brightness, noisiness, and texture.
- **Cadence / Torque** — Set internal rate and depth of density modulation; can track pitch for harmonic effects.
- **FM** — Traditional and linear FM and hard sync for added harmonic complexity or aliasing.
- **Pulsar vs. Square Outputs** — Mix or use separately for cleaner or more complex timbres.

---

## **1. Distorted Percussive Sounds**

For punchy, gritty, or metallic percussion like snares, metallic blips, and "machine" hits:

### **Patch Example**
- **Trigger/Envelope → Linear FM or Density CV In:** Use a sharp envelope or trigger as a CV or audio signal.
- **Shape:** Mid to high (rectangle, saw, or stepped saw for more harmonics).
- **Density:** Set low or high (extremes for clickiness or metallic texture).
- **Cadence:** Moderate to fast; try high values for rapid modulation.
- **Torque:** High, to create extreme grain modulation (for noisier or unstable attacks).
- **Coupling:** OFF (for chaos) or ON (for tuned metallic effects).
- **Quantization:** OFF for randomness, ON for stepped, robotic percussion.
- **Sync:** Hard sync with another VCO/LFO for metallic or ringing effects.
- **Output:** Use the Pulsar out for grit, mix in Square out for a more structured attack.

### **Extra Tips**
- Automated or random modulation of **Density** and **Shape** via fast LFO, gate, or sample-and-hold can simulate analog drum machine randomness.
- Try audio-rate density modulation (another VCO patched to Density CV) for extreme aliasing and industrial overtones.

---

## **2. Dubstep / DnB Basslines**

For heavy, morphing, tearing bass that's alive with movement and harmonics:

### **Patch Example**
- **V/Oct:** Sequence with a pitch CV from your MIDI-to-CV/gate.
- **Shape:** Sweep across the center point for complex harmonic movement; automate with envelope or LFO for "wub" sounds.
- **Density:** Modulate with envelope or LFO synced to the bass pattern—extremes for gnarly, broken digital bass, middle values for harmonically rich "formant" bass.
- **Cadence:** Tie to pitch (Coupling ON) for consistent sub presence.
- **Torque:** High, to exaggerate modulation.
- **FM:** Use moderate linear FM from another oscillator (possibly envelope FM for "growls"), modulate FM Index to sweep between harmonics.
- **Quantization:** Try ON for stepped vowel/formant sounds; OFF for smoother morphs.
- **Output:** Rout Pulsar output through a VCA and filter for extreme sounds, Square out to layer solid sub.

### **Extra Tips**
- Automate **Density** and **Shape** simultaneously for formant basslines (classic dubstep technique).
- Routing sequencer gates to the **Sync** input can produce gnarly resets and tight rhythmic effects.

---

## **3. Haunting Atmospheric Pads**

For eerie, shimmery, textural beds (think sci-fi or horror ambiences):

### **Patch Example**
- **Pitch:** Low to mid, slow LFO slight modulation for sluggish drift.
- **Shape:** Slowly sweep with LFO or random CV for evolving tonality.
- **Density:** Keep low to mid (gentle formants and breathy texture). Animate with slow random mod or slow S/H.
- **Cadence:** Slow, or coupled to pitch for shimmer.
- **Torque:** Moderate, just enough to keep movement without becoming rhythmically obvious.
- **Coupling/Quantization:** OFF for unpredictable, ghostly movement; ON for subtle, familiar organ-like timbres.
- **FM:** Try very shallow, slow audio-rate FM for detune/phasing.
- **Output:** Use only Pulsar out, or combine with subtle Square for slower, rounder undertones.

### **Extra Tips**
- Send multiple, unsynced slow LFOs or random voltages to different CV ins for organic drift.
- Try self-patching the Pulsar output (attenuated) back to Torque or Density CV input for chaotic, feedback-like modulation.

---

## **Parameter Modulation Summary Table**

| Sound Type   | Key Params             | Modulation Suggestions               |
|--------------|------------------------|--------------------------------------|
| Percussion   | Density, Shape, Cadence, Torque, FM, Sync | Fast envelope/trig modulate Density & Shape, hard sync, high Torque |
| Basslines    | Shape, Density, FM, Cadence (Coupled), Quant | Automated formant sweeps, FM growls, Quant for stepped movement |
| Pads         | Shape, Density, Cadence, Torque (all slow) | Slow/random LFOs and S/H, light FM, uncoupled modes for drift |

---

## **Final Tips**

- **Extreme settings** are encouraged: push Density/Cadence/Torque to their limits and modulate deeply for digital artifacts.
- Abuse the **Coupling** and **Quantization** toggles to flip between organic flow and stepped robotic sound.
- **Pulsar Output** excels at bright, harmonically rich tones; **Square Output** for foundation/subs.

---

[**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)