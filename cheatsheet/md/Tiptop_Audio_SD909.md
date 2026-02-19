# Tiptop Audio — SD909

- [Manual PDF](../../manuals/Tiptop_Audio_SD909_ns.pdf)

---

[SD909 Manual (PDF)](https://tiptopaudio.com/909-2)

---

# TIPTOP AUDIO SD909 – Cheat Sheet

The SD909 is a Eurorack recreation of the classic Roland TR-909 snare drum. This module brings all the original snare controls, adds voltage control to key parameters, and provides a separate noise output.

---

## Front Panel Controls

**Knobs:**
- **TONE:** Sets the length of the noise (Decay).
- **TUNE:** Adjusts the pitch of the internal VCOs (snare body).
- **SNAPPY:** Adjusts the amplitude/gain of the noise. (Note: Can go beyond original 909 settings.)
- **NOISE:** Sets the gain/balance of the noise component in the snare mix.
- **909 (NOISE) DOT:** Marked region for classic TR-909 sound balance.
- **ACC (ACCENT):** Sets amount of accent (volume emphasis) both manually and under CV control.
- **909 (ACCENT) DOT:** Marked region for classic TR-909 accent setting.
- **LEVEL:** Controls final output volume.

**Buttons:**
- **TRIGGER:** Manual trigger to test/play the snare sound.

---

## Inputs & Outputs – Reference

| Jack Label     | Type       | Description                                                      | Voltage Range                |
|:-------------- |:---------- |:---------------------------------------------------------------- |:---------------------------- |
| **SD OUT**     | Output     | Main snare drum audio output                                     | Audio signal (modular level) |
| **NOISE OUT**  | Output     | Raw, unfiltered TR-909-style white noise output                  | Audio signal (modular level) |
| **GATE IN**    | Input      | Main trigger for snare sound (accepts gate/trig)                 | Typical trigger: 5V–12V      |
| **ACCENT IN**  | Input      | CV or gate/trigger for accent amount (overrides internal accent) | 0–5V CV or gate/trigger      |
| **VC-NOISE**   | Input      | CV to control noise generator clock frequency                    | 0–5V CV (approx.)            |
| **VC-TUNE**    | Input      | CV to control snare Tune (VCO pitch)                             | 0–5V CV (approx.)            |

---

## Usage Tips

### Creating a Classic 909 Snare
1. **Connect `SD OUT`** to your mixer/output.
2. **Set all knobs** to positions indicated by the “dot” regions labeled "909" for authentic TR-909 sound.
3. **Trigger** with either the TRIGGER button or an external gate to GATE IN.  
   - No ACCENT IN: Accent knob acts as gain/level “fine” control (recommended for classic workflow).
   - Use ACCENT IN: Patch CV or triggers for dynamic snare accents between steps.

### Sound Shaping
- **TONE**: Increasing = longer noise burst (decay).
- **SNAPPY**: Higher values = more pronounced/“snappier” white noise.
- **TUNE**: Higher = higher snare pitch.
- **NOISE**: Blends noise with snare “body”; classic amount at “909” dot.
- **LEVEL**: Controls output volume.

### Extended Features
- **NOISE OUT:** Use as a white noise source for other patches—excellent for hats, SFX, filtered percussion.
- **VC Inputs:** Modulate `VC-TUNE` and `VC-NOISE` for dynamic pitch/metallic FX and noise timbre changes—try sequencers or envelopes for evolving snare textures.

### Dynamics & Accent
- **ACCENT:** Provides per-hit loudness variation (classic groove feel).
  - **Unpatched:** Accent knob affects every hit, also sets max output gain.
  - **Patched:** ACCENT IN allows accent variation per note (CV or gate).

---

## Voltage Ranges (Summary)

- **Gate/Trigger Inputs:** 5V–12V (safe range, standard for Eurorack)
- **CV Inputs (Tune, Noise, Accent):** 0–5V typical (always check with manual or test for range/response)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)