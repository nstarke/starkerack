# Bastl Instruments — Dark Matter

- [Manual PDF](../../manuals/manual-dark-matter.pdf)

---

[**Bastl Instruments Dark Matter Manual (PDF)**](https://bastl-instruments.com/content/manuals/DarkMatterManual.pdf)

---

# Sound Design with Bastl Dark Matter: Feedback Observatory

The **Bastl Dark Matter** is a feedback-based voltage-controlled audio processor and distortion unit for Eurorack, known for producing wild, self-oscillating timbres, gritty distortion, and dynamic feedback textures. Below is a focused analysis for achieving **distorted percussive sounds**, **crushing basslines**, and **haunting pad textures** using modulations and features outlined in your manual scans.

---

## 1. Distorted Percussive Sounds

### Key Sections to Use
- **Drive** section for clipping and saturation
- **Dynamics** section for envelope following and transient shaping
- **Feedback (FBK) and Tone** for chaotic or saturated harmonics
- **X-Fade** for rhythmical crossfading

### Patch Suggestion
1. **Input**: Send drum triggers or sharp envelopes (from sequencer or trigger source) into the **INPUT** jack.
2. **Drive Setting**:  
   - Crank up **DRIVE** for hard clipping.
   - Use the **HYPERDRIVE** switch for extra saturation.
   - Adjust **DRIVE CV** with a fast/steep envelope for punchy attacks.
3. **Dynamics**:  
   - Engage **DYNAMICS** envelope follower for amplitude-reactive effects—great for emphasizing percussion transients.
   - Route **DYNAMICS OUTPUT** to modulate **FBK CV** or **TONE CV** for evolving attack/release filtering and feedback.
4. **Feedback**:
   - Slowly increase **FBK**. Feedback instability introduces raw, broken textures.  
   - Patch **FBK OUT** to external FX (reverb or delay), then back to **FBK IN** for metallic/echoed hits.
5. **Tone**:
   - Use the **TONE CV** input for envelope or sequencer modulation.
   - Emphasize mid/high frequencies for snappy percussion.
6. **X-Fade**:
   - Use an external CV (e.g., clocked random or trigger sequencer) to alternate between **DRIVE** and **FBK** paths for glitchy, percussive gating.

---

## 2. Dubstep/Drum & Bass Basslines

### Key Sections to Use
- **Drive, Dynamics, Tone, Feedback**, and **CV modulation everywhere**

### Patch Suggestion
1. **Input**: Patch a saw or square bass VCO into the **INPUT**.
2. **Drive**:
   - Engage **DRIVE** past saturation for heavy grit.
   - Modulate **DRIVE CV** with an envelope synced to your bassline for rhythmic accents.
3. **Tone**:
   - Patch a synced LFO to **TONE CV** for evolving vowel or formant sweeps.
   - Use the **BASS** and **TREBLE** boost for sculpting the sub and high-end.
4. **Feedback**:
   - Raise **FBK** amount to dial in wild resonance/growl.
   - Modulate **FBK CV** with sequencer steps, random CV, or audio-rate sources for “talking” basslines.
5. **Dynamics**:
   - Enable the envelope follower; use its output to modulate **DRIVE** or **TONE** for basslines that change character depending on their own amplitude.
6. **X-Fade**:
   - Fade between **DRIVE** (cleaner) and **FBK** (nastier) using a sequenced or free-running LFO.

**Expert Tip:**  
Insert an external distortion or filter between **FBK OUT** and **FBK IN** for truly unpredictable, filthy results.

---

## 3. Haunting Atmospheric Pad Sounds

### Key Sections to Use
- **Tone** for bandpass-like shaping
- **Slow, moving modulation of FBK/Tone**
- **X-Fade** for subtle textural morphs

### Patch Suggestion
1. **Input**: Use a pad sound (rich waveform, slow attack) from your synth/oscillator.
2. **Drive**:
   - Keep **DRIVE** moderate for warmth; avoid hard clipping unless you want grit.
   - Use slow, shallow LFOs on **DRIVE CV** for gentle drift.
3. **Tone**:
   - Add subtle EQ via **BASS** and **TREBLE** boost as needed.
   - Modulate **TONE CV** with a slow, cycling LFO or an attenuated random source.
4. **Feedback**:
   - Set **FBK** just before oscillation for haunting feedback wisps.
   - Modulate **FBK CV** with a very slow S&H or unipolar LFO for evolving atmospheres.
5. **Dynamics**:
   - Engage envelope follower if you want the pad to react dynamically to your playing.
   - Patch **DYNAMICS OUTPUT** to **TONE** or **FBK** for amplitude-sensitive evolving movement.
6. **X-Fade**:
   - Slowly modulate crossfade with a wide, slow LFO to morph subtly between clean and processed signals.
7. **External Feedback**:
   - Try routing **FBK OUT** through reverb/fx before returning to **FBK IN** for endless, ghostly atmospheres.

---

## General Modulation Suggestions

- **Sequencer CV > FBK or TONE CV**: Rhythmic morphs and timbral variation.
- **Random CV > FBK / X-FADE**: Evolving chaos, especially effective on pads or basses.
- **Audio-rate mod > FBK or TONE**: Extreme FM, vocal-like or broken digital timbres.
- **Envelope Follower**: Use dynamic output to self-modulate for organic, responsive sounds.

---

#### Explore these patching techniques with your **Bastl Dark Matter** and discover unique, evolving, and sometimes uncontrollable textures!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)