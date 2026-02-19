# Bored Brain — EQx5

- [Manual PDF](../../manuals/EQx5-UserGuide_1.0.pdf)

---

[**eqx5 User Manual PDF**](https://boredbrainmusic.com/wp-content/uploads/2022/12/Boredbrain_eqx5_Manual_EN.pdf)

---

## Creative Use of the **eqx5** for Dense, Hyper-Complex Percussion in Eurorack

The **Boredbrain eqx5** is a five-band CV-controllable equalizer, which is more of a powerful sound sculpting tool (effect/processor) than a sound source or voice. However, it can be used to shape, modulate, and emphasize percussion and other rhythmic material to generate dynamic, punchy, and unique timbres — perfect for complex polyrhythmic and multimeter electronic music.

### Key Features Relevant for Percussion and Rhythm

- **Five CV-controlled frequency bands:** Band Gain AND Band CV (±12dB per band with up to ±15dB with full CV).
- **Resonant filter curves:** Each band selectable between wide, narrow, or resonant — excellent for sculpting or emphasizing transients.
- **Voltage-controlled balance (wet/dry):** Morph between processed and dry signals on the fly.
- **High headroom & modular levels.**
- **Crossfader style CV control:** Animate between heavily processed and clean signals.

---

## Musical Strategies for Dense & Complex Rhythmic Music

### 1. **CV Animate the Bands with Rhythmic or Polyrhythmic Modulators**

- **Route clock-divided or polyrhythmic gate/trigger CV sources** into the EQ band's CV inputs.
- Modulate certain frequencies (e.g., low for kick, mids for snare, highs for hats) to dynamically punch, scoop, or emphasize hits **in time** with multiple rhythmic patterns.
- **Envelope followers** from percussion can duck or boost specific ranges per hit.

**Example Patch Idea:**
- Split a clock into two or three gate patterns (Euclidean, polyrhythmic divisions).
- Convert these to stepped random or shaped envelopes.
- Send them to eqx5 band CV inputs—e.g., Band 1 gets a 5/4 rhythm, Band 3 gets 7/8.
- The effect is complex spectral movement that's tightly synchronized with (or cross-cutting against) your percussion.

---

### 2. **Transform Percussion into New Textures with Band Resonance**

- Set certain bands to **resonant** mode.
- Patch snare or hi-hat sources through the eqx5.
- Use envelopes, LFOs, or stepped random to modulate the **resonant** bands for whipcrack, zappy, or “buzzy” timbres.
- You can **resonate only when a trigger hits** by using envelope generators.

---

### 3. **Wet/Dry Blending for Accent Patterns or Groove Switches**

- Sequence the CV controlled **BALANCE** input with a rhythmic pattern.
- Jump or sweep between dry and wet EQ'd versions in real time — can be used as **ghost notes**, fills, or dramatic accent pattern switches.
- Combine with a random gate source for unpredictable rhythmic excitement.

---

### 4. **CV Sequence Smears & Timbral Morphs**

- By sending stepped random or sequenced voltages to one or more band CVs, you can create percussive timbre morphs at every beat, creating dynamic and unfamiliar drum textures.
- Use slow LFOs or sample & hold to make evolving, granular feeling percussion beds.

---

### 5. **Sidechain/Envelope Modulated Ducking**

- Send a fast envelope (from a kick drum, for instance) to scoop mid or high frequencies every time the kick hits—sidechain-style timbral ducking for clarity and punch.

---

### 6. **Spectral Polyrhythms**

- Feed the CVs for different bands different time signatures, creating a mesh of rhythmic spectral movement. For example, Band 2 (mid scoop/boost) modulates in 3/16, Band 4 (presence) in 5/16—resulting in ever-shifting interactions and evolving grooves.

---

## Tips for Maximum Uniqueness, Punch, and Percussiveness

- Use the **narrow or resonant settings** for snappiness and punch.
- Combine with **distortion**, **wavefolding**, or other dynamics modules post-eqx5.
- Use **fast modulation** (audio-rate CV) for frequency shifting, warbling, or even pseudo-FM effects on percussion.
- Animate between contrasting EQ curves using the BALANCE CV input.

---

## Example Hyper-Complex Sequence Patch

1. **Drum Pattern Source:** Multiple gate/trigger streams from a polyrhythmic sequencer.
2. **Percussive Audio:** Drum machine or sampled breaks into eqx5 **IN**.
3. **Band CV Control:** Map each band’s CV to different rhythmic patterns or random stepped voltages.
4. **BALANCE CV:** Sweep or gate blend via another rhythmic CV pattern.
5. **OUT:** To VCA/mixer or straight to FX chain.

**Result:** Evolving, spectral-rich, rhythmically active percussion that mutates with every measure, never sounding static or predictable.

---

## Inspiration

- **Patch random/sample & hold to band CVs for every snare hit.**
- **Switch EQ curves abruptly (“pseudo slice”) for glitchy fills.**
- **Feed slow polyrhythmic LFOs for shifting spectral beds over complex drum programming.**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)