# Tiptop Audio — SD808

- [Manual PDF](../../manuals/Tiptop_Audio_SD808_ns.pdf)

---

[**SD808 Manual PDF**](https://www.tiptopaudio.com/808-2)

---

# Tiptop Audio SD808 Eurorack Module  
### (Roland TR-808 Snare Clone)

## Quick Start  
1. **Patch a gate trigger** into **GATE IN**.  
2. **Patch SD OUT** to your mixer/audio interface.  
3. Set **LEVEL** to halfway to begin.
4. Tweak **TONE, SNAPPY, ACCENT** for desired snare timbre and dynamics.

---

## Panel Reference

| **Control** | **Type**      | **Function**                                                                                                                                             | **Voltage Range**   |
|:------------|:--------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|:--------------------|
| LEVEL       | Knob          | Sets output gain (hot output enables overdrive/distortion).                                                                                             | -                   |
| TONE        | Knob          | Crossfades between 2 sine waves: CCW = low, CW = high, center = both mixed.                                                                             | -                   |
| SNAPPY      | Knob          | Controls white noise amount/envelope (crack/brightness of snare).                                                                                       | -                   |
| ACCENT      | Knob          | Manual accent amount for snare hit; increases volume, noise amount, and attack.                                                                         | -                   |
| ACCENT IN   | Gate jack     | Separate accent input. Gate/trigger here overrides default normalization (see below). Increases snare intensity when high.                                | 5V/12V gate         |
| GATE IN     | Gate jack     | Main trigger input. Fires snare sound. Auto-normalizes to ACCENT IN for single cable "maximum" snare punch.                                              | 5V/12V gate         |
| SD OUT      | Audio out     | Snare drum audio output. Very hot – up to **20Vp-p** (watch your input staging!).                                                                        | up to 20Vp-p        |
| Noise Trim  | Trimmer       | Sets internal white noise gain (side of module), for character tweaks.                                                                                   | -                   |

---

## Input/Output Summary

### Inputs
- **GATE IN:** Gate or trigger, 5V or 12V. Triggers the snare.
- **ACCENT IN:** Gate/trigger, 5V or 12V. Boosts attack and output level. If unused, GATE IN is normalized to ACCENT IN (max punch).

### Outputs
- **SD OUT:** Snare audio output, up to 20V peak-to-peak.

---

## Voltage Levels
- **Input Trigger/Gate:** 5V–12V (Eurorack standard)
- **Output Audio:** Up to **20Vp-p** – much hotter than typical Eurorack line levels (be careful patching to line-level gear).

---

## Knob & Trimmer Cheat Sheet

- **LEVEL:** Adjusts output loudness and drive (higher = hotter, more overdriven/distorted).
- **TONE:** CCW = Low sine; CW = High sine; between = both. Sets snare body color.
- **SNAPPY:** Amount/envelope of white noise. Low = dry/tonal snare; high = crispy/bright/snappy snare.
- **ACCENT:** Manual amount of hit "hardness."
- **Noise Trim (side panel):** Tweak internal noise generator (factory calibrated, but user-adjustable).

---

## Usage Tips

- For classic soft 808 sound: LEVEL 0–50%, ACCENT low/mid, SNAPPY low-mid.
- For aggressive overdriven snare: LEVEL max, ACCENT max, SNAPPY at noon.
- Trigger **ACCENT IN** separately with rhythmic triggers for dynamic snare variation.
- Internal circuit is an authentic TR-808 clone – adding modular effects (filters, VCA, waveshapers, etc.) massively expands sound.

---

## Quick Patch Ideas

- Patch multiple drum modules into a VCA or ring mod for amplitude modulation.
- Run the snare through filters or wavefolders for new textures.
- Use hot SD OUT signal to smash guitar pedals or tape preamps for analog distortion.

---

## Internal Normalization
- If **ACCENT IN** is NOT patched, GATE IN also triggers accent circuit for that signature "punch."
- Patch a gate to both for independent trigger/accent control.

---

[**SD808 Manual PDF**](https://www.tiptopaudio.com/808-2)  
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
