# Tiptop Audio — SD808

- [Manual PDF](../../manuals/Tiptop_Audio_SD808_ns.pdf)

---

[SD808 Manual PDF](https://tiptopaudio.com/manuals/808/SD808-User-Manual.pdf)

---

# Creative SD808 Patching for Unique Eurorack Sounds  
*Tips for Distortion, Bass, and Atmospheric Pads*

The Tiptop Audio SD808 is a specialized snare drum module but, like many Eurorack modules, it's capable of far more than its original function if you experiment! Here’s how you can push the SD808 into new sonic territory—distorted percussion, killer basslines, and even evolving ambient atmospheres.


## 1. **Distorted Percussive Sounds**

**Harnessing Internal Gain Stages**
- Dial the LEVEL knob to maximum and set ACCENT to max as well. This drives the output to up to 20Vp.p, well past line level—perfect for intentional overdrive/distortion.
- Turn SNAPPY to at least 50%; this ensures lots of noise and attack for a saturated, crunchy snare.
- Run the SD OUT into other Eurorack modules with additional overdrive, wavefolding, or bitcrushing—such as distortion pedals or in-rack processors (e.g., the Bastl Waver, Intellijel Bifold, or Tiptop’s own Z-DSP with Bat Filter as recommended in the manual).

**CV Modulation for Aggressive Movement**
- Use a fast LFO or envelope generator patched to the ACCENT IN or modulate LEVEL with a VCA to bring the perceived output gain and distortion in and out rhythmically.
- Tap the SD808 output, split it, and feed one channel back into a modulation source (like a comparator or envelope follower) to create a self-modulating feedback distortion loop.


## 2. **Crazy Basslines (Dubstep/DnB) Techniques**

Though it’s a snare, the SD808 uses T-Network sine waves—these can be abused for bass!

**Patching Tips:**
- TONE full CCW selects only the lower frequency sine wave—useful for deeper kicks and bass.
- Patch a gate sequencer or fast clock into GATE IN to "play" the SD808 at audio rates; rapid triggering will turn it into a pitched drone or bass "note."
- Mult the same gate or a separate sequencer into ACCENT IN for wild amplitude/frequency shifts.
- **External Pitch Processing:** Route SD OUT through a filter with 1V/Oct tracking (like the Doepfer A-124 Wasp) and a VCA. Modulate the cutoff with another sequencer or random voltage for wobbly, growling basslines.
- Heavy distortion post-processing can push the output into the saturated, tearing range of neuro or dubstep bass.

**Bonus:**
- Use a fast decay envelope on the SNAPPY control via voltage-controlled switching (e.g., with a VCS or Maths through a vactrol) to sync the noise snap tightly with a blasting sub-bass.


## 3. **Haunting Atmospheric Pad Sounds**

While the SD808 is designed for percussion, the combination of analog noise and sine oscillators gives textural potential:

**Texturing Approaches:**
- Trigger SD808 less percussively—slow gates or envelopes (e.g., from a quadrature LFO or stepped random via Turing Machine). Allow long decays for each hit to ring out.
- Use LEVEL and ACCENT at low-mid settings for a more subtle timbral palette.
- TONE set mid-way for a balance of high and low sine content—great for drone layering.

**Modulating for Texture**
- Snappy (noise content) is key: Patch a slow LFO or random (Wogglebug, S&H, etc) to the SNAPPY knob via an external DC offset + VCA chain for evolving timbres.
- Send the SD OUT through lush effects chains—reverb, long delays, or granular modules (Mutable Clouds, Qu-Bit Nebulae) to spread short hits into evolving washes.
- Modulate TONE with fluctuating voltages to sweeps sine highs and lows through your ambience.

**Layering**
- Stack several SD808 hits at staggered times using a sequencer with probability or burst (MI Marbles, etc).
- Use ring modulators to blend SD808 outputs with other melodic or chordal patches for metallic, eerie overtones.

---

### **Summary Table**

| Goal                        | SD808 Settings/Mod Patching     | External Patching Ideas                  |
|-----------------------------|----------------------------------|------------------------------------------|
| Distorted Percussion        | LEVEL & ACCENT maxed, SNAPPY 50%+ | Run thru wavefolder, bitcrusher, distortion  |
| Crazy Basslines             | TONE CCW, fast gates to GATE IN & ACCENT IN | Post-filter, modulated cutoff, heavy distortion |
| Atmospheric Pads            | LEVEL/ACCENT lower, TONE/SNAPPY modulated   | Post through reverb, granular, ring mod, delay |

*Remember, you can also adjust the module’s internal noise level with the trimmer for even more variety!*

---

Explore, patch widely, and experiment!  
Let the SD808 become much more than a snare—turn it into a mutating analog voice for your modular system.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)