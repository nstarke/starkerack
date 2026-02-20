# Noise Engineering — Terci Ruina

- [Manual PDF](../../manuals/Terci Ruina - Noise Engineering Documentation.pdf)

---

[**Terci Ruina Manual PDF**](https://manuals.noiseengineering.us/tr/)

---

# Using Terci Ruina for Full-Length Songs in Your Eurorack

The Terci Ruina by Noise Engineering is a triple analog distortion module, uniquely chaining three classic distortion circuits in series (or patched separately) for intense, customizable sonic destruction. While distortion is often associated with spice, grit, or texture, in the context of full-length modular compositions, Terci Ruina can be a powerful tool for sculpting dynamic song structures, buildup and release, transitions, and emotional impact.

Below are ways to incorporate Terci Ruina as a _songwriting device_ rather than just as a 'static' sound enhancer, along with techniques and patch strategies in combination with other modules.

---

## 1. **Macro Dynamics & Transitions**

- **Automated Distortion Amounts**  
  Use voltage-controlled attenuators (VCAs) or a sequencer with mutes (like Mutable Instruments Frames, or Doepfer A-138n) to fade Terci Ruina in and out of the signal path at key moments—introducing grit for choruses, breakdowns, or builds.
- **Scene-Based Processing**  
  By creatively patching into different In/Out points, you can re-order, bypass, or parallel process the distortions for each "section" of your song:  
  - Verse: Subtle saturation (e.g., only FB or FZ)
  - Chorus: Full signal chain (FB > FF > FZ)
  - Bridge: Only FF with extreme settings for special flavor

---

## 2. **Multitrack Processing (Parallel Use for Structure)**

- **Use Terci Ruina on Different Sound Sources for Sectional Contrast:**  
  - Feed your drum bus through all three stages for explosive drops.
  - Process only the bass line or melody in a verse to create a restrained sound; automate which voice receives distortion as the song builds. 
  - Hit vocals or samples through just one stage (e.g. FZ for fuzz) in breakdowns.
- **Splitting Drums**  
  Send kick and snare through FB and the rest of the drums through FF+FZ, recombine for a dynamic drum "kit" that morphs across the track.

---

## 3. **Morphing Sounds Over Time**

- **Manual or CV-Controlled Knob Sweeps**  
  Assign the knobs (FB, FF, FZ) to CV controllers or hands-on performance, morphing between clean and destroyed states to mark intros, climaxes, and outros.
- **Envelope or LFO Modulation**  
  Patch an LFO, envelope, or random voltage to one or more distortion drive controls. Increasing intensity creates tension for transitions; releasing back to cleaner tones offers relief and resolution.

---

## 4. **Creative Performance Tool**

- **Live Improvisation**  
  Use mute switches or sequential switches to suddenly "punch in" the Terci Ruina on melodic, percussive, or harmonic elements.
- **DJ-Style Drops and Effects**  
  Before a big drop, route the whole mix or group through Terci Ruina, max the distortion, then suddenly kill the effect for impact.

---

## 5. **Contrast with Clean Elements**

- **A/B Processing for Arrangement**  
  Duplicate a melodic or drum line with a buffered multiple; run one copy clean and one through Terci Ruina, crossfade between them with VCAs or a matrix mixer (such as Happy Nerding PanMix Jr.).
  - Use this to keep verses smooth and choruses gritty, making it easy for listeners to distinguish the song's structure.

---

## 6. **Post-Distortion FX for Clean/Dirty Interplay**

- **Filtering After Distortion**  
  After Terci Ruina, use a filter (patch idea: Endorphins Squawk Dirty to Me, Make Noise QPAS) controlled by envelopes or performance knobs for sweeping tonal movement—think acid bass for climaxes or muffled breakdowns.
- **Enveloping the Output**  
  Route Terci Ruina's output through a VCA controlled by a slow macro envelope—for dramatic "fade-ins" or "fade-outs" of intensity during a track.

---

## 7. **Thematic & Textural Cohesion**

- **Signature Sound**  
  Terci Ruina can become a "sonic glue" for your tracks—running common elements (hats, leads, FX) through it across your song can give tracks their own identity.
- **Noise, Chaos, and Happy Accidents**  
  Use radio interference or its unpredictable character intentionally in breakdowns, intros, or outros for lo-fi or experimental genres.

---

### Example Patch Flow for Full-Length Song Dynamics

| Song Section | Instrument(s)     | Terci Ruina Stage(s)          | Post-EFx           | Notes                                          |
|--------------|-------------------|-------------------------------|--------------------|------------------------------------------------|
| Intro        | Pads, Noise       | None or just FZ               | Filter + Delay     | Soft, clean textures                            |
| Verse        | Bass, Drums       | FB (medium), rest bypassed    | None               | Add subtle edge                                 |
| Pre-Chorus   | Melody, FX        | FB > FF                       | VCA (envelope)     | Tension, bit more distortion                    |
| Chorus       | Whole mix/group   | FB > FF > FZ (full)           | Filter open        | Maximum energy, wide spectrum                   |
| Bridge       | Percussion        | FZ only (high), radio noise   | Reverb             | Textural, experimental, unexpected moments      |
| Breakdown    | Vocals, FX        | FF high, others low           | Lowpass filter     | Muted, grimy breakdown sound                    |
| Outro        | Anything          | Manual knob sweep             | Fade out           | Dynamic release, evolving texture               |

---

## **Final Tips**

- Treat **Terci Ruina as a performance instrument**: Wiggling knobs or repatching stages live during a track can go a long way to keep listeners engaged.
- Reverb, delay, and modulation FX after Terci Ruina can help sculpt the tails and glue distorted parts into the mix.
- **Contrast and movement** are your friends: Use clean and dirty moments to your advantage for emotional impact and structural clarity.
- Remember: Noise and chaos are part of its charm; embrace unpredictability for unique musical moments.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)