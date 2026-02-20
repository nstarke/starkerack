# 2hp — EG

- [Manual PDF](../../manuals/EG_Manual-7ja4.pdf)

---

[EG 2HP Envelope Generator Manual (PDF)](https://2hp.com/wp-content/uploads/2018/10/2hp_eg_manual.pdf)

---

# Creative EG Modulation Techniques for Eurorack Synthesis

Based on your attached EG module manual, here are deep-dive ideas for using this compact, powerful envelope generator to create a huge variety of sounds—focusing on **distorted percussive hits**, **crazy dubstep/drum & bass basslines**, and **haunting ambient pads**.

## 1. Distorted Percussive Sounds

**Key technique:** Use ultra-fast attack & decay times, extreme envelope shapes, and dynamic CV modulation.

- **Set Attack and Decay Fully CCW:**  
  Dial both knobs hard left for the snappiest transients (attack/decay ~3ms).
- **Patch into Audio-Rate Destinations:**  
  Send the envelope OUT to a filter or VCA controlling a drum oscillator—modulate a wavefolder or even FM input for a noisy *clap* or *kick* transient.
- **CV Over Attack/Decay for Glitch:**  
  Feed a stepped random CV or trigger sequence into ATTACK CV or DECAY CV. This will shift the shape each time, giving clicky, shifting percussion.
- **Switch Response Toggle:**  
  Flip between **linear** for metallic/sharp clicks or **exponential** for “punchier,” curved percussive envelopes.
- **Amp for Distortion:**  
  Crank AMP knob or overdrive a following stage for envelope-based gain distortion.

**Bonus tip:** Patch TRIG to a fast LFO or burst generator for machine-gun, laser zap or metallic sounds.

---

## 2. Crazy Dubstep/Drum & Bass Basslines

**Key technique:** Use the envelope to animate a filter, oscillator FM, or VCA for *moving*, *growling* modulation.

- **Modulate Filter Cutoff:**  
  OUT → LP/HP filter cutoff for classic “wobble.”  
  Use DECAY CV modulation from a sequencer/LFO for variable note lengths.
- **Exponentially Shaped Envelope:**  
  Set toggle to EXPO for aggressive, deep sweeps.
- **Dynamic Modulation:**  
  Vary ATTACK or DECAY with CV signals from sequencer accent tracks for ever-changing bass movement.
- **Layer Multiple Destinations:**  
  Use stackcables/mults to send envelope OUT to filter **and** VCA—and maybe an FM input—giving huge moving tonal complexity.
- **Manual Performance:**  
  Sweep AMP or decay times by hand in performance for live “wobble” control.

---

## 3. Haunting Atmospheres & Pads

**Key technique:** Exploit super-long envelopes, slow modulations, and shape morphing.

- **Exaggerated Envelope Times:**  
  Set ATTACK and/or DECAY far right for 10+ second swells and fades.
- **CV Morph Between Shapes:**  
  Slowly LFO the ATTACK/DECAY CV, so the pad subtly evolves in amplitude shape.
- **Manual or Automated Toggle Swaps:**  
  Switch between linear/exponential mid-note (or “flicker” with a gate/solenoid if DIY-hacked), for eerie volume curves.
- **Amplitude as Depth Control:**  
  Set AMP low for “fade in/out” ghostly effects, or up for enveloped drones.
- **Layer With Reverb:**  
  EG isn't a sound source, but modulates other layers—long envelopes into dark filters, or VCA opening noise or soft oscillators for classic ‘clouds.’

---

**Extra General Tricks:**
- **Velocity Sensitive Percussion:**  
  Use a velocity CV from a MIDI-CV module to ATTACK/DECAY/AMP for expressive playing.
- **Double-Envelope** with two EGs for more stages (patch one OUT to the other's TRIG for multi-segment shapes).

> **Tip:** With the EG’s compact form, pairing it with sequential switches, logic, or CV-addressed modules multiplies its creative use.

---

**Explore More:**  
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)