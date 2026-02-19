# Erica Synths — Bassline

- [Manual PDF](../../manuals/BASSLINE_web.pdf)

---

[**Erica Synths Bassline Drum Module Manual (PDF)**](https://www.ericasynths.lv/media/Bassline_1.03.pdf)

---

## Harnessing the Erica Synths Bassline Module for Dense, Hyper-Complex Percussion

The Erica Synths Bassline is a full analog synth voice with a BASS VCO, transistor ladder VCF, and envelope generator. Here’s a focused guide for wrangling dense, polyrhythmic, and highly percussive sequences using this module:

---

### 1. **Patch as a Percussive Voice**
- **Self-Oscillation & Clicks:** Push the RESONANCE high, reduce CUTOFF, and ping the VCF with sharp gate or envelope signals into the VCF cutoff CV input. This will generate chirpy, biting percussive sounds beyond typical basslines.
- **VCA Envelope:** Keep DECAY short and trigger the envelope with fast or irregular gate patterns for staccato, punchy hits.

### 2. **Complex Gating & Triggering**
- **External Sequencers:** Use clock dividers, polyrhythmic step sequencers, or trigger/gate sequencers (Pam’s New Workout, Euclidean Circuits, etc.) for feeding the module’s GATE and ACCENT inputs. This sets up intricate rhythmic bursts, tuplets, and polymetric patterns.
- **Accent Input:** Patch high-velocity trigger patterns to the ACCENT input to punch through—think flams, ratchets, or sudden percussive spikes.

### 3. **CV Modulation for Hyper-Complexity**
- **VCO & VCF CV Inputs:** Modulate SUB-OSC, TUNE, or CUTOFF using complex LFOs or random stepped voltages (e.g. Batumi, Ornament & Crime, or Turing Machine) locked to various rhythmic clocks. This adds unpredictability and variation to your percussive voice in real time.
- **At Audio Rate:** Try patching audio-rate modulation sources to the VCF cutoff input for aggressive, noisy metallic percussion timbres.

### 4. **Unconventional Oscillator Techniques**
- **FM Input:** Patch rhythmically gated audio or LFOs into the FM input for plucky, metallic, or atonal percussion.
- **Detune Play:** Rapidly CV the DETUNE input in time with gates, alternating between microtonal offsets for clangorous, spectral drum sounds.

### 5. **External Processing & Resampling**
- **Multi-Layering:** Mult the output and process one copy through distortion, bitcrushing, or wavefolders to build stacked, richly rhythmic textures.
- **Gate/Envelope Automation:** Sequence envelope depth or shape with external voltage-controlled switches or logic modules for morphing percussive behaviors within polyrhythmic sequences.

### 6. **Advanced Eurorack Integration Concepts**
- **Polyrhythmic Sequences:** Use multiple asynchronous clocks/dividers to trigger the Bassline module alongside standard drum voices, forming cross-rhythms (e.g. 3 vs 4 vs 5).
- **Accent Randomization:** Use sample & hold modules to occasionally fire the ACCENT gate in odd, non-repeating polyrhythms for sudden accent shifts.

### 7. **Performance Tips for Rhythm Complexity**
- **Manual Tweaks Live:** Bring out unique percussive flavors by manually manipulating the CUTOFF, RESONANCE, and envelope decay during a sequence.
- **Voltage Control Morphing:** Morph between preset CV patterns using addressable sequencers (like the Malekko Voltage Block), changing rhythms on the fly.

---

## **Summary Table: Creative Percussive Patching**

| Control/Input | Use For Percussion                    | Rhythmic Complexity Ideas                                  |
|---------------|--------------------------------------|-----------------------------------------------------------|
| Gate          | Sharp env, triggers percussive hits  | Sequence with polyrhythmic gate patterns                  |
| Accent        | Extra punch/varying attack           | Random or Euclidean accent patterns                       |
| Cutoff CV     | Noisy/tonal drum tuning via CV       | Modulate via rhythmic LFOs, S&H, or audio-rate signals    |
| FM            | Rich metallic/atonal percussive hits | Audio-rate gated FM from sequencer-controlled VCOs        |
| Detune CV     | Machine-y, metallic FX               | Clocked micro-modulations for synthetic "hi-hat" feeling  |
| VCA Envelope  | Tight, punchy hits                   | Automate decay for ghost notes and dynamic shifts         |
| Output        | Layer, distort, or bitcrush          | Process in parallel for multi-timbre polyrhythm           |

---

### Final Inspiration

The Bassline is not just for bass! Push it into harsh, clocked, or pinged regimes for one-of-a-kind percussion. Combine complex CV/gate modulation, dynamic filter pinging, and external logic to generate hyper-dense, evolving, polyrhythmic rhythms.

---
**Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)**