# IO Labs — Flux Sequencer

- [Manual PDF](../../manuals/IO Labs - Flux Sequencer - 107 User Manual.pdf)

---

[**IOLabs FLUX Open Beta V1.07 User Manual (PDF)**](https://iolabs.co.uk/downloads/FLUX_OPEN_BETA_USER_MANUAL.pdf)

---

# Using IOLabs FLUX for Hyper-Complex, Densely Rhythmic Percussion in Eurorack

FLUX is one of the most advanced Eurorack rhythm sequencers available. Its Temporal Modulation Synthesis® (TMS) engine allows you to break away from conventional grid-based sequencers, creating dense, intricate, and organic percussion patterns. Here’s how you can exploit its features as a modular artist seeking the edge of rhythmic experimentation:

## 1. **Temporal Modulation Synthesis®: Foundation for Polyrhythm and Complexity**

- **Curvature Control (`CURV`, `VAL`):** Manipulate the distribution of triggers within a step to create exponential (VAL > 0), linear (VAL = 0), or logarithmic (VAL < 0) placements. Combine with high density (`DENS`) settings to push into millisecond territories for glitchy micro-structure or fluid, rushing drum clusters.
    - _Tip:_ Negative `VAL` for log-compressed bursts, positive for stretched, crackling cascades.

- **Freeform Step Lengths and Densities:** Each channel and step may have its own `LENG` (length) and `DENS` (density). Assign odd values (e.g., 7, 11, 13) on different channels—layering 5 against 7, or 13 against 8, unlocks cross-rhythms and polyrhythms not possible on standard grids.
    - _Example:_ Ch1: 11 steps, Ch2: 7 steps, Ch3: 16 steps, Ch4: 13 steps.

- **Phase (`PHAS`) and Compression (`COMP`):** Phase-shift events within steps for offset grooves. Use compression/expansion to bunch or space triggers unpredictably for evolving, dynamic patterns.

## 2. **Masking, Modulation, and Algorithmic Variation**

- **Mute Masks (`MASK`, `MSK>`):** Step-level logical masks (e.g., “1in2”, “2in3”) can stochastically/algorithmically drop or shift triggers, lending organic unpredictability reminiscent of human improvisation.
- **Auxiliary Outputs (`AUX1`, `AUX2`):** Deploy logic-based outputs (Boolean AND/OR/XOR etc) to generate related rhythmic lines, complex clock divs, or sidechain triggers for punchy ducking FX.
    - AGGRESSIVE HYPER EDIT: Use Boolean logic to create irregular, interlocking secondary percussion from main tracks.

## 3. **Deep Modulation** 

- **Macro Pots & CV Inputs:** Assign Macro Pots or external CV to virtually any parameter. Use attenuverters in the modulation matrix for extreme, dynamic modulation of density, curve, or mask parameters—twist, automate, or voltage-control your way into evolving, restless patterns.
- **Evolve LFO System:** Up to 85 recallable LFOs per preset modulate any step/parameter. Use them to morph density, mask, probability, compression, etc., creating polyrhythmic evolving landscapes and generative structures.
- **Multi-Bus System:** Assign up to three independent modulation buses per step for selective modulation—enables step-by-step algorithmic or performative variation; switch which mod sources are active at each position.

## 4. **CV Outputs as Percussion Modulation**

- **Step-based CV Envelopes, LFOs, Randoms:** CV outputs can fire envelopes or voltages per step/trigger for unique dynamics—patch to VCA, filter, or modulation inputs on your voices for timbral or amplitude modulation that “breathes” with the groove.
- **Quantization Per Step:** Quantize CV to scales, and even mask specific scale degrees per step for evolving pitch/sequenced percussion tone changes.
- **Random per Trigger (RANDT):** Assign new random voltage on every trigger for wild micro-modulation of percussion synth voices.

## 5. **Hyper Dense/Groove Tricks**

- **Extreme Densities (`DENS` > 32):** Go beyond drum machine possibilities. Experiment with how your percussion sound source responds to bursts at audio rates—filtered noise, analog drum modules, or even effect inputs can create 'crunchy grain' sounds.
    - _Caution:_ Watch for "dropped triggers" if connected voices can’t keep up. Use density and compression to tune for taste.

- **Humanize (`HUMA`):** Range 1–127 for subtle to wild microtiming randomization—perfect for shifting between cybernetic precision and swinging, "drunk" rhythms.

- **Probability (`PROB`):** Set per step or per trigger for controlled chaos.

## 6. **Presets, Scenes, and Morphing**

- **Rapid Preset Load/Save:** Use µSD presets to swap between entire song structures, dense to sparse, glitch to groove. 
- **Performance Use:** Assign parameters to Macro Pots and morph them live, or sequence via external CV.

## 7. **Integrative/Sync Capabilities**

- **Polyrhythmic MIDI + Modular:** Send MIDI for digital drums or DAW sync, while CV/gates pulse analog gear.
- **Burst Mode:** For drum fills, ratchets, triggered outbursts, or generative staccato “clouds” of events.

## 8. **Voice/Effector Manipulation (If FLUX is Part of Voice Chain)**

While FLUX is a sequencer, these tricks apply:
- Use output CV to modulate morph parameters on wavetable, FM, or physical modeling modules—extract pseudo-musical patterns from pure rhythm.
- Gate density to trigger 'freeze'/'granule' functions in effects, or hard/soft clip modules for extra punch.

---

### **Practical Example Patches**

1. **Triplet Against 5/4 Bass Drum Polyrhythm:**
   - CH1 (Kick): LENG = 5, DENS = 5, CURV = -0.8, PHAS = 0%
   - CH2 (Snare): LENG = 3, DENS = 3, CURV = 0.5, COMP = 20%
   - CH3 (HiHat): LENG = 8, DENS = 7, MASK = 2in3
   - CH4 (Perc): LENG = 13, DENS = 11, CURV = 0.2, Macro Pot mod on DENS

2. **Evolving Percussion Cloud:**
   - All channels: LENG = 16
   - DENS modulated by Evolve LFOs (different freq/waveform, out of phase)
   - CURV, VAL, and MASK modulated by separate Macro Pots
   - CV OUT: ENV mode to modulate VCA input on percussive voices for living amplitude movement

3. **Boolean Logic Groove-Echos:**
   - AUX1: DEL3 (delayed trigger)
   - AUX2: & (AND, triggers only if both main outs of CH1+CH3 active)
   - Use as side-trigger for FX or accent channel

---

# Resources

* [**Official Flux Manual PDF**](https://iolabs.co.uk/downloads/FLUX_OPEN_BETA_USER_MANUAL.pdf)
* [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
