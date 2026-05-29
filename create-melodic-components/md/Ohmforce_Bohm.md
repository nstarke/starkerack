# Ohmforce — Bohm

- [Manual PDF](../../manuals/Bohm documentation.pdf)

---

[Ohm Force Bohm Eurorack Manual](https://ohmforce.com/wp-content/uploads/2025/03/Bohm-Manual.pdf)

# Using Bohm, Groove, and Performer to create melodic components

Although **Bohm** is presented as a stereo dual-voice **kick** system, the manual makes it clear that it can do much more than drum duties. Used together, **Bohm + Groove + Performer** can become a compact **melodic bass / riff / drone / resampling / performance FX voice** for Eurorack.

## Big picture

These modules can create melody in four main ways:

1. **Bohm as a pitched synth voice**
   - The manual explicitly states that **pitch tracking can be used to play bass lines**.
   - Bohm’s kick engine becomes a playable oscillator/enveloped synth when you use:
     - **PITCH CV**
     - a long enough **LENGTH**
     - optionally a **gate** on **HIT** instead of a short trigger

2. **Groove as a second related melodic voice**
   - Groove is a second kick voice triggered by **CLOCK**
   - Its **PITCH** and **LENGTH** are **relative to Bohm**
   - That makes it ideal for:
     - harmonically related bass doubling
     - octave / interval reinforcement
     - rhythmic melodic repeats
     - drones and rumble beds

3. **Performer as a melodic processor**
   - Performer adds:
     - stereo input
     - ducking
     - performance FX
     - selectable processing of **kick**, **input**, or **both**
   - This means Bohm/Groove can be used as melodic sources, while Performer shapes them into playable transitions, filter sweeps, beat-roll textures, and sidechained musical layers.

4. **Snapshots and Live modes as “preset melody states”**
   - A snapshot stores:
     - model variations
     - knob positions
   - Programs and Live modes let you sequence or cue different melodic states:
     - bassline section
     - chorus octave
     - breakdown drone
     - distorted lead-like hit

---

# 1. Bohm as a melodic voice

## Pitch tracking

The most important melodic feature in the manual is here:

- Bohm **PITCH** spans approximately **C1 to C2**
- It supports **1V/oct pitch tracking**
- For proper pitch tracking:
  - set **PITCH knob fully counterclockwise**
  - set **PITCH attenuverter fully clockwise**
  - choose the proper **Pitch CV system setting**:
    - `0..1V`
    - `1..2V`
    - `2..3V`
  - ensure your sequencer outputs **1 Volt per octave**

This means Bohm can function as a **monophonic bass synth voice** over a one-octave window, depending on configuration and model behavior.

## Use HIT as a gate, not only a trigger

The manual says:

- **HIT can work both as a trigger or a gate**
- If **HIT remains on**, the kick sustains
- When HIT is released, the sound decays

For melody, this is huge. It means you can send:
- a **gate sequence**
- a keyboard/gate
- a sequencer with variable gate lengths

This transforms Bohm from a percussive one-shot into a **sustained playable voice**, especially for:
- basslines
- drone notes
- acid-like plucks
- sustained sub melodies

## Envelope controls for note shaping

Even when using Bohm melodically, the kick controls become useful synth-shaping controls:

- **LENGTH** = total note duration / tail length
- **SUSTAIN** = body/level of the sustained note
- **ATTACK** = transient amount and attack emphasis
- **CURVE** = pitch envelope behavior
- **TRS DECAY** = click/transient duration
- **TRS TONE** = transient brightness
- **COLOR** = timbral evolution of the oscillator
- **FX** = post effect amount

So for melodic use:
- reduce transient-heavy settings for smoother notes
- lengthen **LENGTH**
- increase **SUSTAIN**
- use **HIT gate** for true sustain
- use **COLOR** and **FX** as musical tone controls

## Which Bohm models are most melodic?

From the manual, these are especially promising:

### FM-2X
Best for:
- FM basslines
- techno bass melodies
- metallic subs
- playable low-end riffs

Why:
- 2-operator FM structure
- **ATTACK** controls FM amount
- **TRS TONE** changes modulator waveform
- **RATIO** variation changes harmonic relationship

Musically, this can move from:
- clean sine-ish bass
- to punchy FM bass
- to more overtone-rich melodic lines

### HZ-1
Best for:
- classic electronic basslines
- smoother melodic kick-bass hybrids

Why:
- wavetable oscillator + transient synth
- analog-style wavetable options
- variable click choices

### VX-T
Best for:
- sharper, articulated melodic parts
- percussive leads
- bass + hi-click hybrid sequences

Why:
- transient synth is more pronounced and tunable
- can create top-heavy melodic attacks

### WT-4
Best for:
- rounded “analog-style” melodic bass
- layered, musical low-end phrases

### SP-6 / PX3
Best for:
- more aggressive melodic content
- industrial / experimental riffs
- textured bass hooks

### XT-88
Best for:
- custom melodic design

Why:
- load your own **wavetables**
- load your own **samples**
- tune **BRIGHT** and **LAYER VOL**
- create a hybrid oscillator + sampled layer melodic voice

This is probably the most powerful model if your goal is to turn Bohm into a custom bass instrument.

### PM-K1
Less useful for conventional melodic sequencing:
- It is a **physical model of an acoustic bass drum**
- many usual controls are inactive
- Groove is not supported with it

Still usable for tuned tom-like or acoustic drum-pitched lines, but not the first choice for melodic work.

---

# 2. Groove as a second melodic layer

Groove is described as a **secondary kick voice**, often for rumbles or tops. But the architecture makes it very useful melodically.

## Groove follows Bohm

Its key melodic behavior:

- **PITCH on Groove is relative to Bohm PITCH**
- **LENGTH on Groove is relative to Bohm LENGTH**
- center position = same as Bohm
- left = lower than Bohm, but not below Bohm minimum
- right = higher than Bohm, but not above Bohm maximum

This means Groove is ideal for making a **dependent second voice**, such as:

- tuned reinforcement
- note doubling
- octave-above or octave-below feel
- interval-shifted taps
- moving rumble tied to the bassline

## Groove sound generators as melodic textures

Groove contains 4 sound generators:

1. **Repetitions of the Bohm kick**
2. **Kick reverb**
3. **Noise**
4. **Grit + sub frequency**

Selected/blended with **COLOR**.

### Repetition mode
This is the most obviously melodic:
- every **CLOCK** trigger retriggers a “tap”
- these are not delayed echoes; they are fresh rhythmic retriggers
- tap levels are controlled by:
  - **2**
  - **3**
  - **4**
  - **TAPS CV**

This can create:
- bass arpeggio-feel repeats
- galloping subs
- ratcheted low-end motifs
- pseudo-sequenced melodic subdivisions

If Bohm is pitch-tracked, Groove’s repetitions inherit a harmonically related pitch context.

### Reverb / noise / grit+sub modes
These are not “pitched melody” in the classic sense, but they are useful for **melodic support layers**:
- resonant rumble tails
- tuned sub under a note
- noisy top texture following a bass phrase
- sustained drone synced to melodic events

## Groove can become a drone

The manual notes:
- **GRV ENV** system option can be:
  - `FALL`
  - `SUSTAIN`

With `SUSTAIN`, Groove can hold after the 4th tap level, which is excellent for:
- bass drones
- sustained harmonic beds
- one-note underpinning below a melody
- transitions and breakdowns

Also:
- **Perf Vol option** can be set so Performer VOL controls only **BOHM**
- the manual says this allows **Groove to drone without hearing the Bohm kick**

That is extremely useful melodically:
- Bohm can act as the triggering/pitched event source
- Groove can become the sustained note layer

## Groove FX as tonal shaping

Groove effect variations:
- **LP**
- **HP**
- **BP**
- **DIST**

This means Groove can function as:
- a filtered bass shadow
- a band-passed tonal repeat layer
- a high-passed melodic top
- a distorted harmonic duplicate

And **STEREO** width can widen the melodic layer spatially.

---

# 3. Performer as the melodic glue and live processor

Performer is not a voice generator by itself, but in a melodic patch it becomes the key to making Bohm/Groove feel like a complete musical instrument.

## External audio as another melodic source

Performer has:
- stereo **IN**
- ducking based on **HIT**
- effects
- routing selector

So you can bring in:
- another oscillator voice
- a chord source
- a sampler loop
- a drone
- a bassline from another module

Then combine it with Bohm/Groove.

## Ducking for rhythmic phrasing

The external input is ducked on every **HIT**.
That means if you send in a drone, pad, or sustained oscillator:
- Bohm can carve rhythmic space into it
- creating a pulsing harmonic layer
- synced to the melodic bass events

Performer variations make this more subtle and musical:
- **DUCK TIME** = release time
- **DUCK SMTH** = smoothing
- **DUCK BS** = band split frequency

This is great for melody because you can:
- duck only lows while preserving highs
- create sidechained bass + sustained top
- keep chord clarity while pulsing the low band

## Selective FX routing

Performer **CHN** variation:
- `ALL`
- `KICK`
- `INPUT`

This allows several melodic configurations:

### KICK only through FX
Use if Bohm/Groove are your melodic voice and you want:
- filter sweeps on the bassline
- beat roll on the bass
- live stutter transitions

### INPUT only through FX
Use if Bohm is your rhythmic melodic anchor and incoming audio is a pad/lead/drone.

### ALL
Process the full combined musical texture.

## Performer effects for melody

Available variations:
- **DJ FILTER**
- **HP**
- **LP**
- **BEAT ROLL**
- **SLIP ROLL**

These are excellent for melodic performance:

### DJ FILTER
- center is neutral
- CCW low-pass
- CW high-pass
- **DJ RESO** controls resonance

Perfect for:
- opening/closing basslines
- breakdown filtering
- morphing a bass phrase into a thin lead-like line
- isolating highs from an incoming melodic texture

### HP / LP
Useful for:
- carving low-end vs top-end
- creating arrangement movement
- making one melodic layer sit behind another

### BEAT ROLL / SLIP ROLL
These can turn sustained or repeating melodic material into:
- glitch fills
- stutters
- rhythmic note slicing
- end-of-phrase transitions

---

# 4. Practical melodic patch strategies

## A. Bohm as a bass synth voice

**Patch**
- Sequencer pitch CV -> **PITCH CV**
- Sequencer gate -> **HIT**
- Audio from **OUT**

**Set**
- PITCH knob full CCW
- PITCH attenuverter full CW
- system **Pitch CV** to correct range
- **LENGTH** fairly long
- **SUSTAIN** up
- moderate **ATTACK**
- reduced transient if too clicky

**Result**
- monophonic bassline voice
- especially strong with **FM-2X**, **HZ-1**, **WT-4**, **XT-88**

---

## B. Bohm bassline + Groove octave/tap melody

**Patch**
- Same as above
- Clock divider/multiplier or 16th clock -> **Groove CLOCK**

**Set**
- Groove **PITCH** slightly above or below center
- Groove **LENGTH** to taste
- Use **2 / 3 / 4** to shape repeats
- Groove **COLOR** toward repetition source
- Groove **FX** with BP or DIST

**Result**
- Bohm gives the root note
- Groove gives related rhythmic melodic taps
- feels like a bassline with ratchets or ghost notes

---

## C. Bohm as note attack, Groove as sustained drone

**Patch**
- Melodic gate/pitch into Bohm
- Regular clock into Groove
- Use Performer if available

**Set**
- Groove system **GRV ENV = SUSTAIN**
- Groove level up
- Bohm more transient-forward
- If Performer present, set **PERF VOL = BOHM** so Groove can remain independent
- Optionally duck external audio with Performer

**Result**
- Bohm articulates notes
- Groove forms sustained harmonic/sub layer
- excellent for techno hypnosis and dark ambient low-end melody

---

## D. Bohm + external oscillator/chords through Performer

**Patch**
- Bohm sequenced melodically
- External stereo or mono voice into Performer **IN**
- Optionally send a chord or drone source

**Set**
- **DUCK** to taste
- **DUCK BS** so low band ducks more than highs
- **CHN = INPUT** or `ALL`
- Use **DJ FILTER** or **LP**
- toggle FX synced to **HIT** for phrase changes

**Result**
- Bohm acts as rhythmic/melodic bass anchor
- incoming voice becomes breathing accompaniment
- very effective for live melodic techno

---

## E. Snapshot-based melodic arrangement

Because snapshots save:
- model variations
- knob positions

you can prepare multiple melodic identities:
- Step 1: clean FM sub bass
- Step 2: brighter distorted chorus bass
- Step 3: long drone breakdown
- Step 4: filtered/stuttered fill

Then use:
- **Song mode** for fixed arrangement
- **Jam mode** for improvisational cueing

This is one of the strongest non-obvious melodic uses in the manual: Bohm becomes a **preset-morphing low-end instrument** rather than just a kick generator.

---

# 5. Best model choices for different melodic roles

## Best for basslines
- **FM-2X**
- **HZ-1**
- **WT-4**
- **XT-88**

## Best for aggressive riffs
- **PX3**
- **SP-6**
- **OLP4**

## Best for custom melodic sound design
- **XT-88**

## Best for acoustic/tuned drum melodies
- **PM-K1**

## Best for clicky articulated phrases
- **VX-T**

---

# 6. Most useful system settings for melodic use

These matter a lot.

## Pitch CV
Set to:
- `0..1V`
- `1..2V`
- `2..3V`

depending on your sequencer’s voltage span.

## ATTVERT 2
The **SUSTAIN attenuverter** can instead control **VELOCITY CV**.
This can be useful if you want more expressive sequencing of note dynamics rather than sustain amount.

## GRV ENV
- `FALL` for rhythmic behavior
- `SUSTAIN` for drones and held layers

## TAPS OUT
Can output:
- Groove envelope
- inverted Bohm envelope
- Performer envelope
- Bohm envelope

This is very useful for melodic patches because you can use the output to animate other modules:
- open a filter on another oscillator
- duck a bass drone
- modulate VCA on a melodic layer
- create envelope-following accompaniment

## PANNING
You can hard-pan:
- Bohm
- Groove
- Performer input

This is surprisingly useful for melodic patching:
- route Bohm to left and Groove to right
- process them separately downstream
- build mono dual-line structures from the stereo output

## POST EQ
Useful for tuning Bohm/Groove into a more musical role in a mix:
- tame club boom
- emphasize note definition
- shape bassline presence

---

# 7. Creative melodic techniques

## Use Bohm as a limited-range but very characterful bass synth
It won’t replace a full-range oscillator voice, but within its designed range it can produce very strong, mix-ready melodic low-end.

## Use Groove as “melodic repetition” rather than rumble
Because Groove repetitions are retriggered taps, not delay echoes, they can sound tighter and more intentional than a traditional delay.

## Turn kick changes into harmonic section changes
Different Bohm models and snapshots can behave like:
- verse bass
- chorus bass
- breakdown drone
- fill/stutter preset

## Use Performer to make melodies breathe
With selective ducking and filter FX, Performer can make even static external melodic material feel locked to the kick/bass phrasing.

## Use XT-88 to build a custom melodic hybrid
Load:
- your own wavetable for pitch body
- your own sample for attack/layer

That gives you a very personalized bass instrument.

---

# 8. Limitations to keep in mind

## Bohm is not a general-purpose wide-range melodic oscillator
The manual frames pitch around **C1 to C2**, so this is mainly:
- bassline territory
- low melodic hooks
- tuned percussive phrasing

## Model interpretation varies
Each model interprets controls differently, so “melodic sweet spots” will vary significantly by model.

## Groove pitch is relative, not fully independent
This is great for coherence, but less ideal if you want a completely separate second melody.

## Model loading time matters in live sequencing
In Song mode, steps need enough time for preloading. Extremely rapid melodic preset switching may be constrained.

---

# 9. Best real-world musical roles

Used together, these modules are especially good for:

- **melodic techno basslines**
- **industrial bass riffs**
- **electro low-end hooks**
- **acid-adjacent FM sub sequences**
- **drone + pulse hybrid lines**
- **live performance transitions**
- **sidechained melodic layering**
- **preset-based bass arrangement changes**

In practice, the strongest melodic identity of the system is:

> **Bohm = pitched low-end voice**  
> **Groove = related rhythmic/sub/drone companion**  
> **Performer = sidechain, filter, and transition processor for the whole musical layer**

That combination makes the system much more than a kick module—it can function as a **complete low-end melodic instrument with performance control**.

---

# 10. Recommended starter melodic patches

## Patch 1: FM techno bass
- Model: **FM-2X**
- Pitch sequence -> PITCH CV
- Gate -> HIT
- Long LENGTH
- Medium SUSTAIN
- ATTACK moderate
- TRS DECAY low
- Groove on 16ths, low in mix

## Patch 2: Rolling melodic rumble
- Bohm plays root bassline
- Groove CLOCK on 16ths
- Groove COLOR toward repetitions/reverb blend
- Groove PITCH slightly above center
- Groove BP effect
- Performer DJ filter on ALL

## Patch 3: Drone bass with rhythmic articulation
- Bohm receives sparse gated notes
- Groove set to **SUSTAIN**
- Performer ducks incoming drone or chord source
- Use TAPS OUT or Bohm env to animate another VCA/filter

## Patch 4: Custom hybrid bass
- Model: **XT-88**
- User wavetable for oscillator
- User sample for layer
- Sequence PITCH CV and HIT gate
- Snapshot several variants for song sections

---

## Bottom line

**Yes—these modules can absolutely be used to create melodic components.**  
Not as a conventional polysynth, but as a highly characterful **low-register melodic system**.

If you think of them as:

- **Bohm:** a playable kick-bass oscillator voice
- **Groove:** a harmonically linked second voice / repeater / drone
- **Performer:** a sidechaining and FX performance mixer

then together they become a powerful tool for **bass melodies, rhythmic melodic motifs, drones, and live-evolving low-end arrangements**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)