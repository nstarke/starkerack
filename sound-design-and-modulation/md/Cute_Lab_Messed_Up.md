# Cute Lab — Messed Up

- [Manual PDF](../../manuals/messed-up-manual-rev2.pdf)

---

[**Download the MessedUp Manual PDF**](sandbox:/mnt/data/MessedUp_Manual_Rev2.pdf)

---

# Creative Modulation Techniques for Messed Up (CuteLab)

The **Messed Up** module is a metrically modulating clock generator designed for adventurous polyrhythms and tempo morphing. It can radically transform the rhythmic landscape in your modular system, introducing layers of syncopation, metric modulation, and cross-rhythm—making it a powerhouse for experimental sound design.

Below are tailored modulation strategies to fit three different musical use-cases: **distorted percussion, wonky basslines, and haunting pads**.

---

## 1. Distorted Percussive Sounds

**Goal:** Pulse- and glitch-based grooves, polymetric rhythms, and aggressive stuttering.

#### Patch Suggestions:

- **Truncate Output to Percussion Modules:**
  - Set `divide` and `beat` to **prime number ratios** (e.g., 5 & 4 or 7 & 3).
  - Increase the **Truncate** knob/CV to less than 100%—this creates stuttered, not-quite-even divisions.
  - Route `truncate` out (Jack 19) to trigger a drum or noise source. This will slice off beats in irregular places, chopping audio in unexpected ways.
  
- **Metric Modulation "Triplet Flip":**
  - Patch a regular clock to the module.
  - Use `beat=4`, `divide=3`, latch the modulations to downbeats.
  - Press the **Modulate** button or send a trigger to its input while a phrase is playing.
  - On modulation, everything re-times: 1/4 notes become "quarter-note triplets." This is sonically jarring if the percussive sounds are sustained and distorted.
  
- **CV-Controlled Drunken Divides:**
  - Patch a slow, random LFO or stepped CV to the `divide CV input` (Jack 16). Use the `divide attenuverter` (Knob 12) to taste.
  - Each bar, division amount swerves, causing percussion loops to lose/gain triggers, becoming unpredictable and crunchy.

---

## 2. Crazy Dubstep/Drum & Bass Basslines

**Goal:** Automated wobbles, syncopated switchups, intricate sub sync.

#### Patch Suggestions:

- **Bass Envelope Clocking:**
  - Use `beat out` (Jack 21) or `divide out` (Jack 20) to clock bass envelope generators or modulation oscillators.
  - Regularly `modulate` between (for example) `beat=3`, `divide=8` and vice versa. Use latching so that changes line up with measures.
  - This creates polymetric LFO wobbles that suddenly shift phase or speed, classic for neuro/dubstep leads.
  
- **Truncation For "Bass Gatling":**
  - Patch the `truncate` output to a VCA controlling a bassline oscillator.
  - Modulate the Truncate amount with a fast envelope or random CV; the "gate" for the bassline gets clipped and shifted within every measure.
  - Add audio-rate modulation to the Truncate CV for intense digital distortion artifacts—robotic, shredded bass pulses.
  
- **Divide Ratios as Bass Step Selectors:**
  - Use a sequencer that advances on clock.
  - Modulate between 5:4, 7:3, 3:4, and other ratios mid-riff for machine-gun-style sudden sequence length changes.
  - The **Round Trip** modulation mode lets you "snap back" to the original groove for drop-to-drop contrast.

---

## 3. Haunting Atmospheric Pads

**Goal:** Long-evolving, unpredictable, and phasing textures.

#### Patch Suggestions:

- **Slow Metric Drift:**
  - Use internal clock, set a slow tempo (e.g., 40-80 BPM).
  - Output `beat` and `divide` to different envelopes or VCAs controlling ambient tone generators.
  - Slowly modulate between ratios like 9:8, 7:6 for subtle rhythmic drift.
  - Engage **latch** for both beat and divide to ensure transitions are gentle and line up, for that “falling apart in slow motion” pad feel.
  
- **Clocking Modulation Index/FX:**
  - Use `EoM` (End of Modulation pulse, Jack 18) to trigger random shifts in a reverb, sample-and-hold, or granular effect.
  - Every time the metric mod occurs, the atmosphere "morphs," adding organic complexity.
  
- **Asynchronous Layering:**
  - Patch `downbeat`, `divide`, and `beat` to three different mod destinations on a big reverb pad (filter cutoff, shimmer mixer, vactrol slew time).
  - Use distinctly different `beat/divide` values for a multi-layer phase effect that never repeats exactly, gently pulling apart and tightening pad harmony.

---

### **Power User Tips**

- **Modulation Style (`StyL`):** Experiment with `FLIP` mode for totally swapping beat/divide—ideal for creating sudden metric inversions.
- **Duty Cycle Short Pulses:** For percussive or choppy effects, set duty cycle mode to 0.01 for 10ms pulses. This makes the clocks act like rapid triggers rather than “on” gates—great for clicks or instant bass “zaps”.
- **Chain CVs:** Modulate the `modulation trigger input` and `beat/divide` CVs simultaneously for even more complex metric automation.

---

## In Summary

The Messed Up module is a deep tool for clock bending: with its polyrhythm stretching, truncate gating, and moment-to-moment modulation, it is uniquely placed for sound-designers hungry for new rhythmic terrains—perfect for distorted beats, neurotic basses, and heavenly pads.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)