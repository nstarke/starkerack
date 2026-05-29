# Ohmforce — Bohm

- [Manual PDF](../../manuals/Bohm documentation.pdf)

---

[Manual PDF / Documentation](https://ohmforce.com/wp-content/uploads/2025/03/Bohm-manual.pdf)

# Ohm Force Bohm: using it for dense, hyper-complex percussion

Bohm is extremely good for this goal because it is not just a single kick module. It is really a **multi-layered percussion system**:

- **Bohm main voice** = primary kick / tuned percussion voice
- **Groove expander** = secondary clocked voice for taps, rumbles, tops, repeats, noise, sub grit
- **Performer expander** = ducking + live FX processor for the internal voices and/or external audio

That means you can treat it like a **micro-rhythm section** inside your rack, especially when you drive it with separate clocks, gates, CV modulation, and program changes.

---

# What makes Bohm especially useful for complex rhythms

From the manual, these are the key features for dense rhythmic work:

- **Main kick triggered by HIT**
- **Secondary Groove voice triggered independently by CLOCK**
- Groove creates:
  - **repetitions/taps**
  - **reverb-based rumble**
  - **noise**
  - **grit + sub**
- Groove timing behavior depends on the relationship between:
  - **HIT triggers**
  - **CLOCK triggers**
- Bohm **HIT can act as trigger or gate**
- Bohm supports **snapshots**, **programs**, **Song mode**, and **Jam mode**
- **FUNCTION trigger** can advance live sequences in Song mode
- **Pitch tracking** via 1V/oct can turn kicks into tuned percussion or bassline percussion
- **Performer** can process:
  - only kick
  - only input
  - or both
- **TAPS output** can emit rhythmic envelope data you can use elsewhere
- CV control and attenuverters on many parameters let you animate the voice constantly

So if your aim is **polyrhythm, asymmetry, metric tension, percussion density**, Bohm is actually more interesting than a plain kick drum.

---

# Best high-level strategy

Think of Bohm as a **3-layer percussion engine**:

## Layer 1 — the downbeat body
Use the **main Bohm voice** for:
- anchor kick
- odd-meter accents
- tuned tom-like strikes
- long gated bass drum drones

## Layer 2 — the interlocking subdivision engine
Use **Groove CLOCK** for:
- 16ths against quarter-note HIT
- triplets against straight pulse
- 5s or 7s against 4
- burst-like repetitions
- top-end chatter or rumble tails

## Layer 3 — glue, pump, and disruption
Use **Performer** for:
- ducked external percussion loops
- beat roll / slip roll transitions
- filtered contour shaping
- turning stable patterns into performance gestures

This three-layer approach is the core of making Bohm feel “hyper-rhythmic.”

---

# Patch concepts for polyrhythm and complex time signatures

## 1. Separate HIT and CLOCK immediately
The manual makes this very clear:

- **Bohm main voice** responds to **HIT**
- **Groove** needs **CLOCK** to do its thing

Do **not** send the same exact trigger everywhere if you want complexity.

### Patch idea
- Send your main meter pulse to **HIT**
- Send a different subdivision or clock division/multiplication to **Groove CLOCK**

### Examples
- HIT = quarter notes
- CLOCK = 16ths

This gives classic dense techno internal motion.

Or:

- HIT = every 5 steps
- CLOCK = straight 16ths

Now Groove evolves across the bar against the main kick cycle.

Or:

- HIT = pattern in 7
- CLOCK = pattern in 4 or 8

This creates polymetric drift.

---

## 2. Use Groove as a “rhythmic parasite”
Groove is strongest when it is not just a second kick, but a **subdivision organism** attached to the main voice.

Per the manual:

- When **HIT** is triggered, Groove’s envelope is retriggered
- The following **CLOCK** triggers define the path toward taps **2, 3, 4**
- After that it either:
  - **falls back to 0**
  - or **sustains** depending on **GRV ENV**

That means Groove is ideal for **interior rhythmic articulation** between main accents.

### Great use:
- Main kick on structural pulses
- Groove CLOCK running faster or at a different grouping
- Tap knobs 2/3/4 set to uneven levels

This gives “phrases inside the beat.”

For example:
- HIT on beat 1 of each bar in 7/8
- CLOCK on all 8ths
- Tap 2 low, tap 3 high, tap 4 medium

Now every time the bar resets, the internal contour restarts, creating a repeated but asymmetrical shape.

---

## 3. Exploit triplets and mixed subdivisions
The manual explicitly mentions Groove works well with **triplets**, where taps 2 and 3 become especially relevant.

### Patch ideas
- Main meter straight 4
- Groove CLOCK = quarter-note triplets
- Or main pattern in 12, Groove in 16
- Or switch between straight and triplet clocks with a sequential switch

Use Groove for:
- **repetition source** when you want articulated repeats
- **noise/grit** when you want high-frequency chatter over the kick grid

This is one of the easiest ways to make Bohm sound “advanced” rather than simply techno.

---

## 4. Use odd clock divisions for Groove
If you have clock tools, try:

- CLOCK every **3 pulses**
- every **5 pulses**
- every **7 pulses**
- Euclidean bursts
- logic-derived triggers

Because Groove is not just delay—it is actively retriggered synthesis—odd clocks make it sound like a composed percussion layer rather than an echo.

### Example
- HIT = 1 and 6 in an 11-step sequence
- CLOCK = every pulse from a 16th-note master
- Groove COLOR toward repetition/reverb blend
- Groove FX set to HP or BP

You get a kick with an unstable, rotating halo.

---

# How to make the main Bohm voice punchy, unique, and percussive

The manual describes a consistent architecture across many models:

- **PITCH**
- **CURVE**
- **ATTACK**
- **SUSTAIN**
- **LENGTH**
- **TRS DECAY**
- **TRS TONE**
- **COLOR**
- **FX**

## 1. Short LENGTH + strong transient = percussion, not just kick
If you want Bohm to behave like a **tuned drum hit**, keep:

- **LENGTH** shorter
- **ATTACK** enough to emphasize the front edge
- **TRS DECAY** short
- **TRS TONE** brighter

This shifts the sound toward:
- tom
- zap
- knock
- clicky kick
- industrial percussive hit

Great for fast, intricate sequences.

---

## 2. Use CURVE as your rhythmic articulation control
The manual notes:

- counterclockwise = more **808-style**
- clockwise = more **909-style**
- shorter LENGTH may prevent the oscillator from fully reaching the target fundamental

That is gold for percussive design.

### Practical implication
You can use **CURVE + LENGTH** together to change whether a hit feels:
- rounded
- snapping
- pitched
- almost “conga-like”
- like a transient thud with no stable low tone

For dense rhythms:
- use shorter length
- modulate CURVE slowly or per step

This creates a family of related hits instead of one static kick sample.

---

## 3. Treat PITCH as tuned percussion, not just bass
The manual says Bohm can do **pitch tracking** if set correctly:
- PITCH knob fully CCW
- PITCH attenuverter fully CW
- choose proper system voltage range
- use 1V/oct

This lets you sequence Bohm as:
- bassline percussion
- tuned tom line
- melodic kick pattern
- polyrhythmic pitch accents

### Excellent use for complexity
Sequence **different pitches on different rhythmic layers**:
- low tonic for bar anchors
- higher pitches on offbeats
- perfect fourth/fifth/octave jumps for phrase markers

This makes the rhythm feel more composed and less repetitive.

---

## 4. Modulate VELOCITY for ghosted percussion
Velocity is often overlooked on kick modules. Here it matters.

Use a stepped random source, sequencer lane, or accent pattern into **VELOCITY CV** to create:

- ghost notes
- accented polymeter
- “human” contour
- rolling dynamic contrast

Especially effective in fast patterns where the same sound would otherwise blur.

---

## 5. Use HIT as gate, not just trigger
The manual says **HIT can work as trigger or gate**. If held high, the sound sustains, then decays when released.

This is powerful for advanced percussion because it means you can vary **note duration rhythmically**.

### Patch ideas
Send:
- short triggers on some steps
- longer gates on others

Result:
- some hits are sharp drum strikes
- others bloom into drones, booms, or bass notes

This is especially strong in:
- 5/4
- 7/8
- additive meters
- evolving techno structures

You can make the same voice alternate between kick, tom, bass stab, and low drone.

---

# Best models for complicated percussion use

## FM-2X
Best for:
- punchy FM kicks
- tuned percussive bass
- synthetic drum articulation

Why:
- ATTACK controls FM amount
- TRS DECAY controls FM transient duration
- TRS TONE changes modulator character
- RATIO variation changes harmonic behavior

### For hyper-complex use
Modulate or snapshot different **RATIO** settings across patterns.  
That turns one rhythmic line into multiple related “instruments.”

Use it like:
- low ratio for body
- higher ratio for metallic or snappier hits

This is likely one of the best models for intricate percussion.

---

## HZ-1
Best for:
- clicky transient kicks
- shapeable harmonic front edge
- classic electronic percussion

Why:
- COLOR changes transient distortion behavior over time
- WT variation changes oscillator waveform
- CLK variation changes transient click type

### Use it for:
- click-led fast rhythms
- “top kick” duties
- sharper odd-meter accents

---

## OLP4
Best for:
- experimental FM percussion
- aggressive synthetic hits
- unusual harmonics

Why:
- 4-operator FM architecture
- different algorithms
- waveform selections
- feedback via TRS TONE

### Use it for:
- metallic low percussion
- pseudo-industrial drum sequences
- “not obviously a kick” percussive tones

This may be the best model if you want the kick voice to become a **weird percussion synthesizer**.

---

## PM-K1
Best for:
- acoustic-ish bass drum gestures
- roomy physical body
- less synthetic pulse

Limitations:
- many controls inactive
- Groove not supported

So for hyper-complex layered rhythm, this is less central unless you want one acoustic-like anchor voice.

---

## PX3 / SP-6 / WT-4
Best for:
- layered transient-heavy kicks
- harder, more aggressive percussion
- digital or analog-leaning layered hits

Because they combine oscillator + layering material, they’re ideal when you want the kick to speak through dense arrangements.

### Use them for:
- punchy front-loaded strikes
- industrial or hybrid drum grids
- contrasting snapshots in performance

---

## XT-88
Best for:
- user-defined percussion identity
- custom wavetable and sample layering
- building your own drum machine behavior

This is the most open-ended option.

Load:
- short clicks
- stick hits
- metallic transients
- noisy tops
- odd found-sound percussive samples

Then use Bohm’s kick engine as the body and your own sample as the attack signature.

For complex percussion systems, this is maybe the deepest model.

---

# How to use Groove for dense percussive complexity

Groove is not merely a rumble add-on. It can be your **sub-grid percussion layer**.

## Understand the four generator families
Manual says Groove blends:
- **repetition**
- **kick reverb**
- **noise**
- **grit + sub**

Use **COLOR** as a morphing composition control.

### Practical role of each
- **Repetition** = articulated extra drum hits
- **Reverb** = smear / tail / space / tunnel
- **Noise** = hats / texture / hiss / transient spray
- **Grit + sub** = dirty low percussion or body reinforcement

This is enough to make Groove act like:
- rumble engine
- tops engine
- sub pulse
- noisy chatter layer

---

## 1. Use repetition mode for interlocking rhythms
The repetition engine responds to CLOCK triggers, so it is perfect for:
- 3 against 4
- 5 against 4
- 7 over 8
- Euclidean subdivisions

Keep **COLOR** biased toward repetition.

Then shape:
- **2 / 3 / 4** for the tap levels
- **LENGTH** for relative duration
- **PITCH** for relative pitch

Because Groove pitch and length are **relative to Bohm**, you get a coherent but animated pair of instruments.

### Example
- Bohm main hit = deep body
- Groove repetition = shorter, slightly higher “knock”

This makes a kick family rather than two unrelated drums.

---

## 2. Use noise or grit as a synthetic hi-hat/snare layer
Past around 3 o’clock on COLOR, you can lean into non-repetition sources.

Then:
- 2/3/4 and TAPS CV shape the envelope contour
- PITCH alters the generator character
- Groove FX can filter or distort it

This is a very strong way to create:
- noisy sixteenth chatter
- hat-like syncopation
- rattling triplet overlays
- burst accents in polymeter

### Especially good move
Use Groove **HP** or **BP** effect on noisy material so it occupies upper-mid range and doesn’t muddy the kick body.

---

## 3. Use GRV ENV = SUSTAIN for drones and held rhythmic beds
The manual says:
- **FALL** = envelope falls after tap 4
- **SUSTAIN** = stays at tap 4 level

This means Groove can become a **continuous percussive bed** if your clock density is high.

### Use case
- Main kick sparse
- Groove on dense odd clock
- GRV ENV = SUSTAIN
- COLOR toward noise or grit
- Performer ducks external input against it

Now the patch breathes like a living rhythm texture rather than simple discrete hits.

---

## 4. Modulate TAPS CV for variable internal phrases
Since the tap structure can be shaped by **TAPS CV**, you can animate the envelope contour over time.

Patch in:
- stepped random
- Euclidean CV sequence
- slow chaos
- another envelope

Now every set of taps changes shape:
- 2 weak / 3 strong / 4 absent
- then 2 high / 3 low / 4 high
- etc.

This is one of the best ways to keep dense subdivisions from sounding looped.

---

## 5. Use the TAPS output as a control source elsewhere
The manual says **TAPS output** can output:
- Groove envelope
- inverted Bohm envelope
- Performer envelope
- Bohm envelope

This is huge in a modular context.

Use TAPS OUT to:
- open a VCA for hats
- ping a filter
- modulate a wavefolder depth
- sidechain another voice
- animate reverb send
- drive a LPG
- control another percussion source

So Bohm can become the **timing brain** of a larger percussion ecosystem.

### Great advanced patch
- TAPS OUT = Groove envelope
- Send to VCA controlling noise source or metallic voice
- CLOCK Groove at odd subdivision
- Main HIT on downbeats

Now Bohm generates both its own percussion and the control contour for another instrument.

---

# Using Performer for rhythmic complexity

Performer is not just a utility. It can make your whole percussion network breathe.

## 1. Duck external percussion loops or voices with HIT
The manual says the stereo input is ducked on every **HIT** trigger, with **DUCK** amount control.

Feed into Performer:
- hats
- claps
- modular percussion bus
- breakbeat loop
- noise wash
- synth stab bus

Then duck them from Bohm’s kick.

This creates clarity and pulse, especially in dense patterns.

### Advanced use
If Bohm is in a complex meter and the external loop is straight, the ducking pattern imprints the complex meter onto the loop.  
That’s an excellent way to create polyrhythmic illusion without rewriting every sequence.

---

## 2. Choose effect routing strategically with CHN
Per manual, Performer can process:
- **ALL**
- **KICK**
- **INPUT**

This is important.

### For punch
Set **CHN = KICK**
- Process only Bohm/Groove
- Leave external percussion clean

### For rhythmic transformation
Set **CHN = INPUT**
- Put beat roll/slip roll/filter only on incoming loop or percussion bus
- Let Bohm remain solid

### For chaos
Set **CHN = ALL**
- Everything goes through one gesture processor

---

## 3. Use Beat Roll and Slip Roll as rhythmic mutation tools
Performer FX options include:
- **BEAT ROLL**
- **SLIP ROLL**

These are ideal for:
- fills
- stutters
- phrase transitions
- metric disruptions

### Performance trick
Keep the underlying sequence stable, then use:
- beat roll for temporary subdivision intensification
- slip roll for more glitchy reset-like effects

Because the input can be resampled on every HIT in slip roll, it can become strongly tied to the kick pulse.

This is excellent for making live polyrhythms feel “performed” rather than preprogrammed.

---

## 4. Use synced FX switching
The manual says FX on/off can be:
- **INSTANT**
- **SYNCED** to next HIT

For complex music, **SYNCED** is safer and more musical because transitions land with the rhythm.

Use this for:
- activating beat roll only on the next structural hit
- dropping a filter exactly on the barline
- changing phrase feel without mistimed toggles

---

## 5. Use Duck Time, Duck Smooth, and Duck Band Split
These variation settings are especially useful for dense percussion.

- **DUCK TIME** = release time
- **DUCK SMTH** = smoothing
- **DUCK BS** = ducked band split frequency

### Good settings logic
- Short duck time = tight, punchy, articulate
- Longer duck time = pumping, breathing, larger groove
- More smoothing = preserves some transient from external audio
- Band split = duck lows while preserving highs for transparency

### Great patch use
If your external input is a busy hat/snare/percussion mix:
- set a band split so lows get ducked
- highs remain present
- Bohm punch stays intact without muting all detail

This is one of the best ways to keep a dense mix readable.

---

# Best rhythmic workflows

## Workflow 1: Polyrhythmic kick + tap engine
- HIT: sequencer pattern in 5
- Groove CLOCK: constant 16ths
- Bohm model: FM-2X or HZ-1
- Groove COLOR: repetition/noise blend
- Tap levels 2/3/4 asymmetrical
- Groove FX: BP
- Performer: duck external hats with moderate DUCK

Result: structured but dense rhythmic mesh.

---

## Workflow 2: Odd-meter techno engine
- HIT: 7/8 pattern with missing accents
- CLOCK: straight 8ths
- Bohm LENGTH: medium-short
- CURVE modulated slowly
- VELOCITY sequenced
- Groove PITCH slightly higher than Bohm
- Groove VOL moderate
- Performer FX on kick only with DJ filter

Result: asymmetrical but danceable low-end phrasing.

---

## Workflow 3: Tuned percussion line
- Enable pitch tracking
- Sequence Bohm melodically in 1V/oct
- Use short gates for some notes, longer for others
- Groove CLOCK at faster subdivision
- Groove in repetition mode with shorter relative length
- Use TAPS OUT to trigger another VCA/noise voice

Result: Bohm becomes kick + tom/bass percussion centerpiece.

---

## Workflow 4: Dense industrial percussion
- Bohm model: OLP4, PX3, or XT-88
- Main HIT irregular and sparse
- Groove CLOCK dense and logic-derived
- Groove COLOR toward grit/noise
- Groove FX = DIST or HP
- Performer input fed from metallic/noise percussion bus
- CHN = INPUT or ALL
- Use beat roll for transitions

Result: layered, abrasive, machine-like percussion field.

---

## Workflow 5: Rumble plus articulated tops
- Bohm main kick long and weighty
- Groove COLOR between reverb and repetition
- Groove CLOCK on 16ths or triplets
- Groove LENGTH moderate
- Groove PITCH slightly above or below center
- GRV ENV = FALL for decaying rumble phrases
- Performer ducks external clap/hat loop

Result: rich techno low-end with internal movement.

---

# Snapshot and live mode strategies for advanced rhythm

Bohm’s **snapshots/programs** are very useful for complicated percussion arrangements.

## Why snapshots matter here
A snapshot can store:
- model variations
- knob positions

This lets you create multiple rhythmic personalities:
- one for 4/4 groove
- one for 7/8 bridge
- one for triplet tension
- one for dense roll section
- one for breakdown drone

## Song mode for arranged complexity
Use **Song mode** if your piece has:
- fixed sections
- meter changes
- recurring rhythmic forms

You can advance steps via **FUNCTION trigger**, which means an external sequencer can automate section changes.

That is perfect for:
- bar 1–8 = 4/4
- bar 9–12 = 5/4
- bar 13–16 = 7/8
- bar 17 = roll/fill

## Jam mode for improvisational complexity
Use **Jam mode** if you want to:
- cue different kick/percussion states live
- improvise metric changes
- move between snapshots as performance gestures

This is ideal if your music is exploratory or modular-improv based.

---

# Sound design tips to keep it punchy in dense arrangements

Dense rhythm can turn to mud fast. The manual gives several ways to avoid that.

## 1. Use Bohm FX variations wisely
Common Bohm effects:
- TUBE
- BASS
- SOFT
- HARD
- WAVEFOLD
- BITCRUSH
- DECIM on some models

### Suggested uses
- **TUBE** for warm body and slightly enhanced front edge
- **HARD** for aggressive attack that cuts
- **SOFT** for control without harshness
- **WAVEFOLD** for unusual overtones in sparse mixes
- **BASS** for longer 808-type material
- **BITCRUSH / DECIM** for digital percussion identity

In dense complex percussion, **HARD**, **SOFT**, and selected **TUBE** settings are often best.

---

## 2. Use stereo width carefully
Both Bohm and Groove can have **STEREO** variation.

For highly rhythmic music:
- keep main body more centered/mono-ish
- spread Groove or Performer input wider

This improves punch while preserving complexity.

---

## 3. Use Post EQ as final tuning
The system **Post EQ** affects Bohm and Groove outputs.

This is extremely useful if your complex percussion becomes:
- too boomy
- too honky
- too splashy

Use it to:
- trim low shelf if rumble dominates
- cut a muddy low-mid peak
- add top shelf if noisy taps need more definition

Since it is a system setting, think of it as your final venue/mix adaptation tool.

---

## 4. Use Performer volume behavior strategically
Manual options:
- **PERF VOL** can affect B+G or BOHM only
- **PERF MAX** can limit max level

A clever trick:
- set **PERF VOL = BOHM only**
- let Groove remain more constant

That can create the feel of a persistent rhythmic bed while the main kick body breathes over it.

The manual explicitly notes this also allows Groove to drone without hearing Bohm.

That is useful for experimental percussive textures.

---

# Specific advanced patch recipes

## Recipe A: 4 over 5 evolving kick mesh
- External master clock into clock divider/multiplier
- Generate:
  - HIT pattern every 5 pulses
  - CLOCK every 4 pulses
- Bohm model: FM-2X
- Groove COLOR: repetition + noise
- Groove 2/3/4 at uneven values
- TAPS OUT to modulate external VCA on a separate metallic source

Result: two audible percussion layers plus one derived CV percussion layer.

---

## Recipe B: Additive meter percussion
For a 3+3+2 feel:
- Trigger HIT on the start of each group
- CLOCK continuously on 8ths
- Use Groove taps to emphasize the inner motion
- Change VELOCITY on the third group
- Snapshot alternate states for phrase changes

Result: strong additive-meter articulation.

---

## Recipe C: Kick becomes tom ensemble
- Pitch track Bohm
- Shorten LENGTH
- Increase ATTACK and brighten TRS TONE
- Use HZ-1, VX-T, or OLP4
- Sequence notes across a scale fragment
- Groove repetition one octave or interval offset via relative pitch

Result: tuned low percussion that can replace toms or bass drums.

---

## Recipe D: Controlled chaos with external bus
- Send hats/claps/noise bus into Performer IN
- Bohm on sparse irregular accents
- Groove on dense clock
- DUCK medium-high
- DUCK BS set so highs survive
- Beat Roll on input only
- TAPS OUT = PERF envelope to animate another filter

Result: a whole percussion mix pulsing around Bohm.

---

# A few especially valuable manual-based tricks

## Use Groove LENGTH only when repetition source is active
The manual notes Groove **LENGTH only affects repetition**, roughly from around 3 o’clock to full CW on COLOR behavior.

So if you are on noise/reverb/grit territory and wondering why LENGTH feels inactive—that is expected.

Practical takeaway:
- if you want articulated micro-hits, bias COLOR toward repetition
- if you want texture, use other generator regions and stop relying on LENGTH

---

## Groove pitch/length are relative to Bohm
This is one of the best musical design choices in the module.

Because Groove is relative:
- it naturally follows your main kick’s pitch/length area
- it stays coherent while still being different

So for complex sequences, modulating the main Bohm pitch/length also indirectly changes Groove behavior.

This is a great way to create **macro variation**.

---

## Use FUNCTION CV in Studio mode for randomization
Manual says in Studio mode the **FUNCTION CV** can randomize model variations.

This is useful for exploratory percussion design:
- patch a rare trigger or manual gate
- let Bohm produce fresh variation states
- save snapshots of the good ones

Because Bohm models are designed around sweet spots, this can be a serious creativity tool rather than gimmick.

---

# Recommended setup if your goal is “hyper-complex percussion”

If I were building around Bohm for this purpose, I would pair it with:

- a **master clock / clock divider / multiplier**
- a **logic module**
- a **Euclidean trigger sequencer**
- a **CV sequencer for pitch/velocity**
- one or two **random or chaotic CV sources**
- a **switch** for changing clocks or patterns
- extra voices controlled by **TAPS OUT**

Then Bohm becomes:
- kick synthesizer
- sub-percussion voice
- texture generator
- ducking processor
- modulation source
- snapshot-based performance instrument

---

# Best concise recommendations

If you want the fastest path to dense and advanced percussion:

1. **Use different sources for HIT and Groove CLOCK**
2. **Run Groove on a different subdivision or meter than Bohm**
3. **Sequence VELOCITY and PITCH**
4. **Use short LENGTH and transient shaping for drum-like articulation**
5. **Exploit HIT-as-gate for variable duration percussion**
6. **Use TAPS OUT to animate other modules**
7. **Use Performer ducking to impose rhythm on external loops**
8. **Store multiple metric personalities as snapshots**
9. **Use Song mode for arranged meter changes**
10. **Use OLP4, FM-2X, HZ-1, PX3, or XT-88 for the most percussive variety**

---

# Best model choices by role

- **Punchy synthetic kick percussion**: FM-2X
- **Clicky articulated drum voice**: HZ-1
- **Experimental metallic percussion**: OLP4
- **Hard layered attack**: PX3 / SP-6 / WT-4
- **Custom percussion ecosystem**: XT-88
- **Acoustic-ish bass drum anchor**: PM-K1

---

# Final take

Bohm is very well suited to **densely rhythmic, hyper-detailed percussion music** because it is not locked into “one kick per bar” thinking. Its real strength is the interaction between:

- **main voice pulse**
- **secondary Groove clock behavior**
- **relative timing and pitch relationships**
- **snapshot-based structural changes**
- **Performer ducking and roll effects**
- **control-voltage reuse through TAPS OUT**

If you patch it like a **layered rhythm instrument** instead of a simple kick module, it can become the central engine for:

- polyrhythms
- odd meters
- internal subdivisions
- evolving percussion beds
- sharp transients
- tuned low percussion
- live rhythmic mutation

If you want, I can also turn this into:
1. a **set of 10 concrete patch recipes**,  
2. a **“best companion modules for Bohm” guide**, or  
3. a **“how to build an Autechre/techno/IDM style percussion system around Bohm” guide**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)