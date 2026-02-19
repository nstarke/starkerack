# Pittsburgh Modular — Double Helix Oscillator

- [Manual PDF](../../manuals/Lifeforms Double Helix Oscillator - Pittsburgh Modular Synthesizers.pdf)

---

[Download the Pittsburgh Modular Lifeforms Double Helix Oscillator Manual (PDF)](https://pittsburghmodular.com/_files/ugd/5c8c85_13220e9d7efa4e13a6c238d464befed2.pdf)

---

## Creating Dense, Hyper Complex Percussive Rhythms with the Lifeforms Double Helix Oscillator

The **Lifeforms Double Helix Oscillator** is a powerful analog oscillator *voice* module, exceptionally useful for percussive, rhythmic, and complex sonic designs—the foundation for constructing dense, polyrhythmic, and hyper-detailed percussion in Eurorack modular systems.

### 1. **Percussive Voice Architecture**

#### **Wavefolder + Low Pass Gate as Percussion Engine**

- **Signal Path:** Start by patching either oscillator (or both mixed together using the ‘In 1’ and ‘In 2’ inputs) into the Contour section.  
- **Wavefolding:** The voltage-controlled 6-stage wavefolder excels at turning simple sine or triangle waves into harmonically rich, snappy, attack-transient-laden percussion. Modulate the *Timbre* parameter (and especially the *Timbre CV* input) with stepped random, clocked LFOs, or fast envelopes to shape each hit/strike differently.
- **Dynamic Impulse Low Pass Gate:** The LPG provides a natural, acoustic-like amplitude+filtering response. Patch a gate or trigger sequence (ideally polyrhythmic clock divisions/multiplications or trigger patterns) into the *Impulse Input* to "strike" the LPG for varying decay lengths using the *Dynamics Response* knob and *Dynamics CV*.
- **Result:** Each impulse can have unique tonal and amplitude flavors, sounding like acoustic percussion elements (e.g., bongos, woodblocks, sharply struck cymbals, digital clicks).

### 2. **Exploiting Both Oscillators for Polyrhythmic Layers**

- Use the **primary oscillator** for one main percussive tonal layer (e.g., "kick" or "clap" style), and the **secondary oscillator** (which also runs into LFO range) as a secondary percussive voice (e.g., hats, clicks, toms), or as a frequency modulation (FM) or audio-rate modulation source for gritty, metallic attacks.
- *FM Patching:* Use the FM CV and onboard VCAs to route each oscillator to modulate the other’s frequency. Use clocked/random CV to "play" the FM depth in time with your rhythms.
- Sequence pitch and FM depth independently via external sequencers running in different time signatures for polyrhythmic percussion.

### 3. **Modulation Matrix: Voltage Controlled Routers for Complexity**

- **Dual Matrix Routing:** Patch stepped random from the modulation section, clocked LFOs, or external CV sources to the *In A* and *In B* jacks. Use the source switches to assign modulation to blade/pulse width, FM, timbre, or dynamics destinations—making each percussive hit behave differently.
- Use external sequencers, euclidean pattern generators, or clock dividers/multipliers to send irregular gates or CVs to any modulation path: blade/pulse shape, LPG dynamics, FM, etc.—enabling you to add microtiming shifts and pseudo-randomness to every beat.

### 4. **Sound Design Tricks for Unique Punch and Character**

- **Layered Strikes:** Combine oscillator waveforms in the external or contour mixer, e.g., blend saw and sub for a "fatter" transient, or stack sine from one oscillator and square from another for a tabla-like knock.
- **Impulse Input to LPG:** Use very short triggers for sharp, pointillistic percussion, and longer gates for boomy, decay-heavy hits.
- **CV Modulation Depth as Performance Parameter:** Use voltage controlled routers to fade modulation in and out, either manually or with slow LFO/envelope—perfect for building up or breaking down polyrhythmic intensity live.
- **Random/Noise for Variation:** The built-in noise and random sources, routed through the contour or LPG, can add hi-hat or shaker type elements, or make claps/toms/other percussions unpredictable and lively.

### 5. **Patch Examples for Hyper-Complex Percussion**

#### *Example 1: Polyrhythmic Kick + Snare*

1. **Kick**:  
   - Sine out from primary oscillator → In 1 on contour mixer.
   - CV the LPG * Dynamics* with a synced but offset (polyrhythmic) envelope or gate.
   - Modulate pitch for "glitchy" kicks using random stepped CV in polyrhythmic clock.

2. **Snare/Clap**:  
   - Noise → In 2.
   - Impulse input triggers with a different rhythmic pattern (e.g., 5 against 4).
   - Vary timbre and dynamics CV per hit.

#### *Example 2: Ever-Evolving Percussive Texture*
- Mixer both oscillators with wildly different FM modulation (main osc modulates secondary, vice versa; sequence FM depth in a changing pattern).
- Square LFO or stepped random modulates blade/pulse shape AND LPG dynamics, creating complex, morphing rhythms.
- Send periodic random pulses to the LPG impulse input at rates untethered from your main clock—new percussive attacks appear at (almost) unpredictable times.

---

## Summing Up

The Double Helix is *prime* for dense, polyrhythmic modular percussion by combining:
- Deep analog wave shaping,
- Sine-to-folded-to-noise sound design,
- LPG for organic dynamic responses,
- And a versatile, performable modulation matrix perfect for clocked, divided, or random control sources.

**Pro Tip:** Use external logic modules, clock skippers/dividers, and algorithmic trigger sequencers for even more pattern complexity fed into the CV and impulse inputs.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)