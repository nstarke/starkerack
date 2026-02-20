# Moog — Labyrinth

- [Manual PDF](../../manuals/Labyrinth Manual.pdf)

---

[Moog Labyrinth User Manual (PDF)](https://www.moogmusic.com/sites/default/files/2024-05/Labyrinth_Manual_Web.pdf)

---

# Eurorack Modulation Strategies for Moog Labyrinth

As an experienced eurorack musician, here’s how you can push the Moog Labyrinth into uncharted territory—especially for **distorted percussion**, **aggressive basslines**, and **haunting pads**. Below you'll find modulation routing ideas, parameter tips, and patch bay tricks, all pulled directly from the structure and features described in the manual.

---

## 1. Distorted Percussive Sounds

### Key Parameters & Sections:
- **Wavefolder (VCW FOLD, VCW BIAS, EG1/CV AMT, SEQ1 AMT)**
- **Mixer (Drive oscillators beyond 12 o’clock)**
- **Envelope Generators (EG1/EG2 with short decay)**
- **Noise Generator (NOISE LVL, NOISE TONE)**

### Strategies
- **Inject Bold Harmonics:**  
  Use the **wavefolder** path exclusively (set ORDER to PARALLEL, BLEND to VCW side).  
  - Crank **VCW FOLD** past 12 o'clock for wild folding/distortion.
  - Modulate **VCW FOLD** with EG1 for snappy, percussive harmonic bursts: turn up **EG1/CV AMT**.
  - Play with **VCW BIAS** to skew asymmetry. For even gnarlier distortion, modulate this indirectly by routing the **MOD VCO** to the mix (per manual p. 21 "You can mimic voltage control of VCW BIAS...").

- **Add Envelope "Thwack":**
  - Set **EG1 DECAY** very short for both VCO and MOD VCO modulation for “clicky/plucky” impacts.
  - Use sequencer triggers from **EG TRIG MIX** (favoring one sequencer for rhythm).

- **Inject Noise & Ringmod:**
  - Raise **NOISE LVL** and dial NOISE TONE to taste for sizzly hats/snares.
  - Mix in some **RING MOD LVL** for metallic hits.

- **Patch Bay Extras:**
  - Patch an external LFO or gate into **VCW FOLD** for stepped distortion fuzz.
  - Try patching EG2 out to **BIT FLIP 1 or 2** for evolving, randomized percussion (see patch ideas in manual presets).

### Example Patch Combinations
- **Kick Drum:** MOD VCO set low, max EG1 AMT to MOD VCO FREQ, moderate OVL on mixer for overdrive, VCW FOLD to taste.
- **Clap/Snare:** Use short envelopes, noise, cross-modulate FOLD and BIAS.

---

## 2. Aggressive/Crazy Dubstep & Drum’n’Bass Basslines

### Key Parameters & Sections:
- **MOD VCO FM AMT (Thru-zero FM)**
- **Ring Mod / Mixer Overdrive**
- **SEQ1/SEQ2 AMT for Quantized Step Modulation**
- **Wavefolder, Filter (Resonance, Bandpass), BLEND/ORDER**

### Strategies

- **FM Bass “Vowel” Tones:**
  - Set MOD VCO to audio range, turn up **MOD VCO FM AMT** for deep, animated FM (through-zero keeps bass in tune even at wild settings).
  - Add RING MOD for inharmonic, metallic textures.

- **Create Growls and Wubs:**
  - Sequence filter cutoff (**VCF CUTOFF**) or wavefolder amount (**VCW FOLD**) using SEQ1 or SEQ2.
    - Patch **SEQ1 CV** to FOLD, or bring in external modulation/LFO for sweeping “wub” LFOs.
    - Modulate **BLEND** with step CV or LFO, fading between additively wavefolded and subtracted/filter paths over time.
  - Crank RESONANCE, sweep BANDPASS for formant-like filtering.
  - Put ORDER in VCF > VCW, then heavy wavefolding post-filter for nasty, metallic character.

- **Drive & Distort Everything:**
  - Overdrive EACH channel in the mixer past 12 o'clock, not just at final VCA stage.
  - Use modulated envelopes on VCF cutoff or FOLD for rhythmic filter sweeps.

- **Patch Bay Tricks:**
  - Use **CV inputs** (VCO 1V/OCT, M VCO 1V/OCT, FOLD, CUTOFF) for external CV sequencing, e.g., from a sequencer or external envelope/fader.
  - Patch **NOISE** or an external audio rate source into Mix or FOLD input for extra grit.

### Example Patch Combinations
- **Dubstep Wobble:**  
  - MOD VCO at audio rate, MOD VCO FM AMT high.
  - SEQ2 or external LFO patched to VCF CUTOFF or BLEND.
  - Heavy VCW FOLD for added distortion.
- **Gnarly Reese Bass:**  
  - Use detuned MOD VCO and VCO, ring mod, filter in BP mode with high resonance, FM and distortion simultaneously.

---

## 3. Haunting Atmospheric Pad Sounds

### Key Parameters & Sections:
- **Dual Sequencer (Long sequences, “Corrupt” for mutation)**
- **Blending (BLEND crossfader, PARALLEL routing)**
- **Filter morph (Lowpass to Bandpass), Moderate Resonance**
- **EG1/EG2 (long decay settings)**
- **NOISE and Sine/Tri Mixes**

### Strategies

- **Generative, Evolving Textures:**
  - Slow down the internal clock (**TEMPO**).
  - Set long or chained sequences (16 steps), use **CORRUPT** to semi-randomly mutate melody/timbre for generative drift.
  - Moderate BLEND between filter and wavefolder for morphing timbres.

- **Misty, Blurred Harmonics:**
  - Use sine and triangle from both VCO and MOD VCO for a pure base, then lightly mix in wavefolding—avoid going into harsh distortion.
  - Slow envelope decays for both EG1 and EG2 (set decay times to several seconds or more).

- **Filtered Noise:**
  - Bring in NOISE with the LVL and TONE cranked towards the higher frequencies.
  - Patch NOISE directly into VCF IN, with continuous modulation of CUTTOFF via SEQ2 or external slow LFO.

- **Patch Bay Magic:**
  - Use external sequencer or CV recorder to animate long filter cutoff or blend sweeps.
  - Patch one EG output or external LFO to **BLEND** to automatically drift between VCW and VCF paths.

- **Atmospheric Movement:**
  - Let the dual sequencers work at different lengths for polyrhythmic, drifting melodic elements.
  - Use EG TRIG MIX to trigger envelopes from both sequencers for unpredictable dynamic envelopes.
  - Use quantization modes (e.g., **Hang Drum**, **Minor 11th**) for non-traditional scales.

### Example Patch Combinations
- **Evolving Pad:**  
  - Long decays, slow movement on FOLD/BIAS & Cutoff.
  - “Corrupt” knob mid-way for slowly mutating sequence.
  - BLEND near center for a mix of timbres.

---

## Additional Patch Bay Ideas for Cross-Modulation

- Cross-patch EG1 or EG2 outputs to BIT FLIP inputs for morphing generative sequences
- Send external CVs, S&H, or complex envelopes to BLEND, VCW FOLD, or VCF CUTOFF for deep animation
- Use U MIX to sub-mix and externally process individual synth voices before re-injecting

---

## Further Exploration

The **Moog Labyrinth** is designed for deep modulation and crosspatching. Use the extensive patch bay to interface with other Eurorack gear (clocks, random sources, CV recorders, S&H, or effects) for ever-more complex generative or performance-oriented sound designs.

---

**Reference Links:**
- [Moog Labyrinth User Manual PDF](https://www.moogmusic.com/sites/default/files/2024-05/Labyrinth_Manual_Web.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
