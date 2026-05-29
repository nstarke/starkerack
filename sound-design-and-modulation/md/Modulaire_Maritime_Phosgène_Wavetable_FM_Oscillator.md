# Modulaire Maritime — Phosgène Wavetable FM Oscillator

- [Manual PDF](../../manuals/Phosgène _ Modulaire Maritime.pdf)

---

[Manual PDF / Source](https://www.modulaire-maritime.com/phosg%C3%A8ne)

# Modulaire Maritime Phosgène — patch ideas and modulation strategies

Phosgène is a **2hp digital wavetable / FM oscillator** with a pretty specific personality:

- **60 wavetables** in **2 banks of 30**
- **Two parallel outputs**:
  - **WAVE**: wavetable + folding/waveshaping character
  - **FM**: separate FM-oriented output
- **Shared controls** affect both engines
- **External CV** can push the timbre deeper
- **Tracks 1V/Oct over 8 octaves**
- **Octave up/down switch**
- **“Octave displace”** function for the wavetable side, useful for darker/lower folded tones
- **100 Hz FM base**, which likely makes the FM side less “glassy DX” and more weighty, restrained, and bass-friendly
- **11-bit / lower-resolution digital behavior** and potential aliasing at extremes — which is actually a feature here

This is not a “clean hi-fi all-rounder” oscillator. It sounds like it wants to make:
- aggressive digital percussion
- nasty basses
- dark folded tones
- haunted, low-res atmospheres

Because there’s very little panel space, the module’s real power comes from **fast CV animation**, **audio-rate modulation from elsewhere**, and **crossfading/mixing the two outputs**.

---

## First: understand the best modulation targets

From the panel and text, the important modulation/performance targets seem to be:

- **1V/Oct**
- **Wave Select CV**
- **FM Mod CV**
- **Octave switches / octave displacement**
- Likely **coarse tuning**

The biggest sound-design trick with this module is to think in **layers of motion**:

1. **Pitch motion** — sequencer, glide, pitch envelopes
2. **Timbre motion** — wave select scanning
3. **Intensity motion** — FM MOD CV amount changes
4. **Register motion** — octave/displace changes
5. **Blend motion** — external crossfade between WAVE and FM outputs

If you patch all 5 at once, even a tiny oscillator becomes huge.

---

# General sound design approach

## 1. Use the two outputs as separate voices
Don’t think of WAVE and FM as just “two flavors.” Treat them as:

- **Body** = WAVE output
- **Attack / edge / growl** = FM output

Patch both into:
- a mixer,
- a crossfader,
- separate VCAs,
- or separate filters.

That lets you shape:
- WAVE for low-end and sustain
- FM for click, metallic transient, or moving upper harmonics

This is probably the single best way to get “finished” sounds from Phosgène.

---

## 2. Slow CV for wavetable position, fast CV for FM MOD
A great rule of thumb:

- **Slow modulation** on **Wave Select**
  - triangle LFO
  - random slew
  - stepped random through a slew limiter
  - envelope with long attack/decay

- **Fast modulation** on **FM MOD CV**
  - snappy envelope
  - short decay envelope from trigger
  - audio-rate oscillator
  - burst generator / random pulse logic

This yields the classic “stable core + unstable edge” behavior that works especially well for bass and percussion.

---

## 3. Exploit aliasing instead of avoiding it
The manual explicitly says:
- high octaves
- folded timbres
- noise-containing waves
- lower-resolution digital playback

…can produce digital trash.

Good. Use it.

For modern bass music and industrial percussion:
- send the oscillator high
- add aggressive modulation
- then **filter down afterward**
- or resample into a sampler / looper

Often the ugliest raw tone becomes the most powerful once low-passed, saturated, and enveloped.

---

# Patch ideas for distorted percussive sounds

These are ideal because Phosgène already has a digital edge and the FM side can create sharp transients.

---

## 1. Digital kick-drone hybrid

### Patch
- **1V/Oct**: no sequence or fixed low pitch
- **WAVE out** → VCA → low-pass filter → mixer
- **FM out** → separate VCA → mixer
- Trigger a **snappy pitch envelope** into **1V/Oct**
- Trigger a **very short decay envelope** into **FM MOD CV**
- Trigger another envelope to open the WAVE VCA slightly longer than the FM VCA

### What happens
- The pitch envelope gives the kick “thump”
- The FM envelope creates a click/snap or tearing front edge
- The WAVE output provides body
- The FM output provides attack grit

### Tips
- For harder kicks, increase the pitch envelope amount
- For more “broken speaker” character, use a noisier wavetable and high FM MOD
- If the kick is too tonal, scan to a less harmonic wave
- Add a wavefolder, distortion, or clipping after the mixer

---

## 2. Snare from wavetable dirt

### Patch
- Tune the oscillator to mid/high register
- Use a wavetable that contains noise or inharmonic content
- **Wave Select CV**: modulate with a short envelope or random stepped voltage
- **FM MOD CV**: hit with a second short envelope
- Send output through:
  - band-pass filter, or
  - high-pass + VCA

### Layering strategy
- **FM output** = noisy crack
- **WAVE output** = resonant body

### Enhancement
Add:
- short reverb
- gated room reverb
- parallel distortion

This can make convincing industrial snares or electro “claps from hell.”

---

## 3. Metallic percussion / industrial hits

### Patch
- Tune Phosgène high
- Use **FM output** as the main source
- Send a trigger-derived envelope to **FM MOD CV**
- Send a slightly slower random CV to **Wave Select**
- Use a LPG or VCA with short decay
- Optional: feed through resonator, comb filter, or BBD delay

### Why it works
The 100 Hz base FM character should keep it from getting too brittle while still giving metallic sidebands. Short envelopes on the FM amount create evolving clangs rather than static digital tones.

### For more weirdness
- Clock a sample-and-hold into Wave Select each trigger
- Alternate between Bank 1 and Bank 2 manually while recording
- Use different envelope lengths for WAVE and FM outputs

---

## 4. Glitch hats and broken tops

### Patch
- High pitch
- Choose the brightest/noisiest waves
- Clocked stepped random → attenuator → **Wave Select**
- Very fast envelope or burst modulation → **FM MOD CV**
- Output → high-pass filter → VCA with very short decay

### Bonus move
Patch both outputs to separate VCAs:
- WAVE VCA short decay
- FM VCA ultra-short decay

This gives a layered hi-hat where one layer is body and the other is transient fizz.

---

# Patch ideas for dubstep / drum & bass basslines

This is probably where Phosgène shines. The module’s darker FM base and rough digital tone are perfect for hostile low-end.

---

## 1. Reece-style digital bass

### Patch
- Sequence **1V/Oct**
- Use **WAVE output** and **FM output** at the same time
- Detune externally by multing pitch:
  - one output dry
  - one copy through a tiny pitch offset source if available
  - or use a second oscillator layered underneath
- Slow LFO or envelope follower → **Wave Select**
- Medium envelope → **FM MOD CV**
- Both outputs into saturation/filter chain

### Suggested processing
- low-pass filter with moving cutoff
- mild overdrive before filter
- heavier distortion after filter
- stereo chorus or microdelay after everything

### Result
You get a gnarly, animated digital reece with:
- moving harmonic center from wavetable scan
- midrange growl from FM
- dirt from the 11-bit/aliasing texture

---

## 2. Talking dubstep wobble

### Patch
- Sequence bass notes
- **WAVE out** → low-pass or band-pass filter
- **FM out** → separate band-pass or direct distortion path
- LFO synced to tempo → filter cutoff
- A different LFO or envelope → **Wave Select**
- Accent triggers → **FM MOD CV**

### Performance trick
Use accents only on certain steps:
- normal notes = mostly WAVE
- accented notes = FM MOD opens up and adds snarling upper harmonics

This creates the classic bassline pattern where some notes “speak” harder than others.

### Better still
Use a sequential switch or crossfader to alternate:
- mostly WAVE on one bar
- more FM on the next
- mixed on fills

---

## 3. Neuro-style movement bass

### Patch architecture
- **WAVE output** → filter A
- **FM output** → filter B or distortion
- Modulate:
  - **Wave Select** with a slow, irregular CV
  - **FM MOD CV** with a looping envelope
  - filter A cutoff with one LFO
  - filter B cutoff with another LFO at a different rate

### Why it works
The bass becomes complex because multiple layers move at different timescales:
- wavetable movement = identity drift
- FM modulation = aggression pulses
- split filtering = morphing formants

### Key technique
Record 3–5 minutes of improvisation and resample the best phrases. This kind of oscillator excels at finding accidental sweet spots.

---

## 4. Brutal bass stabs

### Patch
- Put the oscillator in lower register using octave displacement for the WAVE side
- Sequence short staccato notes
- Trigger:
  - short envelope to VCA
  - pitch envelope to 1V/Oct
  - short aggressive envelope to FM MOD CV
- Mix WAVE and FM outputs
- Add hard clipping and low-pass filtering after

### Sound result
You’ll get bass stabs with:
- sub impact from WAVE
- ripping upper transient from FM
- a “compressed” digital slam when clipped

This is ideal for:
- halftime dubstep hits
- DnB foghorn-adjacent one-shots
- warehouse techno bass punctuation

---

## 5. Foghorn-inspired patch

Phosgène may not be a traditional foghorn machine, but you can absolutely push it there.

### Patch
- Low note sequence
- Moderate glide/portamento in your pitch source
- **WAVE output** as main bass source
- **FM output** mixed low for bark
- Slow envelope or LFO to **Wave Select**
- Another envelope with more depth on accented notes to **FM MOD CV**
- Filter with resonance after mixing
- Distortion before or after the filter depending on taste

### Important move
Use the **octave displace** function to keep the wavetable side lower and heavier while the FM side retains more range/attack.

That separation can make the patch feel much larger.

---

# Patch ideas for haunting atmospheric pads

A 2hp digital oscillator can absolutely do pads, especially when you embrace the haunted low-res vibe.

---

## 1. Frozen ghost pad

### Patch
- Tune low to mid register
- Use **WAVE output** as primary source
- Slow triangle or random slew → **Wave Select**
- Very subtle slow modulation → **FM MOD CV**
- Send through:
  - low-pass filter
  - long reverb
  - stereo delay / chorus

### Best practice
Keep the modulation depth small. Tiny movements matter a lot on digital oscillators. Too much CV may turn “haunting” into “cartoonish.”

### Good result
A murky, unstable, almost tape-corrupted pad texture.

---

## 2. Split-output spectral pad

### Patch
- **WAVE output** → low-pass filter → reverb
- **FM output** → high-pass filter → shimmer reverb or delay
- Same pitch to both, but process differently

### Modulation
- slow LFO on **Wave Select**
- even slower LFO or random drift on **FM MOD CV**
- manual octave shifts while recording long drones

### Why it works
The WAVE side becomes the pad’s body, while the FM side becomes a mist of unstable harmonics above it.

This is one of the most effective “small module, big texture” techniques.

---

## 3. Worn VHS choir / digital fog

### Patch
- Pick a wavetable with some internal noise or complex harmonic profile
- Low or mid pitch
- Slow attack envelope into VCA
- Slow CV drift into Wave Select
- Slight random pitch drift via very attenuated random voltage to 1V/Oct
- Heavy chorus / wow-flutter / reverb after

### Optional
Mix in a tiny amount of FM output for grain and air.

This creates a pad that feels old, sick, and emotionally unstable in a good way.

---

## 4. Dissonant cinematic drone

### Patch
- Drone the oscillator with no gate
- Use **FM output** more prominently than usual
- Apply slow, deep modulation to **FM MOD CV**
- Use slow stepped random or sample-and-hold with slew on **Wave Select**
- Process through resonant filter and long dark reverb

### Technique
Move the octave switch manually during recording. The abrupt digital register shifts can sound extremely cinematic, especially when drowned in reverb tails.

---

# Modulation tricks that will make this module stand out

---

## 1. Envelope the wavetable position per note
Instead of static wave selection, patch an envelope to Wave Select so each note starts bright and settles darker, or vice versa.

This is one of the best ways to create:
- punchy bass articulation
- percussive transients
- evolving pads

A tiny envelope amount can make a patch feel alive.

---

## 2. Use different CV sources for Wave Select and FM MOD
Avoid using the same LFO for both. Better combinations:

- Wave Select = slow triangle
- FM MOD = rhythmic envelope

or

- Wave Select = slewed random
- FM MOD = audio-rate oscillator

or

- Wave Select = sequencer lane
- FM MOD = accents from trigger sequencer

That separation creates the impression of a much deeper instrument.

---

## 3. Audio-rate modulation from another oscillator
If you have another VCO/LFO:
- patch it into **FM MOD CV**
- keep the amount low first
- then increase until harmonics become unstable

This is especially strong for:
- metallic percussion
- tearing basses
- dystopian drones

If the input accepts wide enough modulation, you can get pseudo-phase-distortion / chaotic wavetable tearing behavior.

---

## 4. Modulate around sweet spots, not across the whole range
With small digital oscillators, the best sounds often live in narrow windows.

Use:
- attenuators
- offset generators
- CV mixers

to find one sweet wavetable region, then wiggle around it rather than scanning the whole bank.

This is crucial for pads and basses.

---

## 5. Use sequenced CV for timbre, not just pitch
Send a stepped modulation lane into:
- Wave Select
- FM MOD CV
- or both via attenuverters

Then each sequenced note can have its own timbre identity. This is how you get basslines that sound “spoken” or “designed,” rather than just played.

Perfect for:
- DnB call-and-response
- dubstep growl patterns
- glitch percussion sequences

---

# Three complete recipe patches

## A. Distorted industrial tom/snare bank
- Phosgène tuned mid-low
- Trigger sequencer to envelope generator
- Envelope 1 → VCA for WAVE output
- Envelope 2 (shorter) → FM MOD CV
- Stepped random per hit → Wave Select
- WAVE + FM outputs mixed
- Into distortion, then band-pass filter

**Variation:** increase pitch envelope for toms, reduce it for snare-like hits.

---

## B. Dubstep monster bass
- Bass sequence into 1V/Oct
- Glide on selected notes
- WAVE output → LPF
- FM output → distortion path
- Sync LFO to filter cutoff
- Accent envelope → FM MOD CV
- Slow random → Wave Select
- Recombine paths and compress lightly

**Performance move:** manually flip octave/displace during fills and resample the result.

---

## C. Haunted pad wash
- Sustained note or slow chord sequencing from another voice layered with Phosgène
- WAVE output dominant, FM output quiet
- Very slow LFO → Wave Select
- Very slow random drift → FM MOD CV
- Attenuated random pitch drift
- Low-pass filter
- Long dark reverb + chorus

**Performance move:** manually change banks between long held notes.

---

# Best external modules to pair with Phosgène

This oscillator will especially benefit from:

- **Attenuators / attenuverters**
- **Fast envelopes**
- **Random CV**
- **Crossfaders**
- **Dual VCAs**
- **Filters** with character
- **Distortion / wavefolder / clipping**
- **Stereo effects**
- **Resamplers / loopers**

If you only add one utility, make it a **CV attenuator/offset** module. Tiny control is everything here.

---

# Final thoughts

Phosgène seems best approached as a **digital character oscillator**, not a pristine “do-everything” VCO. Its strengths are exactly the things many modules try to hide:

- roughness
- fold brightness
- limited-resolution grit
- aliasing
- dark FM
- unstable/noisy waves

For your target sounds:

- **Distorted percussion:** use short envelopes on pitch and FM MOD, randomize wave position per hit, and layer WAVE + FM separately.
- **Dubstep / DnB bass:** sequence pitch, animate Wave Select slowly, hit FM MOD rhythmically, split and process both outputs differently.
- **Haunting pads:** keep modulation subtle, scan narrow timbral zones, exploit low-res instability, and let reverb/delay magnify the ghostliness.

The secret with this module is not complexity on the panel — it’s **careful external CV animation** and **separate treatment of its two outputs**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)