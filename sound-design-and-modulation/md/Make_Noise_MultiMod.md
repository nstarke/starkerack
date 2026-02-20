# Make Noise — MultiMod

- [Manual PDF](../../manuals/multimod-manual.pdf)

---

[**Download the Make Noise MultiMod Manual (PDF)**](https://makenoisemusic.com/manuals/multimodmanual.pdf)

---

# Make Noise MultiMod Creative Modulation Tips

Below are focused strategies for patching the Make Noise **MultiMod** to generate distorted percussion, complex wobble basslines, and evolving atmospheric pads, based on your manual’s features and tips:

---

## **1. Distorted Percussive Sounds**

- **Stepped Random Shapes:**  
  - Select the Orange "Stepped Random" shape. This generates abrupt voltage changes at each channel, perfect for glitchy and unpredictable percussive elements.
  - Modulate the **Time** parameter with audio-rate CV for extra aliasing and digital artifacts.
- **Hold Function:**  
  - Use the **Hold** feature, activated by a gate from another module, to freeze and loop transient CV bursts, turning smooth envelopes into sharp, ghostly repeats—excellent for metallic or stuttered percussion.
- **Spread + Time for Transient Smearing:**  
  - Set **Spread** away from noon so channels are running at various speeds—some sped up, some slowed-down versions of the same trigger CV. Run outputs to percussive voice decay or distortion amount.  
  - Modulate **Time** manually or via CV for shifted, smeared percussive impacts resembling industrial hits.
- **Square Shape as Pulses:**  
  - With nothing patched to Signal In, use Pink “Square” shape for clocked pulses (variable divisions/multiples at outputs), then run each into VCA amplitude or filter cutoff—all will hit at different times.  
  - Drive results through a wavefolder or hard clipping for digital overtones.

**Patch Example:**  
Noise source → MultiMod Signal In; set Shape = Stepped Random; Spread = maximal; outputs to VCA CVs or drum parameters; modulate Time from an envelope or audio-rate oscillator; trigger Hold with snare/rim/click for frozen glitch accents.

---

## **2. Crazy Dubstep/Drum & Bass Basslines**

- **Phase Ablation:**  
  - Use the **Phase** parameter to steadily modulate the relative timings of each bass movement. Assign a synced LFO or envelope into Phase CV in, and automate the knob for shifting, warping bass waves.
- **Internal LFO Mode:**  
  - Leave Signal In empty—set the read Shape to **Sine, Ramp, or Triangle**. Use Time and Spread to generate wobbly, ever-changing movement.  
  - CV control Time with your sequencer’s gate or accent output for rhythmic “woof” or growling bass pulses.
- **Spread for Harmonic Wobble:**  
  - Set Spread so some channels move faster and others slower—patch several outputs to different oscillator FM inputs, filter cutoff, or wavefolder depth. Their combined modulation will sound like a “herd” of LFOs running at clock-divided rates.
- **Sync and Resync:**  
  - Patch a Reset gate synced to your main drum rhythm into MultiMod’s Reset input. This keeps the mad bass movements locked to drops or rhythmic cadences—great for fills and wild “reset” effects.
- **Glitchy “Tape Head” Play:**  
  - Try “Ramplets” (Yellow) or “Ping-Pong” (Blue) shape for non-linear, backwards, or two-way playback—this creates unpredictable, wonky bass phrases.

**Patch Example:**  
MultiMod output 1 → main bass VCO FM; output 2 → filter cutoff; output 3 → VCA; Shape = Purple (Sine) or Blue (Ping Pong); modulate Spread with an envelope; Reset triggered each 4/8 bars for repeatable drop wobbles; control Time with a modulated LFO for dynamic energy.

---

## **3. Haunting Atmospheric Pads**

- **Smooth Random or Sine LFOs:**  
  - Set Shape to “Ramplets” (Yellow) or “Sine” (Purple)—with no signal in, get eight organically drifting LFOs.
  - Patch outputs to stereo imaging modules, filter resonance, reverb diffusion, or VCA amplitude for constantly evolving movement.
- **High Spread, Slow Time:**  
  - Set Spread to a high value (not at noon), and turn Time up (CW). Now each output evolves at its own rate, creating extended, non-repeating envelopes that can drift for minutes.
- **Ethereal “Tape Loop” Trick:**  
  - Use Hold to lock in a frozen modulation state, then slowly scan through Phase or Spread—patch resulting CVs to granular parameters, shimmer pitch, or reverb morphing for a woozy, submerged vibe.
- **Tempo Sync for Rhythmic Drones:**  
  - Patch in a slow external clock to Tempo In; now all channels drift but periodically re-align. Good for pads that “breathe” in sync but never repeat precisely.
- **Spatial Movement:**  
  - Channel Index out can be used to automate which of your eight pad voices (or audio effects) is emphasized, slowly moving spectral focus across your mix.

**Patch Example:**  
MultiMod outputs 1-8 → different voices’ filters and VCAs. Shape = Sine or Ramplets. Time = long. Spread = wide. Modulate Spread and Phase with S&H LFO or slow envelope. Option: Use Reset to periodically return drifting modulations to unity, momentarily aligning all layers for a “phantom orchestra” effect.

---

## **General Pro Tips**

- **Abuse Modulation:**
    - Patch audio-rate or random CVs into Phase/Spread/Time to push the MultiMod into digital distortion and glitch territory.
    - Extreme (beyond panel) CV values take channels up to x24 or /24 speeds for digital “shred.”
- **Tempo and Reset:**
    - Sync to external clocks/sequencers for musical control, or deliberately disrupt with offbeat Resets for organized chaos.
- **CV Mixing:**
    - Mix outputs with CV processors or crossfaders for morphing between movements.
    - Use outputs to modulate effects (delay, reverb, bitcrusher) for modulation across the FX tail, not just dry sound.

---

## **Summary Table**

| Musical Goal             | Shape           | Key Parameters | Patch Notes                                                      |
|------------------------- |-----------------|---------------|------------------------------------------------------------------|
| Distorted Percussion     | Stepped Random  | Time, Spread  | Use external noise/CV in, glitch with Hold, push Spread, reset   |
| Dubstep/DnB Bass         | Sine/Triangle   | Phase, Spread | Sync Time to rhythm, reset for drops, modulate FM/cutoff         |
| Haunting Pads            | Sine/Ramplets   | Time, Spread  | Slow Spread/Time, outputs to pads, sync Reset for alignment      |

---

**[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**