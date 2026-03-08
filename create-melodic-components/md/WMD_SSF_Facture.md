# WMD SSF — Facture

- [Manual PDF](../../manuals/manual_black_fracture.pdf)

---

[Manual PDF](attachment)

# WMD Fracture — using it for melodic components

Fracture is not a traditional oscillator/VCO voice. It is a **multi-particle percussion synthesizer** built from bursts of very short samples, pseudo-random pitch assignment, filtering, stereo spread, and reverb. So its natural habitat is claps, applause, ticks, snaps, and granular percussion.

That said, as a Eurorack musician, I’d absolutely use it for **melodic support, tuned percussion, and pitch-adjacent textures** rather than only drums.

## What in the manual matters for melody

From the manual, the key features for melodic use are:

- **PITCH CV input**
  - This is the main melodic hook.
  - It “takes control of the center pitch of the particle burst” and disables the FREQ knob’s control over pitch.
- **FREQ**
  - Depending on **PUNCH** mode, this affects filter frequency and sometimes pitch.
- **PUNCH modes**
  - Mode 1: filter only
  - Mode 2: filter + pitch
  - Mode 3: filter + pitch with parallel bandpass
- **SPREAD**
  - Adds variance in pitch and panning around the center
  - For melodic work, lower settings give more pitch focus
- **SURFACE**
  - Selects among 23 transient microsample families
  - Some surfaces will read as much more “pitched” than others
- **DECAY / TAIL**
  - Shape whether the result is a tight, struck note, a looser cloud, or a decaying applause-like texture
- **DENSITY**
  - Controls how many particles attempt to occur
  - Lower density tends to sound more pointillistic and articulate
  - Higher density becomes more cloud-like/noisy
- **TRIG / TICK / ACC**
  - TRIG starts a burst
  - TICK fires a single particle on a rising edge
  - ACC changes the burst to louder/longer/accented if high during TRIG
- **Stereo outs**
  - Helpful for widening melodic layers or creating animated stereo ornamentation
- **INF mode**
  - Lets you sustain a particle cloud instead of a normal decaying burst

## The big idea: Fracture as a “pitched transient voice”

Fracture can make melodic material when you stop thinking of it as a clap and start thinking of it as:

- a **tuned granular percussion source**
- a **struck microsample voice**
- a **stereo ornament generator**
- a **pitched noise/chime layer**

It will not behave like a stable sine/triangle oscillator. Instead, it gives you notes with:
- an unstable or clustered pitch center
- transient-rich attack
- pseudo-random variation
- strong spectral character

That makes it especially useful for:

- melodic percussion
- glitch melodies
- arpeggiated accents
- top-line texture
- tuned fills
- stereo counter-melody
- generative melodic clouds

---

## Best controls for tuning Fracture melodically

## 1. Use PITCH CV as the note source
Send sequencer CV, quantized random CV, or keyboard CV into **PITCH**.

Why:
- The manual states this input takes over center pitch.
- This gives the clearest pitch relationship to your patch.

Best practice:
- Use a **quantizer** before PITCH if you want recognizable scales.
- Use a precision adder for transposition.

## 2. Keep SPREAD low for clearer note identity
SPREAD increases pitch variance from the center.

For melody:
- **Low SPREAD** = more focused pitch
- **High SPREAD** = cluster/chord-ish/noise-ish smear

A very small amount of SPREAD can be beautiful because it gives a chorus/ensemble effect without destroying note center.

## 3. Choose surfaces that read as pitched
Because SURFACE chooses different transient microsamples, some will feel:

- woody and clicky
- noisy and clap-like
- snappy and broad-spectrum
- object-like and resonant

For melody, favor surfaces that seem to have:
- a short resonant body
- less broadband noise
- more distinct “tap,” “stick,” or “object” tone

You’ll have to audition by ear, but typically:
- stick-like
- ball-like
- toggle-like
- tighter microsamples

…will often pitch-track more convincingly than pure clap/noise textures.

## 4. Use PUNCH mode carefully
PUNCH changes how FREQ affects the sound.

For melodic work:
- **Mode 1** is useful if you want pitch from PITCH CV only, and FREQ only as timbral shaping.
- **Mode 2** is useful if you want FREQ to co-shape tone and pitch.
- **Mode 3** is good when you want more aggressive, resonant, cutting melodic transients.

If you need stable note relationships:
- patch your melody to **PITCH**
- use **PUNCH mode 1**
- use **FREQ** as spectral emphasis

That gives the cleanest division between note and timbre.

## 5. Use TICK for plucked melodic points
The manual says **TICK** plays a single particle sample on the rising edge.

This is extremely useful for melody:
- one trigger = one tiny struck event
- less clouding than a full TRIG burst
- more “Mallet / pluck / glitch note” behavior

If you want Fracture to behave like a strange melodic percussion synth, **TICK is often the best entry point**.

## 6. Use TRIG for fuller notes
TRIG creates a burst, so it sounds more like:
- clap note
- fluttering strike
- granular flam
- mini-cloud

For melody, this works well when:
- DECAY is moderate
- DENSITY is not too high
- SPREAD stays low
- surfaces are chosen for resonance rather than noise

## 7. Shape note articulation with DECAY and TAIL
These determine how each note decays.

Useful melodic interpretations:

- **Short DECAY + TAIL mode 1**
  - tight struck notes
  - best for rhythmic sequences
- **Medium DECAY + TAIL mode 2**
  - more natural tails
  - nice for melodic ostinatos
- **Longer DECAY + TAIL mode 3**
  - drifting, probabilistic decay
  - ideal for ambient melodic particles

If you want “pitched applause” or “tuned granular shower,” use longer decays and probability-based tails.

---

## Musical patch approaches

## 1. Tuned percussion line
This is the most direct melodic use.

Patch:
- Sequencer CV → Quantizer → **PITCH**
- Trigger sequencer → **TICK**
- Audio out L/R → mixer

Settings:
- Low to medium **DENSITY**
- Low **SPREAD**
- Short **DECAY**
- **PUNCH mode 1 or 2**
- Adjust **FREQ** for brightness/resonance
- Moderate or low **REVERB**

Result:
- glockenspiel-like glitches
- tuned wood/click percussion
- microsampled marimba-ish line
- IDM melodic percussion

## 2. Burst-note melody
Use full TRIG instead of TICK.

Patch:
- Sequencer CV → Quantizer → **PITCH**
- Gate/trigger sequencer → **TRIG**
- Accent pattern → **ACC/TICK high during TRIG**

Settings:
- Medium **DECAY**
- Medium **DENSITY**
- Low **SPREAD**
- TAIL mode 2

Result:
- each note becomes a little burst or flam
- good for animated lead fragments
- especially good in broken beat, electro, or experimental pop

## 3. Stereo counter-melody
Exploit the stereo panning and spread.

Patch:
- Slow sequencer or random quantized CV → **PITCH**
- Sparse triggers → **TRIG**
- Stereo outs to left/right mixer channels

Settings:
- Medium **SPREAD**
- Longer **DECAY**
- Moderate **REVERB**
- TAIL mode 2 or 3

Result:
- drifting stereo melodic dust
- a secondary melodic layer behind the main voice
- excellent for ambient, kosmische, and soundtrack work

## 4. Chord illusion / cluster harmony
Fracture won’t make true chords in the normal subtractive sense, but SPREAD gives a convincing cluster around a pitch center.

Patch:
- Quantized root-note CV → **PITCH**
- Trigger pattern → **TRIG**

Settings:
- Medium **SPREAD**
- Medium/high **DENSITY**
- Medium **DECAY**
- TAIL mode 3
- Hall reverb

Result:
- each note becomes a little harmonic cloud
- suggests suspended chords or upper extensions
- good for intro pads made of particles

## 5. Arpeggio ornament layer
Use Fracture over another melodic voice.

Patch:
- Mult your melodic sequencer CV:
  - one copy to your main oscillator voice
  - one copy to Fracture **PITCH**
- Send a faster rhythmic subdivision to **TICK**
- Optionally send accents to **ACC**

Settings:
- Short **DECAY**
- Lower **DENSITY**
- Low **SPREAD**
- Bright **FREQ**
- Light room reverb

Result:
- your main melody gets a sparkling top layer
- Fracture behaves like note dust, grace notes, or a pseudo-arpeggiator

## 6. Generative melodic cloud with INF mode
The manual notes INF disables the decay envelope and freely produces particles, with trigger/button modulating density to suggest a burst inside an infinite cloud.

Patch:
- Slow random quantized CV → **PITCH**
- Slow modulation → **FREQ**
- Occasional triggers → **TRIG**
- Optional slow CV to **SURFACE** if available from external modulation source through attenuator

Settings:
- **INF on**
- Low/medium **DECAY** to control the parameter that would have been enveloped
- TAIL mode 2 or 3
- Moderate **SPREAD**
- Reverb up

Result:
- sustained tuned particle atmosphere
- shimmering semi-melodic pad
- evolving bell-fog texture

---

## How I would combine Fracture with typical Eurorack modules for melody

Since Fracture is a texture-forward voice, it really shines when paired with standard utility and pitch modules.

## With a quantizer
Essential for tonal music.

Use:
- random CV → quantizer → PITCH
- sequencer CV → quantizer → PITCH

Why:
- Fracture’s internal randomness benefits from a stable pitch center
- quantization makes the melody legible

## With a precision adder
Great for:
- octave jumps
- transposition
- harmonic movement

Use:
- melodic CV to PITCH
- transposition CV through precision adder upstream

## With a sequencer
Three good strategies:
1. Step CV to PITCH, triggers to TICK for clean note events
2. Step CV to PITCH, triggers to TRIG for denser note bodies
3. Independent trigger sequencing for polyrhythmic melodic percussion

## With envelopes and VCAs downstream
Even though Fracture has internal dynamics, external shaping helps.

Use:
- Fracture output → VCA or LPG → effects/mixer
- envelope triggered from same gate source

Why:
- lets you tighten or exaggerate note contour
- allows sidechain-like dynamics
- makes Fracture sit like a melodic instrument in a mix

## With filters
A great pairing.

Use:
- Fracture output → resonant LPF/BPF

Why:
- can emphasize a clearer fundamental-like region
- can remove noisy highs and make notes sound more tonal
- can turn harsh clatter into tuned mallet-like signals

## With delay/reverb
Especially effective because Fracture is transient-rich.

Use:
- stereo delay after Fracture
- ping-pong delay for melodic repeats
- shimmer or hall reverb for ambient tuned particles

## With a comparator / clock logic
To create melodic accents:
- main triggers to TRIG
- selected logic-derived pulses to ACC

This can make certain notes bloom into bigger “accented melodic hits.”

---

## Good melodic roles in a track

Fracture works best in these melodic roles:

### 1. Top percussion melody
Short, high, tuned, articulate notes above the main synths.

### 2. Counter-line
Sparse notes answering a lead or vocal.

### 3. Harmonic glitter
Quantized pitch fed into long-decay bursts with reverb.

### 4. Intro/outro atmosphere
INF mode plus slow pitch shifts creates evolving tonal particles.

### 5. Layer with another voice
Use it to add attack complexity to a pluck, chord stab, or bassline.

A particularly strong trick:
- pair Fracture with a sine or triangle voice on the same sequence
- tune Fracture by ear to reinforce upper partials
- keep its level lower than the main voice

That gives a hybrid sound: stable pitch from the main oscillator, expressive attack from Fracture.

---

## Practical melodic settings to try

## Patch A: “Glitch Marimba”
- PITCH: quantized melody
- Trigger source: TICK
- SURFACE: woody/object-like
- SPREAD: very low
- DECAY: short
- DENSITY: low
- PUNCH: mode 1
- FREQ: tuned for resonant brightness
- REVERB: low

## Patch B: “Granular Lead Accent”
- PITCH: same sequence as main lead
- Trigger source: TRIG on selected steps
- ACC: accents on downbeats
- SPREAD: low
- DECAY: medium
- DENSITY: medium
- TAIL: mode 2
- PUNCH: mode 2
- REVERB: moderate

## Patch C: “Ambient Bell Cloud”
- PITCH: slow random quantized CV
- Trigger source: sparse TRIG
- SPREAD: medium
- DECAY: long
- DENSITY: medium
- TAIL: mode 3
- PUNCH: mode 3
- REVERB: hall/high
- stereo out used fully

## Patch D: “Pseudo Chords”
- PITCH: root notes only
- Trigger source: TRIG
- SPREAD: medium-high
- DECAY: medium-long
- DENSITY: medium-high
- TAIL: mode 3
- REVERB: moderate-high

This won’t create exact triads, but it will imply harmony through clustered resonant particles.

---

## Limitations for melodic use

To be realistic, the manual suggests Fracture is still fundamentally a **particle percussion** module. So:

- It likely won’t track pitch as cleanly as a dedicated VCO.
- Timbre may dominate over note identity depending on SURFACE.
- High DENSITY and high SPREAD reduce melodic clarity.
- Randomized per-particle pitch/amplitude/pan means repetition is intentionally imperfect.

So if your goal is:
- exact basslines
- stable leads
- calibrated 1V/oct behavior across many octaves

…Fracture is probably not the primary voice.

But if your goal is:
- expressive tuned percussion
- melodic textures
- sparkling sequence layers
- stereo note clouds
- humanized, lively pitch material

…it is excellent.

---

## Best overall recipe for getting melody from Fracture

If you want the shortest path to a usable melodic result:

1. Send **quantized CV** into **PITCH**
2. Use **TICK** instead of TRIG at first
3. Keep **SPREAD low**
4. Keep **DENSITY low to medium**
5. Pick a more resonant/woody **SURFACE**
6. Use **PUNCH mode 1**
7. Use **FREQ** to find the sweet spot
8. Add a little reverb
9. Optionally filter the output further

That gives the clearest “pitched percussion instrument” behavior.

If you want, I can also turn this into:
- a **quick-start patch sheet**
- **techno / ambient / IDM-specific patch recipes**
- or a **control-by-control cheat sheet** for Fracture.  

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)