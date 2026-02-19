# Make Noise — Mimeophon

- [Manual PDF](../../manuals/mimeophon-manual.pdf)

---

[Download the Soundhack Mimeophon Manual PDF](https://makenoisemusic.com/content/manuals/soundhack_Mimeophon_Manual.pdf)

---

## Using a Make Noise Soundhack Mimeophon for Dense, Hyper-Complex Percussion & Polyrhythms

The **Mimeophon** is a stereo, multi-zone color audio repeater and can function as both an effect and, in certain settings, as a percussive voice (Karplus-Strong/physical modeling). Here’s how you can push it into *hyper-complex* rhythmic territory for advanced Eurorack percussion and sequence processing:

---

### 1. **Exploit the Tempo Sync, Rate, and Zone Controls**

#### **External Clocking and Polyrhythms**
- **Feed several rhythmic sources** (polyrhythmic clocks, different divisions/multiples) into the TEMPO input.
- Use **different sequences or modulation sources** to change Zone and Rate—each Zone is a radically different “buffer size” (delay time), from microseconds (flange/Karplus) to 40+ seconds (long loops).
- By switching Zones (with sequencers, random sources, or step CV), your repeats can instantly jump to new time grids *without Doppler or pitch artifacts*. This is great for sudden complex pattern changes.
- **Manipulate the Rate knob after clocking**: Slewless jumps between divisions/multipliers of the incoming clock—use this for sudden polyrhythms within a single pattern!

#### **Patch Idea - Polyrhythm Machine**
- Sequence the Zone input with stepped random or other sequencer signals *unsynced* to your main clock.
- Use the Rate CV in conjunction with separate division clocks to achieve complex interlocking.
- For every clock tick or bar line, force a Zone or Rate change. This "re-maps" the time base for the repeats—perfect for breakbeats, glitches, or evolving groove.

---

### 2. **Use Skew, Halo, and Ping Pong for Spatial & Temporal Complexity**

#### **SKEW**
- The SKEW function lets Left and Right repeats run at different Rates. Patch an LFO or divide/multiply clocks (*one for Rate, another for SKEW control*).
- Engage Ping Pong or Swap for alternating/phase-shifted patterns in stereo: "echoes" or percussive hits shift and bounce across the stereo field in a non-repetitive way.
- With HOLD engaged, change SKEW for evolving gating and “hocketing” effects.

#### **HALO**
- For dense, spatialized percussion: set HALO near max for a stereo “smear” or diffusion. Combine with high Repeats for a metallic/plate-reverb dreamscape effect—great as a percussive bed or layer.

---

### 3. **Mimeophon as a Percussive Voice (Karplus-Strong/Physical Modeling)**

#### **Zone 0 & Karplus Mode**
- Patch a short noise burst or impulse (e.g., from Make Noise MATHS or a trigger to noise generator) to the input.
- Set Zone to 0 and Rate high (full CW); adjust Repeats for “pluck decay.”
- MicroRate becomes 1V/Oct—sequence with pitch CV for percussive pitched hits, almost like a quick acid bass drum or tuned percussion.
- *Flip* the buffer for unusual metallic or shifted harmonics.

#### **Patch: “Karplus Drum Kit”**
- Rapidly change Zone or Rate alongside triggering audio bursts, turning every percussion step into a *different sound engine instance* (snare, bongo, kick, etc.).
- Modulate Color and Halo for each “hit” for ever-changing texture.

---

### 4. **Advanced Tricks for Rhythmic Density**

#### **Zone Jumps for Micro-Macro Patterning**
- Use a fast pulse on the Zone input (sequenced) to alternate between micro (Zone 0) and macro (Zone 6/7) repeat sizes, creating both glitch stabs and giant “room” echoes cascading within the same phrase.

#### **Feedback/Repeats Macrocontrol**
- Automate the Repeats via CV to punch holes or add rolls in the echo. For every hit, you can set Repeats briefly to max for ratchets/rolls, then drop back for staccato fills.

#### **Flip for Off-Grid/Reverse Hits**
- Gate the FLIP input in odd patterns—suddenly reverses the loop buffer. Use at audio rate for digital distortion textures or at percussive rates for off-grid, glitchy reversals.

#### **RATE Output as a Pattern Source**
- Use RATE OUT as a clock divider/multiplier for other sequencers/drum voices. Skew, Zone, or Rate adjustments on the Mimeophon will now propagate pattern changes to the rest of your drum voices—automatic evolving patterns.

---

### 5. **Color, Halo, and Input Gain Modulation for Punch**

- **Color:** Use as a dynamic per-hit EQ/distortion. Random modulation here adds variability and punch.
- **Halo/Repeats:** Vary in time, not just set-and-forget! Try patterning both for fills, ghost notes, swells.
- **Input Gain:** Set hotter for overdrive/crunch, or attenuate for pristine ‘ghost’ repeats in the background.

---

### Example Modular Patch Structure

```diff
Kick Drum (Trigger) ─> Noise Burst ─> Mimeophon IN L
MATHS Envelope ─> MicroRate (tonality/pitch sweep)
Random CV/Sequencer ─> Zone, Rate, Repeats CV
Stepped Clock Divider A ─> TEMPO
Main Clock ─> Skew (for stereo pulses)
Mimeophon OUT L/R ─> Mixer/Stereo Bus
Rate OUT ─> Envelope Trigger for another drum voice
```

---

### Summary Table - Perceptual Effects by Parameter

| Parameter        | Use for Polyrhythms/Complexity                              | Use for Percussive Impact         |
|:-----------------|:-----------------------------------------------------------|:----------------------------------|
| Zone             | Macro time changes, polyrhythm jumps                        | Micro time for attack, loop for tails |
| Rate             | Immediate time division/mult, manual groove changes         | Fast for punchy, slow for dub/echo |
| Skew             | Stereo polyrhythms, ping-pong, complex grid overlays        | Tight or wide image, phase tricks  |
| Halo             | Smear, glue, pseudo-reverb for layering                     | Zero for sharp/repetitive hits     |
| Color            | Modulate for timbral counterpoint, dense freq interplay     | Set for attack/decay shaping, dirt |
| Flip             | Time-reversal, glitch, pattern morph                        | Sharp metallic, reverse hits       |
| Repeats          | Fills, ratchets, cycle pattern complexity                   | Low for dry/punch, high for roooooooll|
| Input Gain       | Clip for digital grit, attenuate for only backghosts        | Boost for hit, cut for room        |

---

### Manual Link

[Soundhack Mimeophon Manual PDF](https://makenoisemusic.com/content/manuals/soundhack_Mimeophon_Manual.pdf)

---

Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)