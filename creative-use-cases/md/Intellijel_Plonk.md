# Intellijel — Plonk

- [Manual PDF](../../manuals/plonk_manual_v1.16_2020.11.08.pdf)

---

[Plonk Physical Modeling Percussion Synthesizer Manual (PDF)](https://intellijel.com/downloads/manuals/plonk_manual_1.16.pdf)

---

# Creative Eurorack Patching with Intellijel Plonk

The Intellijel Plonk is a deep and unique percussion module utilizing physical modeling techniques, making it ideal both as a realistic percussive sound source and as a wild, modular-centric experimental tool. Below, you'll find creative patch ideas and module combination suggestions to unlock new sonic territory.

---

## 1. **Dynamic Kits & Live Performance Switching**
**Idea:** Use the MOD input set to "Preset Step" and feed it voltage from a sequencer (like [Malekko Voltage Block](https://malekkoheavyindustry.com/product/voltage-block/), [Make Noise Pressure Points](https://makenoisemusic.com/modules/pressure-points)), or a random source, to morph between banks of related sounds ("kits") in real time.

- **Pro tip:** Group presets as kits (Kick, Snare, Hi-hat, Perc FX) and automate switching so that every trigger produces a unique percussive element.
- **Bonus:** Use a clock-divider ([4ms RCD](https://4mscompany.com/products/rcd)) to switch kits every bar, or for complex polymetric switching.

---

## 2. **Naturalistic Velocity Modulation**
**Idea:** Patch a random stepped voltage or envelope generator (e.g., [Mutable Instruments Marbles](https://mutable-instruments.net/modules/marbles/), [Intellijel Quadrax](https://intellijel.com/eurorack-modules/quadrax/)) to the VEL input for dynamic accenting and humanized grooves.

- Set VEL mode to "dynamics" for realistic articulations.
- Try a touch controller ([Make Noise 0-CTRL](https://makenoisemusic.com/synthesizers/0-ctrl)) for real-time manual dynamics.

---

## 3. **Physical Modeling "FM" with External CV**
**Idea:** Assign the MOD, X, or Y input to "R Pitch (Resonator Pitch e.g. 'FM')" and frequency-modulate the model with a fast LFO ([Intellijel Dixie II+](https://intellijel.com/eurorack-modules/dixie-2-plus/)), audio oscillator, or random source for metallic, warped, or outlandish sounds.

- Set short DECAY for percussive "carrier" FM/East Coast x West Coast fusion.
- Use stepped random to create randomized, every-hit-different percussion.

---

## 4. **Evolving Textures via Morphing**
**Idea:** Assign MOD to "Morph," and fading between two wildly divergent presets with a slow LFO ([Mutable Instruments Tides](https://mutable-instruments.net/modules/tides/), [XAOC Batumi](https://xaocdevices.com/product/batumi/)) or sequenced envelope for slowly shifting percussive timbres or bowed/struck hybrids.

---

## 5. **"Choke" Techniques for Rhythmic Control**
**Idea:** Patch a gate from another percussion module or track (e.g., hi-hat trigger) to the MOD input with destination "Choke Noise"/"Choke Res"/"Choke Both" to implement tight hats, open/closed hi-hat trills, or articulate rhythmic cutoffs.

---

## 6. **Processing External Audio through Plonk**
- **Not directly possible**, as Plonk does not accept audio input for the resonator. But you can use Plonk's outs as a "triggered exciter" alongside other resonator modules, like [Mutable Instruments Rings](https://mutable-instruments.net/modules/rings/) or [Physical Modelling FX modules](https://www.synthtech.com/eurorack/E352), for creative layering and call-and-response patches.

---

## 7. **Self-Modulation & CV Feedback**
**Idea:** Take Plonk’s OUT and mult (split) it to an envelope follower ([Doepfer A-119](https://www.doepfer.de/a119.htm), [Mutable Instruments Ears](https://mutable-instruments.net/modules/ears/)), then feed that CV to the MOD/X/Y input mapped to parameters like "Noise Density" or "Resonator Decay" for audio-reactive, evolving percussion.

---

## 8. **Drum Brains in a Full Modular Kit**
**Idea:** Use multiple Plonk modules—each loaded with different preset kits (one for drums, one for tuned percussion, one for textural/FX hits)—sequenced by a euro-drum sequencer ([Endorphin.es Ground Control](https://endorphin.es/modules/ground-control.html), [Intellijel Metropolix](https://intellijel.com/eurorack-modules/metropolix/)), and mix for full modular drum set.

---

## 9. **Auxiliary FX Processing**
- **Pass Plonk’s OUT through LPGs, wavefolders, or granular processors ([Make Noise Mimeophon](https://makenoisemusic.com/modules/mimeophon), [Mutable Instruments Clouds](https://mutable-instruments.net/modules/clouds/), [Happy Nerding FX Aid](https://www.happynerding.com/category/fx-aid/))** to extend the range from natural percussion to lush, shimmering drones or digital chaos.

---

## 10. **Algorithmic & Euclidean Percussion**
**Idea:** Use a Euclidean rhythm generator ([Euclidean Circles](https://vpme.de/euclidean-circles/), [Pamela's PRO Workout](https://busycircuits.com/alm017/)) to trigger Plonk, modulating parameters with CV for polyrhythms and cross-rhythmic percussive patterns.

---

### **Module Type Recommendations**

- **Sequencers:** for note, velocity, and MOD (Voltage Block, Circadian Rhythms, Eloquencer).
- **Random/Chaos Generators:** for generative modulation (Marbles, Wogglebug, Sapél).
- **LFOs/Envelopes:** for morphing and dynamic parameter movement (Quadrax, Batumi, Zadar).
- **Attenuverters/Mixers:** to combine and tame CV going into Plonk (Mutable Shades, Intellijel Triatt).
- **Envelope Followers:** for self-modulation or external reactive patches.
- **Drum Mixers & VCAs:** to blend, process, and effect multiple Plonk voices or kits.

---

## Advanced Tip

**Preset Randomization for Inspiration:**  
Assign "Randomize" to the MOD input and send random or clocked gates for instantly new, wild percussion—great for generative or experimental sessions.

---

> [**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)