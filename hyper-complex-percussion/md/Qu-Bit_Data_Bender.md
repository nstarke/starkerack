# Qu-Bit — Data Bender

- [Manual PDF](../../manuals/QB_Data_Bender.pdf)

---

[**Qu-Bit Data Bender Manual PDF**](https://cdn.shopify.com/s/files/1/2996/6240/files/Databender-Manual-3.0-web-min.pdf)

---

# Using Data Bender For Hyper-Complex, Rhythmic Eurorack Percussion

## Module Overview

The **Qu-Bit Data Bender** is a circuit-bent digital audio buffer acting as a highly musical, glitchable, and clock-manipulable audio mangler. Data Bender can be used both as a creative effect and as a unique percussive voice source, dependent on patching strategy. Its clock and buffer manipulation, stutter/glitch features, and CV-controllable parameters make it ideal for creating rhythmically dense, polyrhythmic, and hyper-detailed percussion sequences.

---

## Strategies for Complex, Rhythmic Percussion

### 1. **External Clock Sync & Polyrhythmic Clocking**

- **Use External Clocks:** Send different clock sources (with polyrhythmic or polymetric relations, e.g. 5/8 against 7/8, or weird division triplets) to the **clock input**. Pair Data Bender with modules like Pamela's New Workout, Tempi, or Zularic Repetitor for experimental timing.
    - **Time Knob in External Mode:** Use Time knob to multiply/divide external clock in musically complex ratios (see manual: multiply/divide by 2, 3, 4, 8, etc.).
    - **Result:** Buffers, repeats, and glitches will "dance" on top of overlapping, cross-rhythmic time bases.

### 2. **Manipulate Buffer Subdivisions With CV**
- **Repeats Knob + CV:** Dynamically alter how incoming audio is subdivided using complex, synced or random CV. Patch unpredictable stepped & curving CV into the Repeats input to fragment the buffer.
    - **Result:** Your percussive loop or hit is diced, stuttered, or atomized at musically shifting rates. Coupled with clock manipulation, this builds complex, unpredictable rhythmic grains.

### 3. **Time-Variant Glitching With Corrupt Modes**
- **Corrupt Section (Decimate, Dropout, Destroy):**
    - Use Dropout for sudden silences, Decimate for bitcrushed "digital percussion," or Destroy for crunchy, striking digital distortion.
    - Modulate the Corrupt CV input with fast, stepped random (sample & hold), triggers, gates, or rhythmic LFOs to make corruption burst in time with your clock/rhythms.
    - **Idea:** Use sequence resets or clock division to regularly "glitch" every nth bar, making fills, breaks, and hyper-detailed rhythmic events.

### 4. **Freeze & Unfreeze For Granular Stutters**
- Use the **Freeze button or gate input** to rhythmically capture, stutter, and remix short buffer sections. 
    - **Trig/gate Freeze with polyrhythmic triggers** to alternate between live input and frozen glitches.
    - **Manual or sequenced toggling** of Freeze at odd intervals creates loose, off-grid, or microtimed glitch percussion.
    - **Tip:** In momentary mode, Freeze acts as a dynamic gate for stuttered micro-loops, great for IDM/Breakcore chops.

### 5. **Break and Bend For Playhead & Speed Tricks**
- In **Macro Mode:**
    - **Bend:** Use for playhead reversals and speed changes; modulate for tape-stop stabs or backwards bursts—percussive and weird.
    - **Break:** Modulates repeats and positions; high settings create random jumps/cuts (CD-skipping or busted tape flutter).
    - **CV these with per-channel (stereo split) rhythm sources** for intricate, stereo percussive mayhem.
- In **Micro Mode:**
    - **Bend (Speed):** Modulate for rapid tape-like pitch snapping, octave jumps, or reversals at tempo.
    - **Break (Traverse/Silence):** Create ghost hits, micro-silences, or triplet/tuple breakdowns in a drum loop.

### 6. **Stereo Tricks**
- **Unique Mode:** Set stereo to unique with Shift+Bend—each L/R channel gets different glitch logic. Send hard-panned percussion (or multi-mic recordings, or L/R split beaters) to Data Bender and let both sides glitch independently for dense, evolving stereo rhythm.
- **Shared Mode:** Use for focused, punchy mono percussive patterns.

### 7. **Glitch Windowing For Transient Shaping**
- **Shift+Time Controls Glitch Window:** Use less windowing for sharp, clicky glitches that mimic extremely fast percussive transients and artifacts; more windowing for ghostly, swelling textural rhythms.

### 8. **Patch Example**

```patch
CLOCK OUT 1 (Pam’s @5/8) ---> DATA BENDER CLOCK IN
CLOCK OUT 2 (Pam’s @7/8) ---> FREEZE/ BREAK/ CORRUPT (via logic or S&H)
SEQUENCED DRUM HITS ---> DATA BENDER IN L/R
BASS or SYNTH PULSE ---> DATA BENDER IN R (for additional cross-percussion)
MULTIPLE RANDOM CVs (from Batumi, Sapèl, Marbles) ---> TIME, REPEATS, BREAK, BEND CVs
DATA BENDER OUT L/R ---> MIXER/FX/RECORDER (with optional sidechain comp)
```
- Try capturing a dry drum groove and mangling it with all parameters sequenced, using odd-length clocks and complex CV to constantly disrupt and reassemble the rhythmic grid.

---

## Bonus Tips

- **Buffer Memory:** Since Data Bender keeps a ~1min buffer, long-form manipulation is possible—freeze, stutter, and unfreeze "old", previously played material for especially mind-bending rhythmic recapitulations.
- **Punch/Transient Creation:** Use Decimate/Destroy for digital click pops and hard edges—exceptionally effective for modern, punchy percussive sound design.
- **CV Randomization:** Use Eurorack random modules (e.g., Marbles, Chance) to keep the patterns fresh and unpredictable.

---

## Reference

- [Qu-Bit Data Bender Manual PDF](https://cdn.shopify.com/s/files/1/2996/6240/files/Databender-Manual-3.0-web-min.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)