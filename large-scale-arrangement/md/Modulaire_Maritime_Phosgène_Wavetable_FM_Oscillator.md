# Modulaire Maritime — Phosgène Wavetable FM Oscillator

- [Manual PDF](../../manuals/Phosgène _ Modulaire Maritime.pdf)

---

[Manual PDF / Source](https://www.modulaire-maritime.com/phosg%C3%A8ne)

# Modulaire Maritime Phosgène — using it to build full-length songs

Phosgène is a **2hp digital wavetable/FM oscillator** with a surprisingly wide range for such a small module. From the manual page, the key musical features are:

- **60 wavetables** in **2 banks of 30**
- **Two parallel sound paths / outputs**:
  - **Wavetable / waveshaping output**
  - **FM output**
- **Shared controls** influencing both sound engines
- **Wavefolding / waveshaping**, manually and by CV
- **FM built around a 100 Hz base**, giving darker, tighter, less splashy FM tones
- **V/Oct tracking over 8 octaves**
- **Octave up/down switching**
- **Octave displace switch** for the wavetable side, useful for keeping timbres in sweet spots and extending lower range
- **Last-state memory** for bank, wave, and octave

That combination makes Phosgène more than “just another voice oscillator.” It is especially useful as a **song-structure oscillator** because it can move between roles quickly:

- bass
- lead
- drone
- harmonic layer
- metallic percussion
- transitions/noise accents
- doubling another voice with a contrasting output

The biggest trick to making full songs in Eurorack is to stop thinking of a module as a single static voice and start using it as a **scene-changing actor**. Phosgène is ideal for this because the same pitch sequence can sound radically different with:

- wave selection changes
- bank changes
- fold amount modulation
- switching between wavetable out and FM out
- octave displacement for register changes
- filtering and VCAs for arrangement

---

# What this module is especially good at in a song context

## 1. One sequence, many sections
A common Eurorack trap is creating one killer loop and not knowing how to evolve it. Phosgène solves that by giving you multiple timbral identities from one melodic source.

For example, one 16-step sequence can become:

- **Intro**: low, mellow wavetable tone
- **Verse**: same sequence, slightly folded, filtered, quieter
- **Pre-chorus**: switch bank or wave, add CV movement to fold
- **Chorus**: octave up, brighter wave, layered with FM output
- **Bridge**: mute wavetable output, use FM output only for a darker alien version
- **Outro**: return to low octave displaced wavetable with slow modulation

This is one of the easiest ways to get from “loop” to “song.”

## 2. Parallel outputs can create arrangement contrast
Because wavetable and FM are available separately, you can route them into:

- separate filters
- separate VCAs
- separate effects
- separate mixer channels
- separate envelope behaviors

That means one oscillator can serve as **two arrangement layers**.

Example:
- Wavetable output = bass voice
- FM output = upper texture or percussive accent

Or:
- Wavetable output = dry and centered
- FM output = drenched in delay/reverb and faded in only during transitions

That gives you song sections without needing a totally separate oscillator.

## 3. The “imperfect digital” aspect is musically useful
The manual explicitly mentions:
- noise-bearing wavetables
- aliasing at high ranges
- 11-bit character
- “digital trash”

That is not a flaw in song-making. It is actually great for:
- intros
- breakdowns
- rises
- fills
- industrial percussion
- transition effects

A full song needs contrast. Clean sounds alone often loop endlessly; rougher textures help define form.

---

# Core patching roles for Phosgène in a full song

## Role A: Primary bass voice
This is probably the strongest use case.

### Why it works
The manual notes the FM implementation has a **100 Hz base** and produces a more controlled, darker FM sound, good for **tight FM basses** and deep modulation. Also, the octave displace function helps keep the wavetable side in the low-end sweet spot.

### Pair with
- Sequencer: Metropolix, René, Voltage Block + quantizer, Bloom, O_C, Mimetic Digitalis + quantizer
- Envelope: Maths, Zadar, Contour, Quadrax
- VCA: Veils, Tallin, Quad VCA
- Filter: ripples-style LPF, SEM filter, ladder filter, Polivoks for aggressive stuff
- Saturation/waveshaping: Bastl Timber, Instruō tanh[3], L-1, drive in mixer
- Compressor or end-of-chain glue module

### Song use
- **Intro**: bass filtered almost closed, sparse triggers
- **Verse**: regular bassline, low fold CV
- **Chorus**: open filter, add FM output layer for edge
- **Bridge**: drop kick, keep only subby Phosgène with long notes
- **Final chorus**: octave jump + stronger fold modulation

### Best trick
Use the same bass sequence through the whole song, but automate:
- filter cutoff
- wave selection
- fold depth
- octave position
- note density via trigger variation

That alone can create a complete arrangement arc.

---

## Role B: Lead that transforms across sections
Phosgène should excel as a lead because wavetable selection and fold modulation make it easy to generate evolving harmonic color.

### Pair with
- Quantized pitch source
- Slew/glide module
- Envelope + VCA
- Delay/reverb
- Sequential switch or preset manager
- Performance mixer

### Song use
- **Verse**: restrained lead, narrow range, little modulation
- **Pre-chorus**: more wave scanning
- **Chorus**: octave up, increased fold CV, stereo delay
- **Breakdown**: switch to FM output only for a glassy/darker lead variant
- **Outro**: reduced modulation, lower octave, long reverb tails

### Good composition tactic
Don’t write a new melody for every section. Instead:
- keep the same motif
- transpose it
- reharmonize externally
- change its timbre and register with Phosgène

That is how many strong songs maintain identity while evolving.

---

## Role C: Dual-layer voice from one pitch source
This is one of the most song-useful features.

### Patch
- Same V/Oct to Phosgène
- Wavetable output -> low-pass filter -> VCA
- FM output -> band-pass or high-pass -> VCA
- Separate envelopes for each output
- Mix them independently

### Result
You get:
- a body/foundation layer
- an edge/air/attack layer

### Song structure application
- **Intro**: FM layer only, atmospheric
- **Verse**: wavetable layer enters
- **Pre**: FM layer gets rhythmic gating
- **Chorus**: both layers full
- **Bridge**: only filtered wavetable layer remains
- **Finale**: both plus effects

This makes one oscillator behave like a multitracked instrument.

---

## Role D: Industrial percussion / metallic fills
Because the module can produce darker FM and rough digital edges, it can do:
- toms
- clangs
- zaps
- metallic hats
- stabs
- transition hits

### Pair with
- Fast envelopes
- LPG or snappy VCA
- Trigger sequencer
- Random voltage or sample-and-hold to wave CV
- Distortion
- Band-pass filtering

### Song use
A song needs small events between larger loops. Use Phosgène for:
- every 8th bar fill
- bar-end accent
- pre-drop metallic stab
- bridge texture percussion
- outro glitches

This helps create arrangement punctuation, which is often what modular songs lack.

---

## Role E: Drone / harmonic bed
A full-length song often needs sustained background material, not just rhythm and riffs.

### Patch
- Phosgène to a filter and VCA
- Slow LFO to wave selection or fold amount
- Very slow random CV to timbre
- Long envelope or manual VCA opening
- Reverb / shimmer / delay
- Maybe a submixer with sidechain ducking from kick

### Song use
- Intro pad/drone
- Under-verse bed
- Breakdown sustain
- End-of-song tail

Even if Phosgène is monophonic, a rich wavetable through effects can fill a lot of space.

---

# How to make full songs with it: practical arrangement strategies

## Strategy 1: Use “section macros”
The best way to get beyond loops is to assign one control gesture per song section.

For Phosgène, your macros could be:

- **Verse macro**
  - low fold amount
  - stable wave
  - low octave
  - wavetable output only

- **Pre-chorus macro**
  - gradual fold CV increase
  - slight wave movement
  - filter opening
  - occasional FM layer

- **Chorus macro**
  - octave up
  - brighter wave
  - wavetable + FM layered
  - more effects send

- **Bridge macro**
  - switch to darker FM emphasis
  - reduce note density
  - increase space/reverb
  - add random modulation

These macros can be implemented with:
- CV presets
- sequential switches
- mutes
- matrix mixers
- offset/attenuator modules
- performance mixers
- scenes on sequencers

If you can recall 4–5 distinct Phosgène states, you can build a whole song.

---

## Strategy 2: Separate composition from orchestration
In modular, people often constantly change notes when what they really need is to change arrangement.

With Phosgène:
- Keep one strong melody or bassline.
- Let section changes happen through:
  - waveform choice
  - bank selection
  - fold amount
  - octave changes
  - output routing
  - effects sends

This is closer to how songs are actually arranged in traditional production.

---

## Strategy 3: Use probability and reset intelligently
Phosgène sounds varied enough that controlled randomness works well.

### Patch concept
- Main sequencer for pitch
- Trigger sequencer with:
  - probability
  - mutes
  - fills
  - bar resets
- Random source to wave CV, attenuated
- Clock divider for slower section changes

### Song result
- stable motif
- subtle timbral evolution
- occasional timbral surprises
- repeatable bar structure

The key is **bar-level predictability** with **note-level variation**.

---

## Strategy 4: Build songs from register changes
Because the module tracks 8 octaves and includes octave switching/displacement, register is a huge compositional tool here.

Use the same sequence as:
- sub bass in one section
- mid-register riff in another
- high synthetic lead in another
- noisy digital percussion at the top end

Register change is one of the easiest ways to make a modular arrangement feel intentional.

---

## Strategy 5: Alternate “identity outputs”
Treat the two outputs as two emotional versions of the same part.

- Wavetable out = more recognizable, tonal, foundational
- FM out = more shadowy, aggressive, unsettling, synthetic

In a full song:
- use one for “statement”
- use the other for “response”

Example:
- Chorus hook on wavetable output
- Chorus answer phrase on FM output

That creates call-and-response structure.

---

# Example full-song patch ideas

## 1. Techno / EBM track
### Modules
- Phosgène
- kick module or sampler
- noise/snare/hat voices
- 16-step sequencer
- filter
- dual VCA
- distortion
- delay/reverb
- performance mixer
- mute module

### Patch
- Pitch sequencer -> Phosgène V/Oct
- Gate sequence -> envelope -> VCA for wavetable output
- Wavetable output -> low-pass filter -> VCA -> mixer
- FM output -> distortion -> VCA -> mixer
- Slow LFO/random -> wave/fold CV
- Kick ducks Phosgène via sidechain VCA/compressor if available

### Arrangement
- **Intro**: FM output only with delay, kick faded in
- **Verse groove**: bass sequence from wavetable output
- **Build**: increase fold and distortion, add percussion
- **Drop/chorus**: both outputs layered, octave up accents every 4 bars
- **Breakdown**: remove drums, let slow FM drones take over
- **Final section**: reintroduce bass, more open filter, stronger modulation
- **Outro**: mute wavetable, leave FM texture

Phosgène here carries both bassline identity and tension effects.

---

## 2. Ambient / cinematic modular piece
### Modules
- Phosgène
- random source
- quantizer
- slow envelopes/LFOs
- stereo filter or LPG
- granular or reverb processor
- looper/sampler
- mixer

### Patch
- Random stepped CV -> quantizer -> V/Oct
- Very slow gate triggers -> long envelope
- Wavetable output -> LPG/filter -> reverb
- FM output -> granular/delay path
- Slow CV -> fold amount
- Different slow CV -> wave selection

### Arrangement
- **Intro**: drone on wavetable output
- **Section B**: sparse high-register FM notes appear
- **Section C**: loop a phrase and play against it
- **Climax**: both outputs layered with more fold movement
- **Resolution**: reduce note density and move octave downward

Here the song form comes from **density, register, and effects depth**, not drum-based development.

---

## 3. Electro / synth-pop style modular arrangement
### Modules
- Phosgène
- drum machine / sample player
- chord source or polyphonic voice
- sequencer with song mode
- filter
- VCA/envelopes
- chorus/delay/reverb
- mixer with mutes

### Patch role for Phosgène
Use it as the **main hook voice**.

### Arrangement
- **Intro**: single-note motif with delay
- **Verse**: bass role, low octave displaced wavetable
- **Pre**: melody rises with more wave modulation
- **Chorus**: octave up lead hook with layered FM output
- **Verse 2**: back to bass, but altered bank/wave
- **Bridge**: remove drums, use FM output in spacious mode
- **Last chorus**: stack bass and lead by multitracking or live re-patching/muting

A modular song often becomes convincing when one voice can act as both bass and hook at different times. Phosgène seems excellent for that.

---

# Specific module pairings that help turn Phosgène into song material

## With a sequential switch
A sequential switch can route:
- different CV sources into wave/fold control
- different trigger patterns to the VCA envelope
- different outputs into different processing chains

This creates section-by-section identity changes.

Good uses:
- verse = subtle modulation
- chorus = aggressive modulation
- bridge = random stepped timbre changes

---

## With a preset manager / CV memory module
This is one of the best “song form” tools in modular.

Store different offsets for:
- wave selection
- fold depth
- filter cutoff
- VCA level
- effects send
- FM layer level

Then recall those presets as:
- intro
- verse
- chorus
- bridge
- outro

If your system has something like:
- Acid Rain Maestro
- Ornament & Crime scenes
- Verbos Sequence Selector
- presets in a digital controller
- ADDAC/manual scene manager concepts

you can make Phosgène behave like a structured instrument, not just a patch element.

---

## With a matrix mixer
A matrix mixer is great for songs because it lets you blend modulation sources differently per section.

For Phosgène:
- LFO 1 -> fold CV
- Random -> wave CV
- Envelope -> FM depth-related timbral movement
- Manual offset -> base timbre

Then mix those amounts differently in real time.

This creates controlled evolution without repatching.

---

## With a clockable modulation source
To keep the song coherent, sync modulation to bars.

Useful modulation rhythms:
- wave shift every 8 bars
- fold swell every 4 bars
- octave accent every 16 bars
- FM output gate only on fill bars

Clocked modulation is much more song-like than free-running chaos.

---

## With a looper/sampler
One secret to full songs in modular is to **print** parts.

Use Phosgène to record:
- a bass riff
- a drone bed
- a noisy FM texture
- a lead phrase

Then free the module to play a new role on top.

This is one of the fastest ways to get from “one-voice patch” to “arranged track.”

Modules/processes:
- Morphagene
- Lubadh
- Arbhar
- Bitbox
- 1010 Blackbox
- external DAW/looper

---

# Arrangement recipes

## Recipe 1: “Bass to lead” song
1. Write a strong 8- or 16-step sequence.
2. Start with Phosgène as low bass via wavetable output.
3. In chorus, transpose the sequence up 1–2 octaves.
4. Add fold CV and effects.
5. Blend in FM output for edge.
6. Bring bass back in later by looping/sampling or switching to another voice.

This creates a clear narrative from the same motif.

---

## Recipe 2: “Shadow double” arrangement
1. Wavetable output carries the main line.
2. FM output is muted most of the time.
3. Bring FM output in only:
   - at phrase endings
   - every fourth bar
   - in choruses
   - during transitions

This creates tension/release and makes sections feel bigger.

---

## Recipe 3: “Timbral chorus” instead of harmonic chorus
If you don’t have a lot of harmonic voices, make your chorus bigger by changing timbre, not chords.

- Verse: simple, dark wave, low fold
- Chorus: brighter bank, stronger fold, more open filter, layered outputs

Even with the same notes, the chorus feels lifted.

---

## Recipe 4: “Bridge by degradation”
Use the digital edge creatively.

- Reduce drums
- Push Phosgène into noisier/aliasing territory
- High-pass or band-pass it
- Add delay/reverb
- Let it become unstable and textural

Then snap back to a cleaner bass/lead tone for the final section.

That contrast reads as structure.

---

# A practical full-song workflow

## Step 1: Decide its song role
Pick one:
- bass anchor
- lead hook
- dual-layer motif
- drone/percussion utility

Don’t ask it to do everything at once live unless your patch is designed for that.

## Step 2: Make 4 section states
Create:
- A = intro
- B = verse
- C = chorus
- D = bridge/breakdown

Each state should differ in:
- octave/register
- wave or bank
- fold amount
- output balance
- filtering/effects

## Step 3: Keep pitch material simple
Use:
- one riff
- one hook
- one transposed variant

Too much melodic churn often weakens modular songs.

## Step 4: Add punctuation
Every 4, 8, or 16 bars:
- wave jump
- FM stab
- octave accent
- filter sweep
- mute/re-entry

## Step 5: Record passes if needed
If your rack is small, record one Phosgène role, then repatch/use it for another role. Full songs often come from layering time, not only layering hardware.

---

# Potential strengths and limitations to be aware of

## Strengths
- Very compact
- Broad timbral range
- Bass-capable FM character
- Parallel outputs are arrangement-friendly
- Can go from tonal to textural quickly
- Saved state helps patch continuity

## Limitations
Because this is a tiny module, hands-on control may be compact and immediate CV control options may be limited compared to larger oscillators. That means for song work, it benefits greatly from:
- attenuators
- VCAs for modulation depth
- external switching/mixing
- good envelope and filter companions

In other words, Phosgène is likely best as part of a **voice architecture**, not used naked.

---

# Best companion modules for full-song use

If your goal is full arrangements, pair Phosgène with:

- **Sequencer with song mode or pattern memory**
- **Performance mixer with mutes**
- **Filter**
- **At least two VCAs**
- **Clocked modulation**
- **Preset/scenes module or sequential switch**
- **Delay/reverb**
- **Sampler/looper if your system is small**

That combination turns the oscillator into a section-capable instrument.

---

# Bottom line

Phosgène looks especially strong for full-length songs because it is not just “a sound source,” but a **compact timbral arranger**:

- the **wavetable side** gives you body, identity, and harmonic content
- the **FM side** gives you shadow, aggression, and contrast
- **octave displacement** helps keep sounds in useful musical ranges
- **CV-controlled folding/waveshaping** creates section evolution
- the **lo-fi digital character** provides transitions, fills, and breakdown material

If you use it with:
- a structured sequencer,
- clocked modulation,
- separate processing for its two outputs,
- and clear section-based performance decisions,

then Phosgène can absolutely help you move from “cool loop” to “actual song.”

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)