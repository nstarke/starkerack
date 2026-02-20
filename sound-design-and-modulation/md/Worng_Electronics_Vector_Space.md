# Worng Electronics — Vector Space

- [Manual PDF](../../manuals/Vector Space Manual v1.00.pdf)

---

[WORNG Electronics Vector Space User Manual - PDF](https://manuals.plus/worng-electronics/vector-space-manual)

---

# Creative Patch Ideas with Vector Space  
#### For Distorted Percussion, Dubstep/Drum & Bass Basslines, and Atmospheric Pads

The WORNG Electronics Vector Space is an extremely powerful and flexible modulation and mixing hub for Eurorack systems. Its core purpose is to take three input signals— **i, j, and k**—and turn them into 17 related, but unique, CV or audio outputs via an all-analog circuit. By leveraging its *Cube, Plane,* and *Sphere* outputs, you can create a wide range of complex and evolving results. Below are practical, genre-focused techniques you can try to dial in some unique timbres and motion.

---

## 1. Distorted Percussive Sounds

#### **Goal:**  
Create struck, glitched, or industrial percussion using Vector Space's complex output combinations.

**Patch Concept:**  
- **Inputs:**  
  - i: Snappy Envelope (or fast, sharp LFO)
  - j: Noise source or random stepped voltage
  - k: Short audio click, metallic ping, or audio-rate square wave

- **Output Routing:**  
  - Take *Plane* or *Cube* outs (with major LED activity) to a wavefolder, VCA, or filter set to overdrive.  
  - The *Plane* outs, in particular, will produce rectified, frequency-doubled, and phase-scrambled signals, adding metallic or digital artifact textures.

- **Extra Control:**  
  - Switch the input ranges (+/+-) to alter the baseline offset, resulting in odd clipping or biasing behavior.
  - Patch some of the Vector Space outputs back into decay/fall CV on your envelope generator for feedback-styled percussion movement.

- **Tips:**  
  - Sequence your envelopes/arbitrary stepped voltages randomly for glitchy, IDM-like percussion.
  - Try ring modulating (via a VCA) the Plane out signals with other percussion elements.

---

## 2. Dubstep/Drum & Bass Basslines

#### **Goal:**  
Get those "talking," wobbly, or highly modulated basses typical in these genres.

**Patch Concept:**  
- **Inputs:**  
  - i: LFO (slow to mid, e.g. 0.5–8 Hz, triangle or sine for smooth, square/saw for choppier sound)
  - j: Envelope follower from a drum track, sequencer, or another LFO with different phase/rate
  - k: Audio-rate oscillator (preferably another VCO slightly FM'ed for extra grit)

- **Output Routing:**  
  - Use the *Cube* outs to get classic crossmodulation shapes for cutoff, sync, or waveshaping of a bass VCO or filter.
  - *Plane* outs can create more aggressive, harmonically rich modulations. Patch these as CV to a wavefolder, filter cutoff, or oscillator FM input.
  - Modulate a stereo VCA or panner with a *Cube* or *Plane* output for moving/wandering basses.

- **Extra Control:**  
  - Use the Unipolar/Bipolar switches to abruptly change the modulation pattern mid-bar for growls or glitch effects.
  - Patch an output from Vector Space back to modulate the rate or depth of your primary LFOs for wilder, evolving sounds.

- **Tips:**  
  - Route the NegSphere out as audio to distorters, or modulate resonance for weird additional movement.
  - Try using audio-rate signals for all three inputs, and then listen to the Sphere/UnSphere outs for chaotic, wavetable-like timbres.

---

## 3. Haunting Atmospheric Pad Sounds

#### **Goal:**  
Generate evolving, ethereal movement across stereo or multi-channel pad textures.

**Patch Concept:**  
- **Inputs:**  
  - i: Slow LFO (sine or triangle, 0.1–0.5 Hz)
  - j: Field recording or sample playback (looped atmosphere, e.g. rain or wind)
  - k: Expression pedal/joystick, or a gentle random voltage source

- **Output Routing:**  
  - Send various *Cube* outs to the panning, filter, or amplitude modulation of multiple pad voices so each floats gently through the stereo field.
  - Use different *Plane* outputs to control reverb send amount, grain position, or wavetable scan position.
  - The *Sphere* and *UnSphere* outs are excellent for slow, undulating modulation of overall mix parameters—global lowpass, feedback, or spatialization.

- **Extra Control:**  
  - Use the input switches to add gentle variations to the global modulations, emphasizing movement as you play.
  - If you have more than three pads, use different outs to control different sets, amplifying the “shifting cloud” effect.

- **Tips:**  
  - Patch the post-effect return of one pad voice back into a Vector Space input, creating a feedback network where the texture modulates itself.
  - Tempo-sync LFOs for subtle pulse/phase effects that evolve over many bars.

---

## **Advanced Tips for All Genres**

- **Feedback Routing:** Try patching one or more Vector Space outs to modulate the CV sources you’re using as inputs, leading to “recursive modulation” and highly organic sounds.
- **Switch Flicking:** Perform live by toggling the input polarity switches, introducing shifts, offsets, and mod mutations in your mod matrix.
- **Audio-Rate Inputs:** Don’t be afraid to use audio-rate signals (even drums, samples, or chords) for FM/AM-style wildness—Vector Space processes audio just as well as CV.

Explore, combine, and experiment—Vector Space’s strength is unlocking new forms of movement and interaction in any patch.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)