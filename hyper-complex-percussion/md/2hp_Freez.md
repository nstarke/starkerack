# 2hp — Freez

- [Manual PDF](../../manuals/Freez_Manual.pdf)

---

[Freez Manual PDF](https://www.2hp.com/manuals/freez.pdf)

---

## Using Freez for Densely Rhythmic, Hyper-Complex Percussion in Eurorack

The **Freez** module is a voltage-controlled locked looper, not a sound source/voice, but an **audio processor/effect**. Its core abilities—freezing, looping, and manipulating incoming audio buffers—make it a creative powerhouse for complex percussion, especially when combined with other rhythmic generators. Here’s how to harness its power for dense, punchy, and uniquely percussive sequences, including complex time signatures and polyrhythms:

---

### 1. **Getting Percussive Input**
- **Feed it with Percussion:** Send drum hits, complex loops, short percussive bursts, or glitch sources into Freez's **IN**.
- **Try Multiple Hits:** Sequence diverse percussion patterns, including non-standard (non-4/4) sequences or polyrhythms from other modules or drum machines.

---

### 2. **Locking, Chopping, and Mangling**
- **Use** ***momentary or latching*** **mode** via the **MODE TOGGLE** for different rhythmic interactions:
  - **Momentary Mode:** The buffer “freezes” *only* as long as the button/trig is held high; ideal for tight rhythmic chopping.
  - **Latching Mode:** Press or trig to lock/unlock the buffer in sync with complex rhythmic events (e.g., accent pulses in a polymeter).

- **Patch gate/trig sources** (from polyrhythmic sequencers, clock dividers, or logic patterns) to the **TRIG** input for rhythmically controlled buffer captures, *perfect for locking audio on odd divisions or syncopations*.

---

### 3. **CV Rhythmic Variations**
- **Send polyrhythmic CV** and **trigger/gate sequences** to the **SIZE** and **S. RATE CV INPUTS**
  - **SIZE CV:** Modulate buffer length with evolving LFOs, sequencers, or random gates for dynamic, unpredictable loops.
    - Patch a sequential switch, step sequencer, or odd/even divider to create shifting lengths following your intended polyrhythm.
  - **S. RATE CV:** Use rhythmic CV to introduce bitcrushing, aliasing, or time-domain warping tied to your clock or accent signals, *adding crisp “grain” and transient punch*.
    - Try sending tightly quantized or bursty random CV to sync with complex drum patterns.

---

### 4. **Percussive Texture Generation**
- **Beat Repeat:** Rapidly retrigger the TRIG input in microtimed “fills” or tuplets; with short buffer and low sample rate, you get synthy, glichy retriggers that are very distinct in a drum mix.
- **Granular & Glitch:** Modulate the buffer size or sample rate at audio rates (via fast LFOs or random gates) for digital spikes, artifact accentuation, and unique glitch-percussion layers.
- **Extreme Modulation:** Use envelope generators or stepped random sources clocked in irrational time divisions to modulate SIZE and S. RATE for complex “not-quite-repeat” textural percussions perfect for breakbeats, IDM, or mathy rhythms.

---

### 5. **Making the Output Punchy and Unique**
- **Short Buffers:** Tune buffer to “microsecond” range for instant, one-shot blips and digital clicks, creating synthetic hi-hats or claps when sampling percussive input.
- **Bit-Crushed Compression:** Push sample rate low to decimate transients, leaning into circuit-bent, hard-edged digital percussion.
- **Dynamic Layers:** Chain multiple Freez “captures” alongside dry percussion for polyrhythmic, syncopated percussion textures layering unaffected and looped elements.

---

### 6. **Integration in Complex Patterns**
- **Trigger Logic:** Use AND/OR/XOR logic gates to combine triggers of different clocks (3, 5, 7, etc. divisions) for true polyrhythms—control Freez freezing events with these.
- **Pattern Shifting:** Use rotating clock dividers or shift registers to create non-repeating freeze/unfreeze patterns for intricate groove changes.

---

### Example Patch Ideas

```plaintext
[TRIG IN] <--- Gate pattern from clock-divider running at (3/4 of master clock)
[SIZE CV IN] <--- Patterned random stepped CV clocked at (7/16 master clock)
[S. RATE CV IN] <--- Envelope/Accent CV from each bar, or another LFO at a different prime rate
[IN] <--- Hi-hat, snare, or FM drum hit sequence
[OUT] ---> Mixer for punchy, bitcrushed, polymetric percussion layer
```

---

**Tips for Uniqueness:**  
- Modulate every parameter with *unsynced* clocks—or clocks related by non-integer ratios—for brain-melting, non-repeating shifts.
- Use very short freeze times and abruptly modulate sample rate for grainy, modern digital percussion.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)