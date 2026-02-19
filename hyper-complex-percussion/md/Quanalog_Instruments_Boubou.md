# Quanalog Instruments — Boubou

- [Manual PDF](../../manuals/Boubou – Quanalog Instruments.pdf)

---

[Quanalog Boubou Manual (PDF)](https://quanalog.com/boubou/)

---

# Creative Strategies for Densely Rhythmic, Hyper Complex Percussion with Quanalog Boubou

The Quanalog Boubou is an exceptional module for anyone seeking advanced, hybrid analog percussion within a compact Eurorack format. It excels as a set of drum voices **and** as a semi-modular analog signal processor. Here’s how you can leverage the **Boubou’s unique architecture** and control scheme for highly complex, polyrhythmic, and intricate music.

## **1. Voice Architecture: A Modular Playground**

- **Kick**: 2-part design with sine-based analog filter + click circuit. Tunable overdrive, compression modes, and CV for decay/tune.
- **Dual Tom**: Lo and Hi toms can be manipulated as drums or as notch filters—each with voltage-controlled pitch/resonance. The retrig knob lets you “flam” and “roll” for hand-play feel.
- **Snare**: Noise-based, with resonant bandpass filtering + voltage control. Resonance and decay are both CV-controlled for energy per hit.
- **Hi Hats**: Independent noise source through resonant highpass filter, plus mixer for external source. CV-controlled decay for continuous “pedal” expressive playing.

## **2. Rhythm Complexity: Sequencing Techniques**

### **A. Polyrhythms and Multitimbral Layering**

- **Trigger inputs** on each voice react independently—use multiple sequencers or clock dividers for unsynced/offset pulses (e.g., run toms on 5-step pattern vs. kick on 4).
- **Dual Tom retrig** knob lets you dial in variable accent and “second hit” volume. Gate length from sequencer thus adds stepwise articulation—use triggers AND gates from separate tracks.

### **B. Complex Time Signatures**

- Employ separate trigger/gate channels per voice, each running different pattern lengths: e.g., 7-step trigger loop for Snare, 5 for Kick, 11 for Hats.
- Modulate pitch/decay CVs per step: cycle CV sources (LFOs, random stepped voltage, sequencers) in cycles mismatched to trigger patterns for pseudo-generative odd signatures.

---

## **3. Hyper-Complicated Patterns: Sound & CV Modulation**

### **A. Unique, Evolving Percussion via External Modulation**
- **CV Inputs** on kick, tom, and snare for pitch/tune and decay: send irregular LFOs, envelopes triggered by unrelated sequences, or manually played sources (with pressure or touch CV).
- **Patch cross-modulation**: Feed Boubou tom’s audio or triggers into snare/hats, or vice versa—chaining causes complex percussive inter-modulation (e.g., trigger the tom section with the audio out from the kick for a feedback/bitcrush effect).
- **Dynamic accenting**: Replace trigger/gate input with a stepped CV signal (quantized or not); the Boubou detects intensity/velocity, giving you step-to-step volume and timbre variation.

### **B. Voice Re-patching for Texture**
- Don’t trigger each voice every time:
    - Leave tom or snare “untriggered,” pass other signal/audio through for filtering or resonance boosting—yielding layered, thicker, and evolving drum “bodies”.
- Use **external audio** in Hi Hats’ Ext In for metallic/FM/complex cymbal timbres—modulate hats with pitched oscillator sequences or “choke” the hats by CVing decay with a fast envelope.
- **Self-oscillation** of the kick (cranking overdrive) can become a bassline or drone—sequence pitch CV for melodic/rhythmic crossover.

---

## **4. Signal Processing & Effects**

- Any drum engine can act as a bandpass/notch processor—patch melodic or chordal content through and modulate resonance, tune, or decay CV in syncopated or random patterns for rhythmic filter sweeps.
- Use toms as *dual notch filters* for external signals, modulating hi/lo frequencies to add “percussive flutter” or animated filtering to other drum or synth tracks.

---

## **5. Suggested External Pairings for Maximum Complexity**

- **Sequencer:** Anything with independent track lengths and CV out, like Hermod, NerdSeq, or even analog sequential switches.
- **Modulation:** Befaco Rampage, Batumi, or Voltage Block for generative envelopes and LFOs.
- **Random Sources:** Wogglebug, Turing Machine, Sapèl for irregular CV patterns on pitch/decay.

---

## **Summary: Pushing Boubou to the Edge**

- Multiple unsynced/odd-length triggers enable organically shifting polyrhythms.
- CV-modulate pitch/decay/resonance for each drum per step for animated, non-repetitive patterns.
- Re-route triggers/audio between engines for generative, cross-modulated sequences.
- Exploit Boubou’s filter architecture to process and warp other modules’ audio for percussive surprise.

---

**Explore further:**  
- [Official Quanalog Boubou Manual](https://quanalog.com/boubou/)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)