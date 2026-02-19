# Rebel Technology — Stoicheia

- [Manual PDF](../../manuals/Stoicheia – Rebel Technology.pdf)

---

[Stoicheia Manual PDF (Source: Rebeltech.org)](https://raw.github.com/pingdynasty/EuclideanSequencer/master/EuclideanSequencerManual.pdf)

---

# Creative Patch Ideas for the **Rebel Technology Stoicheia**  
*Dual Euclidean Sequencer for Eurorack*

The Stoicheia is a versatile rhythm generator based on Euclidean algorithms, which allows you to algorithmically create a rich variety of rhythmic sequences. Here are some creative ways to integrate the Stoicheia with other modules:

---

## 1. **Dual Rhythmic Layering for Polyrhythms**
Because Stoicheia provides two independently controllable Euclidean sequencers, patching each output to individual sound sources (e.g., two drum modules like [2hp Snare](https://2hp.com/products/snare) and [Tiptop Audio BD909](https://tiptopaudio.com/bd909/)) allows immediate polyrhythmic interplay.  
- **Tip:** Vary sequence lengths and fills to create evolving, interlocking patterns.  
- **Extra:** Use rotation to create syncopation and rhythmic displacement.

---

## 2. **Sequenced CV/Gate Modulation**
Use one sequence not for triggering audio but to modulate the behavior of another module.  
- Patch output to the gate/trigger of an LFO reset, a sample & hold, or a slew limiter like [Doepfer A-171-2](https://www.doepfer.de/a1712.htm).
- Create Euclidean-based filter modulations by triggering envelope generators (Intellijel Quadra, ALM Pip Slope, etc.) to modulate a filter cutoff.

---

## 3. **Melodic Sequencing with Quantizers**
Feed Stoicheia’s rhythm into a quantizer (e.g., [Intellijel Scales](https://intellijel.com/shop/eurorack/scales/)) for melodic/random note sequences.  
- Pair sequence output with a random voltage source ([Mutable Instruments Tides](https://mutable-instruments.net/modules/tides/) in random mode, [Wogglebug](https://makenoisemusic.com/modules/wogglebug)) for generative melodies, only allowing notes through on certain Euclidean triggers.

---

## 4. **Rhythmic CV Routing via Sequential Switch**
Send Stoicheia triggers into the clock input of a sequential switch (e.g., [Doepfer A-151](https://www.doepfer.de/a151.htm)), for regularly or irregularly stepping through multiple pitch or timbre sources.  
- Result: Changing textures or instrument focus based on rhythmic patterns.

---

## 5. **Cross-Modulation and Self-Referencing Patches**
Patch one sequence output to the reset input of the other, or use alternating reset signals (from the [Pamela's New Workout](https://busycircuits.com/alm017/) or similar) for complex, evolving patterns.

---

## 6. **Conditional/Probability Rhythms**
Insert logic or probability modules (e.g., [Mutable Instruments Branches](https://mutable-instruments.net/modules/branches/), [Doepfer A-166 Dual Logic]) after one or both Stoicheia outputs:
- **Branches:** Get “occasional” triggers for ghost notes or fills.
- **Logic:** Use “AND”/“OR” to combine Euclidean rhythms for hybrid patterns.

---

## 7. **Chained/Complex Song Part Sequencing**
Use Stoicheia’s chained mode to build longer or multi-part song patterns—send chained outputs to a drum module with multiple voices (e.g., [Endorphines BLCK_NOIR](https://www.endorphin.es/modules/blck-noir)).
- **Pro tip:** Alternate between chain mode and normal mode using manual or voltage-controlled switching for even more dynamic structures.

---

## 8. **Live Performance Parameter Morphing**
Use external CV sources (e.g., [Mutable Instruments Stages](https://mutable-instruments.net/modules/stages/), [Intellijel Planar2](https://intellijel.com/shop/eurorack/planar-2/)) to modulate Stoicheia’s length, fills, or rotation parameters in real time during a performance.

---

## 9. **Clock Division/Multiplication: Groovy Clocks**
Send Euclidean outputs to trigger clock dividers/multipliers ([4ms RCD/RCM](https://4mscompany.com/products.php?cat=rcd), [Doepfer A-160-2](https://www.doepfer.de/a1602.htm)), then clock other sequencers for rhythmic grooves that evolve with your Stoicheia patterns.

---

## 10. **Synchronizing Lighting or Visuals**
If you’re integrating audiovisual elements, Stoicheia outputs can be used to trigger synchronized events in Eurorack video synthesis ([LZX Industries](https://www.lzxindustries.net/) modules) or DMX lighting converters for stage shows.

---

## 11. **Triggering Sample Players with Evolving Grooves**
Run Stoicheia outputs (direct or logic-combined) into a sample player ([1010music Bitbox](https://1010music.com/product/bitbox), [Make Noise Morphagene](https://makenoisemusic.com/modules/morphagene)) for intricate, generative percussion or glitch textures.

---

## General Patch Tips:
- **Rotate and modulate for interest:** Modulating “rotation” opens up morphing, always-evolving beats.
- **Sequence drum fills:** Use short, high-fill sequences alongside longer, sparser patterns for organic drum fills.
- **Microtiming:** Patch a pulse-width–modulated LFO as the input clock for off-grid (“swinged”) rhythms.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)