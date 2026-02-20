# Bored Brain — EQx5

- [Manual PDF](../../manuals/EQx5-UserGuide_1.0.pdf)

---

[Download the bordbrain eqx5 Manual (PDF)](https://boredbrainmusic.com/wp-content/uploads/2022/09/eqx5_manual.pdf)

# Creative Modulation Techniques for the Boredbrain eqx5

The **Boredbrain eqx5** is a five-band voltage-controlled equalizer (EQ) in Eurorack format. Each band can be modulated with CV, and the module features additional level and balance controls for both manual and CV operation. Here’s how you can exploit its capabilities to generate everything from crunchy percussive hits to wild basslines and eerie textures.

---

## 1. Distorted Percussive Sounds

**Key Features To Use:**  
- Five CV-controllable EQ band levels  
- LEVEL CV input with full-range gain and soft-saturation  
- CV input summing (modulate multiple bands and master level simultaneously)

**Patch ideas:**

- **Transient Sculpting:** Patch envelopes (from your ADSR module or Maths) into the **CV IN** jacks of the mid-high or high bands. This will cause percussive hits to have “snap” or “sparkle” as envelope modulation boosts those bands on transients.
- **Distorted Body:** Patch a drum source into the eqx5 input. Use a separate envelope to modulate the **LEVEL CV IN** for overall level modulation, pushing it into the saturation region for quick moments (see "Soft-Saturation" in manual). Adjust the output (OUT) to taste.
- **Extreme Band Boosts:** Use *random voltages* or stepped sequencer as CV into multiple band inputs simultaneously. Push high and low bands to extremes – the internal clipping and EQ filtering will yield gnarly, destroyed timbres.

**Bonus:**  
Try patching the output back into itself through a wavefolder, filter, or external distortion to further mangle the sound.

---

## 2. Crazy Dubstep/Drum & Bass Basslines

**Key Features To Use:**  
- CV control over each frequency band  
- HIGH BAND at 4.8 kHz, LOW BAND at 58 Hz – great for shaping “wobble”  
- LEVEL balance and summing

**Patch ideas:**

- **Wobble Bass:** Route a sub oscillator into eqx5. Patch an LFO (sync to your tempo) into the **LOW MID** or **LOW** band **CV IN** to wobble the frequency emphasis. For wilder movement, layer several LFOs via a CV mixer or stack multiple patch cables at once.
- **Rhythmic Band Swiping:** Use a synced or unsynced sequencer with random/sample & hold to jack voltage into different band CVs in time. Try modulating MID band heavily for a talking/wow effect.
- **Growl FX:** Combine fast LFO (8-20 Hz) to modulate the **HIGH MID** or **MID** bands while modulating the **LEVEL** CV with a slow envelope or LFO for pulsating movements.
- **Distorted Bass:** Slam the input with a saturated, loud sine wave and push the **LEVEL** control high enough for soft saturation as described in the manual.

---

## 3. Atmospheric Pads/Haunting Textures

**Key Features To Use:**
- Wide-range CV per band (±5 V; can be subdued or exaggerated for slow, unpredictable movement)
- Smooth analog equalizer response
- BALANCE A/B (CV or manual): morphs between two EQ shapes for morphing pads

**Patch ideas:**

- **Morphing EQ Pad:** Patch a long reverb or pad source through eqx5. Set up two different EQ curves on A and B. Use a slow-moving LFO or random voltage into **BALANCE CV IN**. The pad will smoothly morph between “dark and boomy” to “bright and thin,” creating movement and suspense.
- **Band Drift:** Use several slow, out-of-phase LFOs or chaos/random sources to modulate each band’s CV input. The resulting pad will always have gently shifting frequency content — perfect for drones or ambient backgrounds.
- **Freezing Winds:** For a ghostly effect, boost high and high-mid bands while cutting lows. Modulate bands slowly with random CV, emphasizing the “air” in source material. Add fine saturation via the **LEVEL** knob for extra grit and presence.

---

## Modulation Pro Tips

- **VCA Before CV:** Use a VCA to scale CV inputs, giving hands-on or velocity/expression-based control over the amount of modulation depth for each band.
- **Feedback:** Patch the eqx5 output into a delay/reverb and feed some of it back through the input—modulate band CVs to constantly transform the repeated wall of sound.
- **Sum CVs:** Stack multiple CV sources into each band’s CV input (passive multi or buffered mult), making extremely rich, unpredictable spectra.

---

For more patch ideas and utilities, check out the [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor).