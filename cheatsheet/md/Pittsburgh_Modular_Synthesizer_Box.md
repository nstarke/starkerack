# Pittsburgh Modular — Synthesizer Box

- [Manual PDF](../../manuals/Synthesizer Box - Pittsburgh Modular Synthesizers.pdf)

---

[Manual PDF](https://pittsburghmodular.com/s/Synthesizer-Box-Manual.pdf)

# Pittsburgh Modular Synthesizer Box — Cheat Sheet

**Type:** Semi-modular analog monophonic voice  
**Status:** Discontinued  
**Format:** Eurorack, **28hp**, **36.5mm** deep  
**Power:** **+12V 125mA / -12V 95mA / +5V not required**

## What it is
A complete analog synth voice with these internally patched sections:

**1V/O IN → Glide → Waveforms Oscillator → LPG → VCA OUT**  
Control/mod defaults:
- **LFO TRI → Oscillator FM CV**
- **LFO TRI → Oscillator MOD CV**
- **ENV OUT → LPG CV**
- **ENV OUT → VCA CV**

Patching into the destination input **breaks/overrides** the internal routing.

---

## Quick Start

### Basic monosynth patch
1. Patch pitch CV to **1V/O IN**
2. Patch gate/trigger to **ENV IN**
3. Take audio from **VCA OUT**
4. Set:
   - Oscillator coarse/fine tune to taste
   - Mixer waveform levels up
   - LPG mode to **LPG** or **VCA**
   - Envelope attack low, decay/release to taste
   - VCA CV attenuator up

### Fast percussive patch
1. **ENV IN** with triggers/gates
2. Use **LPG mode = LPG**
3. Set **Mod/Ping = PING**
4. Short envelope, moderate LPG frequency
5. Audio from **VCA OUT** or **LPG OUT**

### Drone patch
1. Use oscillator outputs or **MIX OUT**
2. Patch directly to **LPG IN** or **VCA IN**
3. Skip envelope, open **VCA** manually with its level knob
4. Add LFO to **FM CV IN** or **MOD CV IN**

---

## Signal Flow Overview

### Oscillator / Waveforms
Main sound source with:
- Triangle
- Saw or Blade
- Square
- Sub oscillator one octave below

The mixer sets the levels of triangle, saw/blade, and square into:
- their respective post-mixer outs
- **MIX OUT**

### LPG
A 3-mode dynamics/tone section:
- **VCA**
- **LPG**
- **Lowpass filter**

### Envelope
ADSR envelope with **ENV IN** gate/trigger input and **ENV OUT**

### LFO
Triangle and square LFO, with low/high range switch. Can also run fast enough for audio-rate FM.

### Glide
Always between **1V/O IN** and oscillator pitch path.

### VCA
Final linear VCA after LPG by default.

---

# Controls Reference

## Waveforms Oscillator Controls
- **Frequency** — coarse tune
- **Fine Tune** — fine pitch adjust
- **Sub** toggle — sub oscillator level:
  - low volume / off / full volume
- **FM CV** knob — attenuates oscillator FM amount
- **Expo FM / Linear FM** toggle — selects FM response
- **Saw / Blade** toggle — chooses saw type sent to mixer/output
  - **Saw** = core saw, not affected by MOD CV
  - **Blade** = complex saw, affected by MOD CV and **BLADE IN**
- **MOD CV** knob — attenuates waveform modulation amount

## LPG Controls
- **MOD CV** knob — attenuates LPG frequency modulation amount
- **Mod / Ping** toggle
  - **MOD** = CV sweeps LPG/filter
  - **PING** = incoming CV is converted to a short strike
- **Frequency** — cutoff / pass level depending on mode
- **Resonance** — active in lowpass mode only
- **Mode** toggle
  - **Up:** VCA
  - **Center:** LPG
  - **Down:** Lowpass

## LFO Controls
- **Rate** — LFO speed
- **Range** toggle — low/high range

## Envelope Controls
- **Attack**
- **Decay**
- **Sustain** control/switch as labeled on panel/manual
- **Release**

## Glide Controls
- **Time** — portamento amount

## Mixer Controls
- **Triangle Wave** — level to TRI OUT and MIX OUT
- **Saw/Blade Wave** — level to S/B OUT and MIX OUT
- **Square Wave** — level to SQR OUT and MIX OUT

## VCA Controls
- **CV Input Attenuator / Output Level** — VCA level / CV amount

---

# Jack Reference

> **Important:** The manual page provided does **not specify numeric voltage ranges** for any CV or audio input/output jacks.  
> Therefore, exact **voltage ranges are undocumented in the manual**.

## Inputs

| Jack | Type | Function | Internal Normal |
|---|---|---|---|
| **1V/O IN** | CV in | 1V/oct pitch input to oscillator via glide | — |
| **BLADE IN** | CV/audio in | Manipulates Blade waveform | — |
| **FM CV IN** | CV in | External oscillator FM input; overrides internal FM routing | **LFO TRI** |
| **MOD CV IN** | CV in | External waveform modulation input; overrides internal modulation routing | **LFO TRI** |
| **LPG CV IN** | CV in | External LPG modulation input; overrides internal LPG CV routing | **ENV OUT** |
| **LPG IN** | Audio in | External signal into LPG; overrides internal audio routing | **Oscillator MIX OUT/internal voice path** |
| **ENV IN** | Gate/trigger in | Triggers envelope generator | — |
| **VCA CV IN** | CV in | External VCA CV; overrides internal VCA CV routing | **ENV OUT** |
| **VCA IN** | Audio in | External signal into VCA; overrides internal audio routing | **LPG OUT** |

## Outputs

| Jack | Type | Function | Voltage Range |
|---|---|---|---|
| **TRI OUT** | Audio out | Post-mixer triangle output | **Not specified in manual** |
| **S/B OUT** | Audio out | Post-mixer saw or blade output | **Not specified in manual** |
| **SQR OUT** | Audio out | Post-mixer square output | **Not specified in manual** |
| **MIX OUT** | Audio out | Mixed oscillator output incl. triangle, saw/blade, square, sub | **Not specified in manual** |
| **LFO TRI OUT** | CV out | Triangle LFO output | **Not specified in manual** |
| **LFO SQR OUT** | CV out | Square LFO output | **Not specified in manual** |
| **ENV OUT** | CV out | ADSR envelope output | **Not specified in manual** |
| **LPG OUT** | Audio out | LPG output | **Not specified in manual** |
| **VCA OUT** | Audio out | Final VCA output | **Not specified in manual** |

---

# Section-by-Section Usage Notes

## 1) Waveforms Oscillator
- The oscillator is the core voice.
- **Saw** gives a stable classic waveform.
- **Blade** gives a more animated/complex wave; best for timbral motion.
- **MOD CV** affects:
  - **Square** via pulse-width modulation
  - **Blade** via waveshape morphing
- **BLADE IN** adds further Blade-specific shaping.
- The **sub oscillator** thickens bass and adds weight.

### Good uses
- **Classic lead/bass:** Saw + sub
- **Hollow/animated:** Square with MOD CV
- **Aggressive/modern:** Blade with LFO or envelope to MOD CV

---

## 2) LPG
Three different personalities:

### VCA mode
- Pure amplitude control
- Best when you want clean level shaping

### LPG mode
- Characterful combo of filtering + amplitude behavior
- Louder sounds get brighter, quieter sounds mellow naturally
- Great for plucks, bongs, wood-like hits, organic decays

### Lowpass mode
- Traditional lowpass filtering
- **Resonance** active here only

### Ping mode
Use **Mod/Ping = PING** and send triggers/CV to **LPG CV IN** for struck/percussive sounds.

---

## 3) LFO
- **Low range:** slow sweeps
- **High range:** fast modulation and audio-rate FM territory
- Triangle is useful for smooth pitch/timbre motion
- Square is useful for stepped/trill/gate-like modulation

Typical destinations:
- **FM CV IN** for vibrato to harsh FM
- **MOD CV IN** for PWM / Blade movement
- **LPG CV IN** for rhythmic tone shaping
- **VCA CV IN** for tremolo

---

## 4) Envelope
Use **ENV IN** from gate or trigger source.

Typical uses:
- Default:
  - controls **LPG**
  - controls **VCA**
- Patch **ENV OUT** to **MOD CV IN** for timbral attack
- Patch **ENV OUT** to **FM CV IN** for pitch envelopes

### Envelope behavior notes
The manual describes standard ADSR behavior, though the Decay description appears unusual in wording. In practical use, treat it as the voice contour source for amplitude, LPG strike, or modulation.

---

## 5) Glide
- Adds portamento to incoming 1V/oct pitch CV
- Always sits between **1V/O IN** and oscillator
- Best for legato leads, acid slides, and smooth interval transitions

---

## 6) Mixer
The waveform mixer controls how much of each waveform hits:
- its own dedicated output
- the **MIX OUT**

The **sub oscillator** is included in **MIX OUT** per the manual.

### Good starting mixes
- **Bass:** Saw/Blade + sub, a little square
- **Lead:** Saw/Blade + triangle
- **Rounded tone:** Triangle dominant
- **Richer PWM lead:** Square + moderate MOD CV

---

## 7) VCA
- Linear VCA
- Normally receives:
  - audio from **LPG OUT**
  - CV from **ENV OUT**
- Final output is **VCA OUT**

Use it as:
- the normal end of the voice
- a standalone VCA for external audio/CV by patching **VCA IN**

---

# Internal Normalizations Summary

| Destination | Normal Source |
|---|---|
| Oscillator FM | **LFO TRI OUT** |
| Oscillator MOD CV | **LFO TRI OUT** |
| LPG CV | **ENV OUT** |
| VCA CV | **ENV OUT** |
| VCA audio in | **LPG OUT** |
| Oscillator pitch | **1V/O IN through Glide** |

---

# Practical Patch Ideas

## Simple bass
- **1V/O IN** from sequencer
- **ENV IN** from gate
- Mixer: Saw + Sub
- LPG mode: **LPG**
- Short attack, medium decay, low sustain, medium release
- Audio: **VCA OUT**

## West-coast style pluck
- Mixer: Triangle + Blade
- LPG mode: **LPG**
- **Mod/Ping = PING**
- Trigger **LPG CV IN**
- Optional slow LFO to **BLADE IN**
- Audio from **LPG OUT** or **VCA OUT**

## PWM lead
- Square wave up in mixer
- LFO TRI to **MOD CV IN**
- Light glide
- Envelope to VCA as normal
- Output from **VCA OUT**

## Audio-rate FM texture
- Set LFO to **high range**
- LFO TRI to **FM CV IN**
- Choose **Linear FM** for cleaner FM behavior
- Start with low FM amount

## Filtered external audio
- Patch external audio to **LPG IN**
- Use LPG in **LOPASS** mode
- Envelope or LFO to **LPG CV IN**
- Take output from **LPG OUT** or route onward to **VCA IN**

---

# Tips
- If a section seems unresponsive, check whether inserting a cable has broken its normalled source.
- Use **LPG mode** when you want the module’s most characteristic sound.
- Use **VCA mode** when you want predictable amplitude shaping.
- **Blade + MOD CV** is the fastest route to unusual animated timbres.
- **High-range LFO** can act as an extra audio-rate modulation source.

---

# Known Documentation Gaps
The supplied manual text does **not provide explicit voltage ranges** for:
- CV inputs
- audio inputs
- CV outputs
- audio outputs
- gate/trigger thresholds

So all jack voltage ranges remain **undocumented in the manual**.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)