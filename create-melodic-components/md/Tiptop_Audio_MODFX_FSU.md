# Tiptop Audio — MODFX FSU

- [Manual PDF](../../manuals/Tiptop_Audio_fx_manual_MODFX_FSU.pdf)

---

[Tiptop Audio ModFX / FSU Manual PDF](https://tiptopaudio.com/manuals/)

# Using Tiptop Audio ModFX + FSU Together for Melodic Eurorack Patches

These two 8hp modules are not “oscillators” in the traditional sense, but together they can absolutely generate and shape **melodic material** from simple sources, short impulses, loops, and external audio.

## Quick take

- **ModFX** is best for turning simple tones into:
  - stereo chorus voices
  - resonant pitched delays
  - Karplus/plucked pseudo-strings
  - phaser/formant/filter movement that emphasizes melody
- **FSU** is best for:
  - pitch-warping and granular melodic fragments
  - Sound-on-Sound looping for phrase capture
  - distortion/frequency shifting for harmonic coloration
  - varispeed and pitch-shifted playback for transposed motifs

Together, they work especially well for:
1. **Karplus and resonator-based pitched voices**
2. **Looped melodic fragments**
3. **Granular/pitch-shifted lead lines**
4. **Stereo doubled melodic textures**
5. **Choir/formant-based pseudo-vocals**
6. **Evolving harmonized delays and chord clouds**

---

# What each module contributes melodically

## ModFX melodic strengths

From the manual, the most melody-relevant programs are:

### Flanger bank
- **Short Karplus**
- **Dual Karplus**
- **Interval Karplus**
- **Chord Resonator**
- **Haas Detune**

These are the most obviously “pitched” functions.  
They can turn triggers, clicks, noise bursts, and percussive audio into tuned tones.

### Chorus bank
- **Vintage Random Vibrato**
- **Dual Vibrato**
- **Tri Stereo Chorus**
- **6 Voice Chorus**
- **Random Chorus 4 Voice**

These don’t generate melody on their own, but they are excellent for making a mono melody into something larger, animated, and harmonically richer.

### Filter bank
- **Formant Ping Pong Delay**
- **Ahh Detuned**
- **Tape Filter**
- **Quad Bandpass LFO**
- **Many 1 Pole**

These are useful for turning harmonically rich oscillators into vowel-like leads, moving spectral melodies, and animated stereo parts.

---

## FSU melodic strengths

### Glitch/Warp bank
- **Glitch Pitch**
- **Varispeed**
- **Varispeed Grains**
- **Random Grain**
- **Pitch Grain**
- **Random Grain Fb2**
- **Many Head Pitch Feedback**

This bank is ideal for taking an existing melody or short motif and turning it into transposed, fragmented, or granulated melodic material.

### Sound on Sound bank
- **Dual Head**
- **Dual Pitch**
- **Chorus**
- **Varispeed**
- **Panning Heads**
- **Random Grains**
- **Buffer Degrade**
- **Frozen Plate**

This bank is very useful for capturing phrases and replaying them as melodic loops, harmonized layers, and shifting textures.

### Distort bank
- **Ring Mod Sine**
- **Dual Ring Mod**
- **Frequency Shifter**
- **Dual Frequency Shift**
- **Tape Saturation**

These are less “melody generators” and more harmonic enhancers/destructors. But used carefully, they can create sidebands and tuned coloration that support melodic lines.

---

# Best ways to create melodic components

## 1. Use ModFX as a plucked-string voice

The strongest melodic trick in this pair is **Karplus-Strong** on ModFX.

### Best programs
- **Short Karplus** — mono plucked voice
- **Dual Karplus** — stereo two-note pitched result
- **Interval Karplus** — easy interval-based harmonies
- **Chord Resonator** — turns impulses into chord-like resonances

### What to feed it
Use:
- trigger clicks
- short envelopes pinging a VCA
- noise bursts
- short percussion sounds
- a filtered impulse
- sharp attack waveforms

### Why this works
Karplus patches create a perceived pitch from a short excitation into a feedback delay line. That means **you do not need a full oscillator voice** to get a note-like result.

### Musical uses
- plucked bassline
- pseudo-harp sequence
- tuned percussion melody
- stereo dyads and interval lines
- chord stabs from triggers

### Patch idea
**Trigger sequencer → short click/noise burst → ModFX Dual Karplus**

Then:
- **Rate** controls right-side pitch
- **Depth** controls left-side pitch
- **Filter** controls feedback/decay

Add CV to Rate and Depth and you get moving interval relationships.

### Great follow-up
Send the result into **FSU Tape Saturation** or **Clipper** to add body and presence.

---

## 2. Capture a melody in FSU and re-harmonize it

FSU’s **Sound on Sound** bank is very strong for melodic phrase processing.

### Best programs
- **Dual Pitch**
- **Dual Head**
- **Varispeed**
- **Random Grains**
- **Frozen Plate**

### Why this works
You can record a short phrase or note into the SOS buffer and then:
- shift pitch independently left and right
- scrub to different positions
- reverse or varispeed playback
- create harmonized or stretched versions

### Musical uses
- canon-style echoes
- harmonized motif layering
- octave-up/down replay
- reversed melodic phrases
- looping micro-phrases as hooks

### Patch idea
**Oscillator melody → VCA → FSU SOS Dual Pitch**

Use:
- **Gain** as recording amount into buffer
- **Filter** = one playback pitch
- **Depth** = the other playback pitch

Record only short note groups. Then tune left/right heads into:
- octave + fifth
- unison + octave
- minor third + fifth

You get a playable harmonizer/phrase doubler.

### Pro tip
The manual notes **Fidelity changes memory time and pitch behavior**, so this becomes a compositional tool:
- record at high fidelity
- reduce fidelity
- transpose playback
- use resulting time-stretch-ish artifacts as melodic texture

---

## 3. Use FSU Glitch/Warp as a melodic variation engine

The **Glitch/Warp** bank can make melodies from incoming notes or loops feel alive and unstable.

### Best programs
- **Glitch Pitch**
- **Pitch Grain**
- **Varispeed**
- **Varispeed Grains**
- **Many Head Pitch Feedback**

### Why it’s useful
This bank doesn’t just “destroy” sound. It can make:
- new transpositions
- fluttering pitch ornaments
- granular repeats that behave like arpeggios
- fractured but musical lead textures

### Patch idea
**Simple saw/square melody → FSU Pitch Grain → ModFX Tri Stereo Chorus**

FSU creates shifting pitch/grain melody fragments.  
ModFX widens and smooths them into a lush stereo lead.

### Good sources
- a dry sequenced oscillator
- a sampled vocal phrase
- a kalimba/pluck sound
- a sine or triangle for clean pitch results
- short loops from the SOS bank

### Musical results
- “Boards of Canada” warped lead
- broken tape melody
- ambient granular arps
- detuned synth-hook fragments

---

## 4. Turn one melody into a stereo ensemble

ModFX excels at taking a plain melodic line and making it sound like multiple performers.

### Best programs
- **6 Voice Chorus**
- **Tri Stereo Chorus**
- **Dimension**
- **Vintage Ensemble**
- **Random Chorus 4 Voice**
- **Dual Vibrato**

### Why this matters melodically
A melody often feels small when it’s a single dry line. These programs add:
- detuning
- motion
- stereo spread
- pseudo-multi-tracking
- ensemble thickness

### Patch idea
**VCO → filter/VCA → ModFX Vintage Ensemble or Tri Stereo Chorus**

For best results:
- use a simple waveform
- try mostly wet or fully wet where recommended
- modulate Rate or Depth slowly with CV for organic drift

### Good uses
- string-machine chords
- animated mono leads
- doubled bass motifs
- chorused arpeggios
- vintage synth-pop melody lines

### Specific standout
**Vintage Ensemble** is especially nice for melodic pads and string-style counterlines.  
The manual notes that **Rate adds octave-down pitch**, which can thicken a melody into a more harmonically grounded line.

---

## 5. Build harmonic intervals with ModFX, then loop them with FSU

One of the strongest pairings is:

1. Generate tuned or interval-based material in **ModFX**
2. Capture and repeat it in **FSU SOS**

### Example workflow
- Use **ModFX Interval Karplus**
- Feed it rhythmic triggers or short bursts
- Dial in a stable interval
- Send stereo output to **FSU Dual Head** or **Dual Pitch**

Now you have:
- a generated dyad or harmonic gesture
- which can be looped, replayed, pitch-shifted, and layered

### Result
This can create:
- ostinatos
- pseudo-sequenced string patterns
- ambient pluck loops
- evolving harmonic motifs

---

## 6. Use formants to make melodies read more clearly

Melody is not just pitch; it’s also **timbre articulation**. ModFX has several programs that help notes speak.

### Most useful
- **Ahh Detuned**
- **Formant Ping Pong Delay**
- **Tape Filter**
- **Many 1 Pole**
- **Quad Bandpass LFO**

### Why they help
A simple saw melody can become:
- vowel-like
- more vocal
- more animated
- more separated in the mix

### Patch idea
**Rich oscillator → ModFX Ahh Detuned**

Use:
- **Filter/Fdback** to tune formants
- **Rate** and **Depth** to detune left/right

This gives you choir-like pseudo-vocals for leads and melodic drones.

Then send that into:
**FSU Frozen Plate** for a sustained vocal cloud.

---

# The best module orderings

## ModFX → FSU
Use this when ModFX is creating the initial melodic identity.

Best for:
- Karplus plucks into looping/granular processing
- chorused leads into varispeed/granular warp
- formant voices into SOS looping

### Example
**Noise burst → ModFX Chord Resonator → FSU Random Grains**

Result:
- pitched chordal resonances
- chopped into moving granular melodic particles

---

## FSU → ModFX
Use this when FSU is generating fragments and ModFX is beautifying or stabilizing them.

Best for:
- warped loops into chorus
- glitch pitch into vibrato/ensemble
- SOS phrases into stereo imaging

### Example
**Melody source → FSU Glitch Pitch → ModFX Dimension**

Result:
- unpredictable pitch movement
- polished into a wide stereo melodic texture

---

## Feedback loop between both
This is where things get very interesting.

### Example
**Source → ModFX Karplus/Resonator → FSU Many Head Pitch Feedback → back to source mixer/send**

You can get:
- cascading tuned resonances
- harmonically smeared repeats
- self-building melodic ambience

Keep levels controlled.

---

# Best melodic patch recipes

## A. Stereo plucked duet
- Trigger sequence into short noise burst
- Into **ModFX Dual Karplus**
- CV sequence to **Rate** and **Depth** for left/right pitch
- Moderate **Filter** for decay
- Into **FSU Tape Saturation**

**Result:** stereo plucked melody with warmth and attack.

---

## B. Harmonized loop canon
- Record a short melody into **FSU SOS Dual Pitch**
- Set one side unison, the other fifth or octave
- Send to **ModFX Tri Stereo Chorus**

**Result:** wide harmonized hook line.

---

## C. Choir lead
- Saw oscillator or wavetable source
- Into **ModFX Ahh Detuned**
- Tune formants with Filter
- Add subtle detune on left/right
- Into **FSU Frozen Plate**

**Result:** vocal-like sustained melodic voice.

---

## D. Broken tape arp
- Arpeggio from oscillator into **FSU Varispeed Grains**
- Modulate speed slowly and unevenly
- Send output into **ModFX Dimension** or **6 Voice Chorus**

**Result:** unstable but lush melodic repeats and shimmer.

---

## E. Chord percussion to melody
- Triggered clicks or percussive bursts
- Into **ModFX Chord Resonator**
- Tune resonance and damping
- Feed result into **FSU Random Grain Fb2**

**Result:** struck chord fragments evolving into melodic clouds.

---

## F. Animated stereo lead
- Clean VCO melody into **FSU Pitch Grain**
- Dial moderate pitch shift and grain movement
- Into **ModFX Vintage Ensemble**
- Mix mostly wet

**Result:** a lead that sounds layered, unstable, and lush.

---

# CV strategies for melodic use

Both modules have **3 CV inputs mapped to the 3 DSP parameters**, which is very important.

## Best modulation sources
- stepped random for note-like jumps
- quantized CV
- slow LFO for drift
- envelopes for per-note movement
- sample & hold
- sequencer rows

## Smart melodic modulation targets

### On ModFX
- **Karplus pitch controls** with quantized CV
- **Chord type / interval** with stepped CV
- **Formant tuning** with slow or sequenced CV
- **Feedback/decay** with envelopes for expressive phrasing

### On FSU
- **Pitch shift amount** with quantized CV
- **Playback position** with stepped voltage
- **Varispeed** with bipolar CV for forward/reverse gestures
- **Grain spread** with envelopes or random for note density changes

---

# Best source materials for melodic results

These modules become more melodic when you feed them the right material.

## Especially good sources
- short filtered noise bursts
- trigger clicks
- plucky envelopes through a VCA
- simple waveforms: saw, pulse, triangle
- speech/vocal snippets
- short melodic loops
- percussion with strong transients

## Less ideal sources
- dense full mixes
- already heavily reverberant sources
- harmonically cluttered audio if you want clear pitch

---

# Programs most useful specifically for melody

## Top ModFX programs
1. **Dual Karplus**
2. **Interval Karplus**
3. **Chord Resonator**
4. **Vintage Ensemble**
5. **Tri Stereo Chorus**
6. **Ahh Detuned**
7. **Formant Ping Pong Delay**
8. **Haas Detune**

## Top FSU programs
1. **SOS Dual Pitch**
2. **SOS Varispeed**
3. **SOS Dual Head**
4. **Glitch Pitch**
5. **Pitch Grain**
6. **Varispeed Grains**
7. **Random Grain Fb2**
8. **Frozen Plate**

---

# Practical musical roles in a patch

## Lead voice enhancer
- Oscillator voice → ModFX chorus/vibrato
- Optional FSU saturation or grain after

## Plucked melodic generator
- Trigger/noise burst → ModFX Karplus
- FSU for looping, pitch layering, degradation

## Harmonizer / doubler
- Melody → FSU Dual Pitch
- ModFX stereo chorus after

## Vocal/formant melody shaper
- Rich waveform → ModFX Ahh Detuned / Formant Ping Pong Delay
- FSU Frozen Plate after

## Ambient melodic looper
- Short phrase → FSU SOS
- ModFX chorus/phaser/filter for movement

---

# My recommended pairings

## Best “musical” pairing
**ModFX Interval Karplus → FSU Dual Pitch**

Creates tuned plucks, then harmonizes or mirrors them.

## Best “lush lead” pairing
**FSU Pitch Grain → ModFX Tri Stereo Chorus**

Creates broken/pitched fragments, then turns them into a polished stereo synth line.

## Best “ambient melody” pairing
**ModFX Chord Resonator → FSU Frozen Plate**

Turns percussive hits into resonant chord tones suspended in reverb-like space.

## Best “vocal melody” pairing
**ModFX Ahh Detuned → FSU SOS Varispeed**

Creates choir-like tones and then stretches/reverses them into phrases.

---

# Bottom line

These modules can work together melodically in three major ways:

1. **ModFX generates or emphasizes pitch**
   - especially with Karplus, resonators, detune, formants, and chorus

2. **FSU captures, transposes, fragments, and repeats melodic material**
   - especially with SOS, pitch/grain, and varispeed modes

3. **Together they turn simple sources into full melodic textures**
   - plucks
   - harmonized loops
   - vocal-like leads
   - evolving stereo hooks
   - granular melodic atmospheres

If you want, I can also turn this into:
- a **“best melodic patches” cheat sheet**
- a **signal-flow diagram**
- or a **program-by-program ranking for ambient / techno / IDM / soundtrack use**

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)