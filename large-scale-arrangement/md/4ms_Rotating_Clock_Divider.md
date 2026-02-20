# 4ms — Rotating Clock Divider

- [Manual PDF](../../manuals/RCD-manual-1.2.pdf)

---

[Rotating Clock Divider Manual PDF](https://4mscompany.com/p.php?p=RCD)

---

# Using the 4ms Rotating Clock Divider (RCD) to Create Full Length Eurorack Songs

One of the most challenging aspects of performing or composing in Eurorack is moving beyond loops—transforming great grooves into engaging, evolving full-length tracks. The 4ms RCD isn’t just a utility for making clock-divided rhythms; it’s a powerhouse for song structure, transitions, and arrangement when creatively combined with other modules. Here’s how you can leverage its features to build dynamic, composed modular pieces.

---

## 1. **Structuring Song Sections with Clock Division and Rotation**

### **A. Song Parts as Division States**
- Patch multiple voices (kick, snare, hats, bass, melody gates, sequencer clocks) to different RCD outputs, each set to a musically relevant divide.
- Use CV Rotate (from an LFO, envelope, footswitch, or sequencer) to shift the pattern across outputs. Each rotation can correspond to a new song section (verse, chorus, bridge).
- Plan your divisions so that each rotation triggers a distinctly different set of events, instantly "morphing" your groove.

### **B. Song Progression with Reset**
- Use CV Reset as a song section reset/transition (triggered by a manual gate, footswitch, sequencer, or end-of-pattern pulse from another module).
- Resetting returns the RCD to a known clock state, perfect for synchronizing fills, drops, or transitions between sections.

---

## 2. **Macro Arrangements and Pseudo-Automation**

### **A. Scene-Based Changes**
- Use sequential switches or voltage addressers (Doepfer A-151, WMD Sequential Switch, or similar) to send different CV to Rotate and Reset at certain bar-length intervals, creating verse/chorus/bridge structures.
- CV addressing can also switch Spread/Max Divide or Counting Direction between sections, drastically changing the rhythmic character and giving a sense of musical progression.

### **B. Clock Speed Automation**
- Change the master clock rate (from your main clock module) for tempo shifts, breakdowns, or uptempo drops. The RCD will maintain division relationships, and timing variations become compositional elements.
- Use Spread On/Off to alternate between “groove” and “machine” sections, e.g., straightforward 4/4 versus offbeat polyrhythms.

---

## 3. **Evolving Percussion, Melodies, and Song Movement**

### **A. Polyrhythm and Variation Generation**
- Chain RCD outputs to percussion, random sources, or quantizers to create polyrhythmic patterns, fills, and evolving textures.
- Rotate or Spread CVs can be sequenced or modulated, evolving the drum groove, melody, or bass part over time—no need for hands-on tweaking.

### **B. Conditional/Alternate Triggering**
- Use odd-numbered divides or high division values for occasional triggers (fills, resets, FX, scene swaps).
- Spread mode outputs classical “musical” divisions: make entire track sections switch to triplets or odd meters for breakdowns or bridges.

---

## 4. **Synchronizing Multiple Voices and Generating Song Endings**

### **A. Master Reset for Song Endings**
- At the end of the song, send a pulse to Reset. All outputs return to phase 1, which can be used to synchronize a dramatic finish (e.g., all sequences hit the “start” at once).

### **B. Self-Patching for Advanced Structures**
- Use an RCD output patched to its own Reset, or cross-patch between multiple RCDs (or RCD + QCD), to generate evolving song structures that never exactly repeat—think generative arrangements or “macro-loops” of many bars.

---

## 5. **Practical Patch Examples:**

### **A. Manual Section Changes**
- **Patch**: Manual gate or foot-pedal to the CV Rotate or Reset input.
- **Use**: Tap to flip between verse and chorus variants live.

### **B. Evolving Complexity**
- **Patch**: Slow LFO or stepped random to CV Rotate, quantized to RCD thresholds.
- **Use**: Groove gets busier or simpler automatically through a track; perfect for hands-free live jams.

### **C. Build/Release Dynamics**
- **Patch**: Sequence high divisions (e.g. /32 or /64) to momentarily fire big impacts, FX, or fill triggers. Lower as you move into breakdowns, raise for drops.

### **D. Synchronized Song End**
- **Patch**: When external master clock stops, send end pulse to Reset. All clocks start from beginning, “ending” all phrases together—great for a live set finisher.

---

## 6. **Essential Module Pairings for Composed Songs**
- **Switches/Matrix/Sequential Addressers:** To “program” song structure by controlling CV Rotate/Reset or clock sources.
- **Varigate, Malekko Voltage Block, etc.:** Pattern voltage output keeps arrangements in sync.
- **Quantizers and Random Sources:** To program melodic/rhythmic variation with clocked pseudo-randomness.
- **Logic modules:** AND/OR gates mute/unmute voices or trigger song events using RCD outputs.

---

## 7. **Summary Table**

| Use Case                        | Modules Needed           | RCD Feature Used     | Function                                                 |
|----------------------------------|-------------------------|----------------------|----------------------------------------------------------|
| Section/Scene Change             | Manual gate, switch     | CV Rotate/Reset      | Jump between different patterns instantly                |
| Macro-variation                  | Sequencer/LFO/random    | Rotate/Spread        | Evolve groove / automate song sections                   |
| Fills & FX triggers              | Clocked random/logic    | High divides/Spread  | Fire fills and effects at musical intervals              |
| Song ending/reset                | Master clock/logic      | Reset                | Synchronized endings or breaks                           |
| Generative structures            | RCD self-patch, logic   | Reset/Rotate, Up/Down| Create long evolving patterns, never precisely repeating |

---

## 8. **Creative “Songwriting” with RCD**
The RCD’s ability to rotate, spread, reset, and divide—with hands-on or CV control—lets you plan and trigger song sections, automate evolution, and build up macro-level arrangements all inside the patch. With a little preparation and practice, you can turn “forever” grooves into tracks that feel arranged, performed, and alive.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---