# Industrial Music Electronics — Piston Honda

- [Manual PDF](../../manuals/phmk3manual11.pdf)

---

[Manual PDF](http://www.industrialmusicelectronics.com/products/21)

# Industrial Music Electronics Piston Honda Mark III
## Using it to create melodic components in music

The attached manual is for the **Piston Honda Mark III**, a **dual wavetable oscillator** with:
- **Two independent oscillators**: Osc A and Osc B
- **3-axis wavetable scanning**: X / Y / Z
- **Preset management and preset morphing**
- **Internal oscillator linking**
- **Internal FM normalization between oscillators**
- **External input waveshaping mode**
- **Unison, octave shifting, waveform CV control, and wavetable loading from SD**

For melodic work, this module is especially strong because it can function as:
- a **precise pitch-tracking voice source**
- a **2-oscillator harmonic stack**
- a **moving wavetable lead**
- a **preset-addressed melodic timbre sequencer**
- a **chord/unison generator**
- a **self-contained complex digital tone source**

---

## What the module does musically

At its core, Piston Honda Mk III is a **melodic oscillator pair**. Unlike a simple analog VCO that gives you saw, square, triangle, etc., this one reads **arbitrary waveforms from memory** and lets you **morph through a cube of 512 waves** arranged as:

- **8 positions on X**
- **8 positions on Y**
- **8 positions on Z**

That means melody can be shaped not only by pitch, but also by:
- where you are in the wavetable cube
- whether axes interpolate smoothly or jump in steps
- whether oscillator B follows oscillator A
- whether presets recall full pitch/timbre states
- whether you use internal FM or unison

So in a melodic patch, **pitch** and **timbre movement** can be composed together.

---

## Important melodic features from the manual

## 1. Accurate 1V/Oct tracking
Each oscillator has its own **1V/Oct input**, so both can be played melodically from:
- sequencer
- keyboard
- quantizer
- precision adder chain

The manual states:
- coarse at minimum
- fine at center
- no external voltage
= about **C0 / 16.35 Hz**

So this module is meant to serve as a proper pitched voice.

### Musical use
You can patch:
- one melodic CV to Osc A only
- a second melodic CV to Osc B only
- or the same melody to both for intervals/unison

---

## 2. Dual oscillator structure
Because there are two oscillators in one module, you can build melodic material in several ways:

### Parallel voice design
- Osc A = main fundamental-rich voice
- Osc B = brighter layer, fifth, octave, or detuned partner

### Independent counterpoint
- Osc A = bassline
- Osc B = lead or countermelody

### Composite mono voice
- A and B mixed together for one richer melodic line

This is one of the strongest uses of the module for music: **one module can create a complete pitched sound with internal complexity before you even add filters or VCAs.**

---

## 3. Oscillator Link for harmonic following
Oscillator B has a **Link** button.

When enabled:
- Osc B copies Osc A’s frequency
- Osc B coarse tune is disabled
- Osc B fine tune and CV still influence its pitch

### Musical use
This is excellent for melody because it gives immediate interval relationships:
- center fine tune on B = unison
- slightly offset fine tune = detuned lead / chorus
- tuned by ear or CV = harmony layer
- octave shifted via menu = octave doubling

This makes it easy to build:
- lead sounds with width
- octave bass reinforcement
- fifths and near-unisons
- stacked wavetable intervals

Because the two oscillators can still use different waveform positions, the result can be harmonically coherent but timbrally varied.

---

## 4. Internal FM normalization
The manual notes that the **FM input of each oscillator is normalled to the output of the other oscillator**.

That means even without patch cables:
- Osc A can modulate B
- Osc B can modulate A
depending on settings

The FM is:
- **audio-rate**
- **thru-zero**
- intended for audio-rate signals

### Musical use for melody
FM can be used very musically if kept subtle:
- add slight FM for animated harmonic richness on leads
- make bells or metallic melodic tones
- use one oscillator as carrier and the other as modulator
- use linked pitch plus subtle FM for stable but lively lines

Important manual note:
- keep FM amount at zero if you do not want FM, since the normalization is always there

For melodic work, a little goes a long way. Small FM amounts preserve pitch identity while adding motion.

---

## 5. Unison per oscillator
Each oscillator has a **Unison** parameter in its menu.

It adds a second oscillator alongside the main one with:
- mostly identical settings
- slight frequency offset
- optional +1 octave / -1 octave variants

### Musical use
This is huge for melodic patching.

A single Piston Honda voice can become:
- Osc A + its unison
- Osc B + its unison

So the module can effectively create **4 oscillators of sound**.

This is ideal for:
- supersaw-like digital leads
- wide pads
- octave-reinforced basses
- pseudo-chordal melodic lines
- dramatic mono hooks

The manual specifically mentions massive 4-oscillator sounds when combining this with linked oscillators.

---

## 6. Octave shift
Each oscillator can be shifted over **±2 octaves**.

### Musical use
Use this to split melodic roles:
- Osc A = root register
- Osc B = one octave above
- or B = two octaves down for sub reinforcement

Combined with Link, this becomes a very fast melodic stack builder.

---

## 7. 3-axis wavetable scanning as melodic articulation
X, Y, and Z each have:
- a manual slider
- a CV input
- an attenuverter

This is where Piston Honda becomes especially expressive for melody.

### Musical use
Rather than treating timbre as static, you can let melody “speak” by modulating the axes:

- **slow X modulation** = evolving phrase color
- **stepped Y modulation** = distinct note-to-note timbral changes
- **Z modulation** = move across different wavetable files / families
- envelope to X/Y/Z = brighter attack, softer sustain
- sequencer row to Z = different timbre per step

This allows a melodic line to carry harmonic and spectral form the same way an acoustic instrument changes tone across articulation.

---

## 8. Morph enable / stepped axis behavior
Each axis can have morphing enabled or disabled.

If morph is disabled:
- transitions become hard steps between waveforms
- sound becomes more glitchy / discrete
- you hear isolated waveform slots without interpolation

### Musical use
This gives two different melodic aesthetics:

### Smooth morph enabled
Best for:
- singing leads
- pads
- fluid bass movement
- expressive timbre sweeps

### Morph disabled
Best for:
- arpeggios with digital bite
- stepped timbre melodies
- chiptune-like note articulation
- rhythmic timbral sequencing

A powerful trick is:
- keep X and Y smooth
- disable Z morph
This gives gradual movement inside a wave family, but hard jumps between wavetable banks.

---

## 9. Preset manager as a melodic composition tool
The preset system is not just for storage — it is a **performance and sequencing feature**.

There are **8 presets**, and they can manage:
- wave positions
- attenuverters
- unison / octave settings
- optionally coarse/fine pitch too

### Preset Scope
Two key modes:
- **Waves Only**
- **All Params**

### Musical use

#### Waves Only
Great for:
- same melody, changing timbre scenes
- step-addressed wavetable articulation
- phrase variation without changing pitch

#### All Params
Great for:
- storing different notes or intervals
- building melodic sequences from preset slots
- creating structured performance states
- changing oscillator pitch and character together

This makes Piston Honda capable of being a kind of **8-state digital melodic memory voice**.

---

## 10. Preset morph
In Preset mode, pressing Preset again enters **Morph mode**.

Then:
- choose a base preset with the encoder
- apply CV to the preset CV input
- presets smoothly morph into one another

### Musical use
This is one of the most interesting melodic features in the manual.

You can morph:
- between lead timbres
- between harmonic interval structures
- between two related melodic scenes
- between bass and lead states

If Preset Scope = All Params, morphing also glides frequency between presets.

That can produce:
- portamento-like spectral-pitch motion
- in-between microtonal motion
- unstable digital glissandi
- animated transitions between notes

If you want melodies to stay tonally clear, **Waves Only** is often more useful.  
If you want transformative, in-between pitch movement, **All Params** is more experimental and dramatic.

---

## 11. Preset CV modes for sequencing melodic states
The preset CV input can work in several ways:

- **CV+Offset**
- **CV+Atten**
- **Trig+Offset**
- **Trig Random**

### Musical use

#### CV+Offset
Use a sequencer or slow CV to scan/morph across presets.
- ideal for evolving melodic timbre phrases
- manual knob acts as offset

#### CV+Atten
Great when you want tighter control over how many preset states are reached.

#### Trig+Offset
Each trigger advances one preset.
- acts like a step-through scene sequencer
- useful for cyclic melodic form
- pair with clock divisions for phrase changes

#### Trig Random
Randomizes parameters on trigger.
- useful for generative melodic design
- especially effective when Preset Scope is limited

---

## 12. External input mode for melodic processing
Each oscillator can switch from internal oscillation to **External Input mode**.

In this mode:
- the oscillator processes incoming audio through the selected wavetable
- signal enters via the FM input
- the large tune knob becomes gain
- the CV input can control gain

### Musical use
This matters for melody if you want to process:
- another oscillator
- a simple sine/triangle
- a melodic voice elsewhere in the rack

You can use Piston Honda as a **wavetable shaper** for an external melodic source:
- feed a clean analog oscillator melody into Ext mode
- scan X/Y/Z for changing harmonics
- use envelope CV for dynamic shaping
- create digital articulation on otherwise simple melodic lines

This is an excellent hybrid patch strategy.

---

# Best melodic patch strategies

## 1. Classic dual-oscillator lead
### Patch
- Sequencer pitch CV → Osc A 1V/Oct
- Link Osc B to Osc A
- Set Osc B fine tune near center or slightly offset
- Use Mix output
- Envelope/LFO to X or Y CV
- Filter/VCA after the output

### Result
A thick melodic lead with:
- stable pitch
- chorused width
- moving wavetable harmonics

### Why it works
You get analog-style “two oscillator lead” behavior, but with much richer wavetable motion.

---

## 2. Octave lead/bass stack
### Patch
- Same pitch CV to Osc A
- Link B to A
- Set B octave shift to +1 or -1
- Use Mix output
- Slow modulation to different waveform axes on A and B

### Result
A musically solid melodic stack:
- sub + mid
- root + octave
- lead + shimmer

### Why it works
Octaves preserve melodic clarity while the separate wave positions keep the sound from feeling static.

---

## 3. Harmonic interval melody
### Patch
- Sequence to Osc A
- Link B to A
- Set B fine tune to a consonant interval by ear
- Optionally set different waveforms for A and B
- Mix output to final voice chain

### Result
One sequenced line becomes a dyad-like harmonic voice.

### Good interval ideas
- slight detune = width
- octave = power
- fifth-ish relation = strong melodic harmony
- fourth = suspended feel

Because tuning is by fine control and not quantized internally, a quantizer or careful ear helps if exact intervals matter.

---

## 4. Animated wavetable melody
### Patch
- Pitch CV to one oscillator
- Envelope to X CV
- Slow LFO to Y CV
- Sequencer modulation row or random CV to Z CV
- Morph enabled on X/Y, disabled on Z

### Result
Each note has:
- attack articulation from X
- phrase drift from Y
- stepped family changes from Z

### Why it works
This is one of the best ways to make a mono melody feel alive without relying entirely on filtering.

---

## 5. Preset-addressed phrase machine
### Patch
- Enable Preset mode
- Preset Scope = Waves Only or All Params
- Program 8 presets as 8 timbral or pitch/timbre states
- Use CV or Trig+Offset to step through presets

### Result
A melody can move through predefined “chapters.”

### Great uses
- one preset per phrase section
- one preset per note accent type
- one preset per harmonic density
- one preset per chorus/verse color

If using **All Params**, presets can act like stored note/harmony states.

---

## 6. Morphing melody scenes
### Patch
- Enter Preset Morph mode
- Set base preset
- Send slow CV or envelope to preset CV input
- Keep a melodic sequence running into 1V/Oct

### Result
The same note sequence transforms continuously in timbre and structure.

### Best for
- intros
- ambient leads
- progressive melodic transitions
- slowly shifting techno hooks

---

## 7. Digital FM melody
### Patch
- Sequence one oscillator as carrier
- Set second oscillator to linked or harmonically related pitch
- Raise FM amount subtly
- Listen from carrier or Mix output
- Modulate wavetable position gently

### Result
A melodic voice with:
- metallic edge
- strong attack complexity
- dynamic harmonic content

### Tip
Keep FM low if you need strong pitch readability.

---

## 8. 4-oscillator supersized mono voice
### Patch
- Enable unison on Osc A
- Enable unison on Osc B
- Link B to A or tune B as interval
- Mix output to filter/VCA
- Modulate waveform axes

### Result
A huge single melodic voice with digital complexity and stereo-like density even in mono.

### Best for
- hooks
- anthem leads
- aggressive basslines
- cinematic mono lines

---

## 9. Two independent melodic parts from one module
### Patch
- Separate pitch CVs to Osc A and Osc B
- Disable waveform CV on one oscillator if needed
- Use A and B individual outputs instead of Mix
- Set distinct wave positions for each oscillator

### Result
One module can produce:
- bass + melody
- melody + counterline
- sequence + drone
- call and response

### Important note
Because waveform controls are shared, the module includes locking behavior and waveform CV can be disabled per oscillator, which helps when treating it as two separate voices.

---

## 10. Wavetable processing of another melodic oscillator
### Patch
- Put Osc A in External Input mode
- Patch another oscillator’s melodic audio into Osc A FM/Ext input
- Use tune knob as gain
- Envelope to CV gain
- Scan X/Y/Z

### Result
A simple melody from another VCO becomes digitally articulated and reshaped through Honda’s wavetable engine.

### Best for
- giving analog oscillators digital edge
- animating simple sine/triangle melodies
- dynamic wavefolding-like melodic motion

---

# Practical melodic workflows

## Workflow 1: Strong, tonal melody
Use:
- 1V/Oct input
- little or no FM
- Link on
- octave or subtle detune
- smooth X/Y morphing
- Waves Only preset control

This keeps melodic identity clear while adding timbral expression.

---

## Workflow 2: Aggressive digital hook
Use:
- hard-stepped morph on one or more axes
- unison
- slight FM
- preset stepping via trigger
- different wave families on Z

This creates memorable, edgy riffs.

---

## Workflow 3: Evolving ambient melody
Use:
- linked oscillators
- slow independent modulation of X/Y/Z
- preset morph mode
- smooth morph enabled
- little or no sync/FM

This turns a simple sequence into a long-form evolving line.

---

## Workflow 4: Harmonic mono synth voice
Use:
- Osc A = root
- Osc B linked and tuned to interval or octave
- both with distinct waves
- unison on one or both
- Mix output

This approximates a chordal or paraphonic impression from a single melodic CV line.

---

# Notes from the manual that matter in practice

## FM input normalization
The FM input is normalled from the other oscillator, so:
- zero the FM control if you want a clean sound
- otherwise subtle internal cross-complexity may be present

## Shared waveform controls
The waveform sliders and attenuverters are shared between oscillators.  
Use the **Select** buttons carefully and note the locking behavior.

## Preset frequency control
If **Preset Scope = All Params**, preset changes also affect oscillator frequency.  
That can be very powerful for melody, but can also disrupt tuning if you expected only timbral changes.

## Morph vs pitch stability
Preset morphing with pitch included creates glides between states.  
Beautiful, but not always “in tune” in the conventional sequenced sense.

## External input mode caveat
If both oscillators are in External Input mode and no signals are patched, the module can feed back in a not-very-useful way.

---

# Best musical roles for Piston Honda Mark III

This module is especially good at:

- **lead melodies**
- **bass melodies**
- **harmonic doubling**
- **digital interval stacks**
- **preset-based phrase changes**
- **evolving timbral sequences**
- **metallic and animated melodic voices**
- **hybrid analog/digital melodic processing**

It is less about “plain subtractive melody” and more about **spectrally alive, composed timbre melody**.

---

# Bottom line

The Piston Honda Mark III is not just a sound source — it is a **melodic architecture module**. Because it combines:
- dual oscillators
- wavetable scanning
- internal linking
- internal FM routing
- unison
- octave shifts
- preset recall
- preset morphing
- external audio waveshaping

…it can produce melodic material ranging from:
- stable tonal basses and leads
to
- harmonically stacked riffs
to
- evolving digital phrase structures

If you want to use it musically, the most effective approaches are:

1. **Use Osc B linked to Osc A** for interval or detune support  
2. **Animate X/Y/Z with envelopes, LFOs, or sequencer rows**  
3. **Use presets as compositional states, not just storage**  
4. **Use unison and octave shift to make single-note lines feel huge**  
5. **Keep FM subtle when melodic clarity matters**  
6. **Choose stepped vs smooth morphing intentionally depending on style**

In short: this module excels when pitch sequencing and timbre sequencing are treated as one musical gesture.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)