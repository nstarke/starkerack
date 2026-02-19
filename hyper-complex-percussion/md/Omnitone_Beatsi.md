# Omnitone — Beatsi

- [Manual PDF](../../manuals/Beatsi_Information_Package.pdf)

---

[**Download the Beatsi Manual PDF**](sandbox:/mnt/data/Beatsi_Information_Package.pdf)

---

# Creative Approaches for Densely Rhythmic, Hyper-Complex Percussion Using Beatsi

_Beatsi_ is a **modular percussion voice** — a compact, digital take on modular drum synthesis, offering deep CV modulation and “kit morphing” timbral possibilities. Here’s how you can push it toward the most intricate polyrhythms, complex time signatures, and adventurous percussive experimentation:

---

## 1. **Patch Planning: Assign Triggers & Gates**

- **Use complex trigger sources:**  
  Patch sophisticated trigger sequencers, clock dividers/multipliers, and logic modules to the KICK, SNARE, HI-HAT, TOM, and CRASH trigger inputs.  
  - For polyrhythms, drive each input with clocks at different divisions (e.g., /3, /4, /5, /7) and/or clock sources with distinct swing/groove.
  - Use sequencers like Euclidean, Grids, or stochastic sources for unpredictable, non-repetitive hits.

---

## 2. **Complex Patterns & Time Signatures**

- **Modulo and probability modules:**  
  Feed the trigger ins with randomized or probability-based bursts, ratchets, or divided clocks.  
  - E.g., send hi-hats fast, Euclidean triggers for nested tuplets.
  - Use sequential switches or gate processors to shift which pieces are triggered over time.
- **Self-generative:**  
  Use asynchronous clocks or LFOs as sources for ever-shifting time signatures.

---

## 3. **Advanced Timbre & Kit Morphing**

- **Animate timbres:**  
  Assign CV1/CV2 to the timbre parameter for a drum (or several), and modulate it with slow LFOs or sample-and-hold for kit morphing "on the fly," fading between acoustic, lo-fi, and alien sounds.
  - *Example:* Snare morphs with every hit from punchy analog smack to crushed digital fizz by modulating Timbre.
- **Morphing between kits** mid-sequence can give a single pattern great variety.

---

## 4. **Assign CV Control to Multiple Parameters**

- **Hyper-expressive sequencing:**  
  Assign CV1 or CV2 to parameters like Pitch, Decay, and Level on multiple voices simultaneously.  
  - Patch CV from sequencers, random voltage, or envelopes for:
    - *Pitch cycling* each 16th note
    - *Decay-length modulation* for “humanized” fills
    - *Level/pan automation* for dynamic shifts

- **Use the attenuverter:**  
  Dial positive or negative polarity for subtle drift or radical flips (e.g., inverted envelopes making decay shorter on louder hits).

---

## 5. **Micro-Editing with Grid Controls**

- **Real-time muting/unmuting:**  
  For stuttered breakdowns, mute drums on demand (press both parameter + value knobs).  
- **On-the-fly sound sampling:**  
  Use the HIT button to quickly audition or "play" beats live.

---

## 6. **Unique/Signature Percussive Results**

- **Exploit the digital engine:**
    - Drastically modulate bitcrushing/downsamping (via Timbre), especially with alien/lo-fi kits, in rhythm with the pattern.
- **Choke or ratchet effects:**  
  Use fast gates/triggers on the HI-HAT for open/closed/ratcheted textures (decay starts at gate-off, so play with gate length!).

---

## 7. **Scope for External Processing**

- **Send OUT to additional FX:**  
  After Beatsi, feed into modular FX (distortions, delays, resonators) for further texturing.
- **Gate muting + live morphing:**  
  Combine grid muting with simultaneous CV timbre morphs.

---

## 8. **Performance & Recall Tips**

- **All CV/assignments and states are autosaved:**  
  No worries about losing your complex patch, encouraging risk-taking and deep parameter automation.
- **Hard reset:**  
  Hold hit, parameter, value during power up to start from scratch if things get wild.

---

### Summary Table: Parameter Manipulation Ideas

| Voice    | Polyrhythmic/Complex Use       | Patch CV to...             | Kit Morph/FX               |
|----------|-------------------------------|----------------------------|----------------------------|
| Kick     | Non-4/4 triggers, triplets     | Decay, Pitch, Timbre       | Acoustic ↔ Lo-fi on fills   |
| Snare    | Offbeat snare, syncopation     | Timbre, Level, Decay       | CV morph for gated fx      |
| Hi-Hat   | Ratcheted, polyrhythmic gates | Decay (with gate length)   | Swap kits mid-pattern      |
| Tom      | Drumline / tuned rhythms       | Pitch (V/Oct), Timbre      | Alien kit for odd times    |
| Crash    | Odd timing, random hits        | Timbre, Decay, Level       | Granular hat sounds        |

---

With its deep CV assignability, kit-morphing timbres, and per-piece control, **Beatsi** can be the rhythmic engine for intricate, ever-shifting percussion, especially when sequenced and modulated from other advanced Eurorack modules!

---

_**Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)**_