# Noise Engineering — Terci Ruina

- [Manual PDF](../../manuals/Terci Ruina - Noise Engineering Documentation.pdf)

---

[**Terci Ruina Manual PDF**](https://manuals.noiseengineering.us/_/downloads/tr/en/latest/pdf/)

---

# Using Terci Ruina for Dense, Complex Percussion

**Module type:** _Effect (Triple Distortion)_  
**Purpose:** _Transform and annihilate your signals for unique, punchy, and percussive sounds._

---

## Philosophy

Terci Ruina is not a voice, but a triple-distortion effect unit designed for dramatic signal shaping and destruction. It features three cascaded (or independently patchable) distortion circuits, each with unique topologies and tonal strengths. For rhythm-driven, hyper-complex music, this module excels at turning drums, percussion, and even CV-driven signals into hyper-aggressive and intricate timbres perfect for polyrhythms and unusual grooves.

---

## Creative Patching for Percussive & Rhythmic Complexity

### 1. **Insert Distortion at Strategic Points in Percussion Chains**

- **Before/After VCA:** Place Terci Ruina after your VCA-contoured percussion for aggressive, dynamic accents.
- **Before/After Envelope or Filter:** Try highly-resonant filters/ADSRs (like Pons Asinorum or Sinc Bucina from Noise Engineering) before the TR for evolving textures.

### 2. **Exploit Normaling & Modular Signal Routing**

- Terci Ruina’s inputs/outputs are normalled in sequence, but patching breaks normalization.
    - **CV Control:** Mult your rhythmic trigger/gate patterns to modulate parameters elsewhere (e.g., filter cutoff, VCA) in perfect rhythm with your percussion.  
    - **Parallel/Serial Experimentation:** Use I/O flexibility to re-order distortion stages or isolate them for distinct percussive layers.

### 3. **Feed Complex Percussion Sources**

- **Feed the TR with:**  
    - Sampled or synthesized drum hits (with intentionally complex/irregular timing, accent, or velocity)
    - Polyrhythmic patterns from step sequencers or trigger generators (e.g., Pamela's NEW Workout, Euclidean Circles)
    - AM/FM patched percussion voices for additional spectral content.

### 4. **Unique, Punchy, and Percussive Sound-Shaping**

- **FB Distortion:**  
    - _Asymmetric transistor-based feedback distortion._  
    - Use this for unpredictable, gnarly clipping that emphasizes attack transients.  
    - Turn the knob to find sweet spots where transient energy overloads for almost “snapping” attacks—great for knocky digital percussion.

- **FF Distortion:**  
    - _Op-amp with diode feedforward clipping_  
    - Offers more conventional, yet aggressive saturation.  
    - Exploit asymmetry for timbral morphing; push it for “spitty” hardclipping snares or hats.  
    - Use as a signal “hotter” to set up the next stage for more dramatic effect.

- **FZ (Fuzz):**  
    - _Two-stage transistor fuzz, blends between phases (affects frequency response)_  
    - Use the knob to move from deep subby thumps (LP response) to harsh, bright attacks (HP response).  
    - Try for booming kicks vs. sizzly cymbals in the same chain using strategic knob placement.

---

## Patch Examples for Complex Percussion

### **A. Triple-Distorted Drum Machine**

- _Input:_ Multiple drum triggers mixed into a single channel, routed to TR input 1 (FB).
- _Output:_ Take Output 3 (FZ) to VCA then to final mix.
- _Knobs:_ Modulate (even manually or via slow LFOs/step CV) to “morph” between thick, boomy, and sharply clipped.
- _Result:_ Heavily processed breaks with evolving distortion “shapes”; each sequencer layer pokes through differently.

### **B. Layered Distortions for Accented Polyrhythms**

- Patch separate polyrhythmic percussion patterns to each distortion input independently.
- Take each output separately to VCA/mix.  
- You will have 3 differently distorted layers that can be panned, EQ’d, or further effected independently or mixed for intricate “meta-rhythms.”

### **C. Eurorack Drum Bus “Destruction Insert”**

- Mix all complex, polyrhythmic percussion through a summed VCA, then into Terci Ruina.  
- Place a filter (VCF) pre/post and modulate its cutoff via yet another rhythmic (possibly polyrhythmic) sequence/envelope.
- Result: Highly evolving, compressed, and lively drum bus—great for “berghain kicks,” distorted claps, or broken-beat hats.

---

## Additional Techniques

- **Voltage Control:**  
  While Terci Ruina doesn’t have CV over drive, you can automate waveshaping further up the chain for rhythmically modulated distortion character.
- **Fights Mud:**  
  Use FZ’s highpass response (full clockwise) to emphasize percussive attacks and clear up low-end mud typical in dense polyrhythmic mixes.
- **Percussive Noise:**  
  Blast noise or fluctuating/random sources through the chain for “glitch percussion.”

---

## Bonus Inspiration

- Stack sequencers with different step lengths (e.g., 7 vs 5 vs 12 steps) to drive gate/trigger-based percussion.  
- Process each with unique distortion topology via Terci Ruina for a polyrhythmic set that is as timbrally complex as it is rhythmically complex.

---

> “Terci Ruina was not designed to be pretty or clean but was meant to invoke some of the chaos that happens when using guitar pedals. It will be noisy. It may pick up radio stations. There is a little gremlin in there.”  
> — _Noise Engineering_

---

**[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**