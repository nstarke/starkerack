# 2hp — Euclid

- [Manual PDF](../../manuals/2hp_Euclid.pdf)

---

[Euclid 2hp Module Manual PDF](https://2hp.com/docs/euclid.pdf)

---

# Creative Modulation Techniques with the 2hp Euclid Module

The **2hp Euclid** is a compact Eurorack rhythmic pattern generator based on the Euclidean algorithm. With CV control over pattern length, steps, and offset, it can generate everything from regular pulses to complex, irregular rhythms for any genre. Below are several ways to exploit its features for **distorted percussion**, **aggressive basslines**, and **haunting pads**.

## Key Modulation Destinations

- **Length**: Number of steps in the polyrhythm (1–16)
- **Steps**: Active pulses per pattern (1—Length)
- **Offset**: Phase/starting point of pattern (0—Length-1)
- All above can be modulated via CV (0–5V for Length and Steps)

---

## Techniques by Sound Type

### 1. Distorted Percussive Sounds

**Patch Idea:** Use randomized or chaotic modulation to get glitchy, broken rhythms, great for industrial or distorted percussion.

- **Clock** the Trig Input with a fast or swung clock for interesting rhythms.
- Use a **sample & hold**, **random voltage**, or **LFO** to modulate the **Steps** and/or **Length** CV. This will cause beats to “fracture” and shift constantly.
- Modulate **Offset** with a slow, slewed random voltage so the pulse placement changes every bar or so, disorienting the groove over time.
- Send the **Trigger Output** into a drum module, noise source, or even a **wavefolder/distortion** to exaggerate the clipped, hard-edged effect.
- **Extra:** Mult the out trigger and use it to flip a VCA opening for processed audio or as a clock for a bitcrusher module to stutter/distort other voices.

### 2. Crazy Dubstep/Drum & Bass Basslines

**Patch Idea:** Use evolving and rhythmically complex gates to trigger envelope generators or sync bass synths for signature “wonky” basslines.

- Use **Euclid Trigger Out** to fire an **envelope** controlling a VCA or filter cutoff on a bass voice, making the bass hit only at Euclid's pattern pulses.
- Patch a fast, cycling **LFO** or envelope to **Steps CV**, so the bass rhythm shifts with each bar, creating unexpected syncopation as in DnB or dubstep.
- Assign a slow triangle or complex wave **LFO** to **Length CV**, modulating how long the sequence is for “gated” or “rolling” effects.
- **Offset CV** can be modulated with stepped random or S&H for “shuffle” and swing-like effects. Try this at audio rates for nasty, “buzzing” rhythms synced to the step sequence.
- Run the trigger through a slew or gate delay for ratcheted effects. Feed this into hard **wave distortion** or **FM** the bass oscillator for extra aggression.

### 3. Haunting Atmospheric Pads

**Patch Idea:** Use Euclid for subtle, evolving gating of shimmer or drone layers.

- Use slow clock divisions on **Trig Input** so outputs are spaced out.
- Modulate **Steps CV** gently with cyclic LFOs for pulses that “breathe”, perfect for pads.
- Use **Offset Knob** to slowly cycle which steps are active, making the pad seem to “wander” in space.
- Mult the **Trigger Out** to both VCA/VCF openings and reverb/delay feedback CV ins for evolving spatial depth.
- Use a **noise/random output** patched to **Length** for unpredictable pad “flickers”, or to make evolving, ghostly rhythmic textures.
- Try self-patching: send Euclid Output to modulate its own Offset (through an attenuator/VCA) for self-generating pattern evolution.
- For lushness, sequence reverb send/return or stereo field with multed Euclid outputs.

---

### Additional Tips

- Exploit the incredibly fast or slow clocking possibilities for granular or ambient glitches.
- For maximum chaos, try modulating all three CVs with unsynchronized, irregular LFOs or random sources.
- Combining Euclid with logic modules (AND, OR, XOR) and comparators can create generative or morphing rhythmic structures.
- Stack the Euclid output with triggers/gates from other sequencers for polymetric, cross-rhythmic effects.

---

**Further Reading:**
- [Official PDF Manual](https://2hp.com/docs/euclid.pdf)

**Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)**
