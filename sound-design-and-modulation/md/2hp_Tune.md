# 2hp — Tune

- [Manual PDF](../../manuals/Tune_Manual_2023.pdf)

---

[2hp Tune Manual (PDF)](https://twohp.com/modules/tune)

---

# Creative Modulation of 2hp Tune for Unique Eurorack Sounds

The **2hp Tune** is a compact and versatile voltage quantizer that turns any CV input into a scale-locked, clean pitch output—perfect for generating musically interesting lines and melodies. But with creative patching and modulation, it can also be teased into generating extreme, percussive, and textural sounds suitable for distorted percussion, crazy basslines, and haunting pads.

Below are example modulation strategies for each of those categories, leveraging the Tune module’s features:

---

## Distorted Percussive Sounds

### Key Patch Points:

- **Input (CV Signal)**
- **Bias CV Input**
- **Scale Knob & Scale LEDs**

### Techniques:

1. **Clip & Smash**:  
   Feed snappy, fast, envelope-generator CVs or triggers (with variable amplitude) into the **Input**. Use heavily-overdriven AD envelopes or complex random LFOs. The Tune will force these wild signals onto scale notes, creating “chopped” melodic rhythms.

2. **Scale Modulation for Unpredictability**:  
   Use an LFO or stepped random source into the **Bias CV Input**. As the Bias shifts, it re-maps which notes the quantizer outputs—the output will “glitch” from note to note, especially if the bias CV is rapidly modulated.

3. **Scale Selection for Flavors**:  
   Twist the **Scale Knob** or voltage-control it with a sequential switch for quick jumps between pentatonic, diminished, and chromatic scales. Chromatic will sound almost like a bit-crusher, while diminished/octatonic will get you angular, metallic percussive pings.

4. **Add Distortion:**  
   Send the quantized voltage into a simple analog VCO, then process through your favorite wavefolder or distortion module to get harsh kicks, snares, and metallic hits.  
   - **Tip**: Use the percussive envelope to open a VCA or LPG after the VCO.

---

## Crazy Basslines (Dubstep/Drum & Bass)

### Key Patch Points:

- **Input (Sequencer, Random CV, Envelope)**
- **Bias CV Input**
- **Scale Selection (Minor, Harmonic Minor, Diminished for dissonance)**

### Techniques:

1. **Wild Sequencing**:  
   Use a sequencer or stepped random generator for the **Input**. Set the scale to Minor or Diminished for darker, more aggressive lines. Turn up Bias and CV-modulate it to transpose basslines rhythmically or cause them to “jump” with accents.

2. **Glitchy Slides and Staircases**:  
   Mult a shape LFO (like a complex Saw/LFO combo) to both the Input and the Bias CV Input; detune their rates for "staircase" basslines, or feed a synced sample-and-hold for broken, unpredictable note stepping.

3. **Dual Layering**:  
   Patch **Output** to two VCOs—one clean, one distorted or FM’ed for higher harmonics. Apply envelope following or additional LFOs to VCO FM depth to intensify the “wobble” or grit.

4. **Sync with Drum Gates**:  
   Sync the CV input with your main rhythm gate generator so that the quantizer spits out new pitches on every drum hit, aligning bass stabs to your beat grid.

---

## Haunting Atmospheric Pads

### Key Patch Points:

- **Input (Slow LFOs, Slow Random CV Generators)**
- **Bias CV Input (Modulated by aftertouch, joystick, or more LFOs)**
- **Scales: Major Pentatonic, Egyptian Minor, Whole Tone for mysterious moods**

### Techniques:

1. **Undulating Motions:**  
   Feed a slow sine or triangle LFO into the **Input** for drifting arpeggio-like motion. Use a S&H random CV, smoothed slightly, for “wandering” melodies.

2. **Expressive Shifts**:  
   Route aftertouch, ribbon controller, or pedals to the **Bias CV Input**. Performers can then shift the base note of the quantized scale for expressive modal changes.

3. **Atmospheric Voicing:**  
   Output to a polyphonic VCO or a resonator module; layering multiple delayed/layered VCOs quantized by Tune creates complex, evolving pads.

4. **Magical Scale Choice:**  
   Switch between scales (Whole Tone, Egyptian Minor, Octatonic) for instantly unfamiliar, cinematic clusters. Automate (with switches or CV) the **Scale Knob** for shifting moods.

5. **Slow, Textural Modulation:**  
   Add stereo spread and reverb after your VCO. Send Bias CV extremely slowly with random modulations for ghostly, evolving tonalities.

---

**General Tips:**

- Remember: all modulation of Input and Bias should be unipolar (0V to +5V).
- The interplay of Input and Bias determines not only pitch, but "which" notes within the scale are available at any given time. This makes fast tampering with Bias especially fruitful for chaos.
- Using fast modulation sources or noisy voltages going through a fast-changing Bias generates glitchy, digital-sounding arpeggiations which can be harnessed for both percussion and fast melodic lines.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)