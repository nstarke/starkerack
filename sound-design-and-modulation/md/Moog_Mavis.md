# Moog — Mavis

- [Manual PDF](../../manuals/MAVIS_MANUAL_V2_06.27.2022.pdf)

---

[**Moog Mavis User Manual (PDF)**](https://www.moogmusic.com/sites/default/files/Mavis_Users_Manual_v2_0.pdf)

---

# Eurorack Sound Design with Moog Mavis: Modulation Strategies

As a fellow Eurorack modular synthesizer musician, exploring the Moog Mavis as a sound generator in your rack offers rich sonic territory—especially for aggressive percussive hits, basslines reminiscent of dubstep/DnB, and eerie pads. Here’s how to patch and modulate Mavis to wring the most unique and interesting tones out of it, focusing on *distortion*, *motion*, and *texture*.

---

## 1. **Distorted Percussive Sounds**

### **Key Techniques on the Mavis**

- **Wave Folding:** That built-in wavefolder is rare for Moog gear! For hard-edged, biting transients and “crushed” percussive sounds, patch your oscillator directly into the wavefolder (`VCO OUT → FOLD IN`). Turn the **FOLD** knob full right for maximum distortion and harmonics.
- **Envelope Modulation:** Use the snappy envelope—set **Attack** and **Release** low and moderate **Decay** & **Sustain** to taste, triggering with Mavis’ own button keyboard or external sequencer/trigger.
- **Filter Drive/Resonance:** Set the **Cutoff** high and use **Resonance** at or near self-oscillation. Try running self-oscillation for “kick” transients.
- **LFO as Percussive ‘Strike’:** Use the LFO in square mode at high rates to make extra clicks or as an envelope retrigger source.
- **External Audio:** With the wavefolder, you can patch in external drum sources, crush them, or layer with internal sounds.

#### **Sample Percussive Patch**

```text
VCO OUT → FOLD IN
FOLD OUT (post-wavefolder) is internal to the filter/VCA—adjust FOLD knob
ENV: Attack ~0, Decay ~100-300ms, Sustain ~0, Release ~0
Filter: Cutoff up, Res high OR full (for “pinged” kicks/snares)
ENV → Filter Cutoff Mod (VCF MOD MIX to EG, VCF MOD AMT positive)
Optional: S+H out to Pitch or Filter for glitchy, ‘circuit bent’ hits
Patch GATE IN for tempo-synced percussion, EG OUT to modulate other modules
```

---

## 2. **Crazy Dubstep/Drum & Bass Basslines**

### **Key Techniques on the Mavis**

- **LFO as Audio-Rate Modulator:** Use Mavis’ LFO at max frequency (audio range, up to ~550 Hz) for deep FM/AM effects and wobble. Patch **LFO OUT** to **PWM** or **1V/Oct** for dirty bass movement.
- **VCO Wave and PWM:** Use the **VCO WAVE** knob to blend saw and pulse for richer, nastier harmonics. Modulate **PW** or **PWM AMT** with LFO/EG for movement.
- **Sample & Hold Modulation:** Use the S+H to inject random or stepped modulations into filter cutoff or pitch (classic for “robotic”/glitchy bass).
- **Oscillator Mixing ("Two Oscillators" Trick):** Patch **LFO OUT** (audio rate) into **ONE (-5)** of the mixer and VCO OUT into **TWO**, take **ONE+TWO OUT** as your sound source—FM and sum for richer bass.
- **Extreme Filtering:** High resonance, cutoff modulation with fast or negative EG for squelches and vocal bass.

#### **Patch Example: “Talking”/Modulated Bass**

```text
Set LFO to max (audio rate), Square or blended with Triangle.
LFO OUT → PWM IN (Pulse Width Modulation Input)
Set VCO WAVE between Saw and Pulse, modulate PWM AMT for gnarly timbres.
ENV: Short attack, medium decay, low sustain, medium release for pluck or growl.
VCF: Lowish cutoff, high resonance; modulate CUTOFF with LFO and/or EG.
VCF MOD MIX set to blend LFO & EG (find rhythmic sweet spots)
ONE+TWO MIXER: Mix LFO OUT (audio rate) and VCO OUT, then route to FOLD IN
Try S+H OUT to VCO 1V/Oct for pseudo-random ‘wub-wub’ pitch jumps
Glide ON for legato slide/portamento effects
```

---

## 3. **Haunting Atmospheric Pads/Textures**

### **Key Techniques on the Mavis**

- **Slower, Moving Modulation:** LFO rate low, modulate VCO wave blend, pulse width, or filter cutoff gently to add subtle evolution.
- **Layered/Stereo Paths:** Use the mixer to blend two sources (e.g., Saw and Folded Saw, or VCO and audio-rate LFO); pan externally for wide pads.
- **Wavefolder for Shimmer:** Use FOLD for shimmering/snarling overtones, just barely applied for shimmer versus full-on distortion.
- **Self-Oscillating Filter:** Use high resonance, filter in self-osc mode, play filter with Envelope (VCF MOD MIX set to EG).
- **Drone Mode:** Use the **VCA MODE** switch ON for constant output (drone), modulate VOLUME, Cutoff, and Fold with slow LFO or S+H.
- **External CV Control:** Patch external slow mod sources or sequencers to filter cutoff, wavefolder, or VCA for motion.

#### **Patch Example: Evolving Pad/Drone**

```text
VCO: Set WAVE to desired timbre (CW for Pulse, CCW for Saw, or blend).
FOLD IN: Patch VCO OUT to FOLD IN, only slightly engage Fold for richness.
Filter: High resonance just before self-osc; mad Cutoff modulation.
LFO: Sweep Rate low; OUT to CUTOFF for drifting filter.
ENV: Long attack, long release, high sustain (pad). EG → CUTOFF or VCA CV
Mixer: Try mixing VCO and LFO (slower rate) for evolving undertones.
VCA MODE: ON for held/ambient drones.
Try S+H OUT to modulate CUTOFF for unpredictable, haunted movement.
Patch MULT outputs to send modulations to VCA and filter simultaneously.
```

---

## **Some Patch Combo/Experiment Tips**

- **Chain Modulation:** Use MULT for splitting S+H or LFO to several destinations (cutoff, PWM, VCA CV, etc).
- **Attenuate/Scale Modulation:** Use the internal ATTENUATOR to scale aggressive modulations for subtle/organic effects.
- **External Interaction:** Interface with other Euro modules! Use audio-rate CV mod on Fold, Freq, or Filter, or layer sounds with multiple Mavis modules.

---

## **Resources**

- [Moog Mavis User Manual PDF](https://www.moogmusic.com/sites/default/files/Mavis_Users_Manual_v2_0.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---

Feel free to ask for more patch ideas or module pairing tips!