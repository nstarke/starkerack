# WMD — Skorpion

- [Manual PDF](../../manuals/SKORPION_Manual.pdf)

---

[Manual PDF](https://wmdevices.com/cdn/shop/files/Skorpion_Manual_Rev1.00.pdf)

# WMD Skorpion modulation ideas for distorted percussion, insane basslines, and haunted pads

Skorpion is not just a wavefolder. It behaves more like a **threshold-driven waveform animator**: your input is constantly compared against up to 8 thresholds, and every crossing changes the behavior of the internal vector core. That means it rewards **modulation everywhere**—especially modulation that changes how and when threshold crossings happen.

The big takeaway from the manual is this:

- **FOLD** changes how hard the input pushes into the threshold system
- **SLOPE** determines how fast the internal core moves, which strongly affects brightness/harmonics
- **SHIFT** offsets the input against thresholds, adding asymmetry and even frequency-shift-like motion when modulated slowly
- **TARGET** changes where the vector core wants to go
- **SHAPE** modulates SLOPE using feedback and internal signals like OUT, DIFF, COUNT, TRGTs, etc.
- The **THLD sliders** and **TRGT sliders** are a huge part of the sound, not just “settings”
- Skorpion also generates many useful CV/audio outputs for **self-patching**

That means the most interesting sounds usually come from:

1. **Audio-rate or fast CV into FOLD / SHIFT / SHAPE / THLDs**
2. **Self-patching from DIFF / COUNT / DAC / ±G(DIR) / DELAY / TRGTs**
3. **Using THLDs and TRGTs as animated structures**, not static positions
4. **Abusing CLIP, HALT, SYNC, and TARGET modes**

---

# First: how to think about modulation on Skorpion

## 1. Modulating FOLD
This is the obvious one, but on Skorpion it does more than “more wavefolding.” It changes how strongly the input drives threshold crossings.

Great sources:
- envelope from a drum trigger
- velocity CV
- stepped random
- audio-rate oscillator
- internal macro LFO/envelope
- self-patched **COUNT/** or **DAC**

Results:
- more/less aggressive folding
- rhythmic changes in transient bite
- unstable tearing sounds when audio-rate modulated
- formant-like movement when modulated slowly on complex material

## 2. Modulating SLOPE
This is one of the most powerful parameters. The manual says higher slope = signal goes further, faster = more harmonics.

Great sources:
- 1V/oct if using Skorpion melodically
- envelope for attack bite
- audio-rate modulation for metallic sideband-like edges
- **DIFF** output for harsh recursive behavior
- **TRGTs** output for stepped timbral changes

Results:
- snappy transients
- aggressive bass growl
- harmonic “snarl”
- dramatic tone shifts from soft to shattered

## 3. Modulating SHIFT
SHIFT is especially good because it changes symmetry and threshold interaction. The manual notes slow modulation can create a **frequency shift effect**.

Great sources:
- triangle or sine LFO
- envelope with slow decay
- random slew
- **ABS(IN)** or **G(IN>0)** for waveform-dependent asymmetry
- audio oscillator for clangorous movement

Results:
- asymmetrical distortion
- animated bass vowel motion
- moving stereo grit
- ghostly drifting pads

## 4. Modulating TARGET
TARGET changes the destination voltage of the vector core:
- **5V** = more static / square
- **CLIP** = overlays input waveform
- **SLIDERs/TRGTs** = sequenced destinations

Great sources:
- TRGT MOD input
- self-patched external audio into **CLIP**
- sequencer CV into **TRGTs input**
- rhythmic gates into target sequencing by driving threshold crossings

Results:
- different “families” of distortion
- pseudo-PWM/square behavior
- spectral overlay from another signal
- stepped animated timbre

## 5. Modulating SHAPE
This is one of the deepest parts of the module. SHAPE modulates SLOPE using feedback sources:
- **IN**
- **OUT**
- **DELAY**
- **COUNT**
- **DIFF**
- **TRGTs**
- **DAC**
- **DIR**

This is where Skorpion gets alien.

Results:
- log/exp-like curves
- recursive screaming feedback behavior
- pulsed segment-by-segment deformation
- skewed or spiky waves
- unstable but playable textures

---

# The most important hidden modulation tools

## THLD sliders as a wavemaking structure
The thresholds decide where folds occur. Uneven thresholds create irregular harmonic events.

Try:
- clustered low thresholds for dense early folding
- sparse upper thresholds for occasional violent bursts
- alternating high/low patterns for pseudo-bitcrushed articulation
- all equalized for a more classic wavefolder behavior

### Equalize THLDs switch
Use this as a modulation destination:
- **ON**: classic, evenly spaced behavior
- **XOR**: equalized until a high gate disables it
- **JACK**: external gate turns equalization on

This is fantastic for switching between:
- smooth/classic fold tones
- weird irregular threshold patterns

A gate sequencer or clock divider into **EQ THLDs jack** can make one pattern sound “normal” on some steps and “broken” on others.

## TRGT sliders as a sequencer
TRGTs aren’t just helper values; they create a true 8-step destination voltage sequence.

Target order:
- **SEQ**: selected by count of active thresholds
- **TIED**: selected by most recently crossed threshold

This matters a lot:
- **SEQ** sounds more staircase/scan-like
- **TIED** sounds more unstable and gesture-based

Modulate or patch for:
- stepped timbre sequence
- threshold-dependent wavetable feel
- pseudo-formant patterns for basses and pads

## HALT and HALT IF TARG=0
This is one of the wildest features.

- **HALT jack** freezes the vector core at current voltage
- **HALT IF TARG=0** makes any target at zero stop motion for that segment

This can create:
- broken-square impacts
- gated tearing bass phrases
- stuck/frozen resonant-like moments
- staircase pad textures

---

# Best self-patch modulation sources

Skorpion gives you unusually useful outputs. These are gold for self-patching.

## DIFF
Difference between TARGET and actual vector core value. The manual says it is usually very high in harmonic content.

Use it to modulate:
- **SLOPE** for harshness and spikes
- **SHAPE** for unstable aggression
- **FOLD** for ripping dynamics
- external filter cutoff for synced screaming motion

This is one of the best “go feral” sources.

## COUNT/
0–4V staircase based on active thresholds, each threshold adds 0.5V.

Use it to modulate:
- **FOLD** for threshold-count-dependent aggression
- **SHIFT** for stepped asymmetry
- **TARGET** or **TRGT MOD** for staircase morphing
- external oscillator FM depth or filter cutoff

## DAC
Weighted version of count; subtler than COUNT.

Use it where COUNT is too coarse:
- gentle bass vowel movement
- subtle brightness sequencing
- evolving pad animation

## ±G(DIR)
+5V when rising, -5V when falling.

Use it to modulate:
- **SHAPE** with source = DIR for skew
- external polarizer/VCA
- filter FM or wave symmetry
- rhythmic directional pumping

## ABS(IN)
Full-wave rectified input.

Use it for:
- envelope-like audio-rate modulation
- making asymmetry related to source amplitude
- dynamic fold response

## G(IN>0)
Gate based on input polarity.

Use it for:
- comparator-like rhythmic switching
- clocking logic externally
- alternating modulation per half-cycle

## DELAY
Delayed signal from the WIDE section.

Use it to:
- feed back into SHAPE or CLIP
- modulate FOLD or SHIFT
- process externally and bring back in
- create chorused spectral instability

## TRGTs output
This is huge. It’s the target sequencer as CV/audio.

Use it to:
- modulate filter cutoff
- FM another oscillator
- animate another wavefolder/VCA
- self-patch into SHAPE, SLOPE, or TRGT MOD

---

# Patch ideas for distorted percussion

These focus on kicks, snares, hats, metallic hits, and glitch percussion.

---

## 1. Broken industrial kick
**Goal:** hard, overdriven, tearing kick with a cracked top transient

### Patch
- Sine or triangle oscillator into **IN**
- Pitch envelope on the oscillator for kick shape
- Set **TARGET** toward **5V**
- Medium-high **FOLD**
- Medium-high **SLOPE**
- **SYNC = HARD**
- **DRY IF NO THLDs = ON**
- Uneven threshold slider pattern, with several low thresholds active

### Modulation
- Fast decay envelope into **FOLD CV**
- Smaller fast envelope into **SLOPE CV**
- Patch **DIFF out** lightly into **SHAPE CV**
- SHAPE source = **DIFF**
- Set SHAPE just above noon

### Why it works
The input kick crosses thresholds during the pitch drop, while DIFF-driven shape adds ripping transient spikes. HARD sync makes the attack feel very reset and percussive.

### Variation
Set one or two **TRGT sliders to 0** and turn **HALT IF TARG=0** on. This adds abrupt “flat” segments in the transient, almost like clipped speaker damage.

---

## 2. Snare from noise + tone overlay
**Goal:** smashed electro/industrial snare

### Patch
- Mix noise + sine/triangle into **IN**
- Put **TARGET** between **CLIP** and **SLIDERs**
- Feed a second oscillator or bursty percussion signal into **CLIP jack**
- THLDs irregular, not equalized
- OUTPUT around wet, maybe a little wide

### Modulation
- Envelope into **SHIFT CV** to create asymmetry on attack
- **COUNT/** into **FOLD CV** attenuated
- **TRGT MOD** fed from a short envelope or audio blip
- SHAPE source = **OUT** or **COUNT**

### Why it works
The noise causes chaotic threshold crossings while the tonal body gives pitch center. External CLIP overlays another waveform onto the destination behavior for more crack and body.

---

## 3. Metallic hats and shards
**Goal:** sharp, digital-analog metallic percussion

### Patch
- Noise or highpassed oscillator into **IN**
- THLDs mostly high, with a few clustered
- **SLOPE** high
- **FOLD** moderate
- SHAPE source = **COUNT** or **DAC**
- TARGET toward **SLIDERs**

### Modulation
- Audio-rate modulation into **SHIFT**
- **±G(DIR)** into external VCA/filter or self-patched to SHAPE
- Use **TIED** target order
- Patch **TRGTs output** to external VCA/filter for synchronized timbral movement

### Why it works
Audio-rate SHIFT causes asymmetry flicker, while TIED target order makes the result more unstable and metallic.

---

## 4. Glitch toms / broken machine hits
**Goal:** crunchy electronic toms that splinter unpredictably

### Patch
- Triangle VCO into IN
- Envelope pitch mod on VCO
- **EQ THLDs** switched by trigger sequence
- Some steps equalized, others irregular
- **SYNC = SOFT**
- **TARGET = SLIDERs**
- TRGT sliders in descending staircase

### Modulation
- Trigger/gate pattern into **EQ THLDs jack**
- Envelope into **TARGET CV**
- Light **DAC** into **SHIFT**
- **HALT jack** pinged with occasional triggers

### Why it works
Switching equalized thresholds on/off changes the folding architecture per hit. HALT adds sudden frozen segments that sound like broken converters or robotic malfunctions.

---

# Patch ideas for dubstep / drum and bass basslines

This is where Skorpion looks incredible. Its combination of threshold sequencing, asymmetry, directional feedback, and self-patching is ideal for modern aggressive bass.

---

## 1. Classic talking reese mutation
**Goal:** moving, vocalized, nasty stereo bass

### Patch
- Detuned saw or square pair mixed to mono into **IN**
- **1V/OCT** from sequencer
- OUTPUT above noon into **WIDE**
- OUTPUT switch = **FILTERs**
- **TARGET** between **CLIP** and **SLIDERs**
- THLDs irregular, with more activity in the middle
- SHAPE source = **OUT**

### Modulation
- Slow triangle LFO or envelope into **SHIFT**
- Medium envelope into **FOLD**
- **DAC** into **TARGET CV** attenuated
- **DELAY out** into **SHAPE CV** attenuated
- Macro envelope controlling internal mod on FOLD and SHIFT

### Why it works
SHIFT adds vowel-like asymmetry motion, OUT feedback makes the slope bend musically, and the WIDE/delay path gives stereo movement while keeping lows centered in FILTER mode.

### Tip
Use **FILTERs** mode for cleaner low end in bass music. The manual says frequencies below 240 Hz stay centered, while highs are widened.

---

## 2. Neuro-style tearing bass
**Goal:** hyper-modulated, tearing, evolving bass

### Patch
- Rich oscillator or FM bass into **IN**
- **FOLD** high
- **SLOPE** high
- **TARGET = SLIDERs**
- Target order = **TIED**
- SHAPE source = **DIFF**
- **SYNC = HARD**
- Uneven THLDs, many active

### Modulation
- **DIFF out** into **SLOPE CV**
- **COUNT/** into **SHIFT CV**
- Envelope follower or LFO into **TRGT MOD**
- Audio-rate oscillator into **FOLD CV**
- Occasional gates into **HALT**

### Why it works
DIFF into SLOPE creates sharp, self-reactive edges. COUNT into SHIFT gives threshold-state-dependent asymmetry. HARD sync keeps it from completely dissolving into chaos.

### Tip
If it becomes too wild, switch SHAPE source from **DIFF** to **DAC** for a subtler but still animated version.

---

## 3. Stepped snarling sequence bass
**Goal:** articulated bassline where each note has internal timbral sequencing

### Patch
- Mono VCO into **IN**
- Sequencer to **1V/OCT**
- **TARGET = SLIDERs**
- Set TRGT sliders to a rhythmic pattern of low/high destinations
- Set target order to **SEQ**
- THLDs in a progressive ramp or alternating pattern

### Modulation
- Gate envelope into **SLOPE**
- **TRGTs output** into filter cutoff or second oscillator FM
- **COUNT/** into **FOLD**
- Macro LFO on **SHAPE**
- Slow LFO into **SHIFT**

### Why it works
The note itself drives threshold crossings, which then step through different target voltages, creating an internal sequence inside each bass note.

---

## 4. Ripping sub-bass with controlled top destruction
**Goal:** stable sub fundamental with aggressive moving mids

### Patch
- Sine/sub oscillator into IN
- Duplicate dry sub to separate mixer if possible
- OUTPUT switch = **FILTERs**
- OUTPUT above noon but not fully wide
- **DRY IF NO THLDs = ON**
- **EQ THLDs = ON** initially
- TARGET toward **5V**
- SHAPE source = **OUT** or **DAC**

### Modulation
- Envelope into **FOLD**
- Small audio-rate mod into **SHIFT**
- **DAC** into **SHAPE**
- Use **EQ THLDs jack** to occasionally disable equal spacing for fill moments

### Why it works
Equalized thresholds keep it more stable and classic, while occasional irregular threshold moments create dramatic fills without losing the sub. FILTER mode helps preserve centered low end.

---

## 5. Bass growls from external CLIP abuse
**Goal:** strange layered bass where one signal “imprints” onto another

### Patch
- Bass oscillator into **IN**
- Different oscillator, vocal sample, drum loop fragment, or noise burst into **CLIP**
- TARGET fully or mostly toward **CLIP**
- SHAPE source = **IN** or **OUT**
- THLDs irregular

### Modulation
- LFO/envelope into **TRGT MOD**
- **ABS(IN)** into **SHIFT**
- **DELAY** into **FOLD** attenuated
- occasional **HALT** triggers

### Why it works
The manual notes CLIP can be a different signal than the input. This lets one waveform act like the target/overlay behavior for another, which is incredible for hybrid bass textures.

---

# Patch ideas for haunting atmospheric pads

Skorpion can do beautiful, uneasy pad textures if you stop thinking of it as only a destroyer.

---

## 1. Drifting haunted pad
**Goal:** evolving, spectral, asymmetric pad with movement

### Patch
- Slow-moving chord or single saw/triangle into **IN**
- Lower **FOLD**
- Medium **SLOPE**
- TARGET between **SLIDERs** and **CLIP**
- OUTPUT in **WIDE**
- OUTPUT switch = **FILTERs**
- SHAPE source = **DELAY**

### Modulation
- Slow sine LFO into **SHIFT**
- Very slow LFO into **SHAPE**
- **DELAY out** into **TRGT MOD**
- THLD LFOs from macro section enabled at low amount/rate
- Macro envelope with long attack/release

### Why it works
The delayed signal feeding shape or target adds memory-like spectral smearing. Slow SHIFT motion creates the ghostly “frequency shift” feel described in the manual.

---

## 2. Broken choir / tape-warp pad
**Goal:** unstable, breathing, damaged-analog atmosphere

### Patch
- Rich waveform or ensemble source into IN
- **SYNC = SOFT**
- **TARGET = SLIDERs**
- Target order = **TIED**
- THLDs uneven and sparse
- Some TRGT sliders near zero
- **HALT IF TARG=0 = ON**

### Modulation
- Slow random CV into **SHIFT**
- Slow envelope into **SLOPE**
- SHAPE source = **DAC** or **TRGTs**
- **TRGTs output** to external reverb/filter modulation

### Why it works
Targets at zero can pause portions of the internal motion, adding frozen chunks and broken continuity. TIED order makes the target selection feel organic rather than rigid.

---

## 3. Dark resonant cloud
**Goal:** eerie, harmonically rich drone/pad

### Patch
- Drone oscillator, filtered noise, or feedback loop into **IN**
- TARGET closer to **CLIP**
- Feed another slow-moving oscillator into **CLIP**
- OUTPUT in **WIDE**
- SHAPE source = **OUT** or **DELAY**
- SLOPE moderate-high
- FOLD moderate

### Modulation
- **DIFF** very lightly into **SHAPE**
- **DAC** into **SHIFT**
- super slow macro modulation on SHAPE and FOLD
- use **DELAY out** externally through reverb, then optionally back into CLIP or TRGT MOD

### Why it works
Separate input and clip sources create spectral superposition. Gentle feedback makes it breathe without becoming too aggressive.

---

## 4. Evolving stepped pad / spectral sequencer
**Goal:** pad that feels like it has internal harmonic stages

### Patch
- Sustained oscillator into IN
- TARGET = **SLIDERs**
- TRGT sliders set to contour: low-mid-high-mid-low etc.
- THLDs arranged to determine how often different segments activate
- target order = **SEQ**
- SHAPE source = **TRGTs**

### Modulation
- Slow LFO into **FOLD**
- Slow LFO into **SHIFT**
- **COUNT/** into **TARGET CV** very lightly
- threshold LFO amount low, threshold LFO rate very low

### Why it works
The pad internally moves through destination voltages and slope shapes as thresholds activate, which sounds almost like wavetable scanning or spectral frame interpolation.

---

# Specific modulation strategies that work especially well

## A. Audio-rate modulation
Skorpion explicitly supports audio-rate CV on THLD-related inputs, and its architecture loves fast modulation.

Try audio-rate modulation into:
- **FOLD** for brutal upper partial shredding
- **SHIFT** for metallic asymmetry
- **SHAPE** for unstable sideband-like motion
- **THLDs/** for global moving threshold geometry
- **TRGT MOD** for aggressive target corruption

Especially good for:
- metallic snares
- neuro bass
- alien drones

---

## B. Self-patching recipes

## 1. DIFF -> SLOPE
The classic chaos patch.
- Start with low attenuation
- Adds intense harmonic edge
- Great for basses and industrial percussion

## 2. COUNT -> SHIFT
Creates stepped asymmetry as threshold activity changes.
- Great for talking basses
- Also good on pads for mechanical movement

## 3. DAC -> SHAPE
A more controlled version of COUNT-driven shaping.
- Great for subtle evolution
- Excellent on pads and rolling basses

## 4. DELAY -> TRGT MOD
Creates memory/imprint behavior.
- Feels like spectral afterimage
- Great on haunted textures and wide basses

## 5. TRGTs -> external filter cutoff
Lets threshold activity sequence another module.
- Great for integrated bass patching
- Makes one voice feel like multiple coordinated systems

## 6. ±G(DIR) -> SHAPE or external VCA
Alternates behavior depending on whether the vector core is rising or falling.
- Creates push-pull asymmetry
- Very expressive for bass growls

---

# How to use the macro section musically

The internal macro system is easy to overlook, but it is perfect for animated patches.

## Best uses
- put slow internal LFOs on **FOLD**, **SHIFT**, and **SHAPE**
- use the **macro envelope** to fade modulation in over long phrases
- use very long attack and release for evolving pads
- use short attack / medium release for bass notes that bloom into chaos
- use threshold LFO amount/rate for subtle constant movement in threshold positions

## Great performance trick
Set:
- macro attack = medium or long
- macro release = long
- FOLD and SHAPE in LFO mode
- SHIFT in ENV mode

Then toggle the macro envelope on/off during a phrase. This makes a patch “wake up” and then slowly decay back to stability.

---

# Switch combinations that are especially powerful

## SYNC
- **HARD**: best for drums, punchy basses, more assertive attacks
- **SOFT**: best for pads, smeared textures, less clicky resets
- **X**: freer, often more chaotic/organic

## TARGET ORDER
- **SEQ**: more structured, great for bassline design
- **TIED**: more unstable, expressive, alive

## EQUALIZE THLDs
- **ON**: classic, more controlled
- **OFF/JACK**: more character and irregularity
- modulating this is very effective for fills and transitions

## DRY IF NO THLDs
- useful when heavily modulating FOLD
- keeps sound present instead of disappearing
- especially valuable in bass patches

## OUTPUT switch
- **DC**: raw, direct, often best for distortion and hard percussion
- **FILTERs**: best for polished bass music and wide pads, because lows stay centered and highs widen

---

# Three “signature” advanced patch concepts

## 1. Threshold-switched bass architecture
Use a gate sequence into **EQ THLDs jack** so every few steps the module flips between:
- equalized thresholds = stable bass growl
- custom thresholds = chaotic mutant bass

Then use:
- **COUNT/** -> filter cutoff
- **DIFF** -> subtle SLOPE
- OUTPUT in FILTERs mode

This gives very performable bassline variation.

---

## 2. Cross-imprinted percussion
Use one signal at **IN** and a different percussive or tonal source at **CLIP**.

Examples:
- kick in, snare in CLIP
- tom in, metallic FM blip in CLIP
- bass oscillator in, hi-hat loop in CLIP

Then modulate:
- TRGT MOD with envelope
- SHIFT with random
- SHAPE from OUT or DIFF

This makes sounds that feel layered in a very nonstandard way.

---

## 3. Frozen spectral pad
Use:
- TARGET = SLIDERs
- some TRGT sliders at zero
- **HALT IF TARG=0 = ON**
- slow modulation of threshold activity
- SHAPE source = DELAY
- OUTPUT wide with FILTERs

This creates a moving pad where certain segments freeze into flat planes before melting back into motion.

---

# Quick starting settings by genre

## Distorted percussion
- SYNC: HARD
- TARGET: 5V or CLIP
- SHAPE source: DIFF or OUT
- THLDs: irregular
- FOLD: medium-high
- SLOPE: high
- OUTPUT: mostly wet, DC mode

## Dubstep / DnB bass
- SYNC: HARD or X
- TARGET: SLIDERs or CLIP
- target order: TIED for chaos, SEQ for groove
- SHAPE source: OUT / DIFF / DAC
- SHIFT: modulated slowly
- OUTPUT: WIDE with FILTERs

## Haunting pads
- SYNC: SOFT
- TARGET: SLIDERs / CLIP blend
- SHAPE source: DELAY / TRGTs / DAC
- THLD LFOs: subtle and slow
- macro attack/release: long
- OUTPUT: WIDE with FILTERs

---

# Final practical advice

## Best “sweet spot” habits
- Start with **THLDs not equalized**, then toggle equalize to compare
- Use **SHIFT** more than you think; it is one of the module’s most characterful controls
- For bass, keep **FILTERs** stereo mode on so low end stays solid
- For aggressive sounds, patch **DIFF** somewhere
- For evolving sounds, patch **DAC** or **DELAY**
- Explore **CLIP with a different source**—this is one of the most unique features in the module
- Don’t overlook **HALT** and **HALT IF TARG=0** for rhythm and segmentation

## If you only try 5 modulation patches, try these first
1. **DIFF -> SLOPE**
2. **COUNT -> SHIFT**
3. **DELAY -> TRGT MOD**
4. **Audio oscillator -> FOLD CV**
5. **External source into CLIP**

If you want, I can also turn this into:
- a **10-patch cookbook**
- a **“best self-patching matrix” table**
- or a **genre-specific cheat sheet** for only percussion, only bass, or only ambient textures.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)