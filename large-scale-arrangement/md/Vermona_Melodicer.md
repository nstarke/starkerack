# Vermona — Melodicer

- [Manual PDF](../../manuals/melodicer manual en 1.1 web.pdf)

---

[**Vermona meloDICER User Guide (PDF)**](https://www.vermona.com/en/support/downloads/detail/product/melodicer/file/melodicer_user_guide/)

---

# Creating Full Length Songs with the Vermona meloDICER & Your Eurorack System

Building evolving, song-length structures in Eurorack can be challenging—patching a groove or motif is easy, but making it unfold over 3-7 minutes like a track in traditional songwriting is another thing entirely. The Vermona **meloDICER** offers a unique set of features merging stochastic (random) and deterministic sequencing, making it a strong centerpiece for creating not just loops, but evolving musical compositions.

Below you'll find strategies for using the meloDICER—often in combination with other modules—to move beyond static patterns and towards fully-structured songs.

---

## 1. **Pattern Variation and Memory Recall**

**meloDICER** stores up to 16 patterns, each containing all rhythm/melody settings, DICE states, step lengths, variation settings, etc.
- **Step-by-step Songwriting:**
   - Compose verse, chorus, bridge, and fill patterns—save each to a pattern slot.
   - Use the **L (Load)** button and rotary encoder to recall different patterns during performance or recording.
- **Combine with CV/Trigger Selectors:**
   - Use trigger sequencers (e.g., Malekko Varigate 4+, Intellijel Steppy, Mutable Instruments Grids, etc.) or manual switches to send gate triggers to meloDICER’s GATE INs.
   - Patch gate triggers to automate pattern changes, mutes, DICE functions, or lock-modes for hands-free arrangement.

## 2. **Dice/Re-dice and Real-time/Locked Evolution**

- **Stochastic Variation:** Pressing the DICE buttons generates new random-based content, whereas holding them switches to continuous randomization (realtime-mode).
- **Song Evolution:**
   - During “choruses” or breakdowns, use real-time mode for more variety, then snap back to diced/static patterns for recognizable hooks.
   - Use external triggers to re-dice patterns at key moments (with GATE IN and “RE-DICE” assigned in Edit Params).
- **Lock Mode for Preparation:**
   - Prep new parameters while a loop is running (lock-mode ON—no changes heard), then deactivate lock-mode at drop/change points for “scene” transitions.

## 3. **Rhythmic and Melodic Probability**

- **Fade in/out parts:** Use REST, LEGATO, VARIATION, and the probability faders for each note to “thin out” or “densify” melodies/rhythms—great for intros/outros or dynamic song sections.
- **Automate with CV:**
   - Use LFOs, random voltage sources (Wogglebug, Turing Machine), or manual controls—patched to meloDICER’s CV INs—to modulate these parameters over song time for organic changes.

## 4. **Sub-Pattern and Pattern Length**

- **Pattern Length & Range Move:** Shorten/lengthen patterns for tension/release, or shift start/end points to create fills or break sections.
- **Automate with Triggers or CV:**
   - Use sequencers, clocks, or manual control to change pattern positions.
   - For even more evolution, shift sub-ranges of patterns gradually across a song.

## 5. **Synchronizing with Your System**

- **Clocking:**
   - Sync meloDICER to your DAW, external clock, or another module for tight integration.
   - Use its “tap tempo” for freeform jams, then resync or lock in as needed.

## 6. **Muting, Fills, and Layer Control**

- **Mute GATE OUT manually or with GATE IN to drop rhythm/melody for breakdowns or tension-building sections.**
- **Combine with other voices or drums:**
   - Mute meloDICER’s output while other lines take focus, or bring it in and out for build-ups.

## 7. **Interaction with Other Modules**

- **Melodic quantization (C or D Modes):** Quantizer modes let meloDICER act as a scale quantizer for other CV sources. Process generative CV and tie everything to your song’s harmonic context.
- **ARPEGGIATION/Polyphony:** Pair two meloDICER modules (as suggested in Seq+Gate Mode) for duophonic interplay—one module sequences gates, the other melodies, for more complex arrangements.

---

## **General Song-Structuring Techniques**

- **Use external modules** for further song control:
  - **Sequential Switches** (e.g., Doepfer A-151) for routing different voices in/out of the mix.
  - **Voltage Presets/Scenes** (e.g., Make Noise Presure Points/Planar, Malekko Voltage Block) to change multiple parameters at once for B-section/drops.
  - **VCAs and Mixers** automate volume/fades or even transpose parts via voltage.
  - **Logic and Probability Modules (e.g., Mutable Branches, Doepfer A-166)** to randomly trigger pattern changes or fills.

- **Layer with Loops & Effects:**
  - Record and loop interesting meloDICER phrases with samplers/loopers.
  - Use delay, reverb, or granular modules to extend and morph sections across the song timeline.

---

## **Practical Song Structure Example**

1. **Intro:** REST and LEGATO set high, probability faders mostly down (minimal, ambiguous motif). Use mute or low pattern length for sparsity.
2. **Build Up:** Gradually increase melody probability faders, lower REST, and increase pattern length. Automate with CV/LFO.
3. **Main Pattern (Drop):** Recall pattern slot with more rhythmic activity and full range, possibly re-dice for fresh motif.
4. **Breakdown:** Engage lock-mode, prepare new pattern with higher rests/variation. Unmute for re-entry.
5. **Fills/Transitions:** Use random RE-DICE or shift pattern range, or quickly mute/restore rhythm with GATE IN.
6. **Outro:** Reduce pattern length/REST up, fade out melody range with faders.

---

## More Reading

- [Vermona meloDICER PDF Manual](https://www.vermona.com/en/support/downloads/detail/product/melodicer/file/melodicer_user_guide/)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---

Let the meloDICER's blend of programmed structure and cosmic chance breathe longform life into your modular songs!