# Tiptop Audio — RS808

- [Manual PDF](../../manuals/Tiptop_Audio_RS808_ns.pdf)

---

[RS808 Manual PDF](https://tiptopaudio.com/808-2/)

---

# Creative Patching Ideas for the Tiptop Audio RS808

The Tiptop Audio RS808 is a specialized Eurorack adaptation of the legendary TR-808 Rimshot/Clavs generator. Beyond producing iconic percussive sounds, its modular format opens up a world of creative possibilities, especially when combined with other Eurorack modules. Below, I suggest some patching techniques and module pairings to unlock its full creative potential.

---

## 1. Modulate Snap and Pitch for Dynamic Percussion

**Patch Idea:**  
Connect an LFO (e.g., Mutable Instruments Tides or Make Noise Maths) to modulate the SNAP and PITCH CV inputs (use attenuators/mults as needed). With slow modulation, you can create dynamically evolving percussive timbres. Use a sequencer or S&H module for stepped changes, mimicking live drummer variations.

- **What you get:** Grooving, animated electronic rimshots and "clav" sounds that morph organically over time.
- **Bonus:** Sending an envelope from a sequencing module like Intellijel Metropolix for polyrhythmic pitch/snare accents.

---

## 2. Sequence Rimshot/Clavs with Accented Triggers

**Patch Idea:**  
Use a trigger sequencer (e.g., Euclidean Circles, Arturia Beatstep Pro, or Erica Synths Drum Sequencer) to send triggers to the GATE IN, and a separate sequence of triggers to ACCENT IN.

- **What you get:** Grooves with "feel"—only some rimshots are accented and louder/punchier. Great for techno/house vibes, fills, or adding “groove” to rigid sequences.

---

## 3. Layer and Pan for Stereo Image

**Patch Idea:**  
Layer the RS808 alongside other percussion modules (e.g., Hexinverter Mutant Rimshot, Accent) and send each to a stereo mixer (e.g., Befaco STMix). Pan the RS808 and other percussion for wide stereo beats.

- **What you get:** A lush, professional-sounding stereo field with distinct spatial placement. Accent or “Clavs” sound can punch through the mix.

---

## 4. Run Through FX and Filters

**Patch Idea:**  
Patch the RS OUT to a resonant filter (e.g., Mutable Instruments Ripples, WMD C4RBN) and then into a delay (e.g., Make Noise Mimeophon, Erica Synths Pico DSP) or a spring reverb (e.g., Doepfer A-199).

- **What you get:** Dub-style rimshots (filter sweeps, echo trails), psychedelic or textural percussion. Filtering "Clav" sounds creates zappy laser-shots, while delays turn clicks/snaps into glitchy artifacts.

---

## 5. Use the "Click" Mode as a Transient Generator

**Patch Idea:**  
Set the switches to Left down/Right up for the short “click” sound. Use it to trigger sidechain compression in a compressor sidechain module (e.g., WMD MSCL, Intellijel Jellysquasher), or layer atop kicks for a punchy attack.

- **What you get:** Clicky/transient "pop" perfect for drum layering, glue/compression sidechaining, or as a clock source in creative logic patches.

---

## 6. Rhythmic MIDI-to-CV Percussion

**Patch Idea:**  
Use a MIDI-to-CV interface (e.g., Yarns, Doepfer A-190, or Befaco MCFx) to trigger the RS808 from your DAW or hardware sequencer, aligning rimshots/clavs with your main patterns.

- **What you get:** Grooves locked with your MIDI ecosystem; live playability with pads or sequencing.

---

## 7. Generative “Broken Machine” Percussion

**Patch Idea:**  
Send irregular/randomized gates from modules like Pam’s NEW Workout, Turing Machine, or Stochastic Inspiration Generator to GATE IN and/or ACCENT IN.

- **What you get:** Experimental, ever-shifting rimshot and clav patterns for IDM, generative ambient, or glitch music.

---

## 8. Mix and Layer with Envelope Followers and VCAs

**Patch Idea:**  
Take the RS OUT through an envelope follower (e.g., Doepfer A-119) to extract dynamic CV control, then use to modulate other drum parameters, or patch through a VCA (such as Intellijel Quad VCA) for further dynamic shaping/automation.

- **What you get:** Dynamic interaction between percussion and other elements; evolving sound textures controlled by your rimshot's activity.

---

## 9. Cross-Modulation & Feedback

**Patch Idea:**  
Feedback possibility: Patch the output of RS808 through a distortion (e.g., Erica Synths Fusion VCF), route to a mixer, sum back into a modulation input (with attenuation for safety). Or try modulating SNAP/PITCH with an audio-rate oscillator for metallic FM rimshots.

- **What you get:** Gritty, overdriven, or metallic percussive textures impossible on a vanilla drum machine.

---

## 10. Live Performance FX via CV Control

**Patch Idea:**  
Assign performance controls (such as Faderbank/Planar2 or Pressure Points) to SNAP/PITCH in real time for interactive drum fills, stutters, or "scratching" of the rimshot sound.

- **What you get:** Humanized, interactive live drum playing beyond step sequencing.

---

*The RS808 is a percussive chameleon—combine its classic sound with the power of modular to create uniquely tailored electronic drum timbres for your patches.*

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
