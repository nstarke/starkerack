# Happy Nerding — FM AID

- [Manual PDF](../../manuals/FM-AID-USERS-GUIDE_2020.pdf)

---

[FM AID Manual PDF](https://happynerding.com/wp-content/uploads/2020/12/FMAID_manual_2020.pdf)

# Happy Nerding FM AID: using it for melodic musical parts

The attached manual covers **one module: Happy Nerding FM AID**.  
So rather than discussing a multi-module system from the PDFs, I’ll explain how **FM AID works with the other kinds of Eurorack modules you likely already have** to build melodic voices, leads, basses, plucks, bells, and evolving tonal parts.

## What FM AID does musically

FM AID is an **analog through-zero linear FM processor**. In practice, it takes:

- a **Carrier** signal at the **CAR input**
- a **Modulator** signal at the **MOD input**
- optional FM-depth control at the **CV input**

and gives you **four simultaneous outputs**:

- **Square**
- **Saw**
- **Sine**
- **Triangle**

If the **carrier is a saw wave**, those outputs behave like wave-shaped versions of the FM result:
- sine = mellowest
- triangle = slightly brighter
- saw = bright
- square = brightest

That makes FM AID especially useful for **melodic duties**, because you can keep one pitch structure but choose different harmonic flavors from the outputs.

## Important manual points that matter in patching

From the manual:

- Preferred signal levels are roughly **-5V to +5V**
- The **FM knob** sets modulation depth/index
- The **CV knob** is **bipolar** and adds/subtracts incoming CV from the FM amount
- **CAR is normalled to MOD** when nothing is plugged into MOD
  - so one oscillator can act as both carrier and modulator
- It works best with **saw as carrier** if you want the named output shapes to behave as labeled
- There is an **onboard trim** for carrier amplitude calibration if the saw output shows artifacts
- Feedback patching from an output back into MOD can produce more aggressive/noisy/digital-like textures

---

# Best ways to use FM AID for melodic components

## 1. Simple 1V/oct melodic voice

This is the most direct use.

### Patch
- VCO A saw output → **CAR**
- VCO B output (sine or triangle is a great start) → **MOD**
- Same **1V/oct pitch sequence** → VCO A and VCO B
- FM AID output (start with **Sine** or **Triangle**) → VCA → filter or straight to mixer
- Envelope → VCA CV
- Optional envelope/LFO/sequencer lane → **CV input**

### Musical result
This gives you a very playable FM voice where:
- pitch remains melodic and trackable
- harmonic complexity comes from the modulator
- different outputs give multiple timbral versions of the same note line

### Why it works
Sending the same melodic pitch CV to both oscillators keeps their ratio fixed, which is ideal for **stable, tonal FM melodies**.

### Good ratios to try
Tune the modulator relative to the carrier:
- **1:1** = solid, centered, classic FM tone
- **2:1** = brighter, more overtone-rich lead or bass
- **3:2** = musical and slightly more complex
- **3:1 / 4:1** = bell-like or metallic
- **1:2** = hollow, subtler upper structure

For melodic writing, start with:
- bass: **1:1 or 2:1**
- lead: **1:1, 3:2, 2:1**
- bells/mallets: **3:1 or 4:1**

---

## 2. Single-oscillator melodic folding voice

Because **CAR is normalled to MOD**, you can patch only one oscillator.

### Patch
- One saw VCO → **CAR**
- Leave **MOD unpatched**
- Pitch sequence → that oscillator’s 1V/oct
- FM AID **Sine/Triangle/Saw/Square output** → VCA → mixer
- Envelope or LFO → **CV input** or manually use FM knob

### Musical result
This gives you a compact melodic voice with a kind of **self-FM / wavefolding-adjacent behavior**.  
It’s not ratio FM in the classic two-oscillator sense, but it can produce:
- animated basses
- growling leads
- harmonically rich mono lines

### Best use
Great if you only have one primary oscillator available but still want a more complex melodic timbre.

---

## 3. Envelope-controlled FM plucks

One of the most musical uses of FM AID is making the FM amount dynamic.

### Patch
- Carrier VCO saw → **CAR**
- Modulator VCO sine/triangle → **MOD**
- Shared pitch CV to both oscillators
- Short decay envelope → **CV input**
- Set **CV knob positive**
- FM AID output → VCA → mixer
- Another envelope → VCA

### Musical result
At the attack, the FM index is high, so the sound is bright.  
As the envelope falls, the tone becomes purer and more focused.

This is excellent for:
- plucks
- electric piano-ish tones
- marimba-like tones
- expressive sequences

### Why this is especially good
This is one of the classic FM behaviors that reads immediately as “musical.”  
You get transient brightness without the note staying harsh.

---

## 4. Velocity-sensitive melodic phrasing

The manual specifically suggests **note velocity** into the CV input.

### Patch
- Velocity CV from MIDI-to-CV or sequencer → **CV input**
- Set **CV knob** to positive or negative amount
- Normal melodic FM voice patch as above

### Musical result
Harder-played notes become:
- brighter
- more complex
- more aggressive

Softer notes stay:
- rounder
- cleaner
- more sine-like

This is extremely useful for expressive:
- bass lines
- leads
- keyboard performance patches

It’s one of the easiest ways to make an FM voice feel alive in a track.

---

## 5. Pitch-dependent timbre compensation

The manual also points out using **pitch CV** in the CV input.

### Why do this?
FM timbre often changes across the keyboard. Sometimes higher notes get too bright or too thin.

### Patch
- Mult your pitch CV
- One copy to oscillator 1V/oct inputs
- Another copy to **CV input**
- Use the **CV knob**:
  - **positive** = brighter as notes go higher
  - **negative** = less FM as notes go higher

### Musical result
This helps balance a melodic patch across its range.

### Practical uses
- **Negative CV setting** is great for bass/lead patches where high notes otherwise get too glassy
- **Positive CV setting** is useful when you want a more synth-pop or digital-style brightness curve

This is a very strong “make it sit in the mix” trick.

---

## 6. Stable melodic intervals with synced oscillators

The manual recommends **hard-synced oscillators** to reduce beating and keep the tone static.

### Patch
- Carrier oscillator as the master melodic oscillator
- Modulator oscillator hard-synced to carrier
- Both tuned to a chosen ratio
- FM AID patched normally

### Musical result
You get a more locked, stable harmonic tone, which is especially useful when:
- writing tonal melodies
- layering with other harmonic instruments
- recording repeated sequences that need consistency

### Best for
- tight basses
- precise arpeggios
- repeated melodic hooks

---

# Understanding the four outputs in a musical context

A big advantage of FM AID is that it gives **four tonal variants at once**.

## Sine output
Use for:
- bass fundamentals
- mellow leads
- sub-rich melodic support
- layering under brighter outputs

It’s the safest starting point for tonal material.

## Triangle output
Use for:
- woody leads
- rounded arps
- melodic lines that need clarity without too much bite

This is often the sweet spot for melodic content.

## Saw output
Use for:
- cutting hooks
- bright sequences
- acid-adjacent lines
- melodic parts that need to stand in front of a mix

Good when you want the FM motion to remain obvious.

## Square output
Use for:
- very bright lead tones
- chiptune-adjacent melody colors
- aggressive arps
- heavily articulated riffs

Can get intense quickly, especially at higher FM settings.

### Very useful trick
Mult or record multiple outputs:
- Sine for body
- Triangle for definition
- Saw or Square for edge

Then mix to taste.

---

# Patch recipes for actual melodic roles

## A. FM bassline

### Patch
- Carrier saw VCO → CAR
- Modulator sine VCO → MOD
- Same pitch CV to both
- Modulator tuned **1:1** or **2:1**
- FM AID **Sine** or **Triangle** out → lowpass filter → VCA
- Snappy envelope to VCA
- Small positive envelope to CV input

### Result
Punchy, harmonically rich bass that still tracks well and keeps low-end focus.

### Tips from the manual
If the bass loses weight as FM increases:
- lower the carrier octave
- lower modulator pitch
- use sine or triangle as modulator

These are directly recommended in the manual and are very effective.

---

## B. Glassy lead

### Patch
- Carrier saw → CAR
- Modulator sine/triangle → MOD
- Shared pitch CV
- Tune modulator to **2:1** or **3:1**
- Use **Triangle** or **Saw** output
- Add moderate FM
- Add aftertouch/velocity/mod wheel CV to CV input

### Result
Expressive FM lead with playable timbral dynamics.

### Performance idea
- low FM for verses
- increase FM manually for choruses or solos
- use velocity for accent notes

---

## C. Bell or mallet sequence

### Patch
- Carrier saw → CAR
- Modulator sine → MOD
- Ratio **3:1, 4:1, or 5:1**
- Short decay envelope into CV input
- Set FM knob low to medium
- Use **Sine** output first
- Fast VCA envelope

### Result
Tonal percussive sequence with a bright attack and cleaner tail.

### Why it works
Classic FM bell behavior comes from:
- nontrivial frequency ratios
- decaying modulation index

FM AID is ideal for this.

---

## D. Animated arp with audio-rate CV modulation

The manual explicitly notes that **audio-rate signals can be patched into the CV input**.

### Patch
- Normal melodic FM voice
- Additional oscillator or audio LFO → **CV input**
- CV knob to taste
- Arpeggiator or step sequencer driving pitch

### Result
A moving, animated harmonic texture where the FM index itself is being modulated at audio rates.

This can produce:
- vocal-like shifting tones
- unstable digital-esque arps
- richly animated sustained notes

Keep this subtle for musical melodic use.

---

## E. Self-feedback lead/noise edge patch

The manual describes sending an output back into **MOD** for feedback.

### Patch
- Oscillator saw → CAR
- FM AID output (start with triangle or saw) multed:
  - one copy → mixer/VCA
  - one copy → **MOD**
- Increase FM gradually

### Result
Starts as aggressive self-FM and can become noisy, tearing, or quasi-digital.

### Musical use
Best for:
- climactic lead lines
- industrial melodies
- transitions
- high-intensity fills

This is usually less “clean melodic” and more “expressive special effect,” but very useful in arrangement.

---

# How to pair FM AID with common Eurorack module types

## With oscillators
Best pairing. You usually want:
- a **saw carrier**
- a **sine or triangle modulator** to start

If your oscillators have stable tracking, FM AID becomes a strong melodic voice core.

## With quantizers/sequencers
Excellent. Use them to:
- keep pitch ratios musical
- automate melodic movement
- send accent/velocity lanes to CV input

A sequencer with extra CV lanes makes FM AID much more expressive.

## With envelopes
Essential for melodic articulation:
- one envelope for amplitude
- another for FM depth via CV input

This is one of the best pairings.

## With filters
Very useful, though not always necessary.
FM already creates harmonic motion, but a filter helps:
- tame harshness
- emphasize sweet spots
- shape bass vs lead role

## With VCAs
Important if you want dynamic control over:
- output loudness
- modulator amplitude before FM AID
- CV depth sent to the CV input

A VCA on the modulator path can be extremely musical.

## With mixers/attenuverters
Helpful for:
- blending outputs
- controlling modulation depth
- offsetting the CV input
- creating parallel voices

---

# Practical melodic strategies

## Keep ratios simple first
For tonal music, start with:
- 1:1
- 2:1
- 3:2

These are easier to tune and sit better harmonically.

## Use the CV input like a “brightness animation” input
Think of FM AID’s CV input less as abstract modulation and more as:
- note attack brightness
- expression
- phrase accent
- register compensation

That mindset makes it much easier to use musically.

## Start from the sine or triangle outputs
If the patch feels unruly, switch to:
- **Sine** first
- then **Triangle**

These outputs preserve musicality better in many melodic contexts.

## Use a saw carrier when you want predictable results
The manual is clear that the module is designed around a saw carrier for the indicated output shapes.

## If the low end disappears, reduce complexity
Again from the manual:
- lower carrier octave
- lower modulator pitch
- use sine/triangle modulator

This is especially important for bass melodies.

---

# A few complete example melodic setups

## Minimal melodic voice
- 2 VCOs
- 1 sequencer
- 1 envelope
- 1 VCA
- FM AID

Patch shared pitch CV to both VCOs, saw to carrier, sine to modulator, triangle out to VCA.  
This gives a clean, controllable FM lead or bass.

## Expressive performance voice
- 2 VCOs
- keyboard/sequencer with velocity
- 2 envelopes
- VCA
- filter
- FM AID

Velocity to CV input, envelope to VCA, optional second envelope to FM depth.  
Great for performable melodic phrasing.

## Evolving melodic drone/sequence
- 2 VCOs
- slow modulator to CV input
- quantized pitch sequence
- FM AID multiple outputs mixed together

This creates a harmonically shifting tonal line that remains melodic but keeps moving.

---

# Calibration note

If the module sounds oddly distorted even at low FM, especially when using a saw carrier, the manual says the **carrier calibration trimmer** may need adjustment.

Basic manual procedure:
- nothing patched to CV or MOD
- saw into CAR
- FM knob fully CCW
- monitor the **saw output**
- adjust trim until the saw is clean and not “two-toothed”

This matters because poor calibration can make melodic patches sound artifacty in an unintended way.

---

# Bottom line

**FM AID is best thought of as a melodic timbre engine for oscillators.**  
It is especially strong for:

- FM basses
- expressive leads
- bell/mallet tones
- plucks with animated attack
- evolving arpeggios
- layered tonal textures from the four simultaneous outputs

Its most musical strengths are:

1. **stable ratio-based FM with two oscillators**
2. **self-patched single-oscillator complexity**
3. **dynamic FM index control via envelopes, velocity, or pitch CV**
4. **multiple simultaneous output flavors from one melodic line**

If you want, I can also turn this into:
- a **set of specific patch diagrams**
- a **“starter patches” cheat sheet**
- or a **module pairing guide** for FM AID with your exact rack.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)