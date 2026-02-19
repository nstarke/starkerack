# Bastl Instruments — Dark Matter

- [Manual PDF](../../manuals/manual-dark-matter.pdf)

---

[**Dark Matter Manual PDF**](https://bastl-instruments.com/files/dark-matter-manual.pdf)

---

## Using Bastl Dark Matter for Densely Rhythmic, Hyper-Complex Percussion

**Module Type:**  
Dark Matter is primarily a feedback processor and effects unit—not a traditional voice, but an extreme tool for mangling, energizing, and rhythmically warping eurorack signals, especially percussion.

### 1. **Rhythmic Feedback Looping**
Dark Matter’s central feature is its analog feedback network—make percussion signals (either from drum modules or external sources) loop through it. Feedback networks, when modulated, introduce shifting rhythms, resonances and artifact bursts that add wild rhythmic complexity.

#### **Techniques:**

- **Feedback X-Fade:**  
  Use the **X-Fade** control and CV input to rhythmically crossfade between clean and feedback-processed signals. Sequence or modulate the X-Fade CV with intricate polyrhythmic LFOs or clocked random voltages.

- **FBK (Feedback) CV:**  
  Modulate the **FBK CV** with complex gates, clock divisions, or a euclidean/polyrhythmic modulator, making the amount of feedback pulse and shift with your own odd-metered patterns.

### 2. **Percussive Distortion & Clipping**
The **Drive** circuit can push anything into saturated, punchy transients. The **Dynamics** section—essentially a fast envelope follower with decay switch—is perfect for accentuating transient percussion character.

#### **Tips:**
- Patch percussion audio to **INPUT** and modulate **Drive CV** & **Dynamics** with different polyrhythmic envelopes or sequenced gates.  
- Use the **Hyper Drive** switch to force hard clipping or “snap” to make your percussion ultra-punchy.

### 3. **Tone Shaping for Clarity**
Use **Bass** and **Treble** EQ—animate these with CV from rhythmic LFOs or clocks so your drums shift tonally in complex time, ensuring clarity amidst distortion.

### 4. **Dynamic Decay & Rhythmic Gating**
The **Dynamics** decay switch (short/long) and CV input allow you to rhythmically gate and “choke” the feedback or process in syncopated, twisted patterns.  
- Patch rhythmic CV or triggers from clock dividers or polyrhythmic trigger generators to the **Dynamics CV**.

### 5. **External Feedback Loops for Meta-Rhythms**
Populate the **EXT FBK** send and return path with external processing (FX, filters, other drum modules!) and modulate its return, opening up additional rhythmic layers and feedback “echoes” in unusual time signatures.

### 6. **Patch Examples (from Manual):**

#### **MO: Deep Modulation**
- Patch percussive audio into the **input**.
- Use sequencer clocks/gates at different divisions to modulate **Tone**, **X-Fade**, and **FBK CV**.
- Pass the **output** through fast VCA for additional rhythmic gating.

#### **Loops: Weird Echo**
- Patch percussion into the **input**. Return output through delay/echo in the **EXT FBK** loop.
- Modulate **FBK** and **X-Fade** with out-of-phase LFOs or trigger patterns.
- Use non-integral clock divisions (e.g., 5/8, 7/16) to inject complex time feel.

### 7. **Advanced: Polymetric Feedback Chopping**
- Use odd/even clock/mults to trigger Dynamics CV.
- Crossfade between processed/clean with unrelated clocks for evolving meter.
- Insert a VCO or resonant filter in EXT FBK as a frequency-specific, rhythmically modulating feedback path.

### 8. **Additional Sound Design Tips**
- The **Polarity** switch can flip the phase of feedback, often creating percussive “flams” and ghost hits.
- Use **SHORT decay** for glitchy, fast-moving articulations and **LONG** for drawn-out feedback “snares” or hats.
- Sequence both EQ parameters (“Bass” and “Treble Boost”) for acid-like morphs across single hits.

---

#### **Summary Table**

| Parameter         | Patch/Modulation Ideas                                                            |
|-------------------|-----------------------------------------------------------------------------------|
| DRIVE/DYNAMICS    | Trigger/gate from polyrhythmic clocks and envelopes                               |
| X-FADE            | Crossfade between clean/feedback on a separate meter                              |
| FBK/FBK CV        | Modulate with complex LFOs or logic-processed gate patterns                        |
| EXT FBK           | Insert delays/reverbs, modulate return CV for multi-timed echoes                  |
| BASS/TREBLE BOOST | CV from slow/fast LFO in a non-standard ratio to drum BPM                         |

---

### **Pro Tips**
- Use Dark Matter as both an insert FX and send/return network for drums.
- Try using envelope followers (from drums or even unrelated sources!) as CV for more organic, audio-reactive percussive modulation.
- Build “meta-rhythms” by clocking everything from different sources/ratios.

---

## [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---

*(All patch suggestions and explanations are directly informed by the Bastl Dark Matter manual and optimized for advanced eurorack percussion patching!)*