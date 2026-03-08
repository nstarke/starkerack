# Sound Machines — Modulor 114

- [Manual PDF](../../manuals/MODULOR114-MANUAL-SEP16-V01.pdf)

---

[MODULÖR114 Owner’s Manual (PDF/manual source)](http://www.sound-machines.it/product/modulor114)

# Creating melodic components with the Soundmachines MODULÖR114

The MODULÖR114 is unusually strong as a **self-contained melodic modular voice** because it combines:

- pitch sources: **USB MIDI/CV**, **Ribbon**, **Quantizer**, **S&H**
- sound sources: **VCO1**, **VCO2/LFO1**, **MIDI square/DCO**
- shaping: **VCF**, **VCA**, **ENV**
- utilities for musical control: **attenuators, mixers, slew, add/sub, multiples**
- time/rhythm tools: **MIDI clock, clock divider, logic**
- finishing: **FX unit**

So instead of thinking of it as “just a synth voice,” think of it as a machine that can generate melody in several ways:

1. **Played melody** from MIDI keyboard  
2. **Performed melody** from the ribbon  
3. **Quantized generative melody** from LFO/noise/S&H  
4. **Layered melodic motion** by mixing/transposing CV  
5. **Rhythmic melodic patterns** via gates, clock division, and logic

---

# Core melodic building blocks in the MODULÖR114

## 1. MIDI section
This is the most direct melodic entry point.

Relevant outputs/functions from the manual:

- **PITCH**: 1V/oct melodic pitch CV from MIDI notes
- **GATE**: gate from note on/off
- **MOD/Q**: either mod wheel CV or quantizer output
- **16TH**: MIDI clock-derived rhythmic pulse
- additional **CV#30–33** analog outputs/functions from MIDI CCs

### Melodic use
- Patch **PITCH** to **VCO1 V/OCT** and/or **VCO2 V/OCT**
- Patch **GATE** to **ENV GATE**
- Use **MOD/Q** as an additional melodic line when the quantizer is active
- Use **16TH** to trigger sample-and-hold or clock divisions for sequenced note movement

This gives you a classic keyboard-controlled monosynth, but it also acts as the central source for transposition and timing.

---

## 2. VCO1
VCO1 is the primary tone generator and one of the main melodic voices.

Outputs include:
- **SAW**
- **TRI**
- **SQU**
- **SUB**
- **WHITE/PINK noise**
- **MIDI** square/DCO output nearby in the system section

Inputs include:
- **V/OCT**
- **CV**
- **PWM**
- **SYNC**

### Melodic use
For melody, VCO1 is your “instrument.” Different outputs give different roles:

- **Saw**: best for leads and basses through the VCF
- **Triangle**: smoother melody, flute-like or softer tones
- **Square/PWM**: excellent for animated lead lines
- **Sub**: reinforces bass notes one octave down

The key melodic patch is:
- **pitch CV into V/OCT**
- optionally another modulation into **CV** for vibrato or expressive movement

You can also create more harmonically rich melodic tones by:
- mixing **SAW + SQU**
- using **PWM** with an LFO for evolving sustained notes
- using **SYNC** from VCO2 for aggressive lead sounds

---

## 3. VCO2 / LFO1
This is dual-purpose: either a second oscillator or a modulation source.

### As a melodic oscillator
Patch the same pitch CV to both VCOs:
- **PITCH -> MULTI -> VCO1 V/OCT + VCO2 V/OCT**

Then use VCO2 as:
- a unison detuned layer
- an interval voice if offset by a mixer/add-sub
- a sync master for VCO1
- a drone root note against a moving melodic VCO1

### As a melodic modulator
Switch it to LFO mode and use it to:
- create vibrato on oscillator pitch
- step or sweep filter cutoff during melodic lines
- animate PWM for sustained melodic parts

This module is crucial because melody in modular often comes from **controlled pitch plus controlled variation**.

---

## 4. Quantizer
This is one of the most important melody generators in the system.

The quantizer takes an incoming CV and forces it to musical notes in a selected scale. The manual mentions multiple scales including chromatic and modal options.

- **Input**: **Q IN**
- **Output**: **MOD/Q** when quantizer is active

### Why this matters
Any changing voltage can become melody:
- ribbon
- LFO
- S&H
- noise
- manual voltage from GEN1/GEN2
- mixed voltages from mixers or ADDSUB

### Melodic use
Without a quantizer, most voltages produce glides or atonal pitch movement.  
With the quantizer, they become note sequences.

Examples:
- **LFO -> ATT -> Q IN -> MOD/Q -> VCO V/OCT**
- **S&H OUT -> Q IN -> MOD/Q -> VCO V/OCT**
- **Ribbon CV -> Q IN -> MOD/Q -> VCO V/OCT**

This is the bridge between “modulation” and “music.”

---

## 5. Ribbon controller
The ribbon is one of the best melodic performance tools on the panel.

Outputs:
- **CV**
- **CV HOLD**
- **GATE**

### Melodic use
You can use the ribbon in two main ways:

#### A. Continuous pitch performance
- **Ribbon CV -> VCO V/OCT**
- **Ribbon GATE -> ENV GATE**

This gives fretless/theremin-like expression.

#### B. Quantized playable melody
- **Ribbon CV -> Q IN**
- **MOD/Q -> VCO V/OCT**
- **Ribbon GATE -> ENV GATE**

Now finger position becomes scale-constrained notes. This is great for improv melodies without worrying about wrong notes.

#### Why CV HOLD matters
CV HOLD preserves the last pitch after releasing, which is very useful if your amp envelope has release time. Otherwise notes would drop immediately in pitch at note end.

---

## 6. S&H (Sample and Hold)
This is the system’s generative melody engine.

Inputs:
- **IN**
- **SAMPLE**
- **TRACK**
- output: **OUT**

### Melodic use
S&H samples a voltage whenever it gets a trigger. If you sample:
- noise -> random melody
- LFO -> stepped cyclic melody
- ribbon/manual voltage -> performed step notes
- slow CV mixtures -> evolving semi-predictable melody

Best melodic patch:
- **Noise or LFO -> S&H IN**
- **Clock trigger -> S&H SAMPLE**
- **S&H OUT -> Q IN**
- **MOD/Q -> VCO V/OCT**

Now you have a stepped sequence of notes in a selected scale.

This is one of the strongest “modular melody” patches in the whole instrument.

---

## 7. SLEW
Slew is vital for melodic phrasing.

### Melodic use
Insert it between pitch source and oscillator:

- **PITCH -> SLEW -> VCO V/OCT**
- or **MOD/Q -> SLEW -> VCO V/OCT**

This creates:
- portamento/glide
- acid-style note slides
- smoother random melodies
- legato-feeling generative lines

It’s especially effective after the quantizer or S&H:
- quantizer gives stepped notes
- slew turns those into expressive glides

---

## 8. ENV + VCA
These don’t create melody directly, but they make melody musical.

### ENV
Shapes note articulation:
- pluck
- stab
- pad
- acid snap
- held lead

### Melodic use
- **GATE -> ENV GATE**
- **ENV OUT -> VCA CV**
- optionally **ENV OUT -> ATT -> VCF CV**

This determines whether your melody sounds:
- percussive
- legato
- punchy
- swelling
- expressive

Short decay + low sustain = sequence/pluck  
Long attack/release = ambient melodic lines  
ENV to filter = classic melodic synth phrasing

---

## 9. VCF
The filter is essential for separating melody from raw oscillator tone.

### Melodic use
A melody becomes expressive when cutoff tracks note articulation.

Use:
- oscillator mix into **VCF IN**
- **ENV OUT -> ATT -> VCF CV**
- optionally **LFO** or **S&H** to VCF CV for evolving timbre

For melodic parts:
- low resonance for smoother leads
- medium resonance for acid-ish basslines
- bandpass for thinner melodic voices
- self-oscillation can even become a sine-like pitched source if carefully controlled

A strong melodic phrase often comes from **static pitch + dynamic filter contour** as much as from note choice.

---

## 10. Mixers, attenuators, ADDSUB, GEN1/GEN2, MULTI
These utilities are where melodic sophistication comes from.

---

# How the utility modules help create melody

## MULTI
Duplicates pitch CV or gate.

### Melodic use
- Send one pitch line to both oscillators
- Send a gate to both ENV and another rhythmic destination
- Split quantizer output to several destinations

Example:
- **PITCH -> MULTI -> VCO1 V/OCT + VCO2 V/OCT**

---

## ATT1/2/3
Control modulation depth.

### Melodic use
- fine control vibrato amount
- control how much ENV affects filter
- scale LFO or random voltage before quantizing
- set subtle pitch drift into oscillator CV input

These are critical for keeping melodic modulation musical rather than chaotic.

---

## MIX1 / MIX2 / MIX3
Useful for audio mixing, but also CV combination.

### Melodic use for CV
You can combine melodic sources:
- base pitch + transposition voltage
- pitch + vibrato
- pitch + envelope pitch sweep
- ribbon + offset
- quantized melody + manual bias

For example:
- **PITCH + GEN1** in a mixer can transpose a played melody
- **PITCH + LFO** can create vibrato before the oscillator
- **S&H + offset** can constrain random melody to a preferred register

Because the system is DC-coupled in many places, these mixers are very useful for control voltages.

---

## GEN1 / GEN2
Manual CV sources from 0–5V.

### Melodic use
These are simple but powerful:
- transposition offsets
- fixed pedal/root note
- manual pitch source into quantizer
- source for S&H to create repeated selectable note pools

Example:
- **GEN1 -> Q IN**
- **MOD/Q -> VCO V/OCT**

This gives a manually tunable note source constrained to a scale.

Or:
- **PITCH + GEN1 -> mixer -> VCO V/OCT**
to shift a keyboard melody up or down.

---

## ADDSUB
A very musical utility for pitch arithmetic and waveshaping.

The manual states:
- output = **IN+ - IN-**
- result saturated/clamped to 0–5V

### Melodic use
This can do several melodic jobs:

#### A. Transposition
- send melodic pitch CV to **IN+**
- send a lower manual offset or modulation to **IN-** or another input arrangement
- use result as altered pitch

#### B. Inverted modulation
If you want filter movement opposite to envelope or opposite to note motion:
- ENV or pitch CV into ADDSUB for inversion/subtraction

#### C. Pseudo-VCA on CV/audio
Can reshape melodic modulation behavior in unusual ways.

Because it clamps to 0–5V, it also helps keep some melodic voltages in the module’s expected range.

---

# Best melodic patch strategies

## 1. Classic monosynth melody
This is the built-in **SYNTH!** idea.

### Patch
- Enable **SYNTH!**
- USB keyboard into HOST, or MIDI from computer/device
- **PITCH** internally drives VCOs
- **GATE** drives ENV
- VCOs -> MIX1 -> VCF -> VCA -> FX -> Output
- ENV controls VCA and VCF through ATT1/ATT2

### Best for
- leads
- basslines
- simple melodic hooks

### Improve it by hand
- detune VCO2 slightly for width
- use PWM on VCO1 square
- send LFO to PWM or VCF
- apply SLEW to pitch if not using only internal prepatch logic

---

## 2. Quantized ribbon melody
One of the most playable patches in the instrument.

### Patch
- **Ribbon CV -> Q IN**
- **MOD/Q -> VCO1 V/OCT**
- **Ribbon GATE -> ENV GATE**
- VCO1 -> VCF -> VCA -> Output

Optional:
- **Ribbon CV HOLD** instead of CV for more stable release behavior
- Duplicate quantized output to VCO2 too

### Result
You get scale-locked melodic performance with tactile control. Excellent for live improvisation.

### Best for
- solos
- modal improvisation
- ambient melody lines
- expressive slides when combined with SLEW

---

## 3. Generative random melody
A classic modular patch made easy on this unit.

### Patch
- **WHITE or PINK noise -> S&H IN**
- **16TH** or **CLKDIV output -> S&H SAMPLE**
- **S&H OUT -> Q IN**
- **MOD/Q -> VCO1 V/OCT**
- rhythmic gate source -> **ENV GATE**

Optional:
- **SLEW** after quantizer for glides
- use **VCF ENV** for articulation
- send same quantized CV to both oscillators

### Result
Random notes constrained to a scale, musically usable immediately.

### Best for
- Berlin-school style sequences
- ambient generative melody
- arpeggio-like motifs
- evolving ostinatos

---

## 4. Cyclic stepped melody from LFO
Less random, more repeatable.

### Patch
- **LFO2 TRI** or **VCO2/LFO SAW/TRI -> ATT -> S&H IN**
- clock source -> **S&H SAMPLE**
- **S&H OUT -> Q IN**
- **MOD/Q -> VCO V/OCT**

### Result
A repeating pattern of notes derived from the LFO phase at each clock pulse.

### Best for
- looping melodic motifs
- techno sequences
- repeating hooks
- tuneful generative patterns

This is better than noise if you want recognizably recurring melody.

---

## 5. Two-oscillator melodic lead
For fuller melodic components.

### Patch
- **PITCH -> MULTI**
- **MULTI -> VCO1 V/OCT + VCO2 V/OCT**
- **VCO1 SAW + VCO2 TRI/SAW -> MIX1**
- MIX1 -> VCF -> VCA

Enhancements:
- detune VCO2 slightly
- tune VCO2 to a fifth/octave
- use VCO2 as sync master for VCO1
- modulate PWM or filter with LFO

### Result
A bigger melodic voice for hooks or solos.

### Best for
- lead lines
- bass melody
- synth-pop/techno lines
- dramatic mono leads

---

## 6. Transposed melody with manual offset
Useful for changing key center or creating intervals.

### Patch
- **PITCH -> MIX2 input 1**
- **GEN1 -> MIX2 input 2**
- **MIX2 OUT -> VCO1 V/OCT**

Or:
- **Quantized sequence -> MIX2**
- **GEN1/GEN2** adds offset before oscillator

### Result
Your played or generated melody shifts register or transposes.

### Best for
- octave shifts
- drone + lead interval relations
- live performance transposition
- moving a sequence into different harmonic zones

Be subtle: raw CV offsets can move by large intervals quickly.

---

## 7. Acid-style melodic lines
The manual strongly suggests this system can do this well.

### Patch concept
- MIDI or quantized sequence -> oscillator pitch
- **SLEW** in pitch path for slides
- **ENV -> VCF CV**
- resonance up
- shorter envelope
- accent-like feel via modulation depth or VCA initial

### Core patch
- **PITCH or MOD/Q -> SLEW -> VCO1 V/OCT**
- **GATE -> ENV**
- **VCO1 SAW/SQU -> VCF LP -> VCA**
- **ENV OUT -> ATT -> VCF CV**
- resonance fairly high

### Result
Sliding, squelchy, melodic bass patterns.

---

## 8. Counter-melody / drone support
The system is monophonic in the classic sense, but you can still create layered melodic roles.

### Method
- Use one oscillator for moving melody
- Tune the other oscillator to a fixed interval or drone
- Mix them before the filter

Example:
- **VCO1** follows main pitch CV
- **VCO2** tuned to a fifth/octave/drone
- mix both into VCF

Alternative:
- use **MIDI square output** as an additional locked pitch layer for reinforcement

### Result
A more harmonically suggestive single-line melody.

---

# How rhythm modules help melody

## MIDI clock / 16TH
If using external MIDI clock, this is your main rhythmic pulse.

### Use for melody
- trigger S&H
- feed CLKDIV
- clock FX tempo
- structure repeating note changes

---

## CLKDIV
Clock division turns one pulse stream into several slower related streams.

### Melodic use
- different divisions can trigger S&H at different rates
- use one division for note changes, another for envelope triggers
- create phrase structures where pitch changes slower than articulation

Example:
- **16TH -> CLKDIV**
- one division -> **S&H SAMPLE**
- another division -> **ENV GATE**

This can create repeating melodic phrases with internal rhythmic variety.

---

## Logic gates
These are very useful for melodic phrasing, even though they’re not pitch sources.

### Melodic use
Use logic to create more interesting trigger patterns:
- XOR two clocks for unusual note trigger patterns
- AND a button with clock to manually allow melody movement
- NAND or NOT for inverted rhythm structures

These affect **when notes happen**, which is half of melody.

---

# The best melodic workflows on this system

## Workflow 1: Traditional melodic synth player
Use:
- MIDI keyboard
- VCO1/VCO2
- ENV
- VCF
- VCA
- FX

Best if you want:
- basslines
- leads
- hooks
- straightforward songwriting parts

---

## Workflow 2: Performative melodic improviser
Use:
- Ribbon
- Quantizer
- VCO
- ENV
- VCF
- delay/reverb

Best if you want:
- expressive live melody
- modal soloing
- ambient lines
- experimental but tuneful phrasing

---

## Workflow 3: Generative composer
Use:
- Noise/LFO
- S&H
- Quantizer
- clock divider
- slew
- filter and FX

Best if you want:
- self-running melodies
- evolving motifs
- ambient sequences
- semi-random arpeggiation

---

# Practical melodic patch recipes

## Patch recipe: warm lead
- **PITCH -> VCO1 + VCO2**
- VCO1 saw, VCO2 triangle
- slight detune on VCO2
- both -> MIX1 -> VCF LP -> VCA
- **GATE -> ENV**
- **ENV -> VCA CV**
- **ENV -> ATT -> VCF CV**
- chorus or delay in FX

Result: classic expressive lead.

---

## Patch recipe: quantized ambient melody
- **Ribbon CV -> Q IN**
- **MOD/Q -> SLEW -> VCO1 V/OCT**
- **Ribbon GATE -> ENV**
- VCO1 triangle -> VCF BP -> VCA
- long attack/release
- reverb FX

Result: smooth, scale-safe ambient lead.

---

## Patch recipe: generative sequence
- **WHITE noise -> S&H IN**
- **16TH -> CLKDIV -> S&H SAMPLE**
- **S&H OUT -> Q IN**
- **MOD/Q -> VCO1 V/OCT**
- divided clock -> ENV GATE
- VCO1 saw -> VCF -> VCA
- ENV to filter
- delay synced from clock

Result: repeating but evolving melodic sequence.

---

## Patch recipe: animated bass melody
- **PITCH -> SLEW -> VCO1 V/OCT**
- VCO1 saw + sub -> mix
- mix -> VCF LP
- resonance medium-high
- **GATE -> ENV**
- **ENV -> VCF CV**
- short decay, low sustain
- VCA controlled by ENV

Result: acid/bassline style melodic content.

---

## Patch recipe: stepped repeating motif
- **LFO TRI -> ATT -> S&H IN**
- **clock -> S&H SAMPLE**
- **S&H OUT -> Q IN**
- **MOD/Q -> VCO1**
- **MOD/Q -> MULTI -> VCO2**
- VCOs mixed and filtered

Result: cyclical musical phrase rather than pure randomness.

---

# Important musical insights from this module set

## Melody comes from both pitch and articulation
On the MODULÖR114, melodic identity is usually a combination of:
- **Pitch source**: MIDI / ribbon / quantizer / S&H
- **Timing source**: gate / clock / divider / logic
- **Tone shaping**: VCF and waveform selection
- **Phrasing**: envelope and slew

A plain scale sequence can become much more musical just by adjusting:
- envelope attack/decay
- filter envelope amount
- glide amount
- clock division
- detuning of the second oscillator

---

## The quantizer is the key to musical modular melody
The most important takeaway from the manual is that the quantizer allows almost any control voltage to become usable melodic material.

That means:
- LFOs become arpeggiators
- noise becomes random note selection
- ribbon becomes a playable scale controller
- S&H becomes a sequencer
- manual voltages become transposable notes

If your goal is melodic music, this is one of the most valuable modules on the instrument.

---

## Utilities are what make melodies interesting
The melody-producing modules are obvious, but the memorable patches come from utilities:

- **SLEW** = phrasing
- **ATT** = musical modulation amounts
- **MIX** = combining pitch influences
- **MULTI** = layered voices
- **ADDSUB** = inversion/offset/transposition tricks
- **CLKDIV/LOGIC** = non-boring note timing

---

# Best combinations specifically for melodic music

## For basslines
- MIDI PITCH or quantized S&H
- VCO1 saw or square + sub
- VCF LP with ENV modulation
- SLEW for slides
- optional VCO2 as detuned support

## For leads
- dual VCOs
- detune or sync
- ENV to VCA and VCF
- LFO to PWM or vibrato
- delay/reverb FX

## For arpeggios / sequences
- clock -> S&H
- S&H -> quantizer
- quantizer -> oscillator pitch
- divided gates for phrasing
- synced delay

## For ambient melodies
- ribbon -> quantizer -> slew
- triangle wave
- bandpass or gentle lowpass
- long envelope
- reverb-heavy FX

## For generative melodic textures
- noise/LFO -> S&H -> quantizer
- slow modulation of filter and FX
- logic-derived irregular triggers
- long release and delay

---

# Final takeaway
The MODULÖR114 is very capable at making melody because it contains the full chain:

- **choose notes**: MIDI, ribbon, quantizer, S&H
- **organize notes in time**: gate, MIDI clock, divider, logic
- **voice the notes**: VCO1, VCO2, DCO square
- **shape the phrase**: envelope, filter, VCA
- **humanize/animate**: slew, LFO, PWM, modulation
- **finish musically**: onboard FX

If I were building melodic patches on it, I’d focus on these three “master combinations” first:

1. **MIDI + dual VCO + ENV/VCF/VCA** for solid musical parts  
2. **Ribbon + Quantizer + Slew** for expressive hands-on melodies  
3. **S&H + Quantizer + Clock Divider** for generative melodic sequences  

Those three approaches cover most melodic duties: composed, performed, and self-generated.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)