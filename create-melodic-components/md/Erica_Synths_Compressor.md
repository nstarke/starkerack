# Erica Synths — Compressor

- [Manual PDF](../../manuals/compressor_manual_2023.04.04.pdf)

---

[Manual PDF](#)

Based on the provided manual pages, the module shown is the **Erica Synths Stereo Compressor**. Since only this module’s manual is attached here, I can explain how it can be used in a Eurorack system to help create and shape **melodic components**, especially when combined with oscillators, envelopes, filters, VCAs, sequencers, and modulation sources.

# Erica Synths Stereo Compressor
## What it does
This is a **stereo compressor** designed for modular-level signals. Key features from the manual:

- **THAT chip-based stereo compressor**
- **DC-coupled sidechain**
- Controls for:
  - **Input Level**
  - **Gain** (makeup gain)
  - **Threshold**
  - **Compression Amount / Ratio**
- **Stereo Link** switch
- **Bypass / Process** switch
- **8-segment output VU meter**
- **Stereo audio inputs and outputs**
- **Stereo sidechain inputs and buffered sidechain outputs**

## Why this matters for melodic music
Compression is often thought of as a drum-mixing tool, but in Eurorack it can be extremely useful for **melodic voices, pads, basslines, arps, and stereo synth layers**. This module helps melodic parts become:

- more **consistent in level**
- more **present in a mix**
- more **rhythmically animated**
- more **glued together** as a stereo pair
- more **dynamic** when using sidechain pumping

---

# Best ways to use it for melodic components

## 1. Glue a stereo melodic voice
If you have a stereo melodic signal path, patch it like this:

- **Oscillator / voice stereo outs** or
- **mono voice through stereo FX**  
into:
- **IN L / IN R** on the Stereo Compressor  
then:
- **OUT L / OUT R** to mixer or output

### Result
This tightens a stereo pad, wavetable voice, supersaw-style patch, or stereo delay/reverb return. It helps the melodic sound feel more polished and controlled.

### Tips
- Turn on **STEREO LINK** to avoid the left and right channels compressing differently.
- Use a moderate **threshold** and ratio for subtle glue.
- Add **makeup gain** after compression if the signal becomes too quiet.

This is especially useful for:
- lush chords
- stereo drones
- melodic techno leads
- wide ambient textures

---

## 2. Sidechain a bassline from the kick
This is one of the most musically useful patches.

### Patch idea
- Patch your **bassline** or mono/stereo melodic synth into **IN L / IN R**
- Patch your **kick drum** signal into **SIDE IN** (left, right, or both depending on your patching setup)
- Adjust:
  - **Threshold**
  - **Compression Amount**
  - **Input Level**

### Result
Each kick hit ducks the bassline or melodic layer, creating rhythmic breathing and space in the mix.

This works very well for:
- acid lines
- sequenced bass
- chord stabs
- sustained pads
- reverb-heavy melodic voices

Because the sidechain is **DC coupled**, it may also respond to more than just audio-like drum transients depending on how your system is patched. That opens more creative control possibilities.

---

## 3. Animate pads and drones rhythmically
A sustained melodic texture can become much more alive when sidechained.

### Patch idea
- Put a **pad, drone, or sustained oscillator stack** into the compressor audio inputs
- Feed a **rhythmic trigger-derived audio pulse**, kick, percussion bus, or other rhythmic source into the **sidechain input**

### Result
The sustained melodic sound pulses in time with the beat.

This is excellent for:
- ambient techno
- Berlin-school sequences
- cinematic drones
- evolving chord beds

Instead of using a VCA for hard gating, compression gives a smoother, more mix-friendly rhythmic movement.

---

## 4. Control transients on plucky melodic sounds
Fast plucks and resonant sequences can sometimes jump out too much in a live modular patch.

### Patch idea
Run:
- plucked voice
- filtered sequence
- resonant ping voice
- FM melody

through the compressor.

### Result
You can:
- tame sharp peaks
- increase sustain perception with makeup gain
- make plucks feel thicker
- even out note-to-note dynamics

This is especially useful when:
- sequencer accent levels vary
- filter resonance causes occasional peaks
- FM patches produce uneven loudness

---

## 5. Make a lead sit better in a live mix
In live Eurorack performance, melodic leads can disappear or suddenly become too loud.

### Patch idea
Put the lead voice through the Stereo Compressor before the final mixer or output chain.

### Result
The lead stays more stable in level and easier to hear without constant manual adjustment.

Use:
- lower ratio for natural leveling
- slightly stronger compression for aggressive techno leads
- makeup gain to keep it forward in the mix

---

## 6. Use dual-mono sidechain behavior creatively
The manual notes that the module has:
- **L and R sidechain inputs**
- ability to **process each channel individually**
- **Stereo Link** option for merged detector behavior

This means you can treat it as either:
- a **true stereo compressor**
- or a more flexible **dual channel dynamics processor**

### Creative melodic use
Send:
- one melodic layer to left
- another melodic layer to right

Then sidechain them differently.

For example:
- Left = bassline
- Right = pad

Feed different sidechain signals into each channel.

### Result
You get independently moving melodic layers with related but different rhythmic compression patterns.

This can create:
- call-and-response movement
- shifting stereo interplay
- evolving melodic dynamics

---

## 7. Compress a post-FX stereo chain
A very practical melodic use is placing the compressor after effects.

### Patch idea
Melodic voice → stereo chorus / delay / reverb → Stereo Compressor

### Result
This helps control:
- overly dynamic delay repeats
- washed-out reverb swells
- stereo modulation peaks

It can make effects-heavy melodic parts feel more intentional and sit better with drums.

---

# Important patching notes from the manual

## Inputs and levels
- Audio input level: **-5V to +5V**
- This is appropriate for Eurorack audio signals

## Main controls
### Input Level
Sets how hard the incoming signal hits the compressor.  
Higher input level means more likely compression, depending on threshold.

### Gain
This is **makeup gain**. After compressing, use this to bring the output back up.

### Threshold
Sets the point where compression begins.

### Compression Amount
This is effectively the **ratio** control.

### Stereo Link
Very important for stereo melodic material.  
If left and right channels differ a lot and Stereo Link is off, the image may shift because each side compresses differently.

Use **Stereo Link ON** for:
- stereo pads
- stereo FX returns
- wide melodic voices
- full stereo submixes

Use it **OFF** for:
- experimental dual-mono dynamics
- independently compressed left/right material

### Process / Bypass
Instantly compare compressed and uncompressed signal.

### VU Meter
Useful for visual output monitoring during performance.

---

# Example melodic patch recipes

## Patch 1: Pumping stereo pad
**Modules needed in addition to compressor:**
- poly/stereo voice or two oscillators
- envelope/filter/VCA chain
- kick drum source

**Patch:**
- Pad L/R → **IN L / IN R**
- Kick → **SIDE IN L** and/or **SIDE IN R**
- Compressor **OUT L / OUT R** → mixer
- **Stereo Link ON**

**Set:**
- medium threshold
- medium compression amount
- enough gain to restore output level

**Sound:**
A wide pad that ducks on every kick, great for melodic techno.

---

## Patch 2: Tight bassline
**Patch:**
- Bass voice → compressor input
- Kick or percussion bus → sidechain input
- Output → final mixer

**Sound:**
Punchier low end with room for drums. The bass feels more energetic and less muddy.

---

## Patch 3: Smoothed arpeggio
**Patch:**
- Arp voice through delay → compressor
- Optional percussion sidechain
- Output to mixer

**Sound:**
The arpeggio becomes more even and polished, and can pulse rhythmically if sidechained.

---

## Patch 4: Stereo chord bus
**Patch:**
- Multiple melodic voices mixed to stereo → Stereo Compressor
- Output → final output module or mixer

**Sound:**
“Glue” across all melodic chord elements, especially helpful if several voices are layered.

---

## Patch 5: Two independent melodic lanes
**Patch:**
- Melody A → IN L
- Melody B → IN R
- Sidechain A → SIDE IN L
- Sidechain B → SIDE IN R
- **Stereo Link OFF**

**Sound:**
Each melodic lane breathes independently. This can produce sophisticated movement across the stereo field.

---

# How it fits into a melodic Eurorack system
This module is not a melodic source by itself, but it is very useful as a **melodic finishing and motion tool**. In a complete system, it works best after modules such as:

- VCOs / digital voices
- filters
- VCAs
- stereo mixers
- delays
- reverbs
- chorus / stereo processors
- drum modules used as sidechain triggers

It is especially valuable in genres where melodic material needs to lock tightly with drums:

- melodic techno
- house
- trance
- synthwave
- IDM
- ambient with pulse
- industrial and DnB-inspired modular sets

---

# Bottom line
The **Erica Synths Stereo Compressor** helps melodic parts by:

- tightening dynamics
- adding glue to stereo voices
- making basslines and pads pump with the groove
- smoothing plucks and leads
- controlling effects-heavy melodic chains
- enabling creative sidechain motion with percussion or other signals

If you want, I can also turn this into:
1. a **“how to patch melodic techno with this module” guide**, or  
2. a **signal-flow diagram** showing exactly how to combine it with common Eurorack module types.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)