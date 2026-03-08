# Erica Synths — LXR Eurorack

- [Manual PDF](../../manuals/LXR_eurorack_manual.pdf)

---

[Erica Synths x Sonic Potions LXR Eurorack Owners Manual (PDF)](https://www.ericasynths.lv/media/LXR_Eurorack_owners_manual_v2.pdf)

# Using the Erica Synths x Sonic Potions LXR Eurorack Module for Melodic Music

Although the LXR is primarily a **6-voice digital drum synthesizer**, the manual makes it clear that it is much more than a fixed percussion box. With per-voice synthesis, modulation, FM, filters, envelopes, CV assignment, 1V/Oct behavior, routing, LFOs, and effects, it can be used as a **melodic percussion synth**, **bass voice**, **FM bell source**, **chord-like layered texture generator**, and **animated tonal FX instrument**.

## Big picture

The LXR gives you:

- **6 synth voices**
- **Different voice architectures** optimized for different sound families
- **5 assignable CV inputs**
- **6 LFOs**
- **3-slot modulation matrix per voice**
- **Accent modulation**
- **Per-voice filter, envelopes, transient, distortion, sample-rate reduction**
- **Output routing to stereo pairs, mono outs, or FX bus**
- A special modulation target called **“v/o”** for **1V/Oct tonal control**

This means the module can move beyond drums and become a playable **multi-timbral melodic sound source**.

---

# What in the manual supports melodic use?

## 1. 1V/Oct pitch control via the mod matrix

One of the most important details in the manual is in the modulation section:

- Each voice has a **3-slot modulation matrix**
- Sources include:
  - **5 CV inputs**
  - **6 LFOs**
  - **6 accent signals**
- There is a special destination called **“v/o”**
- With **amount = 100%**, incoming CV is scaled for **1V/Oct tracking**
- Negative CVs are ignored in this mode
- This gives about a **5-octave range**

This is the core feature that turns the LXR into a melodic instrument.

### Practical use
Patch a sequencer, keyboard controller, or quantized CV source into one of the **CV inputs**, then assign that CV to the selected voice’s **v/o** destination in the mod matrix. Now that drum voice can be played chromatically.

---

## 2. Several voice types can function as pitched synth voices

The manual describes these voice families:

- **Drum voices 1–3**
- **Snare voice (voice 4)**
- **Cymbal/Clap voice (voice 5)**
- **Hihat/open hihat voice (voices 6/7 shared behavior)**

Some are more naturally melodic than others.

## Best melodic candidates

### Drum voices 1–3
These are the strongest general-purpose melodic voices because they include:

- Main oscillator
- FM or mix oscillator behavior
- Pitch envelope
- Filter
- Amp envelope
- Transient generator
- Distortion
- Sample-rate reduction

These can become:

- basslines
- tom-like tuned percussion
- plucks
- acid-style leads
- digital synth stabs
- cowbells and synthetic keys

### Cymbal/Clap voice (voice 5)
This voice uses **3-operator FM**, making it excellent for:

- bells
- metallic keys
- mallets
- dissonant melodic percussion
- evolving inharmonic textures

The manual explicitly points out that this voice is “great for metallic and noisy sounds,” and later in the drum synthesis section it recommends FM for **realistic bells**.

### Snare voice (voice 4)
Less ideal as a conventional lead, but very useful for:

- noisy synth plucks
- tuned electro zaps
- layered body+noise percussion melodies
- clap/snare hybrid melodic hits

The manual even suggests using the tonal part alone with pitch modulation for a **Kraftwerk-style zap**.

### Hi-hat voice
This can be used melodically in an experimental sense, especially for:

- tuned metallic blips
- short digital chord fragments
- glitch arps
- bright noise pings

But it is less straightforward for conventional tonal roles.

---

# How to build melodic parts on the LXR

## Method 1: Turn a drum voice into a bass or lead synth

Use one of **Drum voices 1–3**.

### Setup concept
1. Select voice 1, 2, or 3
2. In the **MOD menu**, assign:
   - **src = CV input**
   - **dst = v/o**
   - **amt = 100%**
3. Send a sequenced pitch CV into the chosen CV input
4. Trigger the voice rhythmically with the trigger input
5. Tune the oscillator to a useful base range
6. Shape with filter and envelopes

### Recommended settings for bass
- **OSC page**
  - waveform: sine, triangle, or rectangle
  - coarse tune: low
  - fine tune: by ear
- **AEG**
  - attack: 0
  - decay: medium
  - slope: slightly exponential
- **MOD**
  - pitch envelope amount: low to moderate
  - decay: short
- **FIL**
  - lowpass
  - moderate resonance
- **MIX**
  - mild drive
  - route to a clean output or FX bus

### Result
You get a playable **mono bass synth voice** that can still retain percussive articulation.

---

## Method 2: Make tuned plucks and synth stabs

The amplitude envelope and filter section make the LXR very good at short, punchy synthesized notes.

### Patch recipe
Use a **drum voice** or the **snare voice**:
- short attack
- moderate decay
- bandpass or lowpass filter
- small pitch envelope amount
- optional transient for sharper attack

This creates:
- plucks
- clave-like tonal hits
- marimba-ish digital percussion
- electro stabs

### Tip
Use the **transient generator** sparingly. Too much transient makes the note feel drum-like; a little gives articulation without losing pitch definition.

---

## Method 3: FM bells, mallets, and metallic melodies

The manual specifically suggests FM for bells.

Use **Voice 5 (Cymbal/Clap)**.

### Why it works
Its 3-operator FM structure naturally creates:
- inharmonic overtones
- metallic spectra
- bell-like decays
- complex tuned attacks

### Recommended approach
- Tune FM oscillator relationships by ear
- Use a **bandpass filter**
- Use an **exponential amplitude decay**
- Add a small amount of **sample-rate reduction** for extra metallic edge
- Sequence pitch using **v/o**

### Musical applications
- bell melodies
- techno mallet riffs
- ambient metallic arpeggios
- gamelan-like textures
- digital keys

---

## Method 4: Use mixed oscillator mode for interval-like timbres

On drum voices, the **FM page** allows:
- **FM mode**
- **Mix mode**

In **Mix mode**, the main oscillator and FM oscillator are mixed rather than one modulating the other.

This is especially useful for melodic work because you can create:
- dual-oscillator tones
- detuned unisons
- interval-like clangs
- richer harmonic lead sounds

### Example
Set:
- main osc = rectangle
- second osc = rectangle or saw
- tune second oscillator to a musically related offset
- use a bandpass or lowpass filter

This is especially good for:
- synthetic cowbells
- harmonically rich stabs
- pseudo-chords
- techno riffs

The manual’s **808 cowbell** example is basically a melodic interval patch built this way.

---

# Melodic sound design strategies from the manual

## 1. Use the filter musically

The filter is a **2-pole state variable filter** with multiple types:

- lowpass
- highpass
- bandpass
- unit gain bandpass
- notch
- peak
- LP2

These are useful for melodic shaping:

### Lowpass
Good for:
- basses
- leads
- warm plucks

### Bandpass
Good for:
- bells
- mallets
- nasal leads
- tuned percussion

### Peak
Good for:
- emphasizing note pitch
- resonant attack focus
- “struck body” feeling

### LP2
The manual describes it as more digital and resonant, good for screaming acid sounds. This makes it excellent for:
- acid basslines
- aggressive resonant leads
- unstable melodic techno sequences

---

## 2. Use the envelopes like synth envelopes, not just drum envelopes

The manual’s envelope section is crucial for melodic use.

You have control over:
- attack
- decay
- slope
- repeat (on some voices)

### Melodic implications
- **Fast attack + short decay** = pluck
- **Fast attack + medium decay** = stab
- **Longer decay** = bell or sustained percussive tone
- **Exponential slope** = natural struck sound
- **Logarithmic slope** = more synthetic tail behavior

For melodic percussion, exponential decay usually feels most natural.

---

## 3. Use pitch envelopes carefully

Pitch envelopes are great for drums, but too much destroys tonal clarity.

For melodic parts:
- keep pitch envelope low
- use short decay
- use it mainly for attack character

This gives:
- plucked articulation
- analog-style “dip” or “snap”
- more presence without detuning the note center too much

---

## 4. Use transient modes to define note articulation

The transient generator has multiple modes:

- **Snappy**
- **Offset**
- **Sample**

These can turn a plain note into something more expressive.

### Best uses for melodic work
- **Snappy**: adds struck attack, good for bass or tom-like notes
- **Offset**: adds pop or phase-defined attack, great for clicky plucks
- **Sample**: good for hybrid percussion-key sounds

For clean melodic lines, use low transient volume.

---

## 5. Use sample-rate reduction as a harmonic shaper

The sample-rate reducer is not only for destruction. At subtle settings it can add:
- metallic overtones
- digital edge
- animated brightness

This is especially effective on:
- FM bells
- leads
- tuned percussion

Too much will obscure pitch, so for melodic roles it works best in moderation.

---

## 6. Use distortion for sustain and presence

Per-voice distortion on the mixer page can make tones more present and stable in a mix.

For melody:
- light saturation = fuller bass
- moderate drive = stronger harmonics for filter shaping
- hard clipping = aggressive industrial lead tones

The FX drive can also process multiple routed voices together, creating glued melodic/percussive hybrids.

---

# LFOs and modulation for melodic animation

The LXR has **6 LFOs**, selectable per voice through the modulation matrix.

These are extremely useful for turning static pitched sounds into musical phrases.

## Good melodic modulation targets
- filter frequency
- oscillator pitch (small amounts)
- FM amount
- pulse width
- distortion amount
- sample rate
- pan

## Musical examples

### Slow filter LFO
Creates:
- animated bassline movement
- evolving bell timbre
- subtle variation across repeated notes

### Retriggered LFO as an extra envelope
The manual explicitly notes that LFO retrigger can be used like an additional envelope.

This is powerful for melodic sounds:
- assign LFO to filter cutoff
- retrigger from the same voice
- choose a one-shot-like waveform behavior by timing the cycle

Result:
- extra pluck contour
- custom filter sweep per note
- pseudo-AD modulation

### Small pitch LFO
Good for:
- vibrato
- unstable analog drift
- detuned metallic shimmer

---

# Building layered melodic arrangements with multiple voices

Because the LXR has 6 voices, it can provide more than one melodic role at once.

## Example multi-voice melodic setup

### Voice 1: Bass
- sine/triangle
- lowpass
- short-medium decay
- 1V/Oct from CV1

### Voice 2: Pluck
- saw or rectangle
- bandpass
- short decay
- mild transient
- same or different pitch CV via another mod slot/CV input

### Voice 5: Bell layer
- FM metallic patch
- longer decay
- bandpass
- subtle LFO on filter
- 1V/Oct from CV input

### Voice 4: Noise accent line
- snare voice with mostly tonal oscillator
- filtered noise mixed low
- short sequence for syncopated zaps

This lets the LXR act almost like an entire compact melodic percussion section.

---

# Using accents musically

The manual explains that accent can modulate:
- voice volume
- any parameter of the voice

This is very useful for melody, because accent is not only about loudness.

## Good accent destinations for melodic phrasing
- filter cutoff
- FM amount
- decay
- drive
- transient volume

### Result
Different notes in a melodic line can have:
- brighter attacks
- different harmonic content
- longer tails
- more aggression

That creates expressive phrasing from otherwise repetitive sequences.

---

# Morphing kits for harmonic transformation

The **Performance Mode** includes **Morph**, which interpolates from the current kit to another kit.

For melodic use, this can be brilliant.

## Best use case
Create:
- one kit with a stable melodic patch set
- another kit with altered tuning, filter settings, FM amount, and decay

Then morph between them.

### Musical outcomes
- timbral modulation across a phrase
- shifting from bass to bell-like tone
- changing interval structure in layered melodic percussion
- live performance transitions

The manual even suggests saving slightly modified versions of favorite presets and morphing between them to control many parameters at once.

For melodic performance, this is one of the most powerful features.

---

# FX as melodic tools

Only one global FX processor can be active at a time, but it can still be very effective.

## Drive FX
Use for:
- thickening bass voices
- aggressive lead textures
- gluing multiple melodic voices together

Because multiple voices can hit the same distortion bus, you can get complex intermodulation between pitched sources.

## Ringmod FX
Excellent for:
- robotic tuned percussion
- atonal melodic textures
- clangorous harmonic enhancement

On already-pitched material, ringmod creates sidebands that can either enrich or destabilize tonality.

## Compressor
Useful if you want the melodic elements to sit more evenly and feel “finished.”

## Delay
Especially strong for:
- arpeggio extension
- metallic echoes
- dub-techno percussion melodies
- stereo movement

Short delay times with modulation can also produce flange-like coloration, which can be very nice on bells or zaps.

---

# Patch ideas for melodic music

## 1. Acid percussion bass
- Voice: Drum 1
- Wave: saw or rectangle
- CV to v/o at 100%
- Short attack, medium decay
- LP2 filter
- medium-high resonance
- accent to filter cutoff
- optional drive

Use trigger sequencing for rhythmic bass patterns.

---

## 2. FM bell melody
- Voice: Cymbal/Clap
- Tune operators for metallic partials
- Bandpass filter
- Exponential decay
- Mild sample-rate reduction
- LFO on filter cutoff
- CV to v/o

Perfect for ambient, IDM, electro, or melodic techno.

---

## 3. Kraftwerk zap lead
- Voice: Snare
- Reduce noise mix
- Raise oscillator pitch
- Use pitch envelope moderately
- Bandpass or highpass filter
- Short decay
- CV to v/o

Great for robotic melodic motifs.

---

## 4. Hybrid marimba/tom line
- Voice: Drum 2 or 3
- Sine or triangle
- Small transient
- Peak or bandpass filter
- Fast attack
- Medium-short exponential decay
- slight distortion
- CV to v/o

Works well for tuned percussion sequences.

---

## 5. Layered metallic chord illusion
Use multiple voices with fixed interval tunings:
- Voice 1 = root
- Voice 2 = +7 semitones
- Voice 5 = complex FM overtone layer

Trigger together from the same rhythmic pattern. Even without true polyphonic keyboard control, you can create harmonic stacks and pseudo-chords.

---

# Best workflow for melodic integration in a eurorack system

## With external sequencers
The LXR becomes much more melodic when paired with:
- quantized CV sequencers
- keyboard controllers
- precision voltage sources
- sequential switches
- logic/rhythm generators for triggers

### Recommended patch structure
- Trigger source -> LXR trigger input
- Pitch CV source -> LXR CV input
- Optional accent gate -> accent input
- Additional modulation CV -> another CV input
- Audio out -> mixer / filter / external effects

This gives separate control over:
- when a note happens
- what pitch it is
- how expressive it is
- how timbre evolves

---

# Limitations to keep in mind

The LXR can be melodic, but it is still a drum-oriented architecture.

## Important practical constraints
- Voices are not all equally suitable for tonal tracking
- Envelopes are drum-oriented rather than full sustain ADSR types
- It excels more at:
  - plucks
  - bass hits
  - bells
  - mallets
  - zaps
  - tuned percussion
  than at long sustaining pads
- Only one global FX processor can run at a time
- 1V/Oct uses the modulation matrix, so setup requires routing

So think of it less as a traditional polysynth and more as a **multi-voice melodic percussion and electronic timbre generator**.

---

# Best melodic roles for the LXR

From the manual, the strongest melodic uses are:

- **Tuned bass drum/bass synth**
- **Electro tom melodies**
- **FM bell lines**
- **Synthetic mallet riffs**
- **Cowbell and tuned metallic percussion**
- **Zap leads**
- **Acid percussive sequences**
- **Layered chord-like rhythmic hits**
- **Morphing timbral melody voices**

---

# Conclusion

The Erica Synths x Sonic Potions LXR is absolutely capable of melodic use when treated as a **CV-playable drum synth voice bank** rather than only a percussion source. The key feature is the **mod matrix destination “v/o”**, which enables proper pitch control from external CV. Once that is in place, the module’s oscillators, FM structures, filters, transient shaping, envelopes, LFOs, accent modulation, and effects make it highly capable for:

- basslines
- bell melodies
- tuned percussion
- plucks and stabs
- metallic leads
- evolving rhythmic harmonic textures

In a eurorack system, it works best when combined with:
- a quantized pitch sequencer
- trigger sequencing
- accent/gate variation
- external mixing and effects

Used this way, the LXR can cover a lot of the melodic and harmonic edge of a track while still retaining the punch and character of a drum synth.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)