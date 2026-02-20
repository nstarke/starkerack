# 2hp — Delay

- [Manual PDF](../../manuals/Delay_Manual.pdf)

---

[Download Manual PDF (images above, assumed from 2hp Delay module)](https://2hp.io/docs/2hp_delay_manual.pdf)

---

# Creative Modulation with 2hp Delay: Unique Sound Design

The 2hp Delay module is a compact, CV-controllable digital delay suited for everything from crispy percussive effects to deep, warping pads. Here are high-impact modulation strategies for **distorted percussion**, **dubstep/drum & bass basslines**, and **haunting pads**:

---

## 1. Distorted Percussive Sounds

- **Key Modulations:** FDBK CV, TIME CV  
- **Process:**  
  - *Patch drums or short percussive sounds* (e.g., from a drum module or synth voice) into the **IN**.
  - Set **TIME** low (short delay times = slapback) for glitchy artifacts.
  - **Modulate TIME CV** from a fast envelope or trigger sequencer, making each hit shift in delay time—this introduces accents, pitch artifacts, and off-kilter pulses.
  - **Increase FDBK**, perhaps modulated with random stepped CV (Sample & Hold, random gates, or even audio-rate CV) to push the repeats into self-oscillation for overdriven, crushed sound.
  - **Option:** Overdrive by pushing the **FDBK** knob to maximum, allowing chaotic feedback loops—a classic distorted, noisy percussion trick.
  - **Mix**: Use MIX CV to dynamically blend dry/wet sound with accent envelopes.

---

## 2. Dubstep/Drum & Bass Basslines

- **Key Modulations:** TIME CV, FDBK CV, MIX CV
- **Process:**
  - *Patch bass synth voice* to **IN**.
  - Use **LFOs or Envelopes** to modulate **TIME CV** between 0V and 5V on the beat. Extreme modulation can cause pitch-smearing and aggressive time-stretched bass movement typical in Neuro, brostep, or techstep.
  - Set **FDBK** high and modulate with another LFO or envelope—increasing feedback during drops and breakdowns for growling, resonant tails.
  - **Audio-rate modulation** to TIME CV or FDBK CV (patch fast LFO or even oscillator) can create FM-like distortion and unexpected bass artifacts.
  - Automate **MIX CV** with sequencer or envelope—bring the delay in and out with quick movements for dramatic, rhythmic variation.

---

## 3. Haunting Atmospheric Pads

- **Key Modulations:** TIME CV, FDBK CV, MIX CV
- **Process:**
  - *Patch drones, chords, or evolving pads* to **IN**.
  - Set **TIME** to longer settings (fully clockwise) for almost 2 seconds of repetition.
  - Use slow, subtle LFO or random voltage to **modulate TIME CV**—this creates gentle pitch modulation and evolving, ghostly motion as repeats smear and shift.
  - Push **FDBK** close to maximum (just before infinite self-oscillation) and gently modulate with slow envelopes/random CV for shimmering echoes and swelling noise layers.
  - Set **MIX** to about 50/50 and automate with slow envelopes or a joystick to pan between dry and wet, moving through blurry, mysterious spaces.
  - **Bonus:** Patch the OUT back into FX or another delay for deep, atmospheric layering.

---

## Additional Patch Tips

- CV inputs are all added to the knob positions (0–5V), so hands-on tweaks plus automation can be combined.
- Use end-of-cycle triggers or rhythm clocks to periodically drive extreme FDBK or TIME jumps for automated fills/breaks.
- Clocked stepped random (Sample & Hold) into TIME or FDBK CV makes granular, evolving effects.

---

For more generative ideas or code-based modular utility, visit the GitHub project below.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)