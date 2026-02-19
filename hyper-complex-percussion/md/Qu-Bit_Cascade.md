# Qu-Bit — Cascade

- [Manual PDF](../../manuals/Getting_Started_Cascade.pdf)

---

[**Cascade Manual PDF**](https://www.qubitelectronix.com/_files/ugd/e5b1ef_9b322b79e5354339a866740d7d6b5b2d.pdf)

---

# Using Qubit Cascade for Hyper-Complex Percussion & Rhythmic Sequences

As a Eurorack modular synthesizer artist, the **Qubit Cascade** is a powerhouse for generating dynamic, percussive, and wildly complex rhythmic material. Here’s a breakdown of strategies, patch ideas, and manipulation tips for creating polyrhythmic, intricate percussion:

---

## 1. **Cascade as a Unique Percussion Voice**

### **Internal Sound Sources**
Cascade can generate percussion sounds directly, thanks to its internal audio algorithms:
  - **White Noise**: Snappy noise bursts → snares, shakers, textures.
  - **808 Drums**: Core electronic hits.
  - **Sine Tone (HiFreq)**: Toms, metallics, clave sounds.

**Tip:**  
Trigger these with short, snappy envelopes (attack/release at minimum) for punch, or dial in more curve/time for organic flair.

---

## 2. **Ratcheting, Loops, and Hyper-rhythms**

### **Ratcheting AD Mode**
- **Repeats control:** This is your gateway to microtiming, ratchets, and tuplets (1x, 2x, 3x, 4x, 6x, 8x, 12x, 16x)!  
- **Complexity:** Patch in non-synchronous clocks or trigger sources to the trigger input for off-grid accents.

**Polyrhythm Example**  
- Set one Cascade channel to repeat at 3x, another at 4x, and trigger both with a master clock; the result is a 3:4 polyrhythm.

---

## 3. **Envelope Tailoring for Percussive Impact**

- **Fast Attack/Decay:** Ultra-snappy for clicky transients.
- **Exponential/Linear/Log curves:** Exponential for extra snap, linear for robotic, logarithmic for soft percussive tails.
- **Envelope Inversion:** Use the invert button with offset for upside-down volume shapes—great for sidechain and pumping effects!

---

## 4. **Advanced Modulation for Intricacy**

- **CV Over Repeats, Curve, Level, Offset:** Use random sources, LFOs, or sequencer modulation to dynamically warp each envelope or ratchet sequence for evolving percussion.
- **Gravity Modes:** Enable amplitude and time gravity for self-modulating envelopes; creates “bouncy ball” complexity or evolving accent patterns.

---

## 5. **Complex Time Signatures & Gate Manipulation**

- Use “Gate Output Modes” (trigger, EOD, EOA) to generate gates not just on main triggers, but at envelope segment transitions—patch these into other percussion voices to create interlocking, follow-on patterns (e.g., kick on envelope end → hi-hat).

---

## 6. **External Sound Shaping and Effects**

- **VCA + Envelope:** Cascade excels as a VCA/envelope for sculpting external percussive sounds—try shaping FM percussion, samples, or noise, especially with envelope follower or compressor mode for dynamic envelope control.
- **Compressor Mode:** Sidechain compression with a virtual sidechain—duck complex rhythmic material or make space for accents.

---

## 7. **Patch Concepts for Dense, Hyper-Rhythmic Grooves**

**A. Multi-Cascade Drumkit:**
  - Use 2–3 Cascades (or mult the gate) for kick, snare, hat.
  - Give each a different repeats/multiplier setting.
  - Offset each envelope’s start/decay so events overlap and phase-shift.

**B. Envelope Follower for Groove Extraction:**
  - Route complex audio into the Envelope Follower input.
  - Use follower output to modulate level or triggers elsewhere, locking percussion to existing material’s groove.

**C. Self-Modulated Ratcheting:**
  - Patch the Gate Output back to the trigger input (with attenuverter), or use CV-ed segments to “auto-ratchet” and randomize rhythm lengths.

---

## 8. **Making Percussion Uniquely Punchy**

- **Max Level, Min Attack:** Get sharp, club-ready transients.
- **CV Modulate Offset:** Flushes ‘ghost hits’ or evolving amplitude response.
- **Use Invert + Offset:** Immediate “ducking”/sidechain or reversed staccato shapes.
- **Exploit Gravity & Internal Sounds:** Unpredictable, lifelike movement.

---

## 9. **General Workflow**

1. **Pick a sound source** (internal or external via VCA in).
2. **Select envelope mode** (AD, ADSR, etc) for each percussion hit.
3. **Patch triggers/gates** (experiment with offset polyrhythms).
4. **Modulate everything—** especially repeats and curves.
5. **Experiment!** Routings + curves = endless unique percussion.

---

For more deep dives, refer to the [full Cascade manual PDF](https://www.qubitelectronix.com/_files/ugd/e5b1ef_9b322b79e5354339a866740d7d6b5b2d.pdf).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)