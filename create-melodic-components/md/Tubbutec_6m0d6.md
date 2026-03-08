# Tubbutec — 6m0d6

- [Manual PDF](../../manuals/6m0d6-User-Manual-1.0.pdf)

---

[6m0d6 Manual PDF / latest manual](https://tubbutec.de/6m0d6/)

# Using the Tubbutec/LPZW 6m0d6 for melodic music in a Eurorack system

The 6m0d6 is presented as a TR-606-inspired drum voice, but the manual makes it clear that it can go well beyond percussion. Its combination of **tunable analog drum circuits**, **CV control**, and especially the **MIDI-playable metal oscillator section** makes it surprisingly useful for melodic and harmonic material.

## Big picture: where the melodic potential comes from

The manual describes three main sound-generation areas that matter for pitched or semi-pitched use:

1. **Bass Drum oscillator section**
   - Tuneable from normal kick range down/up into more tonal territory.
   - Long decay allows it to act like a bass voice rather than just a drum transient.

2. **Tom circuits**
   - High Tom and Low Tom are explicitly pitch-adjustable.
   - Low Tom can be shifted into **sub-bass / second bass drum** territory with **Sub Tom**.

3. **Metal oscillator network**
   - Originally for cymbal and hats, but here it is much more flexible.
   - **Metal Tune CV is 1V/oct compatible**.
   - Over **MIDI channel 1**, the six metal oscillators can be played directly as a **paraphonic six-voice synth source**.
   - Cymbal, hihats, and even snare can use this source, so those drum circuits become resonant pitched/noisy voices.

That means this module can contribute:
- **basslines**
- **pitched tom melodies**
- **metallic leads**
- **string-machine-like drones**
- **paraphonic chordal textures**
- **tuned percussion lines**

---

## 1. Bass Drum as a melodic bass voice

The manual says the bass drum has:
- **Tune**
- **Tone**
- **Decay**
- **Click**

And importantly:

> Tune changes the pitch of oscillator 1, ranging from sub-bass to Tom frequencies.  
> Decay adjusts the decay time of oscillator 1 from the original length up to several seconds.

### Musical use
This is enough to turn the BD into a playable bass component, even if it is not full keyboard-tracking in the classic VCO sense.

### Best approaches
- Set **Click** low or off to reduce the percussive transient.
- Increase **Decay** for sustained low notes.
- Use **Tune** to find a stable sweet spot for a key center.
- Use trigger amplitude and accent creatively for dynamics.

### In practice
- Sequence the BD with a trigger sequencer for **pitched kick-bass ostinatos**.
- Modulate tune slowly for **acid-adjacent bass movement**.
- Use different trigger voltages for dynamic phrasing, since the manual notes that trigger amplitude changes not only volume but also timbre.

### Best role
- **Monophonic bass punctuation**
- **Electro bass drum basslines**
- **Sub-heavy root notes**

---

## 2. Toms as tuned percussion and bass/melody voices

The manual states:
- **HT Tune** adjusts High Tom pitch
- **LT Tune** adjusts Low Tom pitch
- **Sub Tom** halves the pitch of the Low Tom and can create a **sub-bass or second bass drum**
- Toms include a noise/reverb component that can be shaped with **Noise Amount** and **Noise Tune**

### Why this matters melodically
Toms are often the easiest drum circuits to repurpose as tuned percussion. Here, they are explicitly tuneable and can cover:
- woody melodic hits
- electro conga lines
- bass ostinatos
- tuned percussion sequences

### Patch ideas
#### A. Tuned tom duet
- Sequence **LT** and **HT** as alternating trigger streams.
- Tune them to two related notes, like root and fifth.
- Use accent variation to make the line feel played rather than programmed.

#### B. Low Tom as bass, High Tom as melody accent
- Engage **Sub Tom** on LT for low-end.
- Tune HT to a higher pitch for a call-and-response pattern.

#### C. Percussive marimba-ish line
- Reduce noise amount.
- Keep decay moderate.
- Use short triggers and rhythmic sequencing.

### Best role
- **Tuned percussion**
- **Electro tom melodies**
- **Secondary bass voice**

---

## 3. Cymbal / hats / snare as pitched sound sources via the metal oscillator

This is the most important melodic feature in the manual.

The module’s cymbal and hats are based on a **metal sound created by six square-wave oscillators**. The manual adds:
- **Metal Tune**
- **Metal Spread**
- CV control for both
- **Metal Tune CV is 1V/oct**
- MIDI channel 1 can directly play the metal oscillators

This is where the 6m0d6 stops being “just drums.”

---

## 4. Using Metal Tune CV as a melodic control source

From the manual:

> Metal Tune: Controls the tune of the metal sound. This input behaves in a 1V / Oct fashion, which makes it possible to play the metal sound like an instrument.

This means that any instrument using the **Metal** source can become a pitch-controlled voice:
- Cymbal
- Open hihat
- Closed hihat
- Snare, if set to Metal source

### Practical melodic setup
1. Set one of these instruments to **Metal** source.
2. Patch a pitch CV sequencer into **Metal Tune CV**.
3. Trigger the voice rhythmically.
4. Adjust **Metal Spread**:
   - **0 spread** = more in-tune/unison behavior
   - more spread = chorused, detuned, cluster-like sound

### Musical outcomes
- **Cymbal as a metallic pluck voice**
- **Open hat as a resonant lead**
- **Snare as a pitched noise synth**
- **Closed hat as a short digital clave-like melody source**

### Most “melodic” settings
- Lower spread
- Decay tuned to note length
- Reduced transient harshness via source and tone choices

---

## 5. MIDI channel 1 turns it into a paraphonic synth

This is the strongest melodic feature in the document.

The manual says:

> Sending notes on MIDI channel 1 allows you to play the six metal oscillators directly.  
> This effectively turns the oscillators – and with them the Cymbal, Hihats and Snare Drum into a paraphonic six-voice synthesizer.

And:

> With Spread set to 0, all oscillators are in tune; increasing Spread will detune all oscillators.

### What that means musically
You can use the 6m0d6 as:
- a **6-oscillator metallic chord voice**
- a **paraphonic drone instrument**
- a **string-machine-like layer**
- an **inharmonic bell/chime synth**

Because the oscillators feed the cymbal/hihat/snare circuits, the envelope/filtering behavior of those drum voices shapes the final result.

### Great melodic uses
#### A. Cymbal as string synth
The manual explicitly suggests this:
> turn your Cymbal into a string synthesizer

How:
- Use MIDI channel 1 to play notes/chords
- Set **Cymbal decay long**
- Disable the cymbal pulse shaper if desired
- Reduce spread for more tonal behavior, increase for ensemble shimmer

#### B. Snare as paraphonic synth voice
- Set snare noise source to **Metal**
- Tune body as needed
- Use longer decay
- Play from MIDI channel 1
This can create nasal, filtered, reedy lines.

#### C. Hats as harmonic shimmer
- Use open hat with long decay
- Feed notes from MIDI
- Spread slightly above zero
This gives metallic choir / gamelan / string-machine textures.

---

## 6. CY.Pulse off: turning the cymbal into a sustained voice

A crucial detail from the manual:

> For the cymbal, this pulse shaper can be disabled, allowing complete control of the Cymbal sound.  
> Effectively, this can turn the cymbal into a drone sound generator or even string-synthesizer.

This is a major melodic/harmonic feature.

### Why it matters
Normally triggers are shortened to 1.2 ms, which preserves drum behavior. Disabling this for cymbal means incoming gate length can directly shape:
- volume
- envelope
- sustain length

### Patch ideas
#### A. Gate-controlled drone
- Turn off **CY.Pulse**
- Send a long gate
- Use Metal source
- Feed pitch to Metal Tune CV or MIDI channel 1
Result: a sustained metallic pad/drone.

#### B. Pseudo-envelope articulation
- Use variable gate lengths from a sequencer
- Short gates = plucks
- Long gates = sustained notes

#### C. String-machine voice
- Cymbal source = Metal
- Long decay
- Spread low to medium
- MIDI notes/chords in
This is likely the most conventionally melodic patch in the module.

---

## 7. Noise source selection as timbral voice design

For **snare, cymbal, and hats**, the module allows selecting between:
- **Noise**
- **Metal**
- **XOR ringmod source**

This matters for melody because each source produces different pitch clarity.

### For clearer pitch
- Use **Metal**
- Keep **Spread** low
- Tune with Metal Tune

### For dirtier melodic textures
- Use **XOR**
- Use MIDI or CV pitch control where possible
- Explore intermediate decay settings

### For noisy tuned percussion
- Use **Noise**
- Tune via surrounding circuit behavior rather than expecting clear pitch
- Great for industrial tonal percussion

---

## 8. Noise Tune as lo-fi timbre control for melodic percussion

The manual notes that the white noise is digitally generated and its quality can be reduced for **bit-crushed** textures via **Noise Tune**.

That means even if a voice isn’t strongly pitched, it can still contribute melodic identity through consistent timbre.

### Use cases
- Snare tuned into a repeated “note-like” industrial hit
- Toms with altered noise reverb for tuned ambience
- Lo-fi melodic percussion where the “pitch” is partly spectral rather than purely tonal

This is especially useful in:
- IDM
- industrial
- electro
- leftfield techno
- experimental pop

---

## 9. Accent and trigger voltage as expression for melodic phrasing

The trigger/accent section is more expressive than on a typical drum module.

The manual says:
- Trigger inputs accept **1V to 15V**
- Trigger amplitude affects not just volume but also sound
- Accent can be gated or CV-controlled
- Accent amount can be externally modulated

### For melodic use
This gives you articulation layers similar to velocity on a synth:
- soft notes
- hard notes
- accented notes
- timbral variation per note

### Practical results
If you are sequencing toms or metallic voices melodically:
- Use different trigger amplitudes for phrase accents
- Use accent gate for selective emphasis
- Use Accent Amount CV for crescendos and dynamic contours

This is especially effective for:
- tuned percussion lines
- bass drum bass phrases
- animated metallic leads

---

## 10. MIDI channel 10 for dynamic drum-note performance

On MIDI channel 10, the standard drum notes trigger the voices, and the manual says:
- velocity 127 gives simultaneous accent
- velocity below 64 shortens pulse length and reduces volume in interesting ways

So even in drum-map mode, you can play **dynamic melodic percussion** from a keyboard or DAW.

### Good uses
- finger-drummed pitched tom riffs
- expressive metallic percussion
- DAW-sequenced velocity-based phrasing
- hybrid drum/melody parts

---

## 11. How 6equencer and 6m0d6 can work together melodically

The manual mentions direct compatibility with **Tubbutec 6equencer** via LINK. Even though the pages provided are mostly the 6m0d6 manual, there is enough to infer how the pairing supports melodic drum composition.

### What LINK gives you
- direct triggering of instruments and accent
- less patching
- per-voice drum sequencing workflow

### Melodic use of the pairing
With 6equencer handling tight trigger programming and accents, you can use the 6m0d6 as a **pitched percussion sequencer voice bank**:
- program repeating LT/HT patterns as melodic motifs
- create accented hat/cymbal ostinatos
- use external CV or MIDI simultaneously for tonal control of metal-based voices

### Strongest combined role
- **sequenced tuned percussion system**
- **electro bass + tom melody workstation**
- **hybrid drum machine / melodic voice module**

---

## 12. Best melodic patches you can build with this module

## Patch 1: Electro bassline
- Use **Bass Drum**
- Set **Click** low
- Raise **Decay**
- Tune to song root
- Sequence triggers rhythmically
- Use accent sparingly for emphasis

**Result:** punchy mono bass voice with 606 DNA.

---

## Patch 2: Tuned tom melody
- Tune **LT** and **HT** to two scale tones
- Use alternating trigger pattern
- Moderate decay
- Low noise amount for clarity

**Result:** classic electro / synth-pop tuned percussion line.

---

## Patch 3: Sub-bass from Low Tom
- Enable **Sub Tom**
- Tune LT low
- Short-to-medium decay
- Use sparse rhythm

**Result:** second bass voice or bass reinforcement under kick.

---

## Patch 4: Metallic lead
- Set **Cymbal** or **Open Hat** to **Metal** source
- Patch sequencer CV to **Metal Tune CV**
- Set **Metal Spread** near zero
- Adjust decay to taste

**Result:** bright, tuned metallic melody.

---

## Patch 5: String-machine cymbal
- Set cymbal to **Metal**
- Long decay
- **CY.Pulse off**
- Play from **MIDI channel 1**
- Slight spread for ensemble shimmer

**Result:** sustained pad/chord layer from a drum module.

---

## Patch 6: Paraphonic industrial chord voice
- MIDI channel 1 into module
- Use cymbal and/or hats with longer decays
- Increase **Metal Spread**
- Optionally use XOR on snare for roughness

**Result:** clangorous harmonic bed, excellent for EBM/industrial/experimental music.

---

## Patch 7: Lo-fi melodic snare synth
- Snare source = **Metal** or **XOR**
- Tune body
- Increase decay
- Modulate **Noise Tune**
- Trigger from MIDI or sequencer

**Result:** noisy but recognizable note-like stabs.

---

## 13. What the module does best melodically

The 6m0d6 is not a conventional precision melodic voice like a dedicated VCO + VCF + VCA chain. Instead, it excels at:

- **pitched percussion**
- **electro bass**
- **metallic tuned voices**
- **drone/chord textures from cymbal/hats**
- **paraphonic synthetic metal/string timbres**
- **expressive hybrid drum-melody lines**

If you want:
- clean subtractive melodies, use another voice
- characterful, rhythmic, unusual melodic parts, this module is excellent

---

## 14. Best system companions for melodic use

To get the most melodic value from 6m0d6, pair it with:

- **CV sequencer** for Metal Tune CV and dynamic modulation
- **Trigger sequencer** with variable voltage outputs
- **MIDI-to-TRS sequencer or DAW** for channel 1 paraphonic play
- **Envelope/LFO modulation** for accent amount and decays
- **External filter/reverb/delay** to turn cymbal/hihat voices into lush melodic layers
- **Quantizer** if you are modulating Metal Tune CV from freer CV sources

---

## Conclusion

From the manual, the 6m0d6 is far more than a drum clone. Its melodic strengths come from:

- tuneable **BD and tom** circuits for bass and percussion lines
- **1V/oct Metal Tune CV**
- switchable **Metal / Noise / XOR** sources
- **MIDI channel 1 direct play of six metal oscillators**
- **CY.Pulse disable** for sustained cymbal drones and string-like tones
- dynamic triggers and accent for expressive articulation

So if you use it together with a sequencer, MIDI source, or 6equencer, it can function as a **hybrid drum machine plus melodic voice module**, especially for bass, tuned percussion, metallic leads, and paraphonic textures.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)