# Qu-Bit — Cascade

- [Manual PDF](../../manuals/Getting_Started_Cascade.pdf)

---

[Manual PDF / Product Page](https://www.qubitelectronix.com/shop/cascade)

# Qubit Cascade: using it to create melodic components

Cascade is only one module in the attached manual, but it can absolutely become a **melodic utility voice** when combined with the rest of a Eurorack system. From the manual, it is:

- a **ratcheting envelope generator**
- an **analog VCA**
- a **sound source**
- an **envelope follower**
- a **compressor / virtual sidechain**

That means it can contribute to melody in three main ways:

1. **shape notes** with envelopes and VCA control  
2. **generate pitched material** using its internal sine source  
3. **create rhythmic articulation** that makes melodic lines feel alive

---

## What Cascade contributes to melodic patching

From the manual, the key melody-relevant features are:

- **Internal sound sources**:
  - White Noise
  - Hi-Hat
  - Kick
  - **HiFreq Sine**
- **Envelope out**
- **VCA out**
- **Gate out**
- **Trigger input**
- **VCA CV input** that can override the normal envelope-to-VCA path
- Modes:
  - Ratcheting AD
  - AD
  - ASR
  - ADSR
  - Envelope Follower
  - Compressor

Even though Cascade is not a full oscillator with 1V/oct tracking, it can still be used melodically in a few practical ways.

---

# 1. Use Cascade as the articulation engine for a melodic voice

This is the most obvious and most powerful role.

## Patch concept
Use another module as the **pitched oscillator** and let Cascade handle:

- note contour
- note length
- dynamic phrasing
- ratchets
- gate logic

## Basic patch
- Sequencer pitch CV → oscillator 1V/oct
- Sequencer gate → Cascade **trigger**
- Oscillator audio → Cascade **VCA in**
- Cascade **VCA out** → mixer / filter / effects

Now Cascade becomes the envelope/VCA voice controller.

## Best melodic modes

### AD mode
Good for:
- plucks
- basslines
- marimba-like sequences
- short synth notes

Use:
- short attack
- short/medium decay
- exponential curve for punch
- level to set modulation depth / loudness
- offset if you want the envelope to sit above 0V

### ADSR mode
Good for:
- lead lines
- sustained melodies
- keyboard-style phrasing

Use:
- attack for softness
- decay and sustain for body
- release for tail
- gate length from your sequencer determines note hold behavior

### ASR mode
Good for:
- simple sustained lines
- drone melodies
- legato-ish phrase shapes

The manual notes that the **gate length sets sustain**, so this works well with sequencers outputting variable gate lengths.

---

# 2. Create melodic rhythm with ratcheting AD

This is where Cascade gets special.

In **Ratcheting AD**, the repeats control acts as:
- repeat count
- clock multiplier:
  - 1x, 2x, 3x, 4x, 6x, 8x, 12x, 16x

## Why this matters melodically
Even if pitch is static, repeated sub-triggers create:
- trills
- mandolin-like note reiteration
- Berlin-school pulse animation
- fast ornamentation
- pseudo-arpeggiation when paired with pitch changes

## Patch
- Pitch sequencer → oscillator 1V/oct
- Main rhythm gate → Cascade **trigger**
- Oscillator → Cascade **VCA in**
- Cascade **VCA out** → mixer
- Set mode to **Ratcheting AD**

Now one incoming note can become a burst of repeated note articulations.

## Good musical uses
- ratcheting acid bass
- repeated lead note accents
- trap-style fast subdivisions
- Euclidean melody embellishments
- probabilistic melody flourishes when fed irregular gates

## Performance trick
Keep the pitch sequence relatively sparse, then manually move:
- **repeats**
- **attack**
- **decay**
- **curve**

This can turn a simple 8-step melody into something highly expressive.

---

# 3. Use the internal HiFreq Sine as a melodic element

The manual lists **HiFreq Sine** as one of the internal sound sources, normalled to the VCA output when nothing is patched into **VCA in**.

So if no external audio is connected:
- choose **HiFreq Sine**
- trigger Cascade
- take audio from **VCA out**

## Result
You get a built-in struck or gated sine-based voice.

## Best uses
Because the manual does not indicate pitch CV tracking for this internal sine, think of it less as a traditional tuned oscillator and more as:
- a fixed-pitch percussion tone
- a tonal ping
- a high-register melodic accent
- a layer for motifs

## Musical applications
- tuned ostinato accent
- sine blips over a bassline
- minimal melodic pulses
- bell-like transients when using short AD settings

## Patch idea
- Clock / trigger pattern → Cascade **trigger**
- Select **HiFreq Sine**
- Cascade **VCA out** → delay / reverb
- Use **AD** or **Ratcheting AD**

This can create a musically pitched top layer, especially in ambient, IDM, or minimal techno contexts.

---

# 4. Use Envelope Out to shape melodic timbre elsewhere

Cascade’s **Envelope Output** is not only for internal VCA duties. It can animate melodic timbre across your system.

## Typical melodic destinations
Patch **Env out** to:
- filter cutoff
- wavefolder CV
- FM amount
- oscillator shape
- LPG CV
- effect parameter CV

Meanwhile:
- audio still goes through Cascade’s VCA, or not
- same trigger drives both amplitude and timbre movement

## Why this is musical
Melody is not only pitch; it is also:
- brightness
- attack character
- accent strength
- contour

Cascade can create note-by-note timbral phrases.

## Patch example: expressive mono lead
- Sequencer pitch CV → VCO 1V/oct
- Sequencer gate → Cascade **trigger**
- VCO audio → Cascade **VCA in**
- Cascade **VCA out** → filter → mixer
- Cascade **Env out** → filter cutoff CV

Now every note gets synchronized amplitude + filter articulation.

## Better still
Use:
- **ADSR** for synth-lead behavior
- **AD** for plucks
- **invert** if you want the opposite motion, like darker attacks opening into duller sustain or ducking effects

---

# 5. Use VCA CV input for external melodic control

The manual says **VCA CV** overrides Env Out for direct control over the VCA.

That means Cascade can act as a clean analog VCA for whatever melodic CV source you want.

## Why useful
You can use a different modulation source for melodic amplitude, such as:
- another envelope
- LFO
- random voltage
- sequenced CV
- quantized stepped CV

## Melodic applications
- velocity-style accent patterns
- tremolo on sustained notes
- step-based amplitude melodies
- cross-rhythmic volume animation

## Example
- Pitched oscillator → Cascade **VCA in**
- Slow sequenced CV or modulation source → **VCA CV**
- Cascade **VCA out** → mixer

Now amplitude itself becomes a compositional parameter, separate from note pitch.

---

# 6. Use Gate Out as a melodic timing generator

Cascade’s **Gate Output** can be configured in Edit Functions. From the manual:

Gate modes:
- **6ms trigger at start of every envelope**
- **EOD**: gate high when envelope is not in decay stage
- **EOA**: gate high when envelope is not in attack stage

This is extremely useful for melodic patching.

## Practical uses

### A. Trigger a second voice in sync
Use Gate Out to trigger:
- another envelope
- another sequencer advance
- a percussive accent voice
- a sample & hold for melodic variation

This lets Cascade become the timing brain for layered melodies.

### B. Create delayed or phase-shifted melodic events
EOA / EOD logic can offset events relative to the contour of the envelope.

Example:
- Main trigger starts note 1
- Gate out triggers note ornament after attack or after decay phase

That can generate:
- grace-note effects
- call-and-response accents
- filter pings after note onset
- companion voice motion

### C. Advance a pitch source during ratchets
If Gate Out emits triggers with each envelope event, you can patch it into another module that steps a sequencer or sample-and-hold. This can make one incoming note blossom into a melodic subdivision structure.

---

# 7. Use repeats/looping as a melodic modulation source

In AD and ASR, the manual says repeats can go from:
- **1 to 16**
- **infinite looping at knob end**

This means Cascade can become a **cycling contour generator**.

## Melodic uses of looping envelope
Patch **Env out** to:
- oscillator FM
- wavefolder
- filter cutoff
- VCA CV of another voice

This creates repeating contour-based motion that can read as melody-adjacent phrasing, especially when the contour is synced to triggers.

## Patch idea: pseudo-sequence from timbre
- Drone oscillator at one pitch
- Cascade in looping AD
- Env out → filter cutoff and FM attenuator
- VCA out controls amplitude or a second layer

Result: even with static pitch, the ear hears evolving “melodic” motion through harmonics and dynamics.

---

# 8. Gravity modes for decaying melodic ratchets

The edit page shows three **Gravity Modes**:
- No Gravity
- Amplitude Gravity
- Amplitude and Time Gravity

This is great for musicality.

## What it implies
As repeats happen:
- they may get quieter
- and possibly faster/slower in a bouncy-ball style

## Melodic benefit
This creates natural-feeling note reiteration:
- like drumstick bounce
- string retrigger decay
- flam into tremolo
- diminishing trill

## Strong use cases
- ornamented melodic lines
- “bouncing ball” plucks
- decaying repeated accents over arpeggios
- humanized repetition

With a quantized oscillator pitch, these ratchets feel like intentional melodic decorations rather than rigid machine-gun retriggers.

---

# 9. Envelope Follower mode for melody extracted from audio

Cascade’s **Envelope Follower** mode takes audio input and derives an envelope from it. The gate goes high when the signal exceeds threshold.

## Melodic uses
This is not direct pitch extraction, but it is excellent for:
- deriving articulation from another melodic source
- making one voice control another voice’s dynamics
- synchronized melodic modulation

## Patch idea: mirror articulation
- External melodic synth line/audio → Cascade **VCA in**
- Cascade in **Envelope Follower**
- **Env out** → filter CV on another oscillator voice
- **Gate out** → trigger another envelope or sequencer

Now one melodic line can animate another.

## Example result
A vocal sample, lead synth, or plucked sequence can impose its phrasing onto:
- a drone
- a bassline
- another oscillator tuned a fifth above

That creates melodic coupling between voices.

---

# 10. Compressor mode for pumping melodic voices

The compressor may seem less “melodic,” but in modern patching it definitely is.

From the manual:
- audio input is compressed
- trigger can inject a **virtual sound source** into the compressor
- gate out goes high when compression is engaged

## Melodic applications

### A. Sidechain a pad or lead
- Melodic pad audio → Cascade **VCA in**
- Trigger pattern → Cascade **trigger**
- Compressor mode engaged
- VCA out → mixer

Now the pad or sustained melody ducks rhythmically, creating groove.

### B. Use pumping as melodic emphasis
A bass melody can breathe around a rhythmic trigger pattern, making the phrase feel more musical.

### C. Gate Out as a compression activity signal
Use Gate Out to trigger another event whenever the compressor engages:
- accent oscillator
- transients
- secondary melody voice

This turns dynamics processing into compositional timing.

---

# 11. Build melodic voices from Cascade plus common companion modules

Since your prompt asks how modules can be used together, here are practical pairings.

## A. Cascade + sequencer + oscillator
Best for:
- classic lead/bass voice

Patch:
- Sequencer pitch → oscillator
- Sequencer gate → Cascade trigger
- Oscillator → Cascade VCA in
- Cascade VCA out → mixer/filter

Cascade provides articulation and ratchets.

---

## B. Cascade + quantizer + random source
Best for:
- generative melodies

Patch:
- Random stepped CV → quantizer → oscillator pitch
- Clock or burst trigger → Cascade trigger
- Oscillator → Cascade VCA in
- Cascade Env or Gate out → influence random sampling or sequence advance

Why it works:
Cascade turns random pitches into phrased notes instead of static CV wandering.

---

## C. Cascade + filter
Best for:
- expressive melodic patches

Patch:
- Oscillator → Cascade VCA in → filter → mixer
- Cascade Env out → filter cutoff

This is the classic subtractive voice, but ratcheting and gravity modes make it more animated than a standard envelope.

---

## D. Cascade + delay/reverb
Best for:
- ambient melody
- pointillistic motifs

Patch:
- Internal HiFreq Sine or external oscillator → Cascade VCA
- Use short AD or ratchets
- Send VCA out to delay/reverb

This creates sparse but memorable melodic figures.

---

## E. Cascade + second envelope / second VCA
Best for:
- layered melodic articulation

Use Cascade’s Gate Out to trigger a second contour on another voice or harmonic layer.

Example:
- Main melody through Cascade
- Gate Out triggers a second voice one octave above
- Ratchets become harmonized ornaments

---

# 12. Specific melodic patch recipes

## Patch 1: Ratcheting acid melody
- Pitch sequencer → VCO 1V/oct
- Gate sequencer → Cascade trigger
- VCO saw/square → Cascade VCA in
- Cascade VCA out → filter → mixer
- Cascade Env out → filter cutoff
- Mode: Ratcheting AD
- Short attack, short decay, 2x–8x repeats

Result:
A melody with repeating accents and animated filter plucks.

---

## Patch 2: Minimal sine motif
- No cable in VCA in
- Select **HiFreq Sine**
- Trigger pattern → Cascade trigger
- Cascade VCA out → delay/reverb
- Mode: AD or Ratcheting AD

Result:
Tonal pings that function as a melodic top line or counter-rhythm.

---

## Patch 3: Generative plucked melody
- Random CV → quantizer → oscillator pitch
- Clock divisions / Euclidean trigger → Cascade trigger
- Oscillator → Cascade VCA in
- Cascade VCA out → LPG or filter
- Cascade Env out → timbre CV
- Mode: AD
- Optional repeats set low or occasional ratchets

Result:
Organic, plucked melodic fragments.

---

## Patch 4: Call-and-response lead
- Main sequencer → oscillator pitch
- Main gate → Cascade trigger
- Oscillator → Cascade VCA in
- Cascade VCA out → mixer
- Cascade Gate out → trigger second envelope / second oscillator voice

Choose EOA or EOD gate behavior to place the second event after the main attack or during non-decay portions.

Result:
One melodic source generates a second answering phrase or accent.

---

## Patch 5: Audio-followed harmony
- Existing melodic audio → Cascade VCA in
- Mode: Envelope Follower
- Cascade Env out → VCA CV or filter on second voice
- Gate out → trigger a harmonized voice

Result:
A second melodic layer tracks the dynamics of the first.

---

## Patch 6: Pumped pad around melody
- Sustained melodic pad audio → Cascade VCA in
- Rhythmic trigger → Cascade trigger
- Mode: Compressor
- Cascade VCA out → mixer

Result:
The melody breathes rhythmically, fitting tightly around drums or sequenced accents.

---

# 13. Best musical roles for each mode

## Ratcheting AD
Best for:
- ornamented melodies
- trills
- repeated note bursts
- rhythmic lead articulation

## AD
Best for:
- plucks
- basslines
- sequenced motifs
- percussion-toned melody

## ASR
Best for:
- gate-length-controlled phrases
- simple sustained lines
- legato-ish melodic control

## ADSR
Best for:
- traditional keyboard-style melodic playing
- leads and pads
- expressive manual performance

## Envelope Follower
Best for:
- deriving melodic articulation from existing audio
- making one melodic part animate another

## Compressor
Best for:
- dynamic shaping of melodic stems
- sidechain-style groove on pads, leads, basses

---

# 14. Realistic limitations

To keep expectations accurate:

- Cascade is **not primarily a pitch voice module**
- the internal sine is useful, but the manual does **not describe 1V/oct pitch control**
- its strongest melodic role is **articulation, rhythmic subdivision, amplitude shaping, and phrase generation**

So the best way to think about it is:

> Cascade does not usually *create pitch sequences by itself*; it makes pitch sequences far more musical.

That is hugely important in Eurorack, because a plain oscillator + sequencer can sound static, while Cascade adds:
- note contour
- repeated triggers
- dynamic accents
- gate logic
- pumping
- timbral movement

---

# Conclusion

Cascade is a strong melodic support module and, in some patches, a compact melodic accent voice. Its most effective musical uses are:

- **turning external oscillators into expressive voices**
- **adding ratcheted subdivisions to melodies**
- **using envelope out for timbral phrasing**
- **using gate out to synchronize secondary melodic events**
- **using the internal HiFreq Sine for tonal blips and accents**
- **using follower/compressor modes to transfer phrasing and groove between melodic layers**

If you want, I can also turn this into:
1. a **set of concrete patch diagrams**, or  
2. a **“melodic patch cookbook”** for ambient, techno, and generative styles.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)