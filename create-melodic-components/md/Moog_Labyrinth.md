# Moog — Labyrinth

- [Manual PDF](../../manuals/Labyrinth Manual.pdf)

---

[Moog Labyrinth Manual (PDF)](https://api.moogmusic.com/sites/default/files/2024-02/Labyrinth_Manual.pdf)

# Using Moog Labyrinth to Create Melodic Components in Music

Moog **Labyrinth** is unusually strong as a melodic Eurorack/semi-modular instrument because it combines:

- **Two pitch-capable oscillators**
- **Two independent generative sequencers**
- **Built-in quantization/scales**
- **Per-step CV for pitch and timbre**
- **Parallel/serial tone-shaping paths**
- **Patchable triggers, clocks, envelopes, and CV**

In practice, this means Labyrinth can generate:

- repeating melodies
- evolving motifs
- counterpoint
- basslines
- tuned percussion lines
- semi-random lead phrases
- two-voice interlocking parts
- externally transposed or clocked melodic systems

---

## 1. The core melodic architecture

The melodic heart of Labyrinth is the pairing of:

- **SEQ1**
- **SEQ2**
- **VCO** (sine oscillator)
- **MOD VCO** (triangle oscillator)

By default:

- **SEQ1** modulates **VCO pitch**
- **SEQ2** modulates **MOD VCO pitch**

Each active sequencer step stores:

- a **gate state** (bit on/off)
- a **random CV value**

When a bit is turned on, Labyrinth generates a random voltage for that step. That CV can then be:

- scaled with **SEQ1/SEQ2 CV RANGE**
- quantized to a musical scale
- sent internally to oscillator pitch
- sent externally through **SEQ1 CV** and **SEQ2 CV**

This makes Labyrinth more than a “random synth”: it is a **two-lane generative melody engine**.

---

## 2. How to create usable melodies

## A. Start with quantized pitch sequencing

For conventional melodic use:

1. Turn up **VCO SEQ1 AMT** to **QTZ**
2. Turn up **SEQ1 CV RANGE**
3. Select a quantizer scale
4. Turn on a few bits in **SEQ1**

That gives you a melodic line on the main VCO.

Do the same for the MOD VCO:

1. Turn up **MOD VCO SEQ2 AMT** to **QTZ**
2. Turn up **SEQ2 CV RANGE**
3. Activate steps in **SEQ2**

Now you have a second melodic line.

### Why this works musically
The sequencers generate random voltages, but the **quantizer maps them into scales**, so you get notes that stay musically related rather than arbitrary voltages.

Available scales include:

- Unquantized
- Chromatic
- Major
- Pentatonic
- Melodic minor
- Harmonic minor
- Whole tone
- Hirajoshi pentatonic
- chordal scales like Major 7, Minor 7, Major 13
- special tunings like Hang Drum and Quads

So melodically, Labyrinth can move from:

- tonal and consonant
- modal and exotic
- chord-tone driven
- abstract and atonal

---

## B. Control melodic range

The **SEQ CV RANGE** knobs are crucial.

Each step stores a bipolar voltage, but **CV RANGE** determines how wide that voltage spread becomes before quantization.

Use this musically:

- **Low CV RANGE**: compact melodies, narrow interval movement, bassline-like
- **Medium CV RANGE**: singable melodic contours
- **High CV RANGE**: wide leaps, more angular lead patterns

This is one of the easiest ways to shape musical behavior.

### Practical uses
- For basslines: keep CV RANGE low
- For arpeggio-like lines: medium range with pentatonic/major quantization
- For generative ambient melodies: medium-high range with long envelope decays
- For tuned percussion: narrow range plus short EG decay

---

## C. Build rhythm separately from pitch

A key compositional strength of Labyrinth is that **rhythm and pitch are partially decoupled**.

Each step has:

- an on/off bit for whether it triggers
- a stored voltage for pitch/timbre when active

This allows you to compose melody in two layers:

1. **Rhythmic pattern** = which bits are on
2. **Note pattern** = the stored voltages on those active bits

So if you keep the same active bits but mutate voltages, you preserve rhythm while changing melody.

This is exactly what **CORRUPT below noon** does:
- it changes stored voltages
- but preserves the trigger pattern

That makes it excellent for:
- evolving melodies with fixed groove
- ambient ostinatos
- generative lead lines that stay rhythmically coherent

Above noon, **CORRUPT** also starts flipping bits, so rhythm mutates too.

---

## 3. Using both sequencers together melodically

## A. Two-voice counterpoint

The most obvious melodic use is:

- **SEQ1 → VCO**
- **SEQ2 → MOD VCO**

Then mix both oscillators in the mixer.

This creates:

- duet lines
- bass + melody
- melody + countermelody
- melody + drone-like sub-line
- intervallic interplay

Because the **MOD VCO** has a lower and wider range, it can serve as:

- a bass voice
- a low melodic companion
- an LFO-rate modulator that occasionally enters audio range
- a tuned percussion source

### Best method
- Quantize both sequences to the same scale
- Keep one sequence shorter than the other
- Use different sequence lengths for polymetric motion

For example:
- SEQ1 length = 5
- SEQ2 length = 7

This yields melodic phrases that phase against one another over time.

---

## B. Chained 16-step melodic structures

Press **CHAIN SEQ** to link SEQ1 and SEQ2 into a single longer sequence.

This is useful for:
- longer melodic phrases
- less repetitive lines
- verse-length motifs
- more structured 16-step patterns

In chained mode, both sequencers traverse a shared 16-step structure, and you can still scale or offset them separately in useful ways.

This creates possibilities like:
- one oscillator following the shared long phrase
- another voice reading the same phrase at a different range
- round-robin or offset melodic relationships

---

## C. Offset relationships

In chained mode, you can offset SEQ2’s playhead relative to SEQ1.

Musically this is excellent for:
- canon-like imitation
- delayed response phrases
- phase-shifted melodic doubles
- evolving harmony from the same note pool

This is one of the most musically interesting features in the manual because it lets one pitch source feel “related” without being identical.

---

## 4. Timbre as part of melody

Labyrinth is not just a pitch sequencer. It can make melody more expressive by changing timbre per step.

### Internal per-step timbral destinations:
- **SEQ1 → VCW FOLD**
- **SEQ2 → VCF CUTOFF**

So while one sequencer drives pitch, it can also drive articulation.

For example:

- **SEQ1 to VCO pitch + VCW FOLD**
  - each note changes not only in pitch but also brightness/complexity

- **SEQ2 to MOD VCO pitch + VCF CUTOFF**
  - each note changes pitch while the filter shapes each note differently

This makes melodies feel:
- articulated
- phrase-like
- dynamic
- less static

In melodic writing, per-step timbre changes often read like:
- accent patterns
- plucked vs muted notes
- open/closed articulation
- pseudo-velocity changes

---

## 5. Using the oscillators melodically

## A. VCO as the primary melodic voice

The sine **VCO** is the cleanest place to start. Because it begins simple, it’s easy to hear pitch clearly.

Use it for:
- leads
- basslines
- clean melodic motifs
- tuned percussion when modulated by EG1

Then gradually enrich it using:
- mixer saturation
- wavefolding
- filter
- FM
- ring modulation

---

## B. MOD VCO as second melody or interval source

The **MOD VCO** is wider-range and lower by design, but it is still pitch-capable.

Use it as:
- a bass voice
- a second melody
- interval stack with VCO
- “shadow melody” an octave or fifth away
- sub-audio modulator that occasionally becomes audible

A very effective patch is:
- tune MOD VCO to a consonant interval from VCO
- sequence both
- keep one more rhythmically sparse

This creates melodic depth without needing another external oscillator.

---

## C. Ring modulation for metallic melodic lines

The **RING MOD** output in the mixer produces sum and difference tones between VCO and MOD VCO.

For melody, this is useful when:
- both oscillators are tuned to musically related intervals
- sequences are quantized
- you want bell-like, gamelan-like, or inharmonic-but-repeatable pitch material

This can create:
- struck-metal melodic voices
- tuned percussive figures
- alien harmonic lines

Especially effective with:
- short EG decay
- quantized pentatonic or Hang Drum scales
- moderate filter shaping afterward

---

## D. FM-based melodic color

The **MOD VCO FM AMT** routes the MOD VCO into thru-zero FM of the VCO.

Because the manual notes that this preserves the tonal center better, it is particularly useful for melodic work compared to wilder untamed FM systems.

Use small-to-medium FM for:
- vibrato-like motion
- brightening melody
- electric piano-ish tones
- struck digital-style melodic timbres

Use high FM for:
- aggressive leads
- clangorous tuned percussion
- animated melodic motifs

This works especially well when the MOD VCO is itself sequenced, because each note can imply a different FM relationship.

---

## 6. The voice paths as melodic shapers

Labyrinth’s melodic usefulness depends heavily on its two processing paths:

- **VCW** = additive/upper harmonic generation
- **VCF** = subtractive shaping

## A. VCW for melodic presence

The wavefolder is ideal for making simple pitch lines speak more clearly in a mix.

Use wavefolding for:
- brighter leads
- more overtone-rich melodies
- per-note articulation
- expressive upper harmonics without losing the base pitch

Since **VCW FOLD** can be modulated by EG1 and SEQ1, you can make the melody:
- strike harder at note onset
- vary harmonic density from note to note

That is especially musical for:
- plucks
- mallet-like tones
- Buchla-style melodic phrases
- evolving generative leads

### VCW BIAS as melodic color
**VCW BIAS** changes asymmetry and harmonic flavor. This is subtle but powerful for melody because it changes the character of the notes without changing pitch.

---

## B. VCF for phrase contour

The filter path is useful for:
- softening a melody
- creating dynamic phrasing
- adding resonance to emphasize note attacks
- shaping melodic phrases over time

Use **SEQ2 AMT to VCF CUTOFF** to create step-dependent articulation.  
Use **EG1/CV AMT** to make each note open the filter.

This gives melodic parts:
- attack shape
- contour
- breath
- emphasis

The **FILTER MODE** sweep between lowpass and bandpass is especially good for melodic textures:
- **LP** = rounder, more traditional synth line
- **BP** = thinner, more focused, reed-like or percussive melodic tone

---

## C. BLEND as a macro melodic expression control

The **BLEND** knob crossfades between VCW and VCF paths.

That means you can morph a melody between:
- harmonically rich/folded
- filtered/subtractive

This is excellent for performance:
- verse/chorus texture shifts
- moving a melody from soft to bright
- creating call/response timbral evolution

And because **BLEND** has a CV input, you can automate this from external Eurorack modulation for melodic motion over time.

---

## D. ORDER for melodic signal routing

The **ORDER** switch changes how the melodic signal is processed:

- **PARALLEL**: VCW and VCF get the same input
- **VCW > VCF**: folded signal goes into filter
- **VCF > VCW**: filtered signal goes into wavefolder

Musically:

### PARALLEL
Best for:
- clean contrast
- mixing bright/folded and dark/filtered layers
- stable melodic timbre with macro control

### VCW > VCF
Best for:
- taming bright wavefolded melodies
- animated but more controlled leads
- bell-like tones shaped into usable melodic lines

### VCF > VCW
Best for:
- emphasizing specific filtered bands before adding harmonics
- more unusual, vocal, nasal, or sharp melodic sounds
- resonant, gritty leads

---

## 7. Envelopes and trigger behavior for melody

Labyrinth has two decay envelopes:

- **EG1**: modulation envelope
- **EG2**: VCA envelope for both paths by default

## A. EG2 for note length

EG2 controls loudness contour, so it defines whether a melody feels:

- staccato
- plucky
- legato-ish
- droning/percussive

Use:
- **short EG2 decay** for sequences, basslines, tuned percussion
- **long EG2 decay** for ambient melodies and overlapping phrases

---

## B. EG1 for melodic articulation

EG1 can modulate:
- VCO pitch
- MOD VCO pitch
- VCW FOLD
- VCF CUTOFF

This is huge for melody design.

### Uses
- small positive pitch envelope = pluck/strike attack
- negative pitch envelope = falling attack, tom/kick-like note onset
- fold envelope = brighter attack
- filter envelope = classic subtractive melodic articulation

You can apply EG1 differently to each destination, so a melodic note can simultaneously:
- bend in pitch
- brighten at attack
- open the filter

That makes even a simple 4-step melody sound expressive.

---

## C. EG TRIG MIX for accented melodic interplay

**EG TRIG MIX** blends trigger influence from SEQ1 and SEQ2 into the envelopes.

This matters melodically because it determines which rhythm stream articulates the sound.

With two sequencers running, you can create:
- one pitch sequence but another articulation sequence
- accented counterpoint
- melodic ghost notes
- syncopated dynamic emphasis

This is a very compositional feature.

Example:
- SEQ1 carries the main melody rhythm
- SEQ2 has sparse trigger bits
- EG TRIG MIX set between them

Result: some notes hit harder or differently depending on overlap.

---

## 8. Patch-bay uses for melody

The patch bay makes Labyrinth much more than a closed voice.

## A. Use sequencer CV outputs to control external melodic modules

Outputs:
- **SEQ1 CV**
- **SEQ2 CV**
- **SEQ1 TRIG**
- **SEQ2 TRIG**

These can drive external Eurorack voices.

Examples:
- SEQ1 CV → external oscillator 1V/oct
- SEQ1 TRIG → external envelope/gate
- SEQ2 CV → another oscillator or filter cutoff
- SEQ2 TRIG → drum or accent input

So Labyrinth can become the melodic brain for:
- another analog voice
- a sampler
- a wavetable oscillator
- a chord module
- a quantized percussion voice

---

## B. Use external pitch CV to play Labyrinth conventionally

Inputs:
- **VCO 1V/OCT**
- **M VCO 1V/OCT**

This lets external melodic sources control Labyrinth.

Use cases:
- keyboard/sequencer transposition
- DAW-to-CV pitch control
- external precision sequencer for fixed melody
- combining deterministic pitch with Labyrinth’s internal rhythm/timbre mutations

This is one of the best hybrid approaches:
- use external 1V/oct for intentional melody
- use Labyrinth’s internal sequencers for timbral modulation and triggers

---

## C. MIDI note transposition

According to the manual, when quantization is active, a **MIDI Note On** transposes the root of SEQ1 and SEQ2 quantized CVs.

This is very useful musically.

It means you can:
- let Labyrinth generate the pattern
- transpose the whole melodic system from a keyboard, DAW, or MIDI sequencer

That gives you:
- generative phrases that still follow chord changes
- live transposition of evolving patterns
- song-structured harmony from a random engine

This is arguably one of the strongest melodic features in the instrument.

---

## D. Clocking for melodic phrasing

Inputs:
- **CLOCK 1**
- **CLOCK 2**

Output:
- **CLOCK**

Because each sequencer can be clocked separately, you can create:
- independent melodic rates
- polyrhythmic counterpoint
- one slow melody against one fast melody
- phase music structures

For instance:
- external clock division to CLOCK 1
- faster division to CLOCK 2

Then:
- SEQ1 becomes bass pulse
- SEQ2 becomes faster ornament line

---

## E. Use BIT FLIP inputs for algorithmic melody generation

Inputs:
- **BIT FLIP 1**
- **BIT FLIP 2**

These flip the current write-head bit when high.

This is powerful for melody because it allows external modulation to decide:
- when notes appear/disappear
- when new random pitch values are created

Patch ideas:
- LFO or clocked gate → BIT FLIP 1
- random gate source → BIT FLIP 2
- envelope or trigger stream → BIT FLIP inputs

Result:
- self-writing melodies
- probabilistic note insertion
- living melodic textures

The manual even suggests using the MOD VCO to flip bits for rhythmic variation.

---

## F. External CV into BLEND, FOLD, and CUTOFF for melodic motion

Inputs:
- **BLEND**
- **FOLD**
- **CUTOFF**

These let other modules animate melody timbre.

Best uses:
- external envelope → CUTOFF for stronger note shape
- LFO → BLEND for timbral cycling
- random stepped CV → FOLD for changing harmonic emphasis per phrase
- sequencer row → BLEND for sectional contrast

---

## G. Separate VCA control for melodic layering

Inputs:
- **VCW VCA CV**
- **VCF VCA CV**

Since EG2 is normalled here, patching external CV breaks the internal connection.

This lets you independently articulate the two paths.

Musically this means:
- different note lengths for folded vs filtered layers
- one path as a sustained tone, another as short attacks
- pseudo-dual articulation from one melodic source

That can make a single melody feel like two interwoven voices.

---

## H. Utility mixer for melodic rerouting

The **U MIX** can combine audio or CV.

Useful melodic applications:
- mix external CV with sequencer CV before routing
- blend ring mod or another source into a melodic path
- create alternate audio feeds into VCW or VCF
- build duophonic-like routing ideas

Because U MIX 1 is normalled to ring mod, you can turn ring-mod material into a secondary melodic color source.

---

## 9. Strong melodic patch strategies

## Strategy 1: Bass + lead duet
- SEQ1 → VCO pitch
- SEQ2 → MOD VCO pitch
- same scale on both
- short EG2 decay
- VCO cleaner, MOD VCO lower
- FILTER MODE near LP

Result:
- interlocking two-voice melodic part

---

## Strategy 2: Evolving tonal ostinato
- Major or pentatonic quantization
- 3–5 bits active in SEQ1
- medium CV RANGE
- CORRUPT below noon
- EG2 medium decay
- slight EG1 to filter and fold

Result:
- repeating rhythm with slowly changing notes

---

## Strategy 3: Transposable generative harmony
- quantizer enabled
- both sequencers active
- MIDI Note On from keyboard/DAW
- use Note On to transpose root

Result:
- one generated melodic ecosystem that follows song harmony live

---

## Strategy 4: Tuned percussion melody
- short EG2 decay
- EG1 to oscillator pitch for attack snap
- ring mod or FM added
- pentatonic / Hirajoshi / Hang Drum tuning
- bandpass or moderate fold

Result:
- mallet, bell, or drum-like melodic lines

---

## Strategy 5: One melody, changing articulation
- SEQ1 controls VCO pitch
- SEQ2 controls filter cutoff or EG trigger influence
- EG TRIG MIX between SEQ1 and SEQ2

Result:
- pitch pattern stays coherent while articulation evolves separately

---

## Strategy 6: Long-form ambient melody
- CHAIN SEQ on
- longer decay times
- medium CV range
- minor, melodic minor, or whole tone quantization
- BLEND moving slowly
- slight CORRUPT

Result:
- wandering but musically bounded ambient line

---

## 10. Best musical roles for Labyrinth in a Eurorack system

Labyrinth works especially well as:

### A. Melodic generator
Use its internal sequencers as the source of evolving note material.

### B. Dual voice melodic instrument
Use VCO and MOD VCO as two interacting pitch voices.

### C. Transposable generative sequencer
Use MIDI note input or external 1V/oct to impose harmonic structure.

### D. Melodic modulation hub
Use SEQ1/SEQ2 CV outputs to animate external voices.

### E. Timbre-rich lead or bass voice
Use fold/filter/blend/order to keep melodic repetition interesting.

---

## 11. Most important takeaways

If your goal is to make **melodic components for music**, the most important ideas from the manual are:

1. **Use quantization** to turn random voltages into scales
2. **Use CV RANGE** to keep interval motion musically useful
3. **Treat SEQ1 and SEQ2 as two melodic lanes**
4. **Use different sequence lengths** for evolving counterpoint
5. **Use CORRUPT below noon** for melodic variation without destroying rhythm
6. **Use per-step timbre modulation** to make melodies expressive
7. **Use MIDI Note On transposition** to fit generative patterns into harmonic song structures
8. **Use patch-bay CV/trig I/O** to involve external oscillators, envelopes, clocks, and sequencers

---

## Bottom line

Moog Labyrinth is best understood not just as a synth voice, but as a **self-generating melodic ecosystem**. Its two random-but-quantizable sequencers, dual oscillators, and patchable tone-shaping sections make it especially good for:

- evolving melodies
- bass and lead pairings
- melodic percussion
- counterpoint
- scale-constrained generative composition
- external transposition within a larger Eurorack or MIDI setup

It is particularly effective when you want melodies that feel **alive and emergent**, but still remain **musically grounded**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)