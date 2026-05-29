# Pittsburgh Modular — Synthesizer Box

- [Manual PDF](../../manuals/Synthesizer Box - Pittsburgh Modular Synthesizers.pdf)

---

[Manual PDF](https://pittsburghmodular.com/s/Synthesizer-Box.pdf)

# Pittsburgh Modular Synthesizer Box: using the module for melodic music

The **Synthesizer Box** is essentially a **complete analog mono voice** in 28hp. For melodic work, that means you already have the core building blocks you need in one module:

- **Oscillator** for pitch
- **Wave mixer** for timbre
- **LPG / filter / VCA-like dynamics block** for tone shaping
- **ADSR envelope** for note articulation
- **VCA** for final loudness control
- **LFO** for movement
- **Glide** for portamento between notes

Because it is **semi-modular**, it can work immediately as a playable voice with no patching, but the patch points let you break it apart and re-route sections for more expressive melodic lines.

---

## 1. The built-in melodic signal path

Internally, the Synthesizer Box is normalled so it already behaves like a synth voice:

- **1V/O IN** goes to the oscillator through **Glide**
- The **LFO triangle** is internally routed to:
  - oscillator **FM**
  - oscillator **MOD CV**
- The **Envelope OUT** is internally routed to:
  - **LPG CV IN**
  - **VCA CV IN**
- The oscillator mixer output is intended to feed the **LPG**
- The **LPG OUT** is internally routed to the **VCA IN**
- Final output is **VCA OUT**

So for melodic use, the simplest setup is:

1. Send a pitch sequence to **1V/O IN**
2. Send gates/triggers to **ENV IN**
3. Take audio from **VCA OUT**

That gives you a complete monosynth line.

---

## 2. What each section contributes melodically

## Waveforms oscillator: the pitch and harmonic core

The oscillator is the heart of melody here. It provides:

- **Triangle**
- **Saw or Blade**
- **Square**
- **Sub oscillator** one octave below
- A **post-mixer MIX OUT** combining selected waveforms

For melodic writing, this gives you several useful voice types:

- **Triangle**: smooth, flute-like, good for soft leads and basses
- **Saw**: classic bright synth lead for clear note definition
- **Blade**: more complex and animated than a standard saw, excellent for expressive lead lines
- **Square**: hollow, woody tone; good for melodic hooks
- **Sub oscillator**: adds weight for bass melodies and powerful mono leads

### Melodic tip
For lines that must cut through a mix, start with:
- Saw/Blade level up
- A little square
- Sub oscillator at low or full as needed

For gentler melodies:
- Triangle higher
- Less saw/blade
- Minimal sub

---

## Mixer: controlling melodic tone before filtering

The oscillator mixer lets you adjust the amount of:

- Triangle
- Saw/Blade
- Square
- Plus the sub oscillator in the overall mixed sound

This matters musically because melody is not only pitch — it is also **timbre across phrases**. You can make the same note sequence function differently by changing waveform balance:

- More **triangle** = rounder, more legato lead
- More **square** = nasal, defined melody
- More **saw/blade** = brighter, more urgent phrase
- More **sub** = bass-heavy melodic voice

---

## Glide: making phrases sing

The **Glide** control is hardwired between **1V/O IN** and the oscillator.

Use glide for:

- **Acid-style slides**
- **Legato lead phrasing**
- **Expressive mono solos**
- **Basslines with note smearing between selected steps**

For melodic material, small amounts of glide can make a simple sequencer line feel much more performed and vocal.

---

## Envelope: shaping each note

The **ADSR envelope** is triggered from **ENV IN** and sent internally to LPG and VCA.

This is crucial for melody because it determines how notes speak:

- **Attack**: whether notes pluck, bloom, or swell
- **Decay**: how quickly energy falls from the initial hit
- **Sustain**: whether notes hold strongly while the gate is high
- **Release**: whether phrases stop sharply or trail off

### Good melodic envelope settings
- **Plucky sequence**: fast attack, short decay, low sustain, short release
- **Lead line**: fast-medium attack, medium decay, medium sustain, short-medium release
- **Pad-like pseudo-legato mono line**: slower attack, longer decay, higher sustain, longer release

---

## LPG: the secret to organic melodic articulation

The **LPG** is one of the most musically distinctive parts of the module. It can operate in three modes:

- **VCA mode**
- **LPG mode**
- **Lowpass filter mode**

This is especially useful for melody because it lets you choose how each note behaves dynamically and harmonically.

### VCA mode
Use this when you want clean amplitude shaping and more neutral tone.

Best for:
- Precise sequences
- Tight bass melodies
- Simple, controlled synth leads

### LPG mode
This is often the sweet spot for melodic parts. Louder sounds become brighter, and quieter sounds are less altered. This mimics the natural way many acoustic instruments behave.

Best for:
- Expressive plucks
- Organic basslines
- Buchla-like melodic patterns
- Lines that need “wood” or “body”

### Lowpass mode
Use this for classic subtractive voice shaping.

Best for:
- Filtered leads
- Sweeping basslines
- Melodies that evolve in brightness over time

### Ping mode
The **Mod/Ping switch** lets the LPG CV behave differently:
- In **MOD** mode, CV sweeps the LPG normally
- In **PING** mode, incoming CV is converted to a short strike

For melodic work, ping is excellent when you want:
- Percussive notes from a sequencer
- Marimba/pluck-like tones
- Short melodic ostinatos with a natural decay

---

## VCA: final dynamic control

The **VCA** is the final amplitude stage, with:

- **VCA IN**
- **VCA CV IN**
- **VCA OUT**

Internally:
- **VCA IN** gets **LPG OUT**
- **VCA CV IN** gets **ENV OUT**

So in standard melodic use, the LPG shapes tone and/or level, then the VCA applies final amplitude contour. This gives notes definition and polish.

That two-stage dynamic structure is very useful:
- LPG adds organic tone movement
- VCA provides clean final articulation

---

## LFO: adding movement to pitch and timbre

The LFO outputs:
- **Triangle**
- **Square**

Internally, the triangle is already routed to oscillator **FM** and **MOD CV** unless you override with patch cables.

For melody, the LFO can create:

- **Vibrato** via oscillator FM
- **PWM / shape animation** via MOD CV
- **Rhythmic pitch pulses** with square output
- **Timbre evolution** across sustained notes

Because the LFO has a **wide range**, it can also reach audio rates, so you can use it for more aggressive FM textures if you want brighter or metallic melodic tones.

---

# Practical melodic patch ideas

## 1. Straight mono lead
**Goal:** classic playable lead voice

**Patch**
- Sequencer or keyboard pitch CV -> **1V/O IN**
- Gate -> **ENV IN**
- Audio out from **VCA OUT**

**Settings**
- Saw or Blade up in mixer
- Medium sustain
- Short-medium release
- LPG in **lowpass** or **VCA** mode
- Slight glide

**Result**
A straightforward analog lead for melodies, hooks, and solos.

---

## 2. Organic plucked melody
**Goal:** woody, expressive melodic notes

**Patch**
- Pitch CV -> **1V/O IN**
- Trigger or short gate -> **ENV IN**
- **VCA OUT** to mixer/output

**Settings**
- LPG in **LPG** mode
- Mod/Ping in **PING** mode or use short envelope in MOD mode
- Fast attack
- Short decay
- Low sustain
- Short release
- Triangle + a little Blade

**Result**
Bell/pluck-like notes with natural decay, ideal for arpeggios and minimal melodic patterns.

---

## 3. Bass melody with weight
**Goal:** melodic bassline

**Patch**
- Pitch CV -> **1V/O IN**
- Gate -> **ENV IN**
- Audio from **VCA OUT**

**Settings**
- Sub oscillator on
- Square + Saw/Blade mixed
- LPG in **VCA** or **lowpass** mode
- Fast attack
- Medium-short decay
- Low to medium sustain
- Short release
- Small amount of glide

**Result**
A thick mono bass voice that still tracks melody clearly.

---

## 4. Animated lead with internal modulation
**Goal:** moving, expressive timbre without extra modules

**Patch**
- Pitch CV -> **1V/O IN**
- Gate -> **ENV IN**
- Use default internal routings
- Audio from **VCA OUT**

**Settings**
- LFO rate slow-medium
- Turn up oscillator **FM CV** slightly for vibrato
- Turn up **MOD CV** slightly for waveform animation
- Use **Blade** mode
- Medium sustain/release

**Result**
A lead that slowly shifts in pitch color and waveform shape, giving long notes life.

---

## 5. Filtered sequence
**Goal:** classic subtractive melodic sequence

**Patch**
- Pitch CV -> **1V/O IN**
- Gate -> **ENV IN**
- Oscillator mixer normalled to LPG
- Audio from **VCA OUT**

**Settings**
- LPG in **LOPASS** mode
- Envelope routed internally to LPG
- Medium resonance
- Lower frequency setting
- Saw or Blade prominent

**Result**
A melodic sequence with bright attacks and darker tails, very effective for Berlin-school or techno patterns.

---

## 6. Two-layer articulation patch using patch points
**Goal:** separate tone motion from loudness motion

**Patch**
- Pitch CV -> **1V/O IN**
- Gate -> **ENV IN**
- Use **ENV OUT** multed externally if available:
  - one path to **LPG CV IN**
  - another path to **VCA CV IN**
- Take **MIX OUT** -> **LPG IN**
- **LPG OUT** -> **VCA IN**
- **VCA OUT** to output

**Idea**
Even though this is similar to the internal normaling, patching manually makes the signal path explicit and easier to integrate with the rest of a Eurorack system. If you later insert attenuators, offsets, or other CV processors, you can make the filter/LPG movement different from the final amplitude contour.

**Result**
More refined melodic shaping and better integration with external utility modules.

---

# How the sections work together musically

## A. Pitch from the oscillator + glide
This creates the note content.

## B. Mixer sets note identity
This determines whether the melody feels soft, sharp, nasal, heavy, or animated.

## C. Envelope determines note phrasing
This gives the melody articulation: plucked, sustained, legato, or swelling.

## D. LPG/filter determines expressive brightness
This adds acoustic-like behavior and timbral motion to each note.

## E. VCA gives final contour
This tightens the performance and makes phrases sit correctly in a mix.

## F. LFO adds movement
This keeps repeated notes alive through vibrato and waveform animation.

Together, these turn a simple pitch-and-gate sequence into a genuinely musical melodic voice.

---

# Best melodic workflows

## 1. Use it as your main mono voice
The Synthesizer Box is ideal as the central melodic voice in a small rack. Add:
- a sequencer
- a keyboard controller
- maybe delay/reverb after it

and you already have a complete lead/bass instrument.

## 2. Use the LPG for expressive phrasing
If you want less “plain synth” and more “instrument-like” response, spend time with:
- **LPG mode**
- **Ping mode**
- short envelopes

This is where a lot of the module’s personality comes from.

## 3. Use Blade for more modern melodic tones
The **Blade** waveform seems especially useful when you want animated harmonics that feel more complex than a standard saw lead.

## 4. Exploit the internal routings first
Before complicated patching, start with the normalled paths:
- LFO to oscillator FM and MOD
- Envelope to LPG and VCA

These routings already provide a lot of melodic expression with very little setup.

---

# Limitations to keep in mind for melodic use

Because this is a **monophonic voice**, it is best for:

- basslines
- lead lines
- arpeggios
- sequenced melodic motifs
- drones with melodic inflection

It is **not** a polyphonic module on its own, so chords would require overdubbing, multiple voices, or external processing.

Also, there is only one onboard envelope and one VCA, so its architecture is focused on **single-voice expressiveness**, not layered internal polyphony.

---

# Summary

The Pittsburgh Modular **Synthesizer Box** is very strong for melodic composition because it combines:

- a flexible oscillator with multiple waveform colors
- a sub oscillator for strong bass and lead fundamentals
- a waveform mixer for tonal blending
- glide for phrasing
- an ADSR for note articulation
- a distinctive LPG for organic dynamics
- a VCA for clean final shaping
- an LFO for motion and modulation

In practice, it works best as:

- a **mono lead voice**
- a **melodic bass voice**
- a **plucked sequence generator**
- an **organic LPG-based melodic instrument**

Its biggest strength is that it can go from **instant classic monosynth melody** to **patchable modular expressiveness** without needing much external support.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)