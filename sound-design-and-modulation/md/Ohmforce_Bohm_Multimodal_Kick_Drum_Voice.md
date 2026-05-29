# Ohmforce — Bohm Multimodal Kick Drum Voice

- [Manual PDF](../../manuals/Bohm_Eurorack_Manual_Compiled.pdf)

---

[Manual PDF / Source](https://bohm-eurorack-manual.readthedocs.io/en/latest/index.html)

# Bohm Eurorack modulation ideas

Bohm looks much deeper than a simple kick module. Since it’s a **stereo dual-voice kick system** with **different internal models**, plus optional **Groove** and **Performer** expanders, the best approach is to treat it like a **bass/percussion voice** rather than only a drum source.

From the manual, the key sound-shaping controls are:

- **HIT**
- **VELOCITY**
- **LENGTH**
- **SUSTAIN**
- **ATTACK**
- **PITCH**
- **CURVE**
- **TRS DECAY**
- **COLOR**
- **FX**
- **TRS TONE**

And the important note is that **controls behave differently depending on the selected model**, so the most interesting results will come from:
1. choosing a model,
2. sending modulation to several parameters at once,
3. using the module’s pitch and decay behavior as the basis for timbre.

---

## General modulation strategy

For Bohm, I’d think in 3 modulation rates:

### 1. Trigger-rate modulation
Change something every hit:
- velocity accents
- pitch amount
- decay length
- color/tone per step

This is how you get **alive, animated percussion** instead of static kicks.

### 2. Envelope-rate modulation
Use envelopes to shape timbre over the course of each sound:
- short envelope to **PITCH** for punch
- longer envelope to **COLOR** or **FX** for evolving body
- envelope to **SUSTAIN** or **LENGTH** for bass articulation

### 3. Slow CV / LFO modulation
Use slow movement for atmosphere and instability:
- drift **TRS TONE**
- slowly modulate **CURVE**
- stereo movement through **FX** or Performer processing

This is how you push it into **pads**, **evolving drones**, and ominous textures.

---

# 1) Distorted percussive sounds

Bohm should be excellent for industrial percussion, smashed kicks, metallic hits, and broken drum machine sounds.

## A. Overdriven techno kick variations
Start with a model that already has strong low-end or aggressive transient behavior.

### Suggested settings
- **ATTACK:** medium to high
- **PITCH:** low-mid
- **CURVE:** steeper/faster for a hard drop
- **LENGTH / SUSTAIN:** short to medium
- **COLOR:** push until harmonics emerge
- **FX:** increase until it begins to feel unstable or widened
- **TRS DECAY / TRS TONE:** tune for resonance or ringing

### Modulation patch
- Send a **random stepped CV** to **VELOCITY**
- Send a second, attenuated random CV to **COLOR**
- Use an accent trigger to open **ATTACK** or increase **HIT**
- Modulate **CURVE** every 4 or 8 steps with a sequencer row

### What this does
You’ll get kick hits that shift between:
- tight thump
- crunchy knock
- blown-out slam
- resonant industrial toms

If the selected model reacts strongly to COLOR or FX, this can get very nasty in a good way.

---

## B. Broken clap/snare-like percussion from a kick engine
Even though Bohm is kick-focused, fast pitch and tone modulation can push it into hybrid percussion.

### Patch idea
- Set **PITCH** higher than normal kick range
- Keep **LENGTH** very short
- Increase **ATTACK**
- Tune **TRS TONE** to emphasize a noisy or clicky region
- Modulate **COLOR** with a very fast envelope
- Use small random CV into **PITCH**

### Result
You can get:
- zap-like hits
- electro percussion
- woody clicks
- distorted rim / tom hybrids

If Groove is installed, layer the second voice slightly offset in timing for **flammed percussion** or **rumble tails**.

---

## C. FM-like impact sounds
Even without explicit FM in the manual, very fast modulation of pitch-related parameters can fake FM-ish percussion.

### Try this
- Mult your trigger:
  - one copy triggers Bohm
  - another triggers a very short envelope
- Send that envelope to **PITCH**
- Send an inverted or attenuated version to **CURVE**
- Optionally modulate **TRS TONE** at the same time

### Why it works
The pitch envelope and curve interaction can create:
- laser hits
- metal punch
- tearing impacts
- aggressive “speaker rip” attacks

Use a VCA or attenuator because too much pitch envelope will just sound cartoony.

---

## D. Distorted layered percussion with Groove expander
The manual says **Groove adds a secondary kick voice for techno rumbles and layered percussion**. That means you can design one voice as the transient and the other as the dirt/body.

### Layer recipe
**Main Bohm voice**
- short
- punchy
- more attack
- less sustain

**Groove voice**
- lower tuned
- longer decay
- more color / fx
- slightly delayed trigger if possible

### Modulation
- Sequence different velocities to both voices
- Modulate Groove pitch subtly with an LFO or random source
- Send occasional longer gates for selective rumble blooms

### Result
This gives:
- warehouse kick stacks
- distorted low tom barrages
- rolling industrial grooves
- pseudo-reverb rumbles without external effects

---

# 2) Crazy basslines for dubstep / drum and bass

This is where Bohm gets really interesting. Since the manual says **PITCH ranges roughly from C1 to C2**, that’s right in useful bass territory. It won’t be a full-range melodic oscillator in the conventional sense, but for heavy bassline work that limited range can be perfect.

## A. Triggered reese-style bass pulses
Use Bohm as a monophonic bass percussion voice rather than a sustained oscillator.

### Settings
- **SUSTAIN:** medium
- **LENGTH:** medium-long
- **PITCH:** tuned to root note area
- **CURVE:** moderate, not too steep
- **COLOR:** enough to growl
- **FX:** add stereo dirt/motion
- **TRS TONE:** find a sweet spot with midrange bite

### Modulation
- Sequence pitch changes in a low register
- Send an LFO to **COLOR**
- Send a different slower LFO or stepped random to **FX**
- Use accent CV into **VELOCITY**
- Occasionally increase **ATTACK** for selected notes

### Sound
This should create:
- gnarly bass stabs
- wobbling low-end phrases
- distorted “donk” basses
- neuro-ish bass punches

Because Bohm starts from a kick architecture, even pitched notes will retain a percussive front edge, which is excellent for DnB.

---

## B. Dubstep wobble from parameter cross-modulation
Instead of only wobbling filter cutoff like on a subtractive synth, wobble the **body mechanics** of the kick model.

### Core patch
- Clock-sync an LFO
- Send it to **COLOR**
- Send an attenuated inverted copy to **TRS TONE**
- Send another divided clock modulation to **FX**
- Sequence **PITCH** in a repeating 1–2 bar pattern

### Why this is cool
As COLOR rises while TONE falls, or vice versa, the bass can morph from:
- hollow
- nasal
- snarling
- sub-heavy
- torn-speaker distorted

This gets you much more unusual movement than a normal filter wobble.

---

## C. Machine-gun bassline growls
Use very short note retriggers with varying pitch envelope depths.

### Patch
- Rapid trigger pattern from a sequencer
- A modulation lane to **VELOCITY**
- Another lane to **CURVE**
- A burst generator or ratcheting trigger into HIT
- Envelope to **PITCH** amount via VCA

### Target sound
- stuttering bass attacks
- talking growls
- tearing fills
- jump-up DnB style bass punctuation

The trick is to make every rapid hit slightly different. Small CV movement on CURVE and COLOR matters a lot.

---

## D. Sub drop / bass cannon patch
Bohm should be able to produce devastating drops if you extend the decay and pitch motion.

### Settings
- **PITCH:** low
- **LENGTH / SUSTAIN:** long
- **CURVE:** tuned for a dramatic downward sweep
- **COLOR:** moderate
- **FX:** enough to widen or dirty the tail

### Modulation
- Trigger with a long gate
- Use a descending envelope to **PITCH**
- Slowly open **COLOR** over the tail
- If Performer is installed, use its **ducking and stereo processing** around the hit

### Result
- festival-style bass drops
- trailer impacts
- cinematic subs
- huge intros and transitions

---

## E. Fake sidechained bass using Performer
The manual says Performer adds **DJ-style effects, ducking, and stereo processing**. That is extremely useful for bass design.

### Idea
Patch Bohm as both:
- your kick/percussive source
- and a sustained bass element

Then use Performer’s ducking to carve motion around the attacks.

### Outcome
You can get:
- self-pumping basslines
- club-style movement
- huge stereo body with centered attack
- more mix-ready distorted low-end

This is especially effective for dubstep intros and halftime grooves.

---

# 3) Haunting atmospheric pad sounds

This is the least obvious use, but definitely possible if you stop thinking of Bohm as only a drum.

The manual mentions:
- stereo processing
- multiple models
- FX and tone controls
- longer sustain/length options
- expanders for wider processing

That suggests Bohm can be pushed into **drone and pad-adjacent territory**, especially with re-triggering, long decays, and slow modulation.

## A. Ghost drone patch
### Settings
- **LENGTH / SUSTAIN:** high
- **ATTACK:** softened if possible
- **PITCH:** low-mid
- **CURVE:** gentle
- **COLOR:** low to medium
- **FX:** moderate to high
- **TRS TONE:** tuned for a hollow or mournful resonance

### Modulation
- Very slow LFO to **PITCH** (tiny depth)
- Separate slow LFO to **COLOR**
- Random smooth CV to **TRS TONE**
- Sparse triggers or manually tapped HIT

### Result
Instead of a punchy kick, you get:
- foggy resonant blooms
- distant machine drones
- haunted engine-room ambience
- dark underscoring textures

Add external reverb after Bohm and it becomes much more pad-like.

---

## B. Granular-feeling pad from repeated soft retriggers
Use frequent but low-intensity hits to create a cloud.

### Patch
- Send a fast but irregular trigger stream
- Lower **VELOCITY**
- Lengthen **SUSTAIN**
- Keep **ATTACK** modest
- Slowly modulate **FX** and **TRS TONE**

### What happens
Each hit becomes a small fragment in a larger texture. In stereo this can feel like:
- swarming air
- distant choirs of machinery
- unstable ambient beds
- eerie pulsing fog

This works especially well if the model has a resonant or tonal tail.

---

## C. Dissonant haunted pad using pitch drift
Because Bohm only spans roughly **C1 to C2**, the pitch range is constrained, which is actually helpful for dark drone work.

### Try this
- Tune the main pitch to the root
- Send tiny random or sample-and-hold modulation to **PITCH**
- Use another slow modulation to **CURVE**
- Increase **FX** for width or instability
- Layer Groove at an interval-like offset if possible

### Result
You’ll get subtle beating and tonal ambiguity:
- ominous low strings vibe
- degraded tape-organ feeling
- dark ambient resonance
- horror soundtrack undertones

---

## D. Stereo cinematic pad with Performer
Performer’s stereo processing is the key here.

### Patch concept
- Long-decay Bohm sound
- Sparse triggers
- Slow CV to timbral parameters
- Use Performer for width, ducking, and DJ-style effects

### Best use
- huge intro washes
- breakdown textures
- transitions between heavy sections
- hovering stereo dread

Even if the source is still obviously “kick-derived,” once spread and effected it can become very atmospheric.

---

# Best parameters to modulate for each goal

## For distorted percussion
Prioritize:
- **VELOCITY**
- **ATTACK**
- **CURVE**
- **COLOR**
- **TRS TONE**

These shape the impact and harmonic aggression.

## For basslines
Prioritize:
- **PITCH**
- **CURVE**
- **SUSTAIN**
- **LENGTH**
- **COLOR**
- **FX**

These shape note identity, weight, and movement.

## For pads/drones
Prioritize:
- **LENGTH**
- **SUSTAIN**
- **COLOR**
- **FX**
- **TRS TONE**
- subtle **PITCH**

These shape resonance, tail, width, and slow transformation.

---

# Advanced modulation ideas

## 1. Macro modulation
Use one CV source multed to several destinations with different attenuations:
- positive to **COLOR**
- inverted to **TRS TONE**
- slight amount to **CURVE**

One knob or one LFO can then create major morphs.

## 2. Accent-dependent timbre
Instead of only accenting loudness, use accent gates/CV to also open:
- **ATTACK**
- **COLOR**
- **FX**

That makes accented steps brighter, harsher, and more explosive.

## 3. Probability-based mutation
Use a probabilistic trigger or random stepped CV to occasionally alter:
- **PITCH**
- **LENGTH**
- **TRS DECAY**

This makes loops feel less repetitive and more performative.

## 4. Audio-rate abuse
If Bohm accepts sufficiently fast CV on certain inputs, try audio-rate modulation of:
- **PITCH**
- **COLOR**
- **TRS TONE**

Even if it doesn’t behave like clean FM, aliasing and instability can create brutal digital textures.

## 5. Resampling workflow
Since the module uses **microSD / SDHC** and stores models/samples/settings, a practical approach is:
- patch extreme sounds
- record long improvisations
- resample the best moments
- use those snippets in a sampler for further composition

That’s often the fastest path to truly unique bass and atmospheric material.

---

# Performance mode suggestions

The manual mentions:
- **Studio Mode**
- **Live Song Mode**
- **Jam Mode**

## Studio Mode
Use this for:
- dialing exact sweet spots
- calibrating modulation depth
- building resampling material

## Live Song Mode
Use this for:
- sequenced parameter changes
- switching kick/bass character per section
- structured bassline or drum evolution

## Jam Mode
Use this for:
- improvised macro modulation
- live tweaking of color/fx/tone
- chaotic transitions and fills

For your goals, **Jam Mode** sounds especially promising for discovering weird bass and haunted textures.

---

# Practical patch recipes

## Recipe 1: Industrial broken kick
- 4-on-the-floor trigger into HIT
- random CV to VELOCITY
- short envelope to PITCH
- sequencer row to COLOR
- occasional accent to ATTACK
- Groove layer with long rumble tail

## Recipe 2: Dubstep growl stab
- melodic trigger sequence
- tune PITCH to root/fifth
- medium sustain
- synced LFO to COLOR
- inverted LFO to TRS TONE
- stepped modulation to FX
- Performer ducking for pump

## Recipe 3: Neuro percussion fill
- ratcheting triggers
- short decay
- modulate CURVE every step
- random CV to PITCH at low depth
- high COLOR and aggressive FX
- automate mutes for sudden drops

## Recipe 4: Haunted drone bed
- sparse triggers
- long sustain/length
- slow LFO to COLOR
- random smooth CV to TRS TONE
- tiny pitch drift
- stereo processing from Performer
- external reverb after output

## Recipe 5: Bass cannon transition
- one trigger every 8 or 16 bars
- long pitch envelope downward
- long sustain
- increase FX over tail
- optional Groove layer for sub reinforcement
- Performer widening on tail only

---

# Final advice

The big takeaway from the manual is that **Bohm is model-based**, and **controls react differently per model**, so the deepest sound design move is not just modulating more CV, but **finding which model turns a given parameter into something extreme**.

If I were designing the kinds of sounds you want, I’d explore in this order:

1. **Find 2–3 aggressive models** for distorted percussion  
2. **Find 2 models with the strongest tonal sustain** for basslines  
3. **Find 1–2 resonant/atmospheric models** for drone and pad work  
4. Patch:
   - envelope to **PITCH**
   - LFO to **COLOR**
   - inverted LFO to **TRS TONE**
   - stepped random to **VELOCITY** or **CURVE**
5. Use **Groove** for layered rumble/body
6. Use **Performer** for stereo movement, ducking, and live destruction

That combination should get you well beyond “kick drum” territory and into:
- mangled industrial percussion
- dubstep and DnB bass assaults
- eerie cinematic atmospheres

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)