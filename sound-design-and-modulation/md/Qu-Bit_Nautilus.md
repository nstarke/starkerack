# Qu-Bit — Nautilus

- [Manual PDF](../../manuals/Nautilus_v1.1.3.pdf)

---

[**Qu-Bit Nautilus Manual PDF**](https://cdn.shopify.com/s/files/1/0604/4399/7566/files/Nautilus_Manual_v1.1.3.pdf)

---

# Qu-Bit Nautilus: Creative Modulation Patch Ideas

The Nautilus by Qu-Bit is an exceptionally deep (pun intended) delay/FX module for Eurorack, offering 8 delay lines, a multi-colored modulation engine (Chroma), robust CV control, and feedback patching for both conventional and experimental sounds. Here’s a summary of how you can use its modulation capabilities to produce:

- **Distorted Percussive Sounds**
- **Gnarly Dubstep/Drum & Bass Basslines**
- **Haunting Ambient Pads**

---

## Core Modulation Points

- **All main parameters have CV inputs**: Mix, Resolution, Feedback, Sensors, Dispersal, Reversal, Chroma, Depth
- **Attenuverters** are assignable to any CV input (via USB configuration)
- **Chroma/Depth** sections let you morph the FX character (bitcrushing, filters, saturation, wavefolding & more)
- **Complex Delay Modes**: Fade, Doppler (pitch shifting), Shimmer, De-Shimmer
- **Multiple Feedback Modes**: Normal, Ping-Pong, Cascade, Adrift
- **Freeze and Purge**: For glitch-style looping and buffer clearing
- **Sonar Output**: Gate or stepped CV for self-patching and external modulation

---

## Modulation Patch Examples

### 1. Distorted Percussive Sounds

Combine Freeze, Chroma, Depth, and random stepped modulation on Delay/Feedback time or direction for crunchy, glitched textures.

#### Settings & Routing

- **Input**: Feed a short/fast drum hit, percussion, or plucky synth sound
- **Chroma**: Set to *Refraction Interference* (bitcrusher, purple) or *SOS* (red, heavy distortion)
- **Depth**: 80-100% (max for most effect)
- **Feedback**: 9 to 11 o’clock for quick decaying delays, or max for repeats
- **Dispersal**: Low or mid for tight clustering (try modulating this!)
- **Sensors**: 1–2 for sharper articulation, 3–4 for chaos
- **Reversal**: Modulate with stepped/random CV—reverses buffer, causing chopped or reversed artifacts
- **Mix**: 50–100% (more FX)

#### Advanced Modulation

- Modulate *Freeze* with a rhythmic gate for “beat repeat/glitch lock” FX
- Send random or stepped LFOs to *Chroma*, *Reversal*, or *Resolution* for switching between time signatures or suddenly crushing the buffer
- Try assigning an attenuverter to *Feedback* for external or self-patched modulation for build/breakdown FX

#### Quick Patch

```none
Drum Module -> Nautilus IN
CV LFO/Random -> Chroma CV (bitcrush/distort)
Sequencer Gate -> Freeze CV
Random CV/sonar out -> Reversal CV
```

---

### 2. Dubstep/DNB Basslines (Gnarly & Animated)

#### Settings & Routing

- **Input**: Aggressive bass or simple saw wave (try a mono bassline)
- **Chroma**: Try *Pulse Amplification* (orange, saturation), *Receptor Malfunction* (cyan, wavefolding), or *SOS* (red)
- **Depth**: Sweep between 0–100% for “movement” or automate via LFO/CV
- **Resolution**: 9–12 o’clock for short delay times—drive into the audio range for combing/phasing
- **Feedback**: Moderate (oscillate for “growl” effects, or low for tight slap)
- **Dispersal**: Low = mono/fat; Med/Hi = pseudo-stereo movement
- **Sensors**: 1–2 for stable, 3–4 for wild
- **Reversal**: Try modulating with a sequencer or stepped random for “glitch” artifacts
- **Delay Mode**: Doppler (green) or Shimmer/De-Shimmer for pitch mod fx

#### Advanced Modulation

- CV to *Chroma* for moving between filter/distortion types, especially with fast LFOs (for rhythmic movement)
- Send envelopes or LFOs synced to your bassline to *Depth* or *Reversal*, for “wobble” effects and growls
- Try modulating *Feedback* or *Resolution* for complex, FM-like movement

#### Quick Patch

```none
Bass Synth OUT -> Nautilus IN
Envelope/LFO (from VCA or Filter) -> Depth CV (or Chroma/Dispersal CV)
LFO/Fast Random CV -> Reversal CV
Sequencer pitch -> Feedback or Resolution CV for note-locked delay times
```

---

### 3. Haunting Ambient Pads

#### Settings & Routing

- **Input**: Lush chord, drone, or evolving pad
- **Chroma**: *Oceanic Absorption* (blue, lowpass) or *White Water* (green, highpass) for smoothing; *Refraction Interference* for lo-fi
- **Depth**: Swept slowly with an LFO, 30-100% for atmosphere
- **Feedback**: High for infinite soundscapes, or modulate gently for evolving tails
- **Sensors**: 2–4 for spreading sound into a “cloud”
- **Dispersal**: Mid to high for spatial/rhythmic complexity
- **Reversal**: Modulate at slow rates for reversed shards
- **Delay Mode**: Shimmer (octave up) for ethereal harmonics; Cascade or Adrift for smeared stereo drifting
- **Mix**: 100% wet for full effect

#### Advanced Modulation

- Gentle random or slow triangle/sine LFO to *Chroma*, *Depth*, *Dispersal*, and *Reversal*
- *Freeze* at clock divisions—hold/release for momentary sound on sound layering
- Self-patch *Sonar Out* back to *Depth*, *Feedback*, or *Dispersal* for evolving pseudo generative textures

#### Quick Patch

```none
Pad Sound or Drone -> Nautilus IN
Slow LFO (different shapes) -> Depth, Dispersal, Reversal CV
Sonar Out -> Feedback CV or self-patch elsewhere
Freeze via manual or random gate
```

---

## Bonus Tips

- **Assign Attenuverters**: Tailor CV depth and inversion for each modulated parameter for subtle to extreme effects (set via the Narwhal web configurator and USB).
- **Use External Modulators**: Random, machine-learning, or algorithmic CV generators are your friends; Nautilus’s sound comes alive with unexpected, evolving movement.
- **Always Try Self-Patching**: The *Sonar* output provides internal chaos/modulation based on the delay network—patch it to multiple CV inputs (via a splitter) for complexity.
- **Switch Modes Live**: Automate or punch the Delay/Feedback modes for dramatic changes mid-performance—especially Adrift or Ping Pong for stereo trickery.

---

*For full parameter details, refer to the [official Qu-Bit Nautilus Manual PDF](https://cdn.shopify.com/s/files/1/0604/4399/7566/files/Nautilus_Manual_v1.1.3.pdf).*

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)