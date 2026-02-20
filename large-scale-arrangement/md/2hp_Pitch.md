# 2hp — Pitch

- [Manual PDF](../../manuals/2hp_Pitch.pdf)

---

[2hp Pitch Manual (PDF)](https://2hp.com/wp-content/uploads/2022/12/Pitch-User-Manual.pdf)

---

# Using 2hp Pitch to Create Full-Length Songs in Eurorack

Turning great modular riffs, beats, and sequences into cohesive, evolving songs is a common challenge in Eurorack. The **2hp Pitch** module, with its real-time pitch shifting, Wow & Flutter (W&F), and CV-controllable blending, is a powerful tool for composition and arrangement when paired with other modules. Here’s how you can leverage its features to sculpt full-length tracks:

---

## 1. **Thematic Variation and Motif Development**

**Pitch shifting** is an essential musical tool for creating variations on a theme. By using the Pitch module’s **1V/Oct input** and **Pitch knob**, you can transpose melodies, basslines, or rhythmic elements up and down, generating verse/chorus/bridge changes or "call and response" sections. 

- **Automate pitch changes** with sequencers or CV sources to move between song sections.
- Use **W&F** to introduce tape-like character in breakdowns, intros, or outros for lo-fi emotional impact.

### Practical Patch
- **Bass progression**: Sequence a bassline into Pitch, automate pitch via 1V/Oct to create rising chorus sections or lowering breakdowns.
- **Lead voice morph**: Send a melody through Pitch, use a CV sequencer for interval jumps between sections.

---

## 2. **Song Section Transitions**

**Transitions** are crucial for moving smoothly from one song section to another (e.g., verse → chorus, build-up → drop). 
- **Animate W&F**: Use the W&F CV input to gradually increase wow & flutter for a tape-stop or lo-fi transition sound before the drop.
- **Blending Wet/Dry (Mix)**: Morph between the original ("dry") and pitch-shifted ("wet") signal using the Mix knob or CV for dramatic transitions.

### Practical Patch
- **Automated build-up**: Use an envelope or LFO to modulate Mix/fx amount near the end of a bar, shifting the pitch and adding W&F to announce a new song section.

---

## 3. **Harmonic Layering and Counterpoint**

With modular, you’re often limited by the number of oscillators/voices. The Pitch module can “clone” voices at different intervals, thickening the arrangement or creating harmonies.
- **Parallel harmonies**: Take a mono melody or riff, split it, and use Pitch to shift one voice (e.g., a 5th or octave up).
- Use with **loopers/samplers**: Record a motif to a looper (e.g., 2hp Loop), then route through Pitch with varying intervals for simple live reharmonization and chord progressions.

### Practical Patch
- **VCO doubling**: Patch a VCO to both its normal output and the Pitch module, shift one up an octave, mix both in a VCA/mixer for fattened leads or basslines.

---

## 4. **Sound Design for Dynamic Structure**

The **Wow & Flutter** effect recreates analog tape instability, which can be used creatively for signature breakdowns, intros, or textural motion within a song.
- Use W&F as an "audio spotlight" for certain sections.
- Modulate with slow CV for evolving instability, or trigger abrupt bursts with envelopes/gates for fills/glitch moments.

---

## 5. **Song Arrangement with CV Automation**

The 2hp Pitch's **CV inputs** for Pitch, Mix, and W&F let you automate much of its behavior with sequencers, random sources, or performance controllers. This turns static loops or motifs into dynamically morphing parts—essential for full songs.

### Suggestions:
- **Performance macros**: Use voltage presets to instantly change Pitch/Mix/W&F during a live set, emulating classic "scene" changes.
- **Rhythmic effects**: Modulate Pitch in sync with tempo for triggered pitch drops or rises like those in modern electronic music.

---

## 6. **Creative Use Cases for Song Structure**

- **Verse/Chorus Switch**: Route melodic/rhythmic content through Pitch with different settings for verse and chorus sections.
- **Lo-fi Section**: Automate W&F and lower the pitch for a retro breakdown.
- **Glitch/Fill Generator**: Burst modulate W&F or Pitch for quick fills before transitions.
- **Sample Deconstruction**: Route drums, vocals, or samples through Pitch (especially paired with 2hp Play) to create new song sections from the same source.

---

## **Conclusion**

The 2hp Pitch enhances any Eurorack system’s arrangement, structure, and storytelling potential. Pair it with sequencers, loopers, drums, and other effects for nuanced control over song development, transitions, and motifs—transforming simple patches into full-length, evolving music pieces.

---

*Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)*