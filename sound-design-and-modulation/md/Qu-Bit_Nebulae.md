# Qu-Bit — Nebulae

- [Manual PDF](../../manuals/Nautilus_v1.1.3.pdf)

---

[Qu-Bit Nautilus Manual (PDF)](https://patches.qubitelectronix.com/manuals/Nautilus_Manual_v1.1.3.pdf)

---

# Modulating the Qu-Bit Nautilus for Unique and Extreme Sounds

The **Qu-Bit Nautilus** is an incredibly deep and flexible digital delay engine that excels as a modulation playground. Below, we'll cover targeted modulation strategies for achieving **distorted percussive hits**, **wild, modulated basslines**, and **ethereal/haunting pads**, using Nautilus's extensive features.

---

## Core Modulation Opportunities

**Assign CV or internal modulation to:**
- **Chroma/Depth** — Real-time morphing of internal effects (distortion/wavefolding/bitcrush).
- **Feedback** — Dynamically shape repeats, create run-away, noisy delays.
- **Sensors/Dispersal** — Animate the number and spread of delay lines for complex rhythmic/rhythmic textures.
- **Resolution** — Perform glitchy/clocked artifacts and metallic time changes.
- **Reversal** — Morph delay directions for unpredictable movement and chaos.
- **Freeze/Purge** — Freeze for stutter effects; Purge moments for dramatic drop-outs.
- **Sonar Output** — Use algorithmic CV as a modulation source elsewhere or self-patch.

---

## Recipes for Sound Design

### 1. **Distorted Percussive Sounds**

**Goal:** Sharply modulated, punchy, noisy, or glitched rhythmic hits that punch through a mix.

#### **Patch Strategy:**

- **Chroma:** Set to **SOS (heavy distortion)** or **Receptor Malfunction (wavefolding)**
    - **Depth:** Modulate with an envelope from the percussion trigger for dynamic distortion each hit.
- **Feedback:** Keep **low-to-mid**; modulate quickly with per-hit CV for "bouncing" repeats.
- **Resolution/Sensors:** Set sensors low for single/double taps; randomly clock Resolution for rhythmic variety or step it with a sequencer/gate.
- **Dispersal:** Use a second snappy envelope to scatter hits for quick "flams" or glitches.
- **Freeze:** Use a gate to rapidly freeze and unfreeze for dramatic stutter FX.
- **Sonar Output:** Patch to itself (e.g. Depth or Feedback) for evolving, per-hit modulation.

**Extra:** Toss in highpass filter (White Water Chroma) briefly for snare-like crack, or assign Attenuverters for custom CV scaling!

---

### 2. **Dubstep/Drum & Bass Crazy Modulated Basslines**

**Goal:** Gritty, evolving basslines with comb filter, time/space warping, and rhythmic movement.

#### **Patch Strategy:**

- **Source:** Feed a bass oscillator (simple or FM for overtones).
- **Chroma:** Use **Refraction Interference** (bitcrusher/sample-rate) for digital aggression, or **Pulse Amplification** for saturation.
    - **Depth:** LFO modulation for sweepy, tearing movement; CV sequence for step-modulated timbre changes.
- **Feedback:** Set mid-high; modulate with envelope followers keyed to bass notes for growl/swelling repeats.
- **Sensors/Dispersal:** Animate with LFO or sequenced CV to exaggerate stereo/comb filter motion and shifting notches (timbre animation).
- **Resolution:** Try polyrhythmic/microtime modulations with CV for "rolling" artifacts.
- **Reversal:** LFO or step-sequence for wild, reversed hits interspersed with normal ones.
- **Delay Mode:** **Doppler** for pitch-glide delay transitions (makes for wobbly, growling textures).
- **Freeze:** Stutter bass hits on-the-fly for stop-motion rhythms.

**Extra:** Tap out mono input tricks (see manual Ping Pong note), and assign Sonar out to modulate other modules (filters, waveshapers).

---

### 3. **Haunting Atmospheric Pads**

**Goal:** Sprawling, morphing soundscapes—evocative, spectral, underwater, or dreamlike.

#### **Patch Strategy:**

- **Chroma:** Use **Oceanic Absorption** (lowpass) for smoothness, **Pulse Amplification** for subtle warmth, **White Water** for shimmer/ice.
    - **Depth:** Modulate slowly with a looping envelope, joystick, random LFO, or breath/aftertouch for human-feel timbre.
- **Feedback:** Run **high** for infinite, lush trails.
- **Sensors/Dispersal:** Gradually morph from mono to full 8-line stereo spread—CV control with S&H or slow LFO for evolving stereo image.
- **Resolution:** Use longer, dotted, non-4/4 delays. Slow, random mod to Resolution achieves tape-like warble.
- **Reversal:** Turn up for ghostly reversed tails, automated with random stepped CV or aftertouch for organic unpredictability.
- **Delay Mode:** **Shimmer**/De-Shimmer** for pitch-shifted heaven/abyss; automate with CV for transposed trails.
- **Freeze:** Capture chords, fade slowly; play over with new material for lush layers.
- **Sonar Output:** Self-patch for gentle modulation of organically shifting parameters (Resolution, Reversal, Depth, etc.).

---

### **General Tips for Advanced Modulation**

1. **Use Attenuverters Smartly:** Assign to any key modulation point—fine-tune external CV or automate through Narwhal Configurator.
2. **Self-Patch Sonar:** Nautilus can become its own modulation brain for feedback loops and generative sound.
3. **USB Configurator:** Make Chroma/Freeze/Feedback modes respond in new ways—e.g., quantize freeze to clock, tweak pitch shifting ranges for microtonal atmospherics.
4. **CV Input Ranges:** Virtually all modulation points respond to **-5V to +5V**—use bipolar modulation for morphing intensity and direction.
5. **Crossfade Modulators:** Combine envelopes, LFOs, and stepped randoms (via mixers/attenuverters) for deeply evolving timbre.

---

## **Let Nautilus Drown Your Sounds In Otherworldly Modulation**

There is a nearly infinite array of modulation possibilities due to Nautilus's flexible CV mapping, feedback topology, and internal algorithmic control (Sonar out). Exploit stereo variations, polymetric delays, and per-channel reversals for ultra-rich, motion-soaked effects. Experimentation with mod sources, feedback, and Chroma/Depth is rewarded with boundary-pushing sound!

---

[Qu-Bit Nautilus Manual (PDF)](https://patches.qubitelectronix.com/manuals/Nautilus_Manual_v1.1.3.pdf)

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)