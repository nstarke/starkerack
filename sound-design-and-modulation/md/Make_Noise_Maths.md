# Make Noise — Maths

- [Manual PDF](../../manuals/MATHSmanual2013.pdf)

---

[**Download Original Make Noise Maths Manual (PDF)**](https://makenoisemusic.com/content/manuals/maths_manual2013.pdf)

---

# Modulating the Make Noise Maths for Wild & Unique Sounds

The Make Noise Maths is a formidable Eurorack module for sculpting CV, envelopes, LFOs, and more. Here's how you can modulate it to generate distorted percussion, gnarly basslines, and atmospheric pads, inspired by genres like dubstep, DnB, and experimental soundscapes.

## 1. DISTORTED PERCUSSIVE SOUNDS

### **Concepts & Strategies**

- Use Maths as a complex function generator for non-traditional envelopes.
- Take advantage of the variable response (logarithmic → linear → exponential) for punchy or snappy shapes.
- Self-patch for chaos & asymmetry.
- Overdrive via summing with large offsets for harsh, clipped envelopes.

### **Patch Ideas**

#### **a. Kick Drum with Distortion**
1. **CH 1 or 4 = Envelope Generator**  
   - Set Rise = short (counterclockwise for instant attack).  
   - Set Fall = short or moderate for a snappy decay.
2. **Response**: Start in exponential for punch; tweak for more unusual tails.
3. **Distortion/Overdrive**:  
   - Set CH 2 and/or CH 3 to high positive offset.
   - Patch SUM out as the envelope shape.  
   - The over-volted offset will clip downstream VCAs or even the audio path for distortion.
4. **Feedback**: Patch INV SUM back into Rise/Fall CV for further shaping or chaos.
5. **Envelope to VCA**: Patch Signal OUT to open a VCA for your kick drum oscillator.

#### **b. Metallic Percussion**
- Engage CYCLE on CH 1 or 4 for audio-rate oscillation.
- Use EOR/EOC outputs to clock or trigger other envelopes or kick modulations.
- Mix envelopes using SUM or OR outputs for complex, sharp transients with interesting overtones.


## 2. DUBSTEP/DRUM&BASS BASSLINES

### **Concepts & Strategies**

- Maths can be a mod source for crazy wobbles or even act as an audio oscillator at fast cycle settings.
- Use variable response for evolving filter or amplitude movements.
- Use envelope self-modulation and cross-patching for variable movement.
- Create step, glide, or ‘robotic’ movement using BOTH CV input and offset channels.

### **Patch Ideas**

#### **a. Wobble LFO**
1. **CH 1 = LFO**:
   - Engage Cycle, set Rise/Fall for desired rate.
   - Use exponential for sharp LFO, log for slow ramping.
2. **Voltage-Controlled Speed**:
   - Patch an attenuated audio signal (from CH 2/3 or elsewhere) into BOTH CV for rate modulation (FM).
   - Slow manual sweeps, or high frequency for FM “growl.”
3. **Output**:
   - Send Unity OUT or Variable OUT to VCF cutoff or oscillator FM for classic wubs or vocalic formants.
   - Self-modulation: Patch EOR/EOC OUT to trigger further envelopes or cycle inputs for rhythmic accents.

#### **b. Bass Envelope Distortion**
- Patch envelope (from CH 1/4) into VCA, controlling an audio-rate oscillator.
- Use OR/SUM output for aggressive shapes.
- Add CH 2 offset for high amplitude/overdrive.
- Invert envelope at INV SUM for reverse movement.

#### **c. Cross-Mod Wobbles**
- Use CH 1 and CH 4 as dueling cycling envelopes.
- Patch EOC from CH 4 into CH 1 Trigger; EOR from CH 1 into CH 4 Cycle input.
- Attenuvert the outputs and mix; send results to filter/oscillator for wobble sequences with ever-changing rhythms.


## 3. HAUNTING ATMOSPHERIC PAD SOUNDS

### **Concepts & Strategies**

- Take advantage of super-slow cycles (25min!) for drifting modulations.
- Use intertwined envelopes/LFOs for subtle, organic pad movement.
- Employ LOG/EXPO responses for non-linear, living morphs.

### **Patch Ideas**

#### **a. Generative Slow Modulation**
1. Set CH 1 and CH 4 to Cycle.
2. Set Rise and Fall to near max; response near log for extra slow, organic change.
3. Mix outputs (SUM or OR) to modulate a VCF, wavetable position, or oscillator FM index for cloudy, evolving timbres.

#### **b. Chaotic Morphing Pads**
- Use the “Arcade Trill” or “Chaotic Trill” patches (manual pg. 21).
- Cross-modulate with incoming audio-level or offset voltages for unpredictable drifting.
- Modulate BOTH CV (exponential global speed) with a fluctuating, irregular source (field recording, noise).

#### **c. Layered Modulation**
- Use CH 2 and CH 3 for freely offset control voltages (slow LFO/rising/falling with no input creates ramps).
- Sum with primary envelopes for broader, multi-dimensional moves in filter, VCA, or FX.


---

### **PRO TIPS FOR MODULATION MAYHEM**
- Use **Variable Outputs** and the **Attenuverter** controls to invert/attenuate CV sent to destinations.
- Patch **EOR/EOC** outputs to trigger envelopes or clocks in rhythmically interlinked patterns.
- For extreme percussive chaos, feed inverter outputs (INV SUM OUT) back into the module's CV inputs.
- Use **OR OUT** to get rectified (positive-only) signals for CV-ing modules that dislike negative voltages.
- Always experiment with external audio-rate CV sources into BOTH input for crazy FM and distortion tricks.

---

> For all patch diagrams, advanced modulation techniques, and official info, download the full [Make Noise Maths Manual (PDF)](https://makenoisemusic.com/content/manuals/maths_manual2013.pdf).

<br>

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)