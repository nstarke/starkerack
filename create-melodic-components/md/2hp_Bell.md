# 2hp — Bell

- [Manual PDF](../../manuals/2hp_Bell.pdf)

---

[Manual PDF](#)

# Bell — using it to create melodic parts in a Eurorack patch

Based on the manual, **Bell** is a **2HP modal synthesis melodic percussion voice** designed for struck, resonant, pitched sounds: bells, vibraphones, marimbas, bowls, glass, and plate-like tones.

## What the module does musically

Bell is essentially a compact **pitched voice** for:

- melodic percussion lines
- tuned hits and plucks
- chord-like layered strikes via polyphony
- metallic ambient textures
- physically inspired mallet sounds

Its sound engine uses **modal synthesis**, so instead of a typical subtractive oscillator/filter path, it generates the resonant behavior of struck objects. That makes it especially good for:

- **glockenspiel-style melodies**
- **vibraphone ostinatos**
- **marimba riffs**
- **bell arpeggios**
- **bowl/drone accents**
- **hybrid acoustic-impossible percussion**

## Key features from the manual

- **6-voice polyphony**
- **Trigger input** to create notes
- **Pitch control**
- **1V/Oct input** for melodic control
- **Model control** with CV
- **Damp control** with CV
- **Audio output: 10Vpp**
- **8 physical models**:
  1. Pure Bell
  2. Pure Vibraphone
  3. Harmonic Vibraphone
  4. Hard Marimba
  5. Soft Marimba
  6. Tibetan Bowl
  7. Wine Glass
  8. Redwood Plate

---

## How Bell works in a melodic system

To make Bell perform as a melodic instrument, you mainly need three things:

1. **A trigger source**
2. **A pitch CV source**
3. **A way to shape timbre over time**

### 1. Trigger input = note articulation

The **Trig** input causes a new note to sound using the current knob/CV state.

Use this with:

- trigger sequencers
- gate-to-trigger sources
- clock dividers/multipliers
- Euclidean rhythm generators
- manual gate buttons
- logic-based rhythmic patterns

Because Bell is a struck voice, each trigger acts like a mallet hit.

### 2. V/Oct input = melody

The **V/Oct** input accepts **-1V to 6V**, so you can drive Bell from:

- a CV sequencer
- a keyboard controller
- a quantizer
- a precision adder
- a sample & hold into a quantizer

This is the main input for writing actual melodies.

### 3. Pitch knob = base tuning and expressive movement

The **Pitch** knob sets the fundamental frequency, but the manual also notes something musically important:

> The pitch control remains active for the most recently generated note.

That means while a note is ringing, moving Pitch can create:

- **vibrato**
- **pitch bends**
- **slewed transitions**
- **live retuning**
- **expressive struck-metal gestures**

That’s a nice performance feature, especially for bowl and glass models.

---

# How to patch Bell for melodic components

## Patch 1: Basic tuned melodic percussion line

**Goal:** marimba or vibraphone melody

**Patch:**
- Sequencer trigger out → **Trig**
- Sequencer pitch CV / quantizer out → **V/Oct**
- **Out** → VCA, LPG, mixer, or directly to output chain
- Set **Model** to:
  - Pure Vibraphone
  - Harmonic Vibraphone
  - Hard Marimba
  - Soft Marimba

**Musical result:**
- clean, tuned mallet melodies
- excellent for ostinatos, hooks, and counter-melodies

**Tips:**
- Use **Hard Marimba** for more attack and rhythmic clarity
- Use **Soft Marimba** for gentler melodic support
- Use **Harmonic Vibraphone** for more shimmer in sparse arrangements

---

## Patch 2: Bell arpeggios

**Goal:** chiming bell sequence

**Patch:**
- Arpeggiator or stepped CV source → **V/Oct**
- Clocked trigger stream → **Trig**
- Set **Model** to **Pure Bell**
- Set **Damp** low-to-medium for long ringing decay

**Musical result:**
- glassy and metallic melodic figures
- excellent for ambient, techno, soundtrack, and minimal patches

**Extra move:**
- Modulate **Model CV** slowly with an LFO or sequenced CV to morph between bell-like and bowl-like materials.

---

## Patch 3: Animated tuned percussion

**Goal:** keep the melody the same, but change tone over time

**Patch:**
- Quantized sequence → **V/Oct**
- Trigger pattern → **Trig**
- Slow bipolar LFO or sequencer lane → **Model**
- Envelope, random CV, or slow modulation → **Damp**

**Why this works:**
- **Model** changes the resonant object itself
- **Damp** changes resonance/decay and the apparent hardness/softness of the struck body

**Musical result:**
- one melodic line that feels “performed” rather than static
- timbral evolution across phrases
- pseudo-acoustic variation

Because both **Model** and **Damp** accept **bipolar CV (-5V to 5V)** added to the knob positions, they work well with centered modulation sources.

---

## Patch 4: Polyphonic overlapping phrases

**Goal:** create layered melodic textures

Bell offers **6-voice polyphony**, meaning multiple struck notes can overlap naturally before the oldest one is stolen.

**Patch:**
- Fast or medium trigger pattern → **Trig**
- Quantized melodic sequence → **V/Oct**
- Set **Damp** lower for longer decays
- Use **Tibetan Bowl**, **Wine Glass**, or **Pure Bell**

**Musical result:**
- overlapping notes build implied harmony
- works beautifully for:
  - broken chords
  - generative ambient lines
  - shimmering bell clouds
  - gamelan-like textures

This is one of Bell’s strongest uses. Even with a monophonic CV line, the polyphony lets previous notes keep ringing while new notes enter, creating a naturally layered melodic field.

---

## Patch 5: Bowls, drones, and melodic ambience

**Goal:** less “percussion,” more sustained tonal atmosphere

**Patch:**
- Sparse triggers → **Trig**
- Slow quantized CV or manually tuned voltage → **V/Oct**
- Model = **Tibetan Bowl** or **Wine Glass**
- Lower damping for longer resonances
- Add external reverb/delay after **Out**

**Musical result:**
- resonant tuned drones
- meditative tonal strikes
- cinematic punctuation notes

This is especially effective if you trigger only a few notes per bar and let the resonance fill space.

---

## Patch 6: Expressive lead percussion

**Goal:** use Bell almost like a lead voice

Because the **Pitch** knob affects the **most recently generated note while it rings**, Bell can be played expressively.

**Patch:**
- Keyboard or sequencer CV → **V/Oct**
- Gate/trigger → **Trig**
- Perform with the **Pitch** knob by hand
- Optionally route the output through delay/reverb

**Musical result:**
- subtle bends
- hand-played vibrato
- expressive tuned metallic solos

This is especially compelling with:
- Wine Glass
- Tibetan Bowl
- Pure Bell

---

# Understanding the controls musically

## Model

This chooses the resonator/excitor type. Think of it as selecting the “instrument family” or “material.”

### Best uses by model

- **Pure Bell**  
  Bright melodic chimes, lead bells, arpeggios

- **Pure Vibraphone**  
  Jazz-like tuned percussion lines, clean melodic support

- **Harmonic Vibraphone**  
  More overtone-rich melodic parts, lush arps

- **Hard Marimba**  
  Strong attack, great for rhythmic riffs and sequence definition

- **Soft Marimba**  
  Mellow repetitive patterns, understated melody

- **Tibetan Bowl**  
  Long resonances, meditative melodies, drone accents

- **Wine Glass**  
  Fragile, eerie, crystalline melodic textures

- **Redwood Plate**  
  More unusual, experimental struck timbres; good for hybrid percussion melodies

## Damp

The manual describes Damp as changing the resonance of the excitor filters and affecting overall decay time.

In practice, this means:

- **higher damping** = shorter, tighter, more percussive notes
- **lower damping** = longer ringing, more sustained and atmospheric notes

### Musical uses of Damp

- For **fast melodic passages**: increase damping so notes stay clear
- For **ambient or chordal overlap**: reduce damping so notes ring into each other
- For **dynamic arrangement changes**: modulate damping during a section to move from dry marimba to blooming bell cloud

---

# Best partner modules for Bell

Since you asked how modules can be used together, here’s what Bell most benefits from alongside other Eurorack utilities and voices.

## 1. Sequencer + quantizer

Use with Bell for:

- melodies
- arpeggios
- tuned percussion riffs
- transposed patterns

Ideal partners:
- CV sequencer
- quantizer
- precision adder
- keyboard controller

## 2. Trigger sequencer / clock tools

Bell needs distinct note events. Pairing it with rhythmic modules gives:

- syncopated struck melodies
- Euclidean bell lines
- polyrhythmic mallet parts
- generative melodic percussion

Ideal partners:
- trigger sequencer
- clock divider
- logic
- burst generator

## 3. Modulation sources

Model and Damp are both good CV destinations.

Use:
- LFOs
- random stepped voltages
- envelopes
- sequencer modulation lanes

This adds:
- timbral phrase movement
- variation between strikes
- evolving material/decay changes

## 4. Effects

Bell really opens up with effects.

Best choices:
- **reverb** for bowls, bells, glass
- **delay** for arpeggios and melodic echoes
- **chorus** for vibraphone-like lushness
- **filter** for softening top end
- **wavefolder/distortion** for aggressive metallic percussion

## 5. VCA / LPG / mixer

Even though Bell is already percussive, external level control helps in a full patch.

Use these for:
- balancing Bell with other voices
- ducking under drums or bass
- adding extra articulation with a VCA
- warming transients with an LPG

---

# Arrangement roles Bell can fill

Bell can serve several melodic roles in a track:

## Primary melody
Use:
- Pure Bell
- Vibraphone
- Wine Glass

Great for sparse arrangements and melodic techno hooks.

## Countermelody
Use:
- Soft Marimba
- Harmonic Vibraphone

Works behind a lead oscillator or vocal-like synth line.

## Chord illusion / harmonic wash
Use:
- Tibetan Bowl
- Pure Bell
- Wine Glass
with long decay and overlapping triggers.

## Rhythmic melodic ostinato
Use:
- Hard Marimba
- Pure Vibraphone
with short damping and a clocked trigger pattern.

## Textural punctuation
Use:
- Redwood Plate
- Tibetan Bowl
for occasional accent notes in ambient or experimental music.

---

# Practical patch recipes

## A. Minimal techno bell hook
- 16-step sequencer CV → **V/Oct**
- Sparse trigger pattern → **Trig**
- Model = **Pure Bell**
- Damp = medium
- Output → delay + reverb

Result: a bright repeating motif over kick and bass.

## B. Ambient bowl constellation
- Random stepped CV → quantizer → **V/Oct**
- Slow irregular triggers → **Trig**
- Model = **Tibetan Bowl**
- Damp = low
- Output → huge reverb

Result: floating tuned metallic events.

## C. Marimba polyrhythm
- Polyrhythmic trigger source → **Trig**
- Quantized repeating sequence → **V/Oct**
- Model = **Hard Marimba**
- Damp = higher

Result: tight percussive melody with strong attack definition.

## D. Generative glass melody
- Sample & hold → quantizer → **V/Oct**
- Clock divider output → **Trig**
- Slow bipolar LFO → **Model**
- Random CV attenuated → **Damp**
- Model centered near **Wine Glass**

Result: shifting crystalline melodic phrases.

---

# Important operational notes from the manual

- **Trigger creates notes using current knob/CV state**
- **6 voices maximum**; oldest note is stolen when a new one arrives
- **Model and Damp CV are bipolar**, with **-5V to 5V** input range
- **V/Oct input range is -1V to 6V**
- **Output is 10Vpp**
- LED lights for 30 ms when a sound is triggered

That means in practice:
- attenuate modulation if model jumping becomes too abrupt
- use a quantized pitch source for tonal music
- be aware that fast dense patterns may cause voice stealing if decay is long

---

# Overall musical assessment

**Bell** is best thought of as a **compact melodic percussion voice with strong expressive potential**. It is especially useful when you want:

- a full melodic voice in very little HP
- non-standard oscillator timbres
- struck, resonant acoustic-style tones
- overlapping tuned metallic notes
- a voice that can do both tonal rhythm and ambient melody

Its biggest strengths for melodic music are:

1. **true pitch control via V/Oct**
2. **6-voice overlap for naturally layered phrases**
3. **multiple resonant physical models**
4. **Damp control for articulation and decay shaping**
5. **very small footprint**

If you want, I can also turn this into:
- a **clean patch sheet**
- a **beginner-friendly quick-start guide**
- or a **“best musical uses by genre” summary**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)