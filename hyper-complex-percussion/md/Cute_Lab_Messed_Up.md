# Cute Lab — Messed Up

- [Manual PDF](../../manuals/messed-up-manual-rev2.pdf)

---

[**View the MessedUp Module Manual (PDF)**](sandbox:/mnt/data/MessedUp_Manual_Rev2.pdf)

---

# Creating Hyper-Complex Percussion with MessedUp

As a Eurorack musician seeking intricate, evolving rhythms, **MessedUp** is an invaluable module. It’s designed specifically for metric modulation, polyrhythms, and non-standard clock patterns, making it perfect for your goals of **densely rhythmic music** and **complex percussion**. Below is a guide for maximizing MessedUp’s potential in your modular setup.

---

## 1. **Internal & External Clocks for Syncopation**

- **Use MessedUp as a Clock Source:** With no external clock, MessedUp generates its own, settable via tap tempo or encoder adjustment. This is great for creating a master clock with swing or non-standard rates.
- **Sync to an External Clock:** Patch an external sequencer, LFO, or drum machine clock into MessedUp. Now, you can stretch, divide, or modulate this master signal into unexpected time realms.

---

## 2. **Polyrhythm and Complex Meter Generation**

### **Beat** & **Divide** Controls
- **Beat** = Your “measure” length (e.g. 4 for 4/4 feel, 5 for quintuplets, etc.)
- **Divide** = Number of clock pulses spanned/played in that “measure.”

**Classic Polyrhythm Example:**
- Set **beat** to 4 and **divide** to 3 → Output a 3-against-4 rhythm (triplets over quarter notes).
- Reverse for 4-against-3 (divide 4, beat 3) or explore any non-integer relationship for hypercomplex rhythms (e.g. beat 7, divide 5).

### **Truncate** Output
- Adds *syncopation* by chopping the divide output at variable places in the measure. Sweep the truncate knob or modulate via CV for evolving, offset rhythms that land in unpredictable places within the cycle.

---

## 3. **Metric Modulation for Tempo Shifts & Temporal Distortion**

- **Modulate Button/Input:** Instantly stretch or compress the output clock by the current ratio (e.g., 120 BPM × 4/3 = 160 BPM). Great for live “time-warp” effects or compositional pivot points.
- **Round Trip/One Way:** Choose whether you want modulation to bounce back to normal, or recurse deeper into tempo labyrinths.

---

## 4. **Latch & Cue, Stay in Sync**

- **Latch beat/divide encoders** to the downbeat—changes snap in on the “1,” preserving phase relationships and maximizing funkiness and compositional control.

---

## 5. **Complex Time Signatures**

- **Go Beyond Standard Meter:** Set beat or divide to prime numbers (5, 7, 11), or highly composite numbers for shifting groupings (e.g. beat=12, divide=7 for a 7 over 12 groove).
- Use **configuration menu** to fine-tune PPQN, duty cycle, and reset behavior, for fitting MessedUp to unusual gear or external logic.

---

## 6. **Patch Ideas for Hyper-Complex Patterning**

- **Percussion Modulator:** Feed MessedUp’s outputs (*divide*, *truncate*, *beat*) into drum triggers, logic gates, or sample players. Each output gives you a mathematically related pattern.
- **Sequencer Drive:** Use odd beat/divide combos to create shifting downbeats on sequencers or arpeggiators, creating patterns that only realign after many measures.
- **Live “Time DJ”:** Modulate live, flip between round trip/one way, and dynamically change beat/divide for ever-evolving polymeters. Use EoM (End of Modulation) output to trigger fills, FX, or scene changes in sync with metric modulations.

---

## 7. **CV Modulation for Algorithmic Funk**

- Patch random, stepped CV, envelopes, or another rhythmic source into **beat**, **divide**, or **truncate** CV inputs. Use the attenuverter for depth and direction. This makes your polyrhythms evolve in controlled or chaotic ways, generating “algorithmic” density and mutation.

---

## 8. **Presets & Performative Recall**

- Save setups (tempo, ratios, latch states) in one of nine presets for instant switch-ups during performance or composition.

---

### **Further Inspirations:**
- Explore metric modulation techniques (see manual appendix), inspired by contemporary composers for mind-bending time feels.
- Use the **truncate** output to “break” up static patterns for unexpected funk and glitch.

---

## **Summary Table: Outputs for Percussion Channels**

| Output      | Use For                    | Complex Pattern Ideas                                   |
|-------------|----------------------------|--------------------------------------------------------|
| Beat        | Main clock, snare, hats    | Odd beat length = shifting grooves                     |
| Divide      | Kicks, toms, secondary drums | Prime divisions = never-repeating accents              |
| Truncate    | Clave, rim, syncopated triggers | CV-modulated = constantly morphing syncopation     |
| Downbeat    | Phrase markers, fills      | Keeps structure amidst chaos                           |
| EoM         | FX triggers, resets        | Used on metric modulation for time-warp effects        |

---

## References

- [**MessedUp Manual (PDF)**](sandbox:/mnt/data/MessedUp_Manual_Rev2.pdf)
- [**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)

---

Feel free to experiment wildly—the combinatory depth of *MessedUp* for polyrhythms and time manipulation is nearly inexhaustible.