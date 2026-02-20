# Acid Rain — Constellation

- [Manual PDF](../../manuals/Constellation_Manual_Firmware_1.1_4.7.2025.pdf)

---

[Download the Constellation Firmware V1.1 Manual (PDF)](attachment:<file-path>)

---

# Modulating Constellation for Unique Eurorack Sounds

As a Eurorack musician, Constellation offers deep rhythmic and modulation possibilities thanks to its 8 channels, advanced Euclidean pattern engines, CV assignment system, and flexible clocking and logic combinations. Here’s how to exploit these features for experimental sound design, percussive attacks, brutal basslines, and haunting textures.

---

## 1. **Distorted Percussive Sounds**

### **Key Techniques**
- **Euclidean Ratchets & Bursts:** Set patterns with short lengths (e.g., 4–7 steps) and high ratchet/burst parameters. This creates dense flurries of triggers–perfect for glitchy, metallic percussive hits.
- **Randomization & Chance:** Use the **chance** parameter for patterns or assign a slow/random LFO to it via CV. This introduces unpredictability, mimicking analog noise and random percussive artifacts.
- **Clock Division/Multiplication:** Use clock dividers/multipliers on selected channels for uneven, polyrhythmic pulses.
- **OR/XOR Logic:** Combine patterns with XOR or OR to layer rapid hits, causing overlaps, gaps, and unexpected off-beats.
- **Variable Pulse Width:** Crank the channel’s **width** to create “choked” gates or blend pulses into harsh, distorted gates.

### **Sample Patch Idea**
- Channel 1: Short Euclidean pattern, ratchet 6, burst 4, low chance (30–40%), routed to a drum distortion module.
- CV input 1: Assign a stepped random voltage to modulate **events** or **rotate** for aggressive motion.
- Use XOR or OR to combine patterns, maximizing unexpected overlapping triggers.

---

## 2. **Wild Basslines (Dubstep/Drum & Bass)**

### **Key Techniques**
- **Long Patterns, High Events:** Use longer patterns (length 16–32) with moderate events (7–10) for hypnotic movement.
- **Ratchet and Burst for Wobble:** Assign ratchet (2–4) and burst (2–3) for wobbly, shifting gates sent to bass synth envelopes or filters.
- **CV Modulation:** Map an external LFO to **rotate** or **events** for constantly morphing subdivision/groove.
- **Channel Polyrhythms:** Set one or more channels to triplet or quintuplet divisions against the main clock for wonky, rolling grooves.
- **Flip-Flop (Flop) Mode:** Use on bass channels for held gates, letting the event rhythm determine note on/off—useful for classic DnB “stabs.”

### **Sample Patch Idea**
- Channel 3: Length 12, events 5, burst 2, ratchet 3, flip-flop ON, routed to bass VCA envelope or filter for movement.
- CV input 2: Sine LFO (0-5V) modulates **rotate** for sweeping, shifting downbeats.
- Clock division: Channel 3 runs at 3/2 of main clock for groove offset.
- Channel 4: Shorter length, high chance, triggers a synced distorted sub hit.

---

## 3. **Haunting Atmospheric Pads**

### **Key Techniques**
- **Very Long Patterns:** Use maximum pattern length (e.g., 64, 128, 256+) with low events. This causes rare, unpredictable trigger clusters–ideal for slow ambient textures.
- **Slow CV Modulation:** Assign a slowly cycling LFO or manual joystick to **events**, **chance**, or **width** for evolving, organic changes.
- **Wide Pulse Widths:** Set channel width high (70–95%), blending gates for sustained, breathy effect triggers.
- **AND Logic:** Combine sparse patterns with AND logic to make events even less frequent and more spectral.
- **Flip-Flop Mode:** Gate pads or drones, letting Constellation’s logic structure define shifting, ghostly tails.
- **Pattern Rotation:** Mutate the rotation parameter over time for morphing pad entrances.

### **Sample Patch Idea**
- Channel 5: Length 128, events 6, wide pulse width, AND logic, triggers a wavetable/polyphonic pad.
- CV input 3: Patch a slow triangle or sample & hold to **width** and **events** for evolving pads.
- Channel 6: Flip-flop ON, very sparse, triggers granular or reverb-heavy sounds for added texture.

---

### **Additional General Tips**

- **Muting Patterns:** Use the mute menu (page 20) dynamically—either via knob, or with assigned gates for live “dropouts” and lightning-fast rhythm edits.
- **Live Slot Change/Random Modulation:** Assign a CV input to “load” to instantly change whole save slots (entire rhythmic scenes) with voltage or sequencer triggers—great for wild, automated shifts mid-performance!
- **Input Normalization:** Use the CV input cascade feature for global modulation, or disable for per-input control (see page 26).

---

**Manual-specific CV Assignment Examples:**
- Assign 0–5V CV for upward modulation (e.g., from LFO or envelope).
- Assign -5V to +5V for bipolar mod sources (e.g., random voltage, joystick).
- Most parameters can be randomized on gate, allowing for hands-off controlled chaos.

---

# References

- [Download the Constellation Firmware V1.1 Manual (PDF)](attachment:<file-path>)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---