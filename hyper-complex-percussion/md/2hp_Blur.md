# 2hp — Blur

- [Manual PDF](../../manuals/2hp_Blur.pdf)

---

[**2hp Blur Manual PDF**](https://www.twohp.com/_files/ugd/92b4d5_bd1db19a268d4583b694e8037db30c36.pdf)

---

# Using 2hp Blur for Complex, Dense, Rhythmic Percussion in Eurorack

The **2hp Blur** is a *spectral processor* designed to blur, wash, and stretch incoming audio in unique ways. While it's commonly used for pads and ambient textures, it can be highly effective for transforming percussion and rhythmic sources, especially to create hyper-complex, polyrhythmic, and tightly designed percussive music.

Below is an advanced approach to utilizing *2hp Blur* in the context of dense and intricate rhythmic music.

## 1. **Signal Source Choices**
- **Rhythmic Audio Input:** Feed in sequenced percussion hits or complex rhythmic patterns from drum machines, sample modules (like the Tiptop One), or modular drum voices (e.g., 2hp Kick, BIA, etc.).
- **Transient-Rich Material:** The more defined your transient source, the more dramatic and interesting Blur’s effect on percussion will be, allowing you to "smear" and modulate attacks in rhythmically novel ways.

## 2. **Circuit Routing Tricks**
- **Multing and Layering:** Split your drum sequence so one copy goes dry and another routes through the Blur; use subsequent modules to layer and re-process.
- **Parallel Processing:** Combine heavily processed (Blurred) percussion with clean counterparts. Toggle between or crossfade for evolving rhythmic textures.

## 3. **Parameter Modulation Strategies**
- **TIME (Spectral Stretch):**
    - **CV Modulation:** Use rhythmic CV sources like advanced Euclidean sequencers, random LFOs, or stepped modulation to alter the TIME parameter in sync (or offset) from your master clock.
    - **Extreme Stretch for Rhythm:** Rapid CV swings can momentarily freeze bursty transients (granular time-stretch stutters) or smear elements to create "temporal ghost notes" between main hits.
    - **Sync to Clock:** Modulate so that each bar, beat division, or odd-length phrase has a unique stretch signature. Experiment with unsynchronized (off-grid) modulation for polyrhythm creation.

- **VIBE (Frequency Spread):**
    - **Percussive Timbre Variation:** Assign stepped or random CV to VIBE so spectral smearing occurs selectively on certain hits or at specific pulse divisions. This gives the impression of spectral "flams" or harmonic doubling on drums.
    - **Accent Polyrhythms:** Use polyrhythmic gates or CV (e.g., 3-against-4 patterns) to punch certain hits into smeared spectral clouds while keeping others dry and crisp.
    - **Dynamic Sonic Spread:** Manually jam or sequence modulation to burst open the spectral spread on accents, fills, or odd-metered transition points.

- **MIX (Wet/Dry Balance):**
    - **CV Automation:** Sequence or randomize the MIX between dry and fully wet for sharply articulated versus smeared-percussive interplays. For very complex rhythms, automate this on every step of a percussion pattern to make some events "pop" and others "wash."
    - **Accentuate Unique Patterns:** Use burst generators or logic combinations to automate rapid toggling of the MIX, interleaving complex patterns with clean and washed textures.

## 4. **Chain and Layer for Percussive Density**
- **Cascade Blur With Reverbs or Pitch Shifters:** Use the recommended pairings (e.g., Pluck → Blur → Verb, or Blur → Pitch) to build up percussive motifs that twist, shimmer, stretch, and shift over time.
- **Resample and Re-trigger:** Record blurred hits, then re-trigger and further process with granular samplers or additional percussion modules.

## 5. **Advanced Polyrhythmic Techniques**
- **Rhythmic CV Sources:** Use dividers, multipliers, Euclidean sequencers, and complex clock manipulation to drive Blur's CV inputs. The spectral "time bending" capability can transform a steady groove into a polyrhythmic/percussive tapestry, especially when multiple clocks (e.g., 5/8, 7/16, etc.) drive different parameters.
- **Changing Texture Over Bar Cycles:** Use longer, evolving LFOs synced to odd-numbered cycles (e.g., a 7-bar LFO against a 4-bar pattern) to keep spectral rhythmic movement constantly evolving, never repeating.

---

## **Quick Patch Recipe for Punchy Spectral Percussion**
1. **Drum Sequencer → Blur IN**
2. **Fast, Stepped Random or Polyrhythmic CV → BLUR TIME**
3. **Accent or Alternate Pattern CV → BLUR VIBE**
4. **Step Sequence or Burst Generator CV → BLUR MIX**
5. **Blur OUT → Reverb, Pitch, or Resampling Chain**

- *Tip:* Try tying one modulation channel to a polyrhythmic source so only certain hits “blur out,” making the rhythm sound denser and ever-shifting.

---

## **Reference**
- [2hp Blur Manual PDF](https://www.twohp.com/_files/ugd/92b4d5_bd1db19a268d4583b694e8037db30c36.pdf)
- [2hp Blur Product Page](https://www.twohp.com/modules/blur)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)