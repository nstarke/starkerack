# Blue Lantern Modules — Voks Analog Filter

- [Manual PDF](../../manuals/BLM Voks Analog Filter.pdf)

---

[BLM Voks Analog Filter Manual (PDF)](https://www.bluelanternstore.com/store/p133/BLM_Voks_Analog_Filter.html#/)  

---

## Using the BLM Voks Analog Filter for Dense, Hyper-Complex Percussion (Eurorack)

### About the Module  
The **BLM Voks Analog Filter** is a Polivoks-style analog VCF updated with several "hacks" for character and performance.  
**Key Features:**
- 12dB Low Pass & 6dB Band Pass (each with its own output)
- Normal and "Unstable Brite" modes (switchable)
- Internal Limiter Diode (switchable)
- Multiple CV and audio inputs (including direct, attenuated, and bipolar FM)
- 6hp, 13mA current

This is a filter, not a complete voice, but can absolutely be used for percussion shaping and creative processing.

---

## Patch Techniques for Complex Percussion

### 1. Percussive Voice Shaping (Filter as Main Sound Source)
- **Patch a fast, plucky envelope** (ADSR with immediate attack and short decay) to both the *audio input* and either CV or FM inputs. Use the Voks' resonance and brite/unstable mode to make the filter “ping” and self-oscillate, giving you percussive pops or “kick” sounds.
- Mult envelopes to clock-divided rhythms to create *polyrhythmic* bursts through the filter.
- Use comparators or logic modules to mix fast, odd-length triggers/gates that control the envelope, resulting in complex—sometimes generative—percussive patterns.

### 2. Rhythmic Processing & Mutating Loops
- Feed rich audio (e.g., noise, digital drum samples, metallic tones) into the filter’s *direct input*.
- Patch rhythmic envelopes, gates, and complex LFOs (e.g., from Pamela’s New Workout, Zadar, etc.) to the *CV and FM inputs*.
- Crossfade between LPF and BPF outputs dynamically using a VC mixer or switch, modulated by yet *another* polyrhythmic source.
- Flick between Normal and Unstable Brite mode on beats or “off-beats” via a gate or manual performance, taking advantage of its unique, acidic filter distortion for variety and punch.

### 3. Multi-Layer Polyrhythms (Filter as Modulation Target)
- Drive the filter cutoff with separate CVs that are clocked to different divisions/multiples of your master tempo. For example: a 5-step LFO for cutoff and a 7-step sequenced envelope for FM.
- Combine filtered percussion with highly clocked, rhythmically skewed modulations to create movement and groove—making your drum sequences feel "played" and not looped.
- Send the same percussion sound to *both* LPF and BPF, but modulate depths and timbres differently for superimposed cross-rhythms.

### 4. Limiter & Distortion for Percussive Cut
- The internal limiter (switchable by front-panel) can shape transients, making your drums more *punchy* and controlled.
- Toggle the limiter *on and off* in-sync with specific beats or sub-patterns, emphasizing syncopation and attack in unexpected moments.

### 5. Wild FM Percussion
- Route clicky triggers or audio-rate pulses to the *bipolar FM input*, making the filter “chatter” or bark at audio rate or with unpredictable chaos, especially in Unstable Brite Mode.
- You can further accentuate this by using sequenced voltages or S&H, clocked oddly against the drum grid.

---

## Pro Tips
- **Audio Input Overloading:** Push hot signals or stack multiple sounds; the characterful clipping of the filter will help your percussion cut through, especially in dense mixes.
- **External Clock Logic:** Use clock dividers/multipliers and logic modules (AND, XOR, etc.) to generate gate patterns that trigger modulations to the filter in non-obvious polyrhythms.

---

## Summary
The BLM Voks Analog Filter is not just for classic synth filtering—it’s an aggressive, personality-driven sound-shaper. With strategic CV and rhythmic modulation, it becomes a powerful tool for hyper-complex, punchy, and uniquely percussive patches in your Eurorack system.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)