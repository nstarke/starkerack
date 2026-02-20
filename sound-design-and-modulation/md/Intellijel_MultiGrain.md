# Intellijel — MultiGrain

- [Manual PDF](../../manuals/multigrain_manual_v1.2_2025.09.02.pdf)

---

[Download the Intellijel Multigrain Manual (PDF)](attachment-from-user)

---

# Creative Modulation with Intellijel Multigrain v1.2

> **Goal:** Design patch ideas and modulation workflows with Intellijel Multigrain to create…
> - Distorted Percussive Sounds
> - Wild, Modulated Basslines (Dubstep/Neuro/Drum&Bass)
> - Haunting Atmospheric Pads

This analysis pulls directly from the features and functions mapped in the manual—and exploits Multigrain’s unique real-time granular modulation, CV assignment, morphing, and the new Live Sound/Looping Recorder!

---

## 1. General Modulation Framework

**Assignable CV inputs:**  
- X, Y, Z (±10V) — can modulate ANY knob parameter, or REVERSE toggle.  
- Dedicated:  
   - GATE = trigger grains
   - NEXT = step through sounds (or SCAN reset, see below)
   - SELECT = Sound select via CV
   - MORPH CV (±10V, with attenuverter)
   - SYNC = External clock/quants

**Morphing:**  
Each Sound has two Scenes (A/B). You can morph the grain engine’s parameters between ANY two states, by fader or CV:  
- Create drastic contrasts between A & B, and sweep or automate between them for wild timbral movement.
- Modulation assignments can also be morphed (different attenuverter values per scene!).

**Random Modulation:**  
- Internally generated, assignable to ANY parameter.
- Unipolar/bipolar modes selectable.
- Use negative random on LEVEL/TONE for L/R panning craziness.
- RATE randomization introduces stochastic/percussive patterns.

**Key CV/Modulation Shortcuts:**
- Assign CV live: Hold X/Y/Z/RAND, turn parameter to set amount/polarity.
- Control all sounds/scenes: Hold LATCH and/or SCENE.
- Quick randomization: Hold RAND + any button.
- Modulate Freeze on Looper: Assign CV/RAND to ◎SAMPLE in mod page.

---

## 2. Patch Design Recipes

### a) **Distorted Percussive Sounds**

**Sample:**
- Use one-shots, dense transient-rich samples, or drums with abrupt attacks.
- Make sure to trim/start at transient (use advanced sampling page as needed).

**Parameter & Modulation Suggestions:**
- **SIZE:** Set very short (30–100ms). Randomize SIZE for variable hits (assign RAND, ~30–50%).
- **RATE:** Set 0Hz to 20Hz. Try enabling RATE–SIZE link for more glitch artifacts.
- **SHAPE:** Use DECAY, SQUARE, TRI or very sharp window shapes.
- **LEVEL:** Modulate with short, negative/positive envelopes or LFOs for amplitude stuttering.
- **PITCH:** Randomize for tonal irregularity. For metallic percussion, use PITCH + Quantizer to force chromatic percussive notes.
- **REVERSE:** Assign X/Y/Z as triggers, or modulate via RAND for unpredictable reversing.
- **THRU + BLUR:** Disable BLUR send for dry, snappy output. Enable when you want ghostly tails.

**Further tips:**
- Modulate **SCAN** or **START** at audio rate or with envelopes—this "scrubs" the sample for weird, choppy effects (think distorted glitch hats or FM percussion!).
- Use external envelopes or step sequencer CV to **LEVEL** and **PITCH** for synthetic kicks/snares.
- Overlap many grains (high RATE, smaller SIZE) for "buzz" and smearing distortion.

**Experimental:**  
Use Live Sound mode, freeze the Looper, modulate Freeze with an envelope—this gives quasi-granular gating on live input.

---

### b) **Crazy Basslines (Dubstep/Neuro/Drum&Bass Styles)**

**Sample:**
- Use resampled synth patches, single bass notes, or dirty reece/wub samples.
- Mono or stereo—stereo files enable more stereo modulation tricks!

**Parameter & Modulation Suggestions:**
- **PITCH:** Assign a sequencer or Voltage source (1V/Oct possible with 100% mod assign). Combine with unquantized or scale-locked Quantizer mode for scales/riffs.
- **SIZE-PITCH LINK:** Enable to stretch/squeeze grains in sync with pitch moves—classic neuro/dubstep "time warping".
- **TONE:** Assign a strong LFO or envelope (or RAND in negative amount!) for moving filters; this mimics animated DnB/filter sweeps.
- **MORPH:** Make Scene A clean and B brutal with crushed/warped parameters, staggering reverb sends, or even max-level SIZE/WRAP.
- **SCAN/WRAP/START:** Modulate with stepped/random CV/LFO, especially when using rich samples—this alters which fragment of the sample each grain comes from (stuttery or constantly evolving texture).
- **BLUR:** Add subtle tails for width, or crank to max with Scene Morphing for "exploding" grains at phrase ends.
- **REVERSE:** Randomize sparsely for sudden, dizzying bass "sputter" glitches.
- **RATE:** Try mid-high for overlapping grain buzz. Use random mod (RAND– or RAND+) for breakbeat/rhythmic shuffle artifacts.

**Experimental:**  
- *"Scatter Basses"*: High RATE, small SIZE, aggressive modulation of PITCH and START synchronized to drum triggers.
- *"Wub Animation"*: Morph between clean and wobble scenes with the fader or sequencer CV to MORPH input.
- *Random Pan*: Assign negative RAND to LEVEL/TONE for psychoacoustic stereo spread.

---

### c) **Atmospheric Pads and Haunting Textures**

**Sample:**
- Use evolving drones, field recordings, extended instrument notes (cello, flute, guitar harmonics), vocal washes, or full ambient loops.

**Parameter & Modulation Suggestions:**
- **SIZE:** Slow, 500ms–3sec grains. Scene A (long, soft), Scene B (short, sharp, for morphing tension/relaxation).
- **RATE:** Low values (<2Hz) for sparse pointillism, or higher for dense, smudgy clouds.
- **SHAPE:** BELL, TUKEY, SINE for soft fade-ins/outs.
- **START/SCAN/WRAP:** Apply S&H (sample/hold) or smooth LFO CV for gently shifting position through the soundscape.
- **RAND Modulation:** Dust all parameters with 10–30% RAND for organic, evolving movement.
- **BLUR:** Use heavy blur (reverb send) for endless tails.
- **REVERSE:** Sparingly assign to mod/X/Y/Z for ghostly reversed fog.
- **TONE:** Lowpass for dark, HP or modulated for ethereal "whisps".
- **Live Sound Mode:** Use looping recorder to grain-up incoming synth drones, freeze/unfreeze with footswitch or random triggers for everchanging pads.

**Experimental:**  
- Morph between two contrasting pad textures (e.g., bright violin and low cello sample, or urban field recording and pure synth pad).  
- Modulate BLUR send in sync with scene morph to swell into deep reverbs on certain transitions.
- Quantize PITCH and assign light random to only blend specific notes—mysterious, semi-tonal pads.

---

## 3. Advanced Play & Tips

- **Assign Modulation Smartly:** Layer slow LFOs, step-random sequences, and rapid envelopes to different parameters for multidimensional evolution.
- **Morph Dynamic Movement:** Don’t forget that MOD attenuation per Scene is also morphable—use this for "animated" modulation depth transitions.
- **Grain Engine as FX with Live Sound:** Use Live Sound as a real-time FX processor; send percussion, synth, or voice through it, modulate everything for glitching, granulating madness.
- **SYNC Input:** For clocked effects, drive RATE (and Scan/Wrap on Looper) from drum machine or sequencer clock.
- **Mod Output as Feedback Loop:** Use A/B mod outputs to drive further modulation—e.g., envelope out to mod PITCH of another sound source in your rack.

---

**For more patching ideas:**
- Skim the "Shortcuts and Combos" in the manual (page 53+).
- Use the RAND button for rapid, happy accidents!

---

**Manual Link:**  
[Attachment from user (PDF)](attachment-from-user)

**Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)**

---