# 2hp — Pluck

- [Manual PDF](../../manuals/2hp_Pluck.pdf)

---

[2hp Pluck Manual PDF](https://2hp.com/products/Pluck.pdf)

---

## Pluck Eurorack Module: Creative Modulation Tips  
_Let’s explore how to get the wildest and most evocative sounds from your 2hp Pluck module, focusing on modulating it for: distorted percussion, basslines, and ambient pads._

---

### 1. Distorted Percussive Sounds

**Modulation Strategies:**
- **Decay CV Abuse:** Patch a fast, stepped or random modulation (e.g. stepped random/“sample & hold” LFO, or trigger sequencer) into the DECAY CV. Use high bipolar voltages for drastic variations. Short decays create snappy clicks; long decays turn into splatty FM blaps.
- **Damp CV for Grit:** Modulate DAMP CV with a sharp, fast envelope or a chaotic LFO. Use the deepest modulation (-5V to +5V) to swing from tight, dead thuds to resonant pingy hits. This changes the harmonic content and makes metallic hits or wooden blocks.
- **Pitch Tricks:** Use the PITCH KNOB for tuning the “body” of your click or drum. For mechanical distortion, slam very low or high CV into V/OCT for “brap”/“zap” sounds.
- **External Distortion:** Run PLUCK’s OUT through a wavefolder, bitcrusher or analog distortion for extra dirt.
- **Retriggering:** Fire TRIG at audio rates for digital noise and glitch artifacts.

---

### 2. Crazy Basslines (Dubstep/DnB Madness)

**Modulation Strategies:**
- **V/OCT Sequencing:** Sequence the V/OCT input with a pitch CV source. Use slides and pitch bends for wobbly, falling bass sounds.
- **Wobble with Damp:** Modulate DAMP CV with synced or free LFOs for “filter sweep” timbral movements especially effective for growly bass textures.
- **Decay as Movement:** Envelope or LFO modulation on DECAY CV evolves both note length and harmonic spectrum, perfect for morphing neuro-basslines.
- **Manual PITCH Play:** Tweak the PITCH knob mid-note (it stays live for the ringing note!), introducing live vibrato, bends, and pitch instability.
- **Polyphonic Mayhem:** Fire multiple TRIGs for overlapping, detuned bass notes—layer for raucous, reedy and menacing sounds.

---

### 3. Haunting Atmospheric Pads

**Modulation Strategies:**
- **Slow Decay and Damp:** Set DECAY and DAMP to high values for long, harmonically rich tones. Use slow LFOs or random voltages into both CV inputs for evolving, spectral textures.
- **Pitch Drift:** Gently modulate V/OCT with a very slow LFO for tape-like warble.
- **Four-Voice Polyphony:** Sequence chords via the TRIG and V/OCT inputs for lush, ringing pad layers; high DECAY settings let notes overlap.
- **External Reverb / Delay:** The dry Pluck can be sharply percussive; drench it in reverb/delay to blur the attacks into spectral washes.
- **CV Bleed:** Modulate all three (DAMP CV, DECAY CV, V/OCT) simultaneously with related or contrasting voltages for unpredictable, shifting atmospheres.

---

### Patch Example Recipes

**Distorted Perc:**
```patch
TRIG: Fast clock / sequencer
DAMP CV: Envelope with negative offset
DECAY CV: Random stepped
V/OCT: Not connected or fixed low pitch
OUT: External distortion module or hard clipping
```

**Dubstep Neuro Bass:**
```patch
TRIG: Sequencer gate
DAMP CV: LFO at 1/2 speed of sequence (wobble)
DECAY CV: Envelope or sequencer
V/OCT: Bassline sequence with portamento
OUT: Into heavy chorus/drive
```

**Atmospheric Pad:**
```patch
TRIG: Chord trigger sequence (up to 4 notes)
DAMP CV: Slow random LFO
DECAY CV: Slow triangle LFO
V/OCT: Chord generator or slowly morphing voltages
OUT: Massive reverb
```

---

### Key CV Ranges & Controls

- **DAMP/DECAY CV:** Accepts -5V to +5V. Bipolar! This makes them highly modulatable for extreme effects.
- **V/OCT:** Standard 1V/oct. Use with quantizers, sequencers, LFOs for melodic or wild atonal work.
- **Output:** 10Vpp—hot signal, suitable for further processing and distortion.

---

### Creative Takeaways

- **Everything but Output is Modulatible:** Get hands-on or patch in automation for organic, never-static results.
- **Polyphony:** Embrace Pluck’s polyphony for savage unison bass, lush pads, and rhythmic chaos.
- **Not Just “Strings”:** Think of Pluck as a micro-percussion synth, bass monster, or digital resonator—explore beyond “harp.”
- **Stacked Modulation:** Use mults/stackcables to blend LFOs, envelopes, random, and sequencer sources for hybrid behaviors.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)