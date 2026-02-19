# 4ms — Rotating Clock Divider

- [Manual PDF](../../manuals/RCD-manual-1.2.pdf)

---

[**Read the Rotating Clock Divider (RCD) Manual PDF here** (original source)](https://4mscompany.com/p.php?p=186&c=5)

---

# Generating Hyper-Complex Percussion with the 4ms Rotating Clock Divider

As a eurorack musician seeking intricate, ever-evolving rhythmic structures, the **4ms Rotating Clock Divider (RCD)** is an outstanding tool. While not a voice or effect per se, the RCD excels at distributing, rotating, and mutating clock signals—the "DNA" of modular rhythmic activity. Here are strategies, workflows, and creative tips for turning your rack into a polyrhythmic playground using this module.

---

## 1. **Setting Up for Polyrhythms & Complex Patterns**

### **a) Non-Linear Division Spread**
- **Spread Mode ON + Max Divide-By:** Engage Spread mode and set Max Divide to 16, 32, or 64 (using jumpers or Breakout). Now, instead of classic multiples (2, 4, 8, …), your eight outputs are "spread" across the maximal range. For Max 32: `/4, /8, /12, /16, /20, /24, /28, /32`.
- **Result:** Outputs are offset by irregular intervals, enabling rare and "mathematically awkward" polyrhythms when clocking percussion voices or sequencers.
- **Patch Idea:** Fire drums or samples from these offset clocks. Patch clusters together for composite, interlocking patterns.

### **b) Rotate for Rhythmic Evolution**
- **CV Rotate:** Patch a slow LFO, a sequencer row, or a random voltage source to the Rotate input. This rotates the divide assignments dynamically across outputs, shifting triggers between channels.
- **Result:** The rhythmic relationships actively morph, creating motion—try with different types of modulation for "shifting meter" effects!

### **c) Use CV Reset for Controlled Chaos**
- **Spatial Polyrhythm:** Patch one of the RCD’s own outputs (e.g., the slowest (/32 or /64)) or another external division into the Reset input. This will periodically throw all counters back to "1", adding another layer of complexity and pattern restart.
- **Result:** Rhythms can phase, lock, or tumble apart based on reset rates—excellent for live "metric modulation".

---

## 2. **Complicated Time Signatures & Odd Divisions**
- **Divisions Beyond Neat Multiples:** With Spread mode OFF and Max Divide 32/64, you can get */17, /23, /31…* These quirky outputs are _gold_ for polyrhythms and non-4/4 grooves.
- Use these as triggers for non-standard percussion, odd-step sequencers, or for ratcheting effects in melodic lines.

---

## 3. **Up/Down Counting for Accent Patterns**
- **UP Mode:** Outputs act like classic clock dividers – triggers fall on expected beats, great for building up grooves.
- **DOWN Mode:** Everything fires on the downbeat, then waits—use this to create sudden "bursts" of percussion, perfectly synchronized accents, or *reverse* patterns.

---

## 4. **Gate vs Trigger Outputs**
- **Trigger Mode:** Used for snappy, short events (e.g., percussive clicks, short envelopes, drum hits).
- **Gate Mode:** Gates are "high" for a percentage of the clock. In odd divisions, you get asymmetric gating and can drive percussive VCAs for longer accented sounds, pulses, or pressure-like effects.

---

## 5. **Advanced Techniques**
- **Auto-Reset:** Set to 16, 32... for periodic metric "resets"—useful for calculated pattern interruptions or polyrhythmic cycles.
- **Self-Patching:** Patch outputs back into Rotate or Reset for feedback-based polymetric or generative unpredictability.
- **Multiple RCDs:** With two RCDs fed by common or related clocks, you can crosspatch, sync, reset, or CV rotate one with the other: think evolving drum duets or interlocking grooves.

---

## 6. **Sound Design Tips for Percussive Uniqueness**
- While RCD isn’t a voice, use its varied pulses to:
  - **Clock sample players** with overlapping one-shots and polymetric layers.
  - **Trigger synthesizer envelopes** with different decays for fake hand claps, clicks, glitches.
  - **Open short-lived VCAs** on noise bursts or tuned oscillators for synthetic, precisely-timed digital percussion.
  - **Modulate effect parameters** rhythmically—VCAs, delays, distortion, or wavefolders—applying different divisions to modulate cutoff, resonance, or wet/dry for wild grooves.

---

## 7. **Patch Example: Advanced Polyrhythmic Drum Machine**

1. **Master Clock** into RCD Clock Input.
2. **RCD outputs:** `/8`, `/12`, `/5`, `/7`, `/16` to different percussion voices—kick, snare, hats, tom, clap.
3. **LFO to Rotate:** Slowly modulate Rotate for morphing rhythm.
4. **/16 output to Reset:** Periodically restart the pattern for regular accents.
5. Feed some outputs to gates on filter or bitcrusher for changing timbre alongside the rhythm.

---

### **Tip:** Experiment with rotation modulation sources: LFOs, random, sample & hold, sequencer, or envelope to Rotate input = instant generative percussion.

---

**Manual PDF:** https://4mscompany.com/p.php?p=186&c=5  
**Generated With Eurorack Processor:** [https://github.com/nstarke/eurorack-processor](https://github.com/nstarke/eurorack-processor)