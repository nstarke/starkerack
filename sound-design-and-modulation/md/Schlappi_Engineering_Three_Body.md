# Schlappi Engineering — Three Body

- [Manual PDF](../../manuals/three_body_manual_01302023a.pdf)

---

[Download the Three Body Manual PDF (Schlappi Engineering)](https://schlappiengineering.com/manuals/ThreeBodyManual.pdf)

---

# Three Body Module: Creative Modulation Tips

As a fellow Eurorack musician, let's dive into how to wield the **Schlappi Engineering Three Body** for wild sound design—ranging from *wrecked percussion* to *dubstep/drum and bass basslines* to *eerie atmospheric pads*. Here are focused patch ideas and modulation strategies leveraging the module's unique features like through-zero FM/PM, phase relationships, and ratio tracking.

---

## 1. Distorted Percussive Sounds

### Principles  
- **Deep linear FM** and **phase cross-modulation** can create rich, noisy transient-laden tones.
- Using SYNC and RATIO modes enables metallic and evolving percussive qualities.
- Leverage the overdriven index/phase/fm VCAs, especially at audio rates.

### Patching Tips
**A. Snappy Metallic Hits**
- Put the **center oscillator** in FREE, HIGH mode (*acts as voice*).
- **Left and right oscillators** in RATIO mode, both track center, with div/mult settings to place them at non-integer ratios (e.g., 7:3 for clangorous partials).
- Feed a short envelope into FM INDEX or PHASE INDEX on the center oscillator.
- Try sending envelopes or triggers to outer oscillators' FM or PHASE inputs.
- Cross-modulate (patch left phase out to right phase in and vice versa) and push PHASE CV up just to the edge of noise.
- Use the outer oscillators’ sine/triangle outputs for additional ringy percussion layers.

**B. Fuzzy Toms or Kicks**
- Center in FREE, LOW for LFO or low-audio range.
- Short decay envelope into FM (lin) or PHASE to get warbly, laser-like decays.
- Increase linear FM index for "wub" or "boom" artifacts.
- Feed a noise burst or fast LFO into SYNC for pseudo-acoustic scrapes.

---

## 2. Crazy Basslines (Dubstep/Drum & Bass)

### Principles
- Exploit **through-zero linear FM for wild harmonic sweep**, **phase modulation for timbral animation**, and harsh ratio-locking for "tearing" sounds.
- Modulate the RATIO controls with sequenced CVs for stepwise or gliding pitch.

### Patching Tips
**A. Ripping Dubstep Basses**
- Center oscillator as modulator (FREE, HIGH), left or right as carrier (RATIO, HIGH/MULT).
- Use a clock or gate from a sequencer into SYNC to hard-sync the carrier for sharp, digital edges.
- LFO or envelope into FM INDEX or PHASE INDEX for movement—try modulating the modulation index itself with an envelope for evolving grit.
- Turn FM index up high—it will phase-reverse and melt the carrier into unpredictable digital chaos (classic "FM mayhem").
- Patch CV into VOCT/RATIO input on the carrier, use a random sequencer or stepped voltage to create octave jumps and "neuro" scale leaps.
- Try cross modulation between the outer oscillators for thick growl; back off if it gets too noisy.

**B. Reese Bass / Jungle Neuro Swerves**
- Set both outer oscillators in RATIO mode, center as modulator (FM or PHASE).
- Stereo patch: Take both outer sine (or triangle) outs for instant wide, moving sound.
- Use slow LFO on FM INDEX or PHASE to sweep harmonic content.
- For additional stereo movement, use the center cosine and sine outs panned hard left/right.

---

## 3. Haunting Atmospheric Pads

### Principles  
- Gentle **audio-rate phase modulation** and using the stereo outputs (center sine/cosine or saw/cosaw) yield lush, moving textures.
- Modulate ratios with slow LFOs or random stepped voltages for nonrepeating, evolving harmonics.

### Patching Tips
**A. Floating Pads with Shifting Harmonics**
- Center oscillator: FREE, LOW/HIGH depending on desired register.
- Outer oscillators: RATIO modes, set ratios to non-integer or overtone intervals (e.g., 5:3, 8:5).
- Modulate PHASE INDEX on the center with slow LFOs, envelopes, or aftertouch (if using a controller).
- Use both the sine and cosine outs from center oscillator; pan them for a natural stereo shimmer.
- Bring up some PHASE cross-modulation between outer oscillators for “swirling mist” effects.
- Feed slow random or LFOs to the outer oscillators’ VOCT/RATIO inputs for scale drift.
- If you want less harmonic richness, reduce FM/PHASE indexes and rely more on subtle ratio modulations.

**B. Binaural/Motion Effects**
- Exploit the *phase direction* header for true quadrature relationships and wide stereo.
- Use two LFOs with different frequencies modulating left and right phase indexes, while listening to center saw/cosaw outs.

---

## General Modulation Notes

- **Linear FM (lin):** Go deep for intense metallic and digital sounds, but rebounds into noisy regions quickly.
- **Phase modulation:** More harmonically “stable” than exponential FM—good for thick distortion or wavefold-like timbres.
- **Index modulation:** Automate the amount of modulation with external envelopes, for morphing, accent, or decay.
- **SYNC input in RATIO mode:** Hard sync for “brassy” resets; patch in external clocks, triggers, or even audio for quasi-ringmod and sample/hold effects.

---

## Bonus Tweaks

- Adjust **rear headers** (external filter, phase direction, square phase modulation) for advanced behaviors—e.g., thick sub fundamentals via unmodulated square, or true stereo phase operation.

- Experiment with self-patching: use outs from one oscillator to modulate itself via FM or PHASE, using VCAs/external attenuation for feedback control.

---

### Further Exploration

For more advanced signal processing or integrating Three Body in digital/hybrid workflows, check out [Eurorack Processor on Github](https://github.com/nstarke/eurorack-processor).

---

**Generated With Eurorack Processor**