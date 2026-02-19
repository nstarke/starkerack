# TAKAAB — Odd Clock Divider

- [Manual PDF](../../manuals/TAKAAB OCD - Odd Clock Divider – Siam Modular.pdf)

---

[TAKAAB OCD - Odd Clock Divider Manual (Product Page)](https://siammodular.com/products/takaab-ocd-odd-clock-divider)

---

# Using the Takaab OCD Odd Clock Divider for Complex Percussion and Polyrhythms

The **Takaab OCD** is not a sound/voice or effect module but a **2HP clock divider** specializing in odd and less common rhythmic divisions. As a rhythmic utility, it is a powerful tool for generating intricate, interlocking patterns required in advanced percussion programming and modular polyrhythmic sequencing.

---

## How to Use the OCD For Dense and Complex Rhythms

### 1. **Generating Diverse Clock Streams (Odd Divisions)**
- The OCD outputs simultaneous gate pulses from a single clock input at:
  - **/3**
  - **/5**
  - **/7**
  - **/9** (can be changed to **/6** via jumper)
  - **/10**  
Each output provides a mathematically related rhythmic subdivision that does not conform to typical duple/quad patterns, making every stream "offset" and polyrhythmic.

### 2. **Synchronizing Unrelated Patterns**
- Patch different outputs to trigger various percussion modules—each one gets its own unique, cycling rhythm, often lining up only after several cycles (true polyrhythm).
  - Example:  
    - /3 ⟶ Kick  
    - /5 ⟶ Snare  
    - /7 ⟶ Hihat  
    - /9 ⟶ Perc  
    - /10 ⟶ Clap

### 3. **Complex Time Signatures**
- Mix odd dividers (/5, /7, /9) with even dividers (use Takaab ECD for /2, /4, /6, /8, etc.) to build patterns in time signatures uncommon in typical Western music (e.g., 5/8, 7/8, 9/16, etc.).
- Chain/ping sequencers and algorithmic generators (like Euclidean or logic modules) with OCD outputs to create time signatures that morph and phase over time.

### 4. **Rhythmic Accents and Reset Function**
- Use the **RESET input or button**:  
  - Send manual/automated triggers (from a master clock, LFO, or any musical event) to RESET to realign all patterns, creating cycles of tension/release and evolving rhythmic frameworks.
  - Resets serve as metric “glue” for live performances and improvisational structure.

### 5. **Duty Cycle Shaping**
- All outputs have a 50% duty cycle (1:1 high:low, rounded to nearest input pulse), but ratios vary slightly with odd-number divisions (e.g., 1/3 = 1:3, 1/7 = 3:4):
  - These unconventional gate lengths create nonstandard envelope shapes if patched directly to percussive voices with voltage-controlled elements (VCAs, LPGs, sample/holds).

### 6. **Patch Tips for Hyper-Complex Percussion**
- **Layering Clocks:** Use multiple OCD units normalizing RESET/CLOCK inputs to keep many polyrhythmic divisions tightly phase-locked but out of conventional sync (using the included 2-pin Dupont jumpers).
- **Logic Modules:** Combine different OCD outputs via OR, XOR, AND, or sequential switch modules to create new, emergent rhythms and nested tuplets not available from a single divider.
- **Step Sequencer Modulation:** Clock step sequencers or trigger selectors with OCD outs for constantly shifting step patterns, shuffling through different percussion samples, or changing modulation destinations to build evolving polyrhythms.

---

## Example Patch Concepts

- **Polyrhythmic Percussion Engine:**  
  Clock input = 120 BPM master clock.  
  OCD /3 out → kick drum trigger   
  OCD /5 out → snare trigger  
  OCD /7 out → hi-hat envelope  
  OCD /9 out → random sample drum sound  
  OCD /10 out → fill/FX percussion  

- **Polytemporal Sequencing:**  
  Patch clocked sequencers or random voltage sources with various OCD outs to melody and modulation destinations for metric modulation of both pitch and percussive voices.

- **Rhythmic Reset FX:**  
  Automate the RESET (with a random generator, slow LFO, or hand-button) for "rhythmic jump-cuts," re-aligning complex layers on-the-fly.

---

## Bonus: Modulate Odd Divisions
- **Jumper to switch 1/9 to 1/6:**  
  Patch with the Takaab UXS or use the jumper on the board to shift the behaviour of this output—consider this during a performance for sudden time signature/feel changes.

---

## In Summary
While the OCD is not a sound source or effect by itself, **it is an advanced, compact utility** that, especially in combination with other sequencers, dividers, logic modules, and percussion voices, serves as the rhythmic backbone for modular setups that aim for density, complexity, and organic, ever-evolving pattern generation. It excels at **polyrhythmic sequencing**, **complex time signatures**, and **rhythmic modulations**—all hallmarks of cutting-edge modular percussion.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)