# Intellijel — Micro VCF

- [Manual PDF](../../manuals/uvcf_manual_2021.08.15.pdf)

---

[Manual PDF](attachment)

# Intellijel µVCF — using it for melodic musical parts

The attached manual is for the **Intellijel µVCF**, a compact **state variable filter**. Even though it’s “just a filter,” it can contribute a lot to **melodic content** because it can work in two main roles:

1. **As a tone-shaping filter** for an oscillator or other sound source  
2. **As a self-oscillating sine-wave voice** that can track pitch melodically

## What the module does

The µVCF provides:

- **LPF output**: 2-pole low-pass, 12 dB/oct
- **HPF output**: 2-pole high-pass, 12 dB/oct
- **BPF output**: band-pass output
- **FREQ** control for cutoff
- **Q** control for resonance
- **FM1** CV input with attenuator, which can act as **1V/oct**
- **FM2** CV input with **bipolar attenuator**, so modulation can be positive or inverted
- Self-resonance that can produce a **low-distortion sine wave** over a wide range

## Best melodic uses

## 1. Use µVCF as a sine-wave oscillator

This is the most directly melodic use.

The manual says the module:

- tracks **1V/oct over 4+ octaves**
- can be used as a **low-distortion sine VCO when self-resonating**

### Basic patch

- Patch your sequencer or keyboard **pitch CV** into **FM1**
- Turn the **FM1 attenuator fully clockwise** so it tracks **1V/oct**
- Turn **Q** up to maximum so the filter self-oscillates
- Take audio from **LPF**, **BPF**, or **HPF** output
- Send that output to a **VCA**, then to your mixer/output
- Use an envelope to open the VCA

### What this gives you

A clean, stable **sine voice** for:

- basslines
- simple leads
- sub-bass
- FM-style melodic layers
- doubled lines under another oscillator

Because it’s a sine, it sits very well in a mix and is especially useful for **foundation melodies** or **countermelodies**.

## 2. Use it as a melodic filter on another oscillator

Patch any pitched source into **IN**:

- VCO saw
- pulse
- triangle
- wavetable source
- noise for more experimental pitched sounds

Then:

- take one of the filter outputs
- modulate **FREQ** with envelopes, LFOs, or pitch-related CV
- use **Q** to emphasize harmonics near the cutoff

### Why this is melodic

A filter becomes melodic when the cutoff movement is tied to the note being played.

For example:

- Send the same sequence pitch CV to the oscillator and to **FM1**
- Tune the filter cutoff so it follows the note
- Add some resonance

This creates:

- vowel-like lead sounds
- plucky basses
- acid-like melodic phrasing
- harmonically animated arpeggios

## 3. Parallel melodic voicing from the three outputs

A big strength here is the **simultaneous outputs**.

You can patch:

- **LPF** to one VCA/channel
- **BPF** to another
- **HPF** to a third

Then mix them in different proportions.

### Musical uses

- **LPF** for body and warmth
- **BPF** for nasal, focused melodic midrange
- **HPF** for thin, bright articulation

This lets one source become a more complex melodic instrument.

For example:

- LPF as the main bass tone
- BPF as a midrange layer
- HPF mixed quietly for attack detail

If you have separate VCAs, you can even envelope each output differently for animated melodic phrasing.

## 4. FM-based melodic animation

The module “responds very well to frequency modulation.”

That matters musically because you can patch:

- **sequencer pitch CV** to **FM1**
- **envelope**, **LFO**, or another oscillator to **FM2**

Use **FM2** for expressive movement while **FM1** holds the note pitch relationship.

### Good musical examples

#### Vibrato lead
- Pitch CV into **FM1**
- Slow LFO into **FM2**
- Small positive FM2 amount
- Self-oscillating sine out to VCA

Result: expressive sine lead.

#### Pitch envelope pluck
- Pitch CV into **FM1**
- Fast decay envelope into **FM2**
- Slight FM2 amount
- High Q or self-oscillation

Result: percussive, struck melodic tones.

#### Audio-rate FM color
- Pitch CV into **FM1**
- Another oscillator into **FM2**
- Moderate FM2 amount

Result: more complex sidebands and metallic melodic timbres.

Because **FM2** is bipolar, you can invert the modulation for different contour shapes.

## 5. Tracking filter for harmonic emphasis

If you’re using µVCF after a normal oscillator, one powerful patch is to make the filter partially track pitch.

### Patch idea

- Oscillator audio into **IN**
- Sequencer pitch CV multed to:
  - oscillator 1V/oct
  - µVCF **FM1**
- Set **FM1 attenuator** somewhere below full
- Use **LPF** or **BPF** out

Now the cutoff rises as notes rise.

### Why this helps melodically

Without tracking, the timbre may feel inconsistent across the keyboard range.  
With tracking, each note keeps a more similar harmonic character.

That is especially useful for:

- basslines that stay punchy across octaves
- leads with stable brightness
- melodic sequences that sound “played,” not static

## 6. Resonant band-pass melodies

The **BPF** output can be especially musical.

Feed it with a harmonically rich oscillator like a saw wave, then:

- increase **Q**
- tune **FREQ** to the musical range
- optionally patch pitch CV into **FM1**

This creates:

- reed-like tones
- vocal-ish lines
- focused melodic hooks
- pseudo formant sweeps

Band-pass is great when you want a melody that cuts through a dense arrangement.

## 7. Self-oscillation plus external audio

Another nice melodic technique is layering the self-oscillating sine with filtered source audio.

### Patch concept

- External oscillator into **IN**
- Turn **Q** high enough to ring or self-oscillate
- Pitch CV into **FM1**
- Take one filter output

Now the output contains:

- the incoming source being filtered
- the resonant sine component near cutoff

This can make a note feel like it has an internal tuned resonance, almost like:

- a second oscillator
- a tuned resonator
- a vocal/acoustic body resonance

Very useful for melodic leads and basses.

## Practical melodic patch recipes

## Patch 1: Simple sine bass voice

- Sequencer pitch CV → **FM1**
- FM1 attenuator → fully clockwise
- **Q** → high / self-oscillating
- **LPF out** → VCA → mixer
- Gate → envelope → VCA CV

Use **FREQ** to tune the base pitch range.

Sound: pure, round bass.

## Patch 2: Clean lead voice

- Keyboard/sequencer CV → **FM1**
- Q at self-oscillation
- **BPF** or **LPF** out → VCA
- Envelope on VCA
- Slow LFO → **FM2** for vibrato

Sound: pure lead with expressive movement.

## Patch 3: Acid-ish melodic line from another oscillator

- Saw oscillator → **IN**
- Sequencer CV multed to oscillator and **FM1**
- Envelope or accent CV → **FM2**
- **LPF out** → VCA/mixer
- Increase **Q**

Sound: resonant, animated sequence.

## Patch 4: Formant-style melody

- Saw or pulse oscillator → **IN**
- **BPF out** → VCA/mixer
- Pitch CV → oscillator and a bit to **FM1**
- Envelope → **FM2**
- Moderate to high **Q**

Sound: vocal, nasal, cutting melodic timbre.

## Patch 5: Three-layer melodic split

- Oscillator → **IN**
- **LPF**, **BPF**, **HPF** all patched to separate VCAs or mixer channels
- Use different envelope depths or levels on each path

Sound: one melody with low/body, mid/focus, and bright/attack layers.

## Important note on the manual’s instructions

The manual text on the last page appears to contain a likely typo/inconsistency about knob directions for self-oscillation and 1V/oct behavior. Earlier sections are clearer:

- **FM1 attenuator fully clockwise** = unattenuated, tracks **1V/oct**
- **Full Q** = self-resonance and sine generation

Those are the settings to trust for melodic oscillator use.

## Strengths of the µVCF in melodic systems

This module is especially good if you want:

- a compact filter that can also become a **spare oscillator**
- **clean sine tones**
- pitch-tracked resonance
- flexible multi-output filtering for layered melodic voices
- FM-capable, compact utility in a small rack

## Limitations to keep in mind

On its own, the µVCF is not a complete melodic voice. For typical musical use, you’ll still usually want:

- a **sequencer or keyboard CV source**
- a **VCA**
- an **envelope generator**
- optionally another **oscillator**
- mixer/output module

But if your system already has those, the µVCF can become either:

- the **main pitched source**
- or the **timbre-defining melodic shaper**

## Bottom line

The µVCF works well for melodic music in two especially useful ways:

1. **Self-oscillating sine oscillator with 1V/oct tracking** for basss, leads, and simple tonal lines  
2. **Pitch-trackable resonant filter** for shaping another oscillator into expressive melodic parts

Its simultaneous outputs and dual FM inputs make it more musically flexible than a basic small filter, especially in compact Eurorack systems.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)