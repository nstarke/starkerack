# Black Noise — Cosmos

- [Manual PDF](../../manuals/BLACK-NOISE_COSMOS_User-Manual_V1.pdf)

---

[Download the COSMOS Manual (PDF)](https://blacknoisemodular.com/manuals/COSMOS_USERMANUAL.pdf)

---

# COSMOS by Black Noise — Creative Patch Ideas for Eurorack Musicians

The Black Noise COSMOS is a hyper-flexible multifunction analog processor, giving you a dense playground of logic, wave shaping, mixing, and CV manipulation. Here are some creative patch strategies, inspirations, and combo ideas to expand your sonic palette.

---

## 1. **Logic-Based Groove Engines**
**Modules to Use:**
- Clock divider/multiplier (e.g. Pamela's Pro Workout, 4ms Rotating Clock Divider)
- Random source (e.g. Mutable Instruments Marbles)
- Probability gates (e.g. Branches, Erica Pico Random)

**Patch Approach:**
Sequence a few different rhythm sources into the COSMOS. Use the XOR, AND, OR, and their inverted forms to create complex rhythmic triggers. Kick out new, evolving grooves or probability-based drum hits, routing the COSMOS’s logic/trig outputs to drum modules or envelopes.

**Pro Tip:** Self-patch inverted outputs back into other logic inputs for highly syncopated results. Modulate the thresholds with subtle LFOs for dynamically shifting patterns.

---

## 2. **Hybrid Analog Logic/Audio Sculpting**
**Modules to Use:**
- Audio oscillator (e.g. Intellijel Dixie II+, Doepfer A-110)
- Offset/attenuverter (e.g. Happy Nerding 3x MIA, Tiptop MISO)
- Wavefolder (e.g. Serge Wave Multiplier, Joranalogue Fold 6)

**Patch Approach:**
Feed an audio oscillator and a shaped LFO into X and Y. Use the Max/Min outputs as analog wave selectors, then process those with additional folders or wave shapers.

**Pro Tip:** Send an envelope into one input and audio into the other—the result is a dynamic wave shaping or amplitude modulation, but with more character than a classic VCA.

---

## 3. **Analog Comparator-Based Routing**
**Modules to Use:**
- Voltage controlled switches (e.g. Doepfer A-150, WMD SSM)
- Sequential switch (e.g. Doepfer A-151)
- Slew limiter/envelope follower (e.g. Maths, Doepfer A-171-2)

**Patch Approach:**
Let audio or CV signals coming from other voices pass through the comparator or window comparator functions of COSMOS. Use outputs to trigger switches, muting, rerouting, or activating effects chains when certain values are crossed.

**Pro Tip:** Use window comparator to create "zone" effects—e.g., only when LFO is at mid point, an extra reverb gets activated.

---

## 4. **Analog PLL-Sync and Harmonic Exploration**
**Modules to Use:**
- Complex oscillator (e.g. Make Noise DPO, Verbos Complex Oscillator)
- Slew/lag processors (e.g. Mutable Instruments Stages, Pittsburgh Modular Function)
- External instrument interface (for guitar/mic input)

**Patch Approach:**
Send VCO and external sound source into X and Y inputs. Patch through the "Through Zero Clipper" gate and feed back via a slew for analog phase-locked loops—achieve wild, voltage-controllable oscillator sync, and CV the slew for instant modulation of PLL “elasticity.”

**Pro Tip:** Use with a contact mic, voice, or guitar—track pitch with PLL and get vocoder or talkbox-like synthesis without a traditional vocoder.

---

## 5. **Custom Envelope Creators**
**Modules to Use:**
- Dual envelopes (e.g. Make Noise Maths, Intellijel Quadrax)
- End-of-cycle logic outs (EOC/EOF triggers available on AD/AR envelopes)

**Patch Approach:**
Feed separate envelopes into X and Y. The MIN and MAX outs become powerful, non-linear envelope combiners for percussive sounds, evolving drones, or complex amplitude curves. Pipe these curves into your VCA or filter cutoff.

**Pro Tip:** Use CLAMP outputs for envelope following with natural compression/saturation for punchy drums or dynamic effects.

---

## 6. **Clock/Trigger Processors with Swing and Delay**
**Modules to Use:**
- Trigger delay (e.g. 2hp Trigger Delay, Mutable Stages)
- Accent generators
- CV mixers for swing adjustment

**Patch Approach:**
Route your clock/gate patterns into COSMOS. Use the clock multiplier patches as a source of swing and shuffled triggers, or use NOR/OR trigs with a mixer to build complex metrical variations.

**Pro Tip:** Patch output to a trigger sequencer or burst generator for ratcheting and flam effects—especially potent when modulated by the same LFOs that are controlling your sequence.

---

## 7. **Experimental Random and Probabilistic Rhythm Generation**
**Modules to Use:**
- Noise source + S&H (e.g. Mutable Marbles, Wogglebug)
- Clocked random generators

**Patch Approach:**
Feed noise or S&H voltages plus a clock into the inputs and use XOR/AND gating for random rhythm bursts. Output provides unpredictable, yet musically useful, probabilistic triggers.

**Pro Tip:** Use attenuated S&H voltages or LFOs to bias the probability “window” for controllable, semi-random groove or drum sequencing.

---

## 8. **Touch-Plate Performance Control**
**Modules to Use:** 
- No extra modules required, but surface controllers like Make Noise Pressure Points or Random*Source Serge TKB can be complementary.

**Patch Approach:**
Leave an input unpatched for touch-plate control. Perform live, injecting gestural CV, triggering gates, or biasing logic functions with your fingers—great for live fills and morphing transitions.

---

## 9. **Waveshaping and Synthesis Cross-Modulation**
**Modules to Use:**
- Crossfader (e.g. Befaco Hexmix VCA, ALM Tangle Quartet)
- VCAs/LPGs (e.g. Natural Gate, Intellijel Quad VCA)
- Stereo panners

**Patch Approach:**
Mix two independent audio rates or complex LFOs through COSMOS, then use Min/Max, TZ Clipper, or Multi-out arrangements for animated cross-modulation: ring mod, amplitude mod, and logical wave folding. Sending these through more VCAs and panners can create lush stereo or spatial effects.

---

## 10. **Analog Compressor/Sidechain with Flavor**
**Modules to Use:** 
- Envelope follower and VCA
- Audio source (e.g. kick drum)
- Mixer

**Patch Approach:**
Send your main audio to X, sidechain/envelope to Y. Use the MAX or OR gate outs to control VCAs downstream, achieving sidechain pumping and analog compression. The COSMOS can act much like a musical analog comparator-compressor.

---

## More Resources

- [COSMOS Official Manual (PDF)](https://blacknoisemodular.com/manuals/COSMOS_USERMANUAL.pdf)
- Keep an eye on [the Black Noise modular site](https://blacknoisemodular.com/) for new patch ideas and tips.

---

*Generated With Eurorack Processor*: [https://github.com/nstarke/eurorack-processor](https://github.com/nstarke/eurorack-processor)