# Klavis — Grainity VCF

- [Manual PDF](../../manuals/Klavis_-_Grainity_User_Manual.pdf)

---

[Download the Klavis Grainity User Manual PDF](https://www.klavis.com/images/Klavis_Grainity_-_User_Manual.pdf)

---

# Creative Eurorack Patching Ideas with the **Klavis Grainity Granular VCF**

The Klavis Grainity presents a unique platform for both conventional and highly experimental filtering. Below, I’ll suggest a range of creative techniques leveraging its granular and multimode paths, and outline synergistic module combinations to maximize your sonic palette.

---

## 1. **Harmonic Processing with Multiple VCOs**

**Concept:** Feed a complex VCO waveform (e.g., saw + sub, or FM-modulated oscillator) into the main input, and use a cleaner waveform from the same or related VCO in the Detect input.

- **Result:** The Granular VCF steps in time with the clean waveform, but processes the rich harmonics of the complex input, leading to controlled, musical subharmonics and "pseudo-chord" effects.
- **Recommended Modules:**  
  - **Mutable Instruments Plaits** (for easily switching between clean and complex waveforms)  
  - Any dual or complex VCO (e.g., **Intellijel Dixie II+**, **Make Noise DPO**, **Klavis Twin Waves**)

## 2. **Trigger-Driven Rhythmic Filtering**

**Concept:** Use drum triggers, clock dividers, or sequencer triggers (e.g., from **Pamela’s New Workout**, **Make Noise Tempi**) to advance the Granular VCF stepping via the Detect input, while passing audio from a static drone or evolving pad to the main input.

- **Result:** Rhythmic, stepped filtering of a static background indicates "techno" builds, evolving percussive textures, or randomized gating effects.
- **Tip:** Use different clock divisions (even non-integer) on the Detect input to create polyrhythmic filtering movement.

## 3. **Granular Chorus & Flanging**

**Concept:** Modulate the Phase (Φ) CV input with a slow, slightly irregular LFO or slewed random voltage (e.g., from **Make Noise Maths**, **Mutable Instruments Tides**, or **ALM Pip Slope II**).

- **Result:** Animated, chorus-like textures or shifting formants.  
- **Variation:** Patch a sample-and-hold quantized random output (**Mutable Instruments Marbles**, **Noise Engineering Clep Diaz**) for barely-repeating granular timbres.

## 4. **Stereo Expansion & External Mixing**

**Concept:** Route the M.VCF and G.VCF outputs to separate channels of a stereo mixer or two separate effect chains.

- **Result:** Widen the stereo field with very different textures left and right—smooth multimode filtering on one side, wild granular effects on the other.
- **Recommended Mixers:**  
  - **Intellijel Mixup**, **Happy Nerding PanMix**, **Stereo FX modules** (e.g., **Desmodus Versio**)

## 5. **Formant and Subharmonic Generator for Basslines**

**Concept:** Use a monophonic VCO sequence (e.g., a bassline from a sequencer) and set the Grainity for a multi-step structure with a division to introduce subharmonic content.

- **Result:** "Vocoder-like" or throat-singing basses with shifting subharmonics and formants.
- **Recommended Companions:**  
  - **KMI Quadra**, **Acid Rain Maestro** (for complex, sequence-synced modulation)  
  - **Analog VCO** (e.g., **Doepfer A-110**, **Erica Synths Pico VCO**)

## 6. **Audio Realm Ring Modulation/Unison Animation**

- Patch a unison or ring-mod source (Twin Waves, DPO, etc.) to the main input.
- Feed a related — but slightly detuned — wave to Detect, or simply use G.VCF Phase modulation for inharmonic, evolving textures.

---

## **Additional Creative Tips**

- **Granularity as Melodic Generator:** Use Track+Division controls to generate melodic intervals from a single VCO, effectively creating harmonies or chordal effects on the fly.
- **Mixed Music/Field Recording Processing:** Place a comparator (Intellijel µStep, Doepfer A-167) after a bandpass or envelope follower on external music/field recordings, and feed that as Detect input for dynamic, context-sensitive rhythmic filtering.
- **Patchable Feedback:** Route M.VCF or G.VCF output back into the signal chain pre-VCF for wild self-modulations (be careful with levels!).
- **Sequencer + CV Control:** Assign structure, division, or phase to CV lanes from a sequencer (Hermod, Nerdseq) for morphing filter states in sync with your performance.

---

## **General Module Type Recommendations**

- **Complex Oscillators / Dual VCOs** - For maximized interaction with Detect/Main input independence.
- **Flexible LFOs/Function Generators** - For CV modulation of Grainity parameters.
- **CV-Controllable Stereo Mixers** - To blend and spatialize M.VCF/G.VCF/Mix outputs.
- **Comparators/Envelope Followers** - For dynamic Detect input strategies.
- **Sequencers/Modulation Sources with Random & Quantized Outputs** - For unpredictable, musically relevant CV control.

---

For exploration beyond the manual, experiment patching both conventional and unexpected audio and modulation sources to the Grainity’s various CV and audio inputs—you’re unlikely to run out of new territory with this module!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)