# Tiptop Audio — MODFX FSU

- [Manual PDF](../../manuals/Tiptop_Audio_fx_manual_MODFX_FSU.pdf)

---

[Download the Tiptop Audio ModFx/FSU Manual (PDF)](https://tiptopaudio.com/manuals/FSU_MODfx_Manual_web.pdf)

---

# Creative Modulation Techniques with Tiptop Audio MODFX + FSU

These Tiptop Audio Eurorack modules are stereo multi-effect processors that shine with creative CV/gate modulation, both in sound design and live performance settings. Their flexible CV inputs allow for extensive control over effect parameters, making them ideal for wild, distorted percussion, gritty basslines, and evolving, cinematic textures.

## General Modulation Strategies

### 1. **Percussive Modulation**
- Use step sequencer gates or envelopes on the CV inputs to "strike" effect parameters at drum hit moments.
- For distortion/glitch effects, trigger the FSU's **Drive/Depth** or **Rate** with the envelope from your kick or snare.
- Send random/sample & hold or short LFOs to the **Filter/Feedback** input for crunchy, unpredictable textures.

### 2. **Wobble Bass & Buzzy Leads (Dubstep/DnB)**
- Use bipolar LFOs or ADSR envelopes synced to your track's tempo to modulate the **Rate** or **Depth** of chorus/flanger/filter programs.
- Modulate **Drive** or **Depth** of FSU's distortion algorithms with alternating fast/slow LFOs for dynamic movement.
- Inject slow, wide triangle or ramp LFOs into **Filter/Feedback** for moving formant or phaser effects on bass.

### 3. **Haunting Pads / Evolving Atmospheres**
- Very slow LFOs or random stepped voltages to all three parameters for constant motion.
- Fade CV to the **Rate** parameter in chorus or phaser banks to morph pad width and shimmer over time.
- Automate **Fidelity/Clock CV** for lo-fi/hi-fi morphing and ghostly tape warbles.

---

## Patch Ideas

### 1. **Distorted Percussive Sounds**
- **FSU DISTORT Mode:**  
  Patch drums or short percussive loops into FSU. 
  - Mult your drum’s trigger to a short Envelope Generator.
  - Use this EG to hit **Drive/Depth**: higher decay for noisier transient, short for punch.
  - CV randomizer to **Rate/Gain** varies color with every hit.
  - Send **Filter/Feedback** random gates for erratic, unpredictable bite.
- Sound Example: Metallic snare with wild feedback and variable bitcrush on every hit.

---

### 2. **Dubstep/Drum & Bass Basslines**
- **FSU GLITCH Mode / MODFX FILTER Mode:**  
  Patch in a sub or sawtooth oscillator.  
  - Envelope-follower from your kick modulates **Depth** for synchronized squelch.
  - LFO to **Rate** for slow filter sweeps, S&H+clocked random to **Filter** for formant-style wubs.
  - Use FSU's **Ring Mod/Bit Crusher/Varispeed** for throaty, digital basses—modulate **Depth** for glitching pitch/bit depth per note.
- Pro Tip: Try clocked random for unpredictable, reactive bass movement.

---

### 3. **Haunting Pads and Atmospheric Textures**
- **MODFX CHORUS/FILTER / FSU SOUND ON SOUND:**  
  Feed in simple pads, vocal samples, or droney sources.
  - Slow triangle or random LFOs to **Rate**/**Depth** for swirling, never-repeating stereo motion.
  - Patch mod wheel, aftertouch, or manual control to change the **Filter/Feedback** for expressive morphing over time.
  - Use the FSU SOS bank in **Frozen Plate** and send slow-moving CV to **Decay** and **Low Pass**—for spooky reverbs that evolve endlessly.
- Combine both modules: MODFX wide, wobbly chorus into FSU’s granular or SOS programs for complex, smeared ambiences.

---

## Modulation Sources to Try

- **Envelopes** (ADSR/AR): Sync to triggers, modulating Drive, Depth, Feedback for per-hit change.
- **Random Generators & S&H:** Useful for unpredictable, glitchy effects.
- **LFOs:** Use two or more at different rates, patched to different parameters for organic movement.
- **CV Sequencers:** Automate shifts in the effect programs or Fidelity for changing "scenes."
- **Manual Joysticks/Touch Controllers:** For live improvisational control.

---

## CV Tips

- Use **attenuators** and **offsets** to make sure CV is in the right range (sometimes negative voltages have interesting consequences!)
- Self-patch: try using effect output as a CV source for its own input—can create unstable, organic chaos.
- Patch CV to **Fidelity/Clock** for realtime sample-rate/fidelity jumps, creating wild digital artifacts.

---

## Links

- [Download the Tiptop Audio ModFx/FSU Manual (PDF)](https://tiptopaudio.com/manuals/FSU_MODfx_Manual_web.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)