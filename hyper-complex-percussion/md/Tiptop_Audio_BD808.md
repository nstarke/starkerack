# Tiptop Audio — BD808

- [Manual PDF](../../manuals/Tiptop_Audio_BD808_ns.pdf)

---

[**Download the BD808 Manual PDF**](https://tiptopaudio.com/manuals/808-BD808_Manual.pdf)

---

## Using the TipTop Audio BD808 for Hyper-Complex Rhythmic Percussion in Eurorack

The BD808 is a dedicated analog bass drum generator based on the legendary Roland TR-808, but with enhancements perfect for demanding modular synth workflow. Here’s how you can leverage it to craft uniquely dense, polyrhythmic, and experimental percussion sequences.

---

### 1. **Polyrhythms & Complex Patterns with BD808**

- **Utilize Multiple, Independent Triggers:**  
  Use trigger sequencers or clock dividers/multipliers that can generate different rhythmic cycles (e.g., Euclidean pattern generators, clock logic modules, or probability-based trigger modules). 
  - Send a main gate to **GATE IN** for your primary rhythm.
  - Send a different-length (e.g., 7-step, 5-step, etc.) trigger to **ACCENT IN** for cross-accents and polyrhythmic emphasis.

- **Complex Time Signature Programming:**  
  Patch the BD808’s triggers from sequencers capable of outputting odd-length patterns or step-skipped pulses. Try chaining or cross-patching multiple trigger sequencers.

### 2. **Punch and Character Using Module Controls**

- **LEVEL:**  
  - Crank for saturated, harmonically rich kicks that can drive mixers and processors into aggressive territory.
  - Set low for punchy, vintage-style sounds.

- **TONE:**  
  - Dial high for bright “basketball” like kicks, suited for up-front rhythmic detail in busy patterns.
  - Dial low for sub-heavy, darker percussive foundations.

- **DECAY:**  
  - Short decay for rapid, staccato kicks in high-density patterns.
  - Long decay for classic boomy “doof” 808s or evolving pulses—just beware overlapping tails in tight sequences (can sound “messy,” but also organic).

- **ACCENT:**  
  Route trigger gates with polyrhythmic patterns to **ACCENT IN** for rhythmic emphasis that sits *against* (instead of just *with*) your main kick pattern. This makes beats pop out unexpectedly, especially in odd time signatures.

---

### 3. **Processing & Advanced Patch Techniques**

- **Layer BD808 with Other Drum Voices:**  
  Mix with rimshots, snares, hi-hats, and noise-based percussion--especially when using independent rhythms for each.

- **Ring Modulation/Amplitude Modulation:**  
  Patch the BD808 and, e.g., HATS808 or SN808 into a ring modulator or VCA modulated by a third sequencer for wild, metallic/abstract percussion.

- **Filtered/Distorted Chains:**  
  - Run BD OUT through resonant filters tightly modulated by separate clocks/sequencers.
  - Process with wavefolders, bit-crushers, or granular modules for glitchy, fractured kicks.

- **Utilize ACCENT as a Dynamics Mod Source:**  
  Input rhythmic or even audio-rate gates/signals to ACCENT IN for modulation artifacts, unique thanks to the analog design.

- **Self-Oscillation & Feedback Loops:**  
  If your BD808 will self-oscillate (max DECAY), try syncing the feedback with drum triggers for bursty, FM-like low end.

- **Voltage Control Crosspatching:**  
  Use CV-modulated VCAs and sequencers to automate the LEVEL, DECAY, or TONE controls for evolving, never-repeating complex percussion.

---

### 4. **Creative Strategies for Ultra-Dense Patterns**

- **Trigger Overlapping & Conditional Triggers:**  
  Use conditional logic modules to only allow triggers through under specific conditions, creating “ghost notes” and fills.

- **Randomization & Probability:**  
  Probability-based gate modules allow triggers only on certain cycles, making complexity that’s never exactly the same.

- **Audio-Rate Triggering:**  
  Extreme: try fast, even audio-rate trigger bursts for granular, rolling, or bass-texture effects.

---

### 5. **Hybrid/Experimental Approaches**

- **Audio to Accent In:**  
  Patch audio-rate signals, envelopes, or LFOs into ACCENT IN for “pseudo-FM” or choppy dynamic effects.

- **Process BD808 Through DSP & Delays:**  
  As suggested in the manual, use stereo delays, pitch shifters, or reverbs with tempo-synced modulation for spacey, complex echoes and thickening.

---

#### **Short Patch Example: Polyrhythmic Kick Mayhem**

- **GATE IN:** Sequencer 1 (e.g., 4/4)
- **ACCENT IN:** Trigger from Sequencer 2 (e.g., 7-step Euclidean)
- **LEVEL:** 90%, **TONE:** 80%, **DECAY:** 30%, **ACCENT:** 70%
- **BD OUT:** Into wavefolder ➔ multimode filter (sequenced cutoff) ➔ stereo delay

This creates a double-patterned kick sequence with sharp, dynamic accenting and spectral movement--ideal for maximalist techno, IDM, or experimental music.

---

**[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**