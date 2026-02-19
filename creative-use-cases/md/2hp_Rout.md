# 2hp — Rout

- [Manual PDF](../../manuals/Rout_Manual.pdf)

---

[**Download the Rout Manual (PDF)**](sandbox:/mnt/data/rout_manual.pdf)

---

# Creative Patch Ideas for 2hp Rout

The 2hp Rout is a compact, voltage-controlled gate switch, offering dynamic routing of a single gate/trigger input to any of four outputs. Here’s how you can creatively integrate it into your modular system:

---

## 1. **Rhythmic Pattern Distribution**
**Modules Needed:**  
- Sequencer (e.g., **Make Noise Rene**, **Intellijel Metropolix**)  
- Drum modules (kick, snare, hi-hat, etc.)  
**Patch Idea:**  
Feed a single rhythmic gate pattern from your sequencer or clock divider into Rout’s INPUT. Use a CV sequencer, random source, or any modulation source patched to SEL CV to dynamically select which drum voice receives the gate at any moment. This creates constantly evolving drum patterns from a single sequence.

---

## 2. **Generative Percussion Shuffling**
**Modules Needed:**  
- Random CV generator (e.g., **Make Noise Wogglebug**, **Mutable Instruments Marbles**)  
- Drum voices or sound sources  
**Patch Idea:**  
Send random stepped CV to Rout's SEL CV, and the master clock to INPUT. Each clock pulse triggers a different drum or percussion voice, scrambling the groove for generative rhythms.

---

## 3. **Voice Allocation for Shared Gate Patterns**
**Modules Needed:**  
- Polyphonic voice modules or several mono synths  
- Quantizer  
**Patch Idea:**  
Send an arpeggiator or rhythmic gate sequence to INPUT. Use manual SEL or CV-controlled SEL for live or sequenced voice allocation, letting a single pattern "jump" between different voices or timbres for evolving melodic lines.

---

## 4. **Accent Routing**
**Modules Needed:**  
- CV sequence (accent pattern)  
- Drum module/sound source with accent in  
**Patch Idea:**  
Feed a main clock or trigger into Rout’s INPUT, and use SEL CV (patterned with accents) to choose when to send triggers to an accent input, opening up full/partial accents depending on SEL position.

---

## 5. **Performance-Based Output Switching**
**Modules Needed:**  
- Manual offset generator (e.g., **Intellijel Planar**, **Doepfer A-174-2 Joystick**)  
**Patch Idea:**  
Use Rout as a manual performance router by controlling SEL with a joystick or offset knob. This allows "live switching" of gate outputs to different voices on the fly.

---

## 6. **Step-by-Step Gate Distribution from Sequencer**
**Modules Needed:**  
- Multi-channel step sequencer  
- Four different drum modules or effect triggers  
**Patch Idea:**  
Use a CV sequencer channel mapped to 0–5V to step through outputs in sync with your gate pattern. Rout distributes the main trigger sequence in a linear or custom sequence across four destinations.

---

## 7. **Probability-Based Routing**
**Modules Needed:**  
- Probability gate module (e.g., **Mutable Instruments Branches**)  
- Random CV source  
**Patch Idea:**  
Combine a probability gate and a random CV source to occasionally switch Rout’s outputs based on probability thresholds, making some drums or events less or more likely depending on performance context.

---

## 8. **Layered Effects or Fill Switches**
**Modules Needed:**  
- Effect modules with gate/trig input (e.g., gating a delay/reverb)  
- Drum fill trigger source  
**Patch Idea:**  
Send your groove’s "fill" trigger to Rout INPUT. SEL CV determines which effect or fill gets engaged, making fills less predictable and effects timbrally varied.

---

### **Tips for Best Results**
- **Sequence SEL with quantized CV sources** to ensure neat output changes.
- **Stack Rout with other sequential switches** for more complex routing hierarchies.
- **Use LEDs as indicators** when patching live: the Rout’s out LEDs are helpful for visual troubleshooting.

---

By using Rout for gate/trigger signal routing under voltage control, you can bring order, chaos, or new complexity to your rack’s rhythm and event structure.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)