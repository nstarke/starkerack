# Noise Engineering — Terci Ruina

- [Manual PDF](../../manuals/Terci Ruina - Noise Engineering Documentation.pdf)

---

[Terci Ruina Manual PDF / Documentation](https://manuals.noiseengineering.us/tr/)

# Using Terci Ruina to Create Melodic Components

Terci Ruina is a **triple analog distortion** module, not a pitch or sequencing source by itself. So its role in melodic patching is to **shape harmonics, articulation, and perceived note presence**. In other words, it helps turn simple melodic material into something more expressive, aggressive, and mix-forward.

## What the module does

Terci Ruina contains **three distortion stages in series**, each with its own input and output:

1. **FB** — transistor gain with **silicon diodes in feedback**
2. **FF** — op-amp drive with **silicon diodes in feedforward**
3. **FZ** — **two-stage bipolar transistor fuzz**

The stages are **normalled together**, so if you patch into the first input and take the final output, the signal flows through all three in sequence. You can also patch individual ins/outs to:
- use a single stage alone
- reorder stages
- insert other modules between distortion stages

## How it contributes to melody

Melodic parts need some combination of:
- clear pitch perception
- dynamic contour
- harmonic richness
- separation in a mix

Terci Ruina helps mostly with the last three.

### 1. Add upper harmonics to simple oscillators
If you run a **sine, triangle, or mellow wavetable voice** into Terci Ruina, the distortions create extra overtones. This makes a plain melodic line feel:
- brighter
- more present
- more emotionally intense

This is especially useful if your melody feels too polite or gets buried.

**Patch idea:**
- VCO -> VCA/envelope -> Terci Ruina input 1
- Terci Ruina output 3 -> mixer
- Start with low-to-mid settings on FB and FF
- Use FZ lightly to emphasize edge without losing pitch

This works well for:
- lead lines
- bass melodies
- repeating arpeggios

### 2. Improve note articulation
Distortion exaggerates transients and envelope shape. A plucked or percussive melodic sound becomes more defined, which can make sequences sound more rhythmic and musical.

**Good sources:**
- short-envelope saw or pulse lines
- plucky filtered voices
- resonant lowpass sequences
- FM voices with moderate brightness

For melodic use, try:
- **FB** for nonlinear, asymmetric color
- **FF** for stronger clipping and saturation
- **FZ** for fuzz and tone-shaping character

### 3. Create acid-style melodic lines
The manual specifically recommends using a **filter before or after** Terci Ruina, especially **lowpass or bandpass**. This is one of the best melodic uses.

**Patch idea:**
- VCO -> filter -> Terci Ruina -> VCA
- Sequence pitch from your sequencer
- Use an envelope to modulate the filter cutoff

This can produce:
- acidic basslines
- snarling mono leads
- resonant melodic hooks

You can also reverse it:

- VCO -> Terci Ruina -> filter -> VCA

That gives a different result:
- distortion before filter = raw harmonic generation, then sculpt it
- distortion after filter = preserve filter sweep character, then roughen it up

For melody, both are useful:
- **before filter** tends to sound more controlled
- **after filter** tends to sound more aggressive and immediate

### 4. Use each stage as a different melodic “voicing”
Because the three circuits sound different, you can treat them like alternate tone engines for the same sequence.

For example, mult the same melodic voice and send it to:
- FB for a gritty lead
- FF for a saturated bass double
- FZ for a thinner fuzzy counter-layer

Or send one source through different stages one at a time while composing to decide which distortion best supports the melodic role.

## Character of each distortion for melodic use

## FB
The manual describes FB as:
- two-stage asymmetric diode-feedback topology
- high-beta bipolar transistor gain
- sensitive to waveform symmetry
- especially interesting in the middle of the knob range

**Melodic use:**
- great for adding expressive asymmetry
- especially good on triangles, sines, and simple analog waveforms
- nice for leads where you want personality without full destruction

Because it responds to waveform symmetry, it can make small pitch and timbral differences feel more alive.

## FF
The manual describes FF as:
- asymmetric feed-forward diode clipper
- op-amp gain
- from soft clip to heavy overdrive

**Melodic use:**
- best stage for strong note definition
- good for basslines and hooks
- can make sequenced lines feel bold and compressed

This is probably the easiest stage to use if you want melody to stay recognizable while adding aggression.

## FZ
The manual describes FZ as:
- high-gain bipolar fuzz
- blends differently phased sections
- moves from low-pass to high-pass response as the knob increases
- distortion is subtler, but the filter effect is important

**Melodic use:**
- useful for changing where the melody sits in the spectrum
- lower settings can feel darker/thicker
- higher settings can emphasize bite and cut

This makes FZ especially good for:
- tuning a lead into the right frequency space
- making bass notes poke through
- turning a plain sequence into a focused hook

## Best melodic patch strategies

## 1. Saturated monosynth lead
A very practical melodic patch:

- VCO tuned to your melody
- envelope -> VCA
- VCO -> filter -> Terci Ruina -> delay/reverb -> mixer

Suggested approach:
- FB at low-mid
- FF at low-mid
- FZ to taste

This gives you a lead with:
- harmonic density
- stronger sustain impression
- better cut in a mix

## 2. Acid bassline
- Sequencer pitch CV -> VCO
- Gate -> envelope
- VCO -> lowpass or bandpass filter
- Envelope -> filter cutoff
- Filter -> Terci Ruina
- Terci Ruina -> VCA/mixer

Use FF for the main overdrive and FB for added nonlinear bite.

This is one of the strongest melodic uses mentioned by the design philosophy in the manual.

## 3. Distortion-reordered melody shaping
Since the ins and outs break normalization, you can reorder the stages.

Try:
- source -> FF in
- FF out -> FB in
- FB out -> FZ in
- FZ out -> mixer

Or:
- source -> FZ in
- FZ out -> FF in
- FF out -> mixer

Why this matters musically:
- different stage order changes harmonic development
- one order may preserve pitch clarity
- another may create more expressive instability

For melodic material, start with:
- **FF first** if you want a stable clipped tone
- **FB first** if you want waveform-sensitive coloration
- **FZ last** if you want final tonal emphasis
- **FZ first** if you want filtering/fuzz behavior before harder clipping

## 4. Dynamic melody control with VCA after distortion
The manual notes that if a patch becomes too noisy, placing a **VCA after Terci Ruina** helps.

This is also musically useful:
- distortion generates sustain-like density
- the post-distortion VCA restores note contour
- your melodic phrase stays punchy instead of washing out

**Patch:**
- voice -> Terci Ruina -> VCA -> mixer
- envelope -> VCA CV

This is one of the best ways to keep distorted melodies playable and cleanly phrased.

## 5. Melodic percussion and tuned drums
The manual specifically says drums sound especially good through Terci Ruina, including BIA. That also suggests a melodic use:
- send tuned percussion or pitched drum voices through it
- sequence them melodically
- use the different stages to make them read more as “notes”

This works for:
- tuned kicks
- tom-like synth voices
- percussive bass sequences
- industrial melodic riffs

## 6. Resonator or lowpass gate before/after Terci Ruina
The manual specifically mentions **Sinc Bucina** before or after the module. In broader patch terms, any resonant dynamics processor, LPG, or filter with ringing behavior can work beautifully.

Use this for:
- struck melodic tones
- ringing bass motifs
- plucked resonant sequences

General idea:
- resonant source before distortion = richer, unstable harmonics
- resonant source after distortion = more controlled resonance from a complex signal

## Practical tips for melodic results

## Keep pitch intelligibility under control
Heavy distortion can obscure pitch. To preserve melody:
- use less drive than you think you need
- filter after distortion if needed
- keep the fundamental strong at the source
- use a post-distortion VCA for note definition

## Simple waveforms work best
Because distortion adds harmonics, starting with:
- sine
- triangle
- saw with moderate filtering

often gives the clearest musical result.

If the source is already very complex, Terci Ruina may push it into noise quickly.

## Use mid settings first
The manual specifically notes that **FB has interesting tones in the middle knob range**. That’s often where melodic sweet spots live:
- enough harmonic enrichment
- not so much that the note center disappears

## Let filters do cleanup
A filter after Terci Ruina is extremely helpful for melody:
- tame harsh highs
- emphasize the fundamental
- create vowel-like sweeps
- shape leads and basses into a mix

## Layer dry and distorted signals
If your system allows multing:
- one copy stays clean
- one copy goes through Terci Ruina
- mix both

This can preserve clear pitch while adding body and aggression.

## Summary: best role in melodic patching

Terci Ruina is best thought of as a **melodic tone intensifier**, not a melodic generator.

It is especially strong for:
- aggressive mono leads
- acid basslines
- saturated arpeggios
- tuned percussion riffs
- layering harmonic character onto simple sequenced lines

Its three distinct distortion stages let you move from:
- expressive asymmetry (**FB**)
- strong clipping/overdrive (**FF**)
- fuzz plus tonal emphasis (**FZ**)

For the most musical results, combine it with:
- an oscillator or complete voice
- a sequencer
- a filter
- a VCA/envelope after distortion

That combination gives you distorted tones that still behave like playable melodic material.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)