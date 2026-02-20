# 4ms — Rotating Clock Divider

- [Manual PDF](../../manuals/RCD-manual-1.2.pdf)

---

[Download the Rotating Clock Divider (RCD) Manual PDF](https://4mscompany.com/p.php?p=904&c=7)  
*Below is a creative modulation guide for the 4ms Rotating Clock Divider (RCD) tailored for advanced rhythmic distortion, basslines, and haunting atmospheres in eurorack modular synthesis.*

---

# Creative Modulation with the 4ms Rotating Clock Divider

## **Summary**

The **4ms Rotating Clock Divider (RCD)** is a rhythmic powerhouse that can drive wild gates, triggers, and syncopation across your modular. By creatively patching and aggressively modulating its divisions, rotation, and modes, you can coax chaotic percussion, mad wobbling basslines, and ghostly textures from your rack—well beyond straightforward clock divisions.

Below are patching/modulation strategies that unlock unique sounds for:
- Distorted Percussion
- Crazy Basslines (Dubstep, DnB)
- Haunting Atmospheric Pads

---

## **General Modulation Concepts**

1. **CV Rotate Modulation**:  
   - What it does: Shifts the divide-by values on all 8 outputs.  
   - Use LFOs, envelopes, stepped random, or audio-rate signals to modulate for non-repetitive, “rotating” rhythms.

2. **CV Reset**:  
   - Applying gates/pulses resets phase for all outputs.  
   - Resetting at odd intervals (e.g., from another divide out or random gate) can “trip up” looping patterns for more organic or jarring effects.

3. **Spread/Max Divide**:  
   - Spread Mode outputs musical (non-contiguous) divisions for more complex swung or polyrhythmic sequences.
   - Use breakouts/jumpers for quick hands-on reconfiguration.

4. **Gate/Trigger / Up/Down Modes**:  
   - Gate Mode = longer pulses, can create overlapping gates or “roll” effects.
   - Up/Down Counting inverts where pulses land in a measure/metre—musically, this can lend off-beat or on-beat emphasis.

---

## **Distorted Percussive Sounds**

- **Patch Proposal:**
    1. **Clock the RCD** with a fast LFO, audio gate, drum machine, or envelope follower from an acoustic source (for wild timings).
    2. **Output several divisions simultaneously** to different percussive sound sources (drum modules, LPGs, noise generators).
    3. **Heavily modulate the CV Rotate jack** with a fast random signal, stepped random, or an audio-rate oscillator for glitchy, unpredictable trigger shifting.
    4. **Enable Spread Mode & max divide-by lower (8 or 16)** for rapid-fire, constantly morphing drums and fills.
    5. **Mult the fastest division (e.g., /1 or /2) and distort it** with wavefolders, saturation, bitcrushers, or feedback loops for metallic or digital “hi-hats.”
    6. **Patch gate outs to trigger burst generators** or chained envelopes, then run the outputs through VCAs/wavefolders.

- **Bonus**: Patch one divider output back into the CV Reset to “choke” your patterns for broken, staggered grooves.

---

## **Crazy Basslines (Dubstep, Drum and Bass)**

- **Patch Proposal:**
    1. **Clock the RCD at audio rates (1–3kHz!)** from a VCO square.  
    2. **Use lower division outputs (/8, /16, /32) as sub-octave sources**—run these into a self-oscillating filter or a VCA with plenty of distortion.
    3. **Heavily modulate the CV Rotate and/or jump between Max Divide settings** with sample & hold, envelope, or stepped random sources—creates “wobbling” bass where the pulsewidth and rhythm are always morphing.
    4. **Run a division output into the FM input of a wavetable or digital oscillator** for unpredictable hard-hitting sync/folded timbres.
    5. **Try Gate Mode for “chopping” sounds**; the outputs behave like 50% duty cycle square waves, good for “chuggy” or rolling bass patterns.
    6. **Experiment with Down-counting mode** for off-kilter step patterns and “reverse” grooves.

- **Bonus**: Use two RCD outs at different divisions to clock a sample player for sub-bass “ghost notes” and syncopation.

---

## **Haunting Atmospheric Pads & Textures**

- **Patch Proposal:**
    1. **Clock RCD using a slow master clock or tap-tempo LFO**.
    2. **Set Max Divide high, enable Spread Mode.** Now output divisions will be widely spaced (e.g., /8, /16, /24, /32…).
    3. **Patch multiple RCD outputs to sequential switches or VCA gates controlling granular/droning sound sources, reverb tails, or resonator modules**.
    4. **Slowly modulate the CV Rotate input using a gentle LFO or random slew** for evolving, shifting textural rhythms; pulses for different sound “layers" will drift in and out of phase.
    5. **Send Reset pulses at intervals** (maybe from a random module or S&H), occasionally “realigning” all outputs for spectral shifts/ghostly unified swells.
    6. **In Gate Mode, use even high divides for long, overlapping pulses**—good for opening FX loops or delay lines, creating blurred, slowly-pulsing atmospheres.

- **Bonus**: Use an output from the RCD to clock a slow delay/looper, creating chance echoes every few bars.

---

## **Pro Tips**

- **Abuse Audio-Rate Gates**: Run audio VCO square waves into the Clock In for glitchy, sample-reduction-style effects using the pulse outputs as digital audio.
- **LED Trimpot**: Lower the LED brightness for spookier visual feedback, handy for minimal setups.
- **Don’t Ignore Bus Clock**: If you have multiple master clock sources, try switching the RCD to “Bus” mode for sudden, sharp tempo jumps and resyncs.

---

## **Further Exploration**
- Download the [full RCD manual (PDF)](https://4mscompany.com/p.php?p=904&c=7) for all jumper and spread settings.
- Patch, experiment, and record. Layer several outputs, multi-modulate Rotate and Reset, and listen for those moments when grooves and textures "fall apart"—sometimes, that's where the magic is!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
