# Modulaire Maritime — Phosgène Wavetable FM Oscillator

- [Manual PDF](../../manuals/Phosgène _ Modulaire Maritime.pdf)

---

[Manual / Source](https://www.modulaire-maritime.com/phosg%C3%A8ne)

# Modulaire Maritime Phosgène — rhythmic and hyper-complex percussion use

Phosgène is a **2hp digital wavetable / FM oscillator voice**, so for dense percussion it works best as a **sound source** that you hit, gate, frequency-modulate, fold, and switch rapidly with CV. Based on the manual, the key percussion-friendly features are:

- **60 wavetables** in **2 banks of 30**
- **Separate wavetable and FM outputs**
- **Wavefolding / waveshaping**
- **CV over folding / FM depth behavior**
- **V/Oct tracking over 8 octaves**
- **Octave up/down switching**
- **Octave displace switch** for pushing wavetable octaves lower
- **100 Hz FM base**, giving a darker, tighter FM character
- **11-bit lower-resolution digital tone**, including useful grit/aliasing

That combination is excellent for **synthetic drums, metallic hits, digital toms, clanks, glitches, zaps, and pseudo-snare/hat material**.

---

## Core idea: Phosgène is not the sequencer, it is the drum engine

To get **polyrhythms, odd meters, and hyper-detailed percussion**, use external modules to provide:

- **Triggers/gates**
- **Envelopes**
- **VCAs / LPGs**
- **Sequenced CV**
- **Clock dividers / multipliers**
- **Logic / probability / ratchets**
- **Sequential switches / sample & hold**

Phosgène then becomes a **highly mutable oscillator voice** that can sound like many different percussion instruments depending on how you drive it.

---

# Best patch role for Phosgène in complex percussion

## 1. Turn it into a drum voice with a VCA or LPG
Because it is an oscillator, the simplest path to percussion is:

**Phosgène output → VCA or LPG → mixer**

Then patch:
- **Trigger pattern → envelope**
- **Envelope → VCA CV**

This gives each note a defined transient and decay.

### Why this matters
Even if the raw oscillator is continuous, the VCA/LPG creates:
- kick-like plucks
- tom hits
- snappy FM pings
- clipped digital clicks
- short metallic bursts

For denser rhythmic music, use **very short decay envelopes** for some channels and **longer decays** for others so overlapping subdivisions remain readable.

---

## 2. Use the two outputs as two related percussion layers
The manual says wavetable and FM are available through **separate outputs**. That is extremely useful.

### Patch concept
- **Wavetable out** = body / fundamental / tone
- **FM out** = snap / metallic edge / noisy overtone layer

Try:
- Send each output to its **own VCA**
- Use **different envelopes** on each
- Mix them after

### Example
- Wavetable out: medium decay envelope for a tom/kick body
- FM out: very short envelope for click/attack

This creates a **single composite drum voice** with more impact.

You can also sequence them differently:
- Wavetable on quarter-note skeleton
- FM out on offbeats, tuplets, ratchets, or polymetric accents

That yields one module behaving like **two interlocked percussion voices**.

---

# Sound design for punchy percussion

## 3. Low octaves + short envelopes = kicks and toms
The manual notes that the **octave displace** function pushes wavetable octaves lower. That is ideal for percussion.

### For kicks
- Use **wavetable output**
- Set to a **low octave**
- Enable **octave displace** if needed
- Choose a waveform with solid low content
- Add a **pitch envelope** via V/Oct input:
  - fast attack
  - very short downward drop

This creates classic synthesized kick behavior.

### For toms
- Similar to kick patch, but:
  - less pitch envelope
  - slightly higher base pitch
  - moderate fold amount
  - medium-short decay

Sequence toms across different pitches using a CV sequencer in **odd step lengths** like 5, 7, or 9.

---

## 4. FM output for metallic percussion, snares, and industrial hits
The manual’s 100 Hz FM base suggests darker, more controlled FM. That’s especially useful for:
- industrial knocks
- tuned metal
- snare-like digital impacts
- electro percussion
- low metallic bass percussion

### Patch approach
- Use **FM output**
- Set a mid or low pitch
- Use short VCA envelope
- Modulate the shared controls with stepped CV
- Push FM harder for harsher attacks

For snare-adjacent sounds:
- Mix **FM output** with a noise source, or
- Use a noisier wavetable at higher fold settings

Because the module has some intentional lower-resolution character, you can also lean into the grit for **crunchy transient texture**.

---

## 5. Exploit aliasing and 11-bit character for hats, clicks, and digital debris
The manual explicitly mentions:
- noise-containing wavetables
- more pronounced aliasing at high ranges
- “digital trash”

That is excellent for percussion.

### For hats and ticks
- Use **high octave**
- Fast envelope
- Select brighter/noisier waves
- Add wavefolding
- Sequence with irregular trigger streams

### For glitch percussion
- Rapidly modulate:
  - wave selection
  - bank selection if available by switch/performance
  - octave state
  - folding amount

If you cannot CV bank directly, you can still perform manual changes or use the module as a “featured” unstable digital percussion voice.

Use this in:
- 13-step pattern against a 16-step kick grid
- 5-over-4 accents
- burst generators
- Euclidean trigger streams

---

# Strategies for polyrhythms and complex patterns

## 6. Use different rhythmic layers on wavetable and FM outputs
Since there are two outputs, treat them as separate voices in rhythm.

### Example polymeter patch
- **Wavetable output** triggered by a **7-step sequence**
- **FM output** triggered by a **5-step sequence**
- Master clock still in 4/4 or 11/8

Result:
- shifting accents
- repeating composite cycle every 35 steps
- strong hyper-rhythmic texture from one module

---

## 7. Sequence pitch separately from amplitude triggers
For complicated percussion, don’t think melodically first—think **event structure**.

Use:
- one sequencer for **triggers**
- another sequencer for **pitch CV**
- another modulation lane for **wave/fold amount**

### Good pattern lengths
- Trigger pattern: 16
- Pitch sequence: 5
- Fold modulation: 7
- Accent envelope: 3 or 9

These mismatched lengths create evolving composite phrases without requiring constant manual intervention.

---

## 8. Use V/Oct as a percussion animation lane
Because it tracks across **8 octaves**, V/Oct is not only for melody. In percussion patches it becomes a way to create:

- kick vs tom contrast
- tuned percussion runs
- pseudo-congas
- stuttering tonal impacts
- pitched accents in odd meters

### Great use case
Program a pattern in **11/8** where:
- steps 1, 4, 7, 10 = low thumps
- intervening hits jump 1–3 octaves
- FM layer remains constant or inversely modulated

This keeps the groove asymmetrical but coherent.

---

## 9. Use octave jumps as accents
The module has octave switching and octave displacement. Even if not voltage-addressable, these can still be used compositionally.

### Method
Set the module in a range where:
- regular hits are mid-low
- accented sections are manually or sequentially repatched to another octave CV region

If your sequencer can send transposition CV:
- use fixed intervals for “accent classes”
- e.g. main hits low, ghost hits high and thin, fills very high and aliased

This is especially effective in:
- 7/8 with occasional 3-note fill
- 5/4 with one high digital accent every second bar
- nested 3:5:7 percussion systems

---

# Advanced percussive patch ideas

## 10. Composite kick/snare from one module
### Patch
- **Wavetable out** → VCA 1 → mixer
- **FM out** → VCA 2 → mixer

Control:
- Envelope 1: short decay, some pitch envelope to V/Oct
- Envelope 2: ultra-short decay, more aggressive modulation

Pattern:
- Wavetable layer on beats 1 and 3
- FM layer on 2 and 4, plus ghost notes

Result:
- one oscillator acting like a paired drum machine voice

In odd meter:
- body layer on a 4-hit cycle
- FM layer on a 3-hit cycle
- creates constant phase-shifting accents

---

## 11. Industrial rim / clang voice
### Patch
- FM out
- Mid-high pitch
- Very short envelope
- Moderate to high fold/FM tone setting
- Optional bandpass filter after VCA

Sequence with:
- sparse irregular triggers
- probability skips
- 5-step pattern over 4/4 kick
- occasional ratchets

This gives machine-like, hard-edged percussion suitable for industrial, IDM, broken techno, and rhythmic noise.

---

## 12. Digital hi-hat cluster generator
### Patch
- High-pitched wavetable or FM output
- Tiny envelope decay
- Fast clocked modulation to wave select or fold depth
- Highpass filter after the VCA if available

Then feed triggers from:
- Euclidean pattern of 9 in 16
- burst generator for fills
- logic-combined clocks, e.g. /3 XOR /5

The module’s aliasing and low-resolution edge help make each hat cluster sound less static.

---

## 13. Evolving percussion swarm
Use 3 modulation streams at once:

- **Trigger stream A** controls amplitude
- **Stepped random CV** to V/Oct
- **Slow CV** to fold/waveshape amount

Then run triggers at one length and pitch CV at another:
- triggers in 13 steps
- pitch in 8
- fold modulation in 5

Over time Phosgène will move through:
- low thuds
- hollow pings
- metallic cracks
- bright digital splinters

Perfect for dense, self-evolving rhythmic beds.

---

# How to make it more unique and percussive

## 14. Add pitch envelopes
This is one of the most important techniques.

Patch a snappy envelope to the **V/Oct input** through an attenuator.

### Results
- fast downward pitch sweep = kick, tom, zap
- tiny pitch spike = stronger attack
- medium sweep = laser percussion / electro tom

For complicated rhythms, vary the envelope amount by accent so different hits read like different drum types.

---

## 15. Use very short VCAs for click extraction
Even without dedicated transient shaping, an ultra-short envelope can carve clicks and ticks from almost any oscillator setting.

Try:
- 1–10 ms decay
- high or aliased wavetable
- no sustain

This is a great way to create:
- microsound percussion
- granular-seeming ticks
- top-layer detail over slower drum patterns

Use these in tuplets or odd subdivisions to make the rhythm feel hyper-detailed.

---

## 16. Layer filtered and unfiltered versions
Split one output:
- one path direct
- one path through filter/distortion/wavefolder

Then mix.

This gives:
- stable low-end body
- aggressive upper transient

Especially useful when a single Phosgène hit needs to cut through dense polyrhythmic arrangements.

---

## 17. Use modulation as “drum type switching”
Instead of thinking “this patch is a kick,” let modulation determine whether any given trigger becomes:
- a kick
- a tom
- a click
- a metallic ping
- a snare-like burst

You do this by changing, per event:
- pitch
- envelope decay
- fold amount
- output choice
- filtering after the module

This is ideal for complex pattern music because a single voice can generate many timbral identities while staying sonically related.

---

# Rhythm system ideas that work especially well

## 18. 4-against-5-against-7
Use Phosgène as the bright or metallic voice in a larger drum system.

Example:
- Kick module: 4-step cycle
- Phosgène wavetable body hits: 5-step cycle
- Phosgène FM accents: 7-step cycle

This creates a long composite loop with constant internal motion.

---

## 19. Odd meter phrase design
In **11/8**:
- steps 1, 4, 7 = low wavetable thuds
- steps 3, 6, 9, 11 = FM metallic ticks
- wave/fold modulation every 5 steps

This produces a phrase that feels composed rather than random.

---

## 20. Accent logic with probability
Use probabilistic triggers or logic to decide when the FM layer opens.

For example:
- every main trigger hits the wavetable body
- FM layer only opens on:
  - every 3rd trigger
  - random 40% probability
  - XOR of two clocks

That creates unstable, intelligent-feeling complexity without overwhelming the groove.

---

# Practical tips

## 21. Keep low end controlled
Because Phosgène can go low and also bright through folding, separate roles carefully:
- one patch for sub/body
- another path for bright detail

If the patch gets too dense:
- shorten envelope decays
- highpass the bright layer
- reduce modulation depth on busy subdivisions

---

## 22. Save useful startup states
The manual says it saves:
- Bank
- wave
- octave

So if you find a strong percussion setup, you can keep a preferred startup configuration ready for future patches.

That makes it practical as a repeatable drum voice in performance systems.

---

## 23. Embrace the “digital trash”
The manual explicitly frames aliasing and low-res behavior as part of the character. For hyper-complex percussion, that is a strength.

Use it for:
- tops
- transitions
- fills
- machine chatter
- broken digital strikes

Don’t over-clean it unless you want a more conventional sound.

---

# Best companion modules for this purpose

Phosgène becomes much stronger for rhythmic complexity when paired with:

- **Envelope generators** with very fast attack/decay
- **VCAs** or **LPGs**
- **Clock dividers/multipliers**
- **Euclidean sequencers**
- **Trigger sequencers with independent track lengths**
- **Logic modules**
- **Sample & hold / stepped random**
- **Sequential switches**
- **Filters / distortion / wavefolders**
- **Accent VCAs or transient shapers**

---

# Bottom line

Phosgène is very usable for **dense, polyrhythmic percussion** because it offers:

- low-end capable wavetable tones
- separate FM and wavetable outputs
- dark, controlled FM character
- folding / timbral movement
- wide pitch range
- useful digital grit and aliasing

The best strategy is to treat it as a **multi-role synthetic drum voice**:
- **wavetable out** for body
- **FM out** for attack/metal layer
- external envelopes and VCAs for articulation
- independent trigger and CV sequences for polymetric evolution

That will get you kicks, toms, hats, metallic impacts, clanks, glitch hits, and industrial percussion from one very small module.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)