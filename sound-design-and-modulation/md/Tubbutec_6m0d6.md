# Tubbutec — 6m0d6

- [Manual PDF](../../manuals/6m0d6-User-Manual-1.0.pdf)

---

[6m0d6 by LPZW & Tubbutec – User Manual PDF](https://tubbutec.de/files/6m0d6-manual.pdf)

---

# Modulating the 6m0d6 Eurorack Module for Experimental, Hard, and Atmospheric Sounds

The 6m0d6 module is a powerful percussive voice inspired by the classic TR-606, but provides extensive CV, MIDI, and sound-engine modifications for deeply creative sound design. Here’s how you can leverage its features for **distorted beats**, **wild basslines**, and **atmospheric pads**.

---

## 1. **Distorted Percussive Sounds**

**Key features to exploit:**
- Selectable **noise sources**: White, Metal, XOR
- **Noise Bit Reduction** (via Noise Tune knob and CV)
- Individual **decay**, **tuning**, and **click** parameters per drum sound
- External **dynamic triggers** and **CV inputs** for accent/level

**Techniques:**
- **Bitcrushing for Grit**: Set the Noise source to ‘Noise’ and turn down the Noise Tune for intense bit reduction. You can CV modulate this with stepped or random voltages for constantly shifting lo-fi textures.
- **Accentuated Distortion**: Use an external envelope or random LFO in the Accent CV input; combined with trigger amplitude modulation, this creates aggressive dynamic range and clipped artifacts.
- **Metallic Industrial**: Choose the Metal or XOR source for Snare or Cymbals, then modulate **Metal Tune** and **Spread** with audio-rate LFOs or sequenced CV. This produces clangorous, syncopated metallic scrapes and cracks.
- **Decay Smearing**: Set decay times unusually long (especially on Snare or Toms), then rapidly modulate them with stepped or slewed CV for sludgy, smeared drum tails.

---

## 2. **Crazy Basslines (Dubstep/Drum & Bass Style)**

**Key features to exploit:**
- **Bass Drum**: Powerful decay, tune, and click controls
- **Sub Tom**: Changes Low Tom pitch to sub-bass territory
- **Metal Tune** (1V/Oct compatible CV input)
- MIDI: Use channel 1 to play metal oscillators as tuned synth voices

**Techniques:**
- **Percussive Reeses**: Set Sub Tom ON. Use a fast ADSR envelope or a pitch LFO (preferably audio-rate) to modulate Tom or Bass Drum TUNE CV. Layer with long decay for moving, talking bass effects.
- **Tuned Metallic Bass**: Use MIDI channel 1 to play the Metal oscillators chromatically. You can sequence paraphonic lines or chords using the allocated 6 voices; combine this with low METAL TUNE and high SPREAD for thick, detuned bass.
- **Rhythmic Wobble**: Send clock-synced LFO or stepped random voltages to the Bass Drum or Tom decay, or Accent CV. Velocity over MIDI or dynamic triggers further accentuate movement and punch.

---

## 3. **Haunting Atmospheric Pad/Drone Sounds**

**Key features to exploit:**
- **Cymbal Pulse Shaper Bypass**: Lets you use the Cymbal as a long-decay or continuous sound source
- **Multi-voice Metal Oscillators**: Can be played continuously via MIDI
- **Noise Tune**: Emulation of analog white noise and bit-reduced digital noise, controllable via CV
- **Wide-range Tuning and Envelope Controls**

**Techniques:**
- **Cymbal Drone Mode**: Disable the internal pulse shaper via CY.PULSE (or MIDI CC). Trigger the cymbal with longer pulses or gates, or hold via MIDI for sustained, bell-like textures. Modulate TONE, DECAY, and select Metal or XOR sources for richer harmonics.
- **Shimmering Pads**: Send chords over MIDI channel 1 to the Metal oscillators. Modulate METAL SPREAD and TUNE for evolving pad foundations. Blend in NOISE source and modulate with slow LFO for airiness.
- **Evolving Textures**: Use slow random or cyclic CV on NOISE TUNE and ACCENT CV. Play with high decay and overlapping triggers to “smear” drum tails into evolving washes.
- **Atmospheric “Ghost Hits”**: Send very low amplitude triggers (1-2V) for ghostly, understated percussive hits, then layer their long, modulated decays.

---

### **Patch Examples**

**Distorted Clanging Snare:**
1. Snare Noise Source: XOR, METAL TUNE & SPREAD at mid, NOISE TUNE CV with stepped random.
2. Snare DECAY controlled via envelope follower from another module.
3. Accent CV input modulated with a sequencer or stepped random.

**Wobble Bass Drum:**
1. Bass Drum TUNE modulated with fast LFO or sequencer.
2. Sub Tom ON, tuned low.
3. Accent Gate clocked so some hits are accented, others not.

**Haunting Pad:**
1. Cymbal: Pulse shaper OFF, gate input held open.
2. MIDI channel 1 sends occasional chords to metal oscillators.
3. METAL TUNE and SPREAD modulated by slow LFOs.
4. Noise source blended in and tuned for shimmer.

---

#### [Download the 6m0d6 Manual PDF](https://tubbutec.de/files/6m0d6-manual.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)