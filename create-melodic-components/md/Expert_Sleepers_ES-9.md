# Expert Sleepers — ES-9

- [Manual PDF](../../manuals/es9_user_manual_1.3.pdf)

---

[ES-9 Firmware v1.3 User Manual (PDF / source)](https://expert-sleepers.co.uk/es9firmware.html)

# Expert Sleepers ES-9: using it to build melodic parts in a Eurorack system

The attached manual is for the **Expert Sleepers ES-9**, which is primarily a **USB/CV/audio interface and mixer/router** for Eurorack. By itself, it is **not a sound source, oscillator, sequencer, or quantizer**, so it does not directly generate melodies on its own. But in a modular music workflow, it is extremely powerful for **creating, controlling, recording, processing, and performing melodic material** when paired with a DAW, tablet, MIDI controller, or other Eurorack voice modules.

## What the ES-9 does musically

From the manual, the ES-9 gives you:

- **14 analog inputs** on 3.5mm jacks
- **8 DC-coupled 3.5mm analog outputs**
- **Main balanced outputs**
- **Headphone output**
- **S/PDIF I/O**
- **USB audio interface** with 16 ins / 16 outs to a computer/tablet
- **Internal mixer**
- **Optional MIDI breakout support**
- **DC-coupled I/O**, which is crucial for **CV as well as audio**

That combination makes it ideal as the bridge between:

- **DAW sequencing** and **modular voices**
- **Software quantizers/arpeggiators/LFOs/envelopes** and hardware
- **Eurorack oscillators/filters/VCAs** and multitrack recording
- **Live performance mixing** and headphone cueing

---

## Best role of the ES-9 in melodic patching

For melody-making, think of the ES-9 as four things:

1. **A CV output hub**  
   Send pitch CV, gates, envelopes, modulation, clocks, and automation from your DAW or software into the rack.

2. **An audio input hub**  
   Bring oscillators, full synth voices, filters, and final melodic lines back into the DAW for recording or effects.

3. **A monitor/mixer/router**  
   Build cue mixes, layered melodic stems, headphone mixes, or direct monitoring paths.

4. **A MIDI bridge**  
   Use MIDI controllers or a MIDI breakout to control mixer states or integrate external sequencing workflows.

---

## Why it is useful for melodic music specifically

The key feature here is that the ES-9’s **3.5mm analog outputs are DC-coupled**, and the inputs are also DC-coupled. The manual explicitly says the outputs can be used for **audio or CVs**, and the inputs can also be used for **CVs as well as audio**.

That means you can use software to generate:

- **1V/oct pitch CV**
- **gates/triggers**
- **modulation curves**
- **stepped sequencer voltages**
- **envelopes**
- **random voltages**
- **automation lanes**
- **quantized melodic patterns**

and route them from the computer directly into Eurorack voice modules.

This is where melody comes from.

---

## Core melodic use cases

## 1. DAW-to-modular melodic sequencing

This is probably the most important melodic application.

### Patch concept
Use the ES-9 outputs to send:
- **Pitch CV** to an oscillator’s 1V/oct input
- **Gate** to an envelope or function generator
- **Envelope or modulation CV** to filter cutoff, wavefolder, FM amount, or VCA

### Example
- **ES-9 output 1** → oscillator 1V/oct
- **ES-9 output 2** → envelope gate input
- **ES-9 output 3** → filter cutoff modulation
- Oscillator/filter/VCA audio output → **ES-9 input 1**

Now your DAW can act as:
- piano-roll sequencer
- CV recorder
- automation source
- quantizer
- probabilistic melody generator

### Musical result
You can write precise basslines, leads, arpeggios, ostinatos, generative melodies, or harmonic lines in software and play them on real Eurorack voices.

---

## 2. Polyphonic melodic control

Because the ES-9 has **8 DC-coupled analog outputs**, you can drive multiple simultaneous control signals.

For example, each voice usually needs at least:
- 1 pitch CV
- 1 gate

So 8 outputs could become:

- **4-voice pitch/gate polyphony**, or
- **2 voices** with lots of additional modulation, or
- **1 rich melodic voice** with multiple expressive CV lanes

### Example 4-voice patch
- Out 1 → Voice 1 pitch
- Out 2 → Voice 1 gate
- Out 3 → Voice 2 pitch
- Out 4 → Voice 2 gate
- Out 5 → Voice 3 pitch
- Out 6 → Voice 3 gate
- Out 7 → Voice 4 pitch
- Out 8 → Voice 4 gate

Then return each voice or a submix into the ES-9 inputs.

### Musical result
- chords
- harmonized melodies
- counterpoint
- stacked unison riffs
- DAW-controlled modular polyphony

---

## 3. Recording and layering melodic voices

The ES-9 has **14 analog inputs**, so it can capture many melodic sources at once.

### Useful melodic workflow
Patch several melodic modules into separate ES-9 inputs:
- bass voice
- lead voice
- pluck voice
- drone voice
- modulation CV for analysis or reuse

Because the ES-9 can directly route hardware inputs to USB inputs, you can record each melodic component as a separate track in your DAW.

### Musical result
- multitrack modular composition
- separate processing of lead and bass parts
- easier arrangement
- tighter editing and layering

This is especially valuable if your rack has multiple oscillators or complete voices.

---

## 4. Software quantizer + hardware voice

The ES-9 does not quantize pitch internally, but it makes it easy to use a **software quantizer** to produce clean melodies.

### Workflow
- Generate or record a rough CV sequence in software
- Quantize it to a scale in the DAW/plugin environment
- Send quantized pitch out through an ES-9 output
- Send to oscillator 1V/oct

### Musical result
- scale-locked melodies
- modal improvisation
- evolving generative phrases
- easy key changes

This is a strong hybrid approach if your rack does not contain a dedicated quantizer.

---

## 5. Hybrid sequencing with modulation-rich melodic phrasing

Melody in modular is often more than pitch and gate. The ES-9 is useful because it lets you add many simultaneous control streams.

### Example expressive melodic patch
- Out 1 → pitch
- Out 2 → gate
- Out 3 → velocity-style envelope depth
- Out 4 → filter accent
- Out 5 → FM depth
- Out 6 → wavefold amount
- Out 7 → vibrato depth
- Out 8 → clock/reset or an extra articulation signal

### Musical result
A single sequenced melody can become animated and expressive, more like a performed line than a static step sequence.

---

## 6. Use the internal mixer for monitoring melodic work

The manual describes an internal **8x8 crosspoint mixer** and optional second mixer instead of S/PDIF. This matters for composition and performance.

You can:

- monitor melodic voices without relying entirely on the DAW
- create separate **main out** and **headphone** mixes
- cue a melodic part in headphones
- blend DAW playback with live modular audio

### Default mixer behavior from the manual
By default:
- main outputs carry USB 1/2
- headphones mix 1/2 with 3/4

That means you can create a performance workflow like:
- DAW backing track on USB 1/2
- live melodic synth voice on USB 3/4 or routed mixer channels
- monitor both in phones while sending only selected material to mains

### Musical result
This is excellent for:
- live techno performance
- rehearsing melodic improvisation
- overdubbing new melodic lines over an existing arrangement

---

## 7. Standalone melodic submixer in a rack

The ES-9 stores **two configurations**:
- hosted
- standalone

This is very useful if your melodic workflow alternates between:
- computer-connected composing
- standalone rack performance

### Example
**Hosted config**
- DAW outputs become pitch/gate/modulation sources
- all voice audio returns to DAW

**Standalone config**
- analog inputs become mixer inputs
- second mixer enabled
- direct monitor routing for live patching without computer dependence

### Musical result
You can rehearse or perform melodic patches even if the computer is disconnected, then reconnect later for composition/recording.

---

## 8. CV recording and analysis of melodic behavior

Since the inputs are DC-coupled, you can also record **CVs**, not only audio.

That means you can capture:
- pitch sequences from an external sequencer
- envelope shapes
- modulation affecting melodic timbre
- random voltage patterns driving note choice

### Why this matters
You can study and reuse melodic behavior:
- record an analog sequencer’s pitch CV
- edit or scale it in software
- send it back out through ES-9 outputs
- turn one improvised phrase into a composed motif

### Musical result
A strong feedback loop between hardware improvisation and software arrangement.

---

## 9. Building a complete hybrid melodic voice chain

A practical “used together” interpretation for this module is the way its own sections work together:

- **USB audio block**
- **Mixer block**
- **S/PDIF or Mixer 2**
- **Routing matrix**
- **DC-coupled outputs**
- **Audio/CV inputs**

These can all be combined into one melodic ecosystem.

### Example full melodic workflow

#### Control side
- DAW sends:
  - pitch CV
  - gate
  - accent
  - filter automation

through ES-9 3.5mm outputs.

#### Synthesis side
- Eurorack oscillator + filter + VCA create the melodic line.

#### Return side
- dry oscillator output into one ES-9 input
- post-filter output into another
- final VCA output into another

#### Monitoring side
- use internal mixer to hear a cue mix
- headphones carry layered melody + click/backing track
- main outs carry performance mix

#### Composition side
- record each stage separately in DAW
- later re-sequence pitch or automation
- replay through the rack

This is one of the strongest hybrid melodic setups available in Eurorack.

---

## Important technical points from the manual for melodic patching

## 1. Input DC blocking must be off for CV
The manual says input DC-blocking filters are recommended for audio, but **must be turned off for CV**.

So:
- for recording audio from a melodic voice: DC blocking **on** is often appropriate
- for recording pitch CV, envelopes, or gates: DC blocking **off**

This is crucial if you want to capture or process melodic CV accurately.

---

## 2. Balanced main outputs are not DC-coupled
The **balanced 1/4" main outputs are not DC-coupled**, so they are for:
- speakers
- mixer
- audio monitoring

Not for CV.

For melodic CV duties, use the **8 analog 3.5mm outputs**.

---

## 3. Headphone output is DC-coupled
The manual notes the headphone output is DC-coupled, but in practice for melodic patching, the main intended CV outputs are still the dedicated 3.5mm outs. The headphone path is more naturally used for monitoring.

---

## 4. Approximate voltage ranges
The manual states:
- input voltage of approx **±10V** gives 0 dBFS in the DAW
- 3.5mm outputs have max output of approx **±10V**

That is important for Eurorack compatibility and means the ES-9 can interface well with typical pitch CV and modulation ranges.

---

## 5. Internal routing can be confusing
The manual warns that routing can easily end up with audio “going nowhere.” For melodic use, start simple:

- route DAW/CV outputs directly to selected analog outputs
- route melodic voice outputs directly to USB inputs
- only then add mixer and monitor complexity

That will save a lot of troubleshooting.

---

## Good melodic patch ideas using ES-9

## Patch 1: DAW-controlled mono lead
- Out 1: pitch CV to oscillator
- Out 2: gate to envelope
- Out 3: filter cutoff modulation
- Voice audio back to In 1
- Monitor via main outs/headphones

**Result:** tight, repeatable lead melodies with analog tone.

---

## Patch 2: Bass + lead dual voice
- Out 1/2: bass pitch/gate
- Out 3/4: lead pitch/gate
- Out 5: bass accent
- Out 6: lead filter envelope amount
- Bass audio → In 1
- Lead audio → In 2

**Result:** two independent melodic parts recorded separately.

---

## Patch 3: Generative melody rig
- Software random sequencer generates voltages
- Quantizer plugin constrains to scale
- ES-9 sends pitch + trigger to modular voice
- Audio returns on inputs
- Additional DAW automation morphs timbre

**Result:** evolving melodic phrases with hardware sound and software intelligence.

---

## Patch 4: Polyphonic chord stabs
- Use 8 outputs as 4 pitch/gate pairs
- Send to four oscillators or four complete voices
- Return summed or individual audio to ES-9 inputs

**Result:** modular chord progressions, harmonized hooks, lush layered motifs.

---

## Patch 5: Record-and-replay analog melody
- External hardware sequencer sends pitch CV to oscillator and split to ES-9 input
- ES-9 records the pitch CV
- DAW edits timing/quantization
- Edited CV sent back out through ES-9 output

**Result:** improvised analog melody turned into an editable composition.

---

## Patch 6: Live melodic performance mixer
- DAW backing tracks on USB 1/2
- Live modular lead on analog input
- Headphone mix includes cue material
- Main outs carry performance blend

**Result:** perform melodic lines live over arranged material.

---

## Limitations to be aware of

The ES-9 does **not** itself provide:
- oscillator tones
- pitch quantization
- step sequencing
- envelopes
- gates
- note generation
- internal melodic pattern generation

So to create actual melodic content, it needs to be used with:
- a DAW or CV-generating software
- external Eurorack oscillators/voices
- or external sequencers/quantizers/controllers

In other words, the ES-9 is the **infrastructure** for melody, not the melody engine itself.

---

## Best pairings for melodic creation

The ES-9 works especially well with:

- **Oscillators / complete synth voices**  
  for the actual sound source

- **VCAs and envelopes**  
  for note articulation

- **Filters / wavefolders / LPGs**  
  for shaping melodic timbre

- **DAW CV tools or plugins**  
  for pitch, gates, quantization, randomization, automation

- **MIDI keyboard or controller**  
  to perform or automate melodies through the computer

- **ES-5 expansion**  
  if you need expanded gate/clock/control capabilities

---

## Practical summary

## What this module contributes to melodic music
The Expert Sleepers ES-9 is best understood as a **hybrid composition and performance hub** for melodic Eurorack work. It allows you to:

- send pitch/gate/modulation from software to modular
- bring melodic audio back into the DAW
- record multiple melodic voices at once
- monitor and mix parts internally
- store different hosted/standalone configurations
- integrate MIDI and optional expansion modules

## What it is best at
It excels at:
- DAW-driven melodic sequencing
- hybrid modular/software composition
- multitrack recording of melodic patches
- live performance monitoring and routing
- CV generation and capture

## What you need alongside it
To actually produce notes and melodies, pair it with:
- one or more oscillators or voices
- an envelope/VCA chain
- a sequencer or DAW CV software
- optionally a quantizer or MIDI keyboard

So in a musical system, the ES-9 is the **bridge that lets your melodic ideas move freely between software and Eurorack hardware**.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)