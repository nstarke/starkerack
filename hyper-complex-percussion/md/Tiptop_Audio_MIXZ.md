# Tiptop Audio — MIXZ

- [Manual PDF](../../manuals/Tiptop_Audio_mixz.pdf)

---

[Download the Tiptop Audio MIXZ Manual PDF](https://tiptopaudio.com/manuals/MIXZ_Manual.pdf)

---

## Using the Tiptop Audio MIXZ for Hyper-Complex Percussive and Rhythmic Eurorack Patches

The Tiptop Audio MIXZ is a **low-noise, dual 4-channel mixer** with the unique Tiptop Bus Mix feature. While it's not a voice or effect itself, it’s an essential central hub for blending, layering, and creatively routing drum, percussion, and modulation signals in complex rhythmic setups. Here’s how you can harness the power of the MIXZ to generate **densely rhythmic, hyper-complex percussion music with advanced sequencing and time signatures.**

---

### 1. **Leverage the Bus Mix for Fast, Dense Layering**

- **Patchless Drum Mixes**: With the Bus Mix, bring *multiple drum modules* (all Tiptop drum modules and Tiptop ONE) into the mix without using patch cables, leaving your front panel open for complex routing and manipulation.
- **Selective Drum Inclusion**: Use the jumper on the back of each Tiptop drum module to select precisely which voices are part of the Bus Mix during a performance—combine or exclude modules mid-session for evolving textures.

---

### 2. **Dual Mixer Architecture for Polyrhythmic Parallelism**

- **Per-Channel Control**: Mixer A (ch1–4) has *individual gain knobs*. Use these to dynamically accent or attenuate different rhythmic layers, perfect for accentuating certain pulses or cross-rhythms.
- **Routing Tricks**: The output of Mixer A is **normalled into Mixer B**, letting you blend two groups of voices or effects—one could be polyrhythmic hats, the other kick and snare, for example.
    - *Pull* Mixer A’s output to use both mixers independently: process two complex rhythm groups in parallel.
    - *Leave* it connected for easy serial mixing and post-processing.

---

### 3. **Multilayered Polyrhythmic Patches**

- **Example Patch**:  
    - **Mixer A**: Sum fast-modulated drum voices or CV-controlled clocks (e.g., trigger fast polyrhythmic sequences—5 against 4, 3 against 7).
    - **Mixer B**: Blend slow, accent-heavy triggers or gate pulses, plus the overall output from the Bus Mix (shaker, rim, claps).
    - Send Mixer A or B outputs to separate envelope-followers, VCAs, or filters downstream for further rhythmic shaping.
- **Cross-Mix Rhythms**: Use mixers A and B for *real-time* switching between rhythmic “groups”; perfect for genre-bending breakbeats, IDM, or modular techno.

---

### 4. **Tips for Unique, Punchy, Percussive Sound**

- **High Headroom**: The MIXZ is optimized for *audio rate* and *CV/gate* signals—mix gates with audio, or blend multiple clicky percussive sources for high-impact transients.
- **Serial FX Routing**:  
    - Route the combined Mixer B output to delay/reverb/FX modules (like the Tiptop Z-DSP).
    - Take advantage of the excellent summing linearity for accurate, punchy transient stacking.
- **Dynamic Pattern Transformations**:  
    - Use mutes (by patching/unpatching) or level controls as instant fills/break triggers.
    - Patch LFOs or modulation sources to VCAs pre-MIXZ for complex amplitude/frequency entrainment.

---

### 5. **Advanced Rhythm & Patch Ideas**

- **Odd/Compound Meter Overlays**:  
    - Assign different time signatures to channels in Mixer A (e.g., 5-step and 7-step triggers), and Mixer B for more “even” meters or accents.
- **Gate and CV Summing**:  
    - Used as a CV mixer: Merge tempo-divided or Euklidean-triggers to generate truly non-repeating polyrhythms.
- **Spatial Processing with FX**:  
    - Mix all percussion through Mixer B, then send to stereo FX for huge, animated spaces; use modulation on FX parameters to keep textures shifting.

---

### 6. **Noise Notes**

- **Bus Mix Convenience vs. Panel Jack Quality**:  
    - Panel connections are quieter, so for most critical or exposed elements (kick drum, snare for punch), use Mixer A/B directly.
    - Reserve Bus Mix for layered hats, shakers, auxiliary percussion, or heavily processed sources.

---

### Quick Tips

- Only one MIXZ Bus Mix should be on per power row.
- Disable Bus Mix on rows using Doepfer CV/Gate bus, or keep Bus Mix off.
- For maximal density: experiment with all 8 input channels plus the Bus Mix; use as a live performance “mixer” for modular drum racks.
- Use subtle, controlled amounts of noise from Bus Mix-fed modules for gritty, lo-fi percussive layers.

---

With MIXZ as the rhythmic heart, you gain the flexibility to handle huge, intricate, polyrhythmic, and mutating percussion rigs. Let your modular shine as only Eurorack can—packed with detail and rhythmic complexity.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
