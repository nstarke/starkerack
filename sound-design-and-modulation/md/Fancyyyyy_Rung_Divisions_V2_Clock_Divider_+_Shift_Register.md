# Fancyyyyy — Rung Divisions V2 Clock Divider + Shift Register

- [Manual PDF](../../manuals/RungDivisionsManual.pdf)

---

[Manual PDF](attachment)

# Fancyyyyy Rung Divisions: modulation ideas for aggressive percussion, wild basslines, and eerie pads

Rung Divisions is much more than a clock divider. It’s basically a **clock-derived logic voice generator**, **polyrhythmic gate source**, and **chaotic stepped CV/noise oscillator** in one module.

The key things to exploit for sound design are:

- **Bus1 clocks the universal shift register**
- **Clock divisions /2 through /8 can be mixed to Bus1 and Bus2**
- **Direction can be flipped by gate/CV**
- **Length is voltage controllable**
- **Chance is voltage controllable**
- **Data input is XOR’d**, so external data is inherently destabilized
- **3-bit and 8-bit outputs are DAC-encoded stepped CV/audio outputs**
- **Everything runs from sub-audio up to audio rate**

That means the module shines when you modulate:

1. **Clock rate / clock shape**
2. **Which divisions go to Bus1**
3. **Direction input**
4. **Length CV**
5. **Chance CV**
6. **Data input**
7. **Feedback of 3-bit or 8-bit back into the clock source or data path**

---

# What each control does musically

## Clock input
This is the master energy source. Since the dividers and buses preserve clock pulse width, a clock with PWM or odd waveshaping will strongly affect the sound.

**Use for modulation ideas:**
- Audio-rate square/pulse VCO for harsh digital tone generation
- LFO or trigger train for rhythmic sequencing
- Envelope-modulated oscillator as clock for “hit then decay” percussion

## Bus1 / Bus2
- **Bus1** clocks the shift register
- **Bus2** is a second OR-mixed rhythm stream

These are not just utility outputs. They are compositional tools:
- Bus1 defines *when* the internal pattern updates
- Bus2 can trigger envelopes, resets, direction flips, VCAs, LPGs, wavefolders, or effects

## Length CV
This changes the loop point of the register. Smaller lengths create shorter repeating patterns. Modulating it creates sudden reorganization of the pattern.

**Musically:**
- Short lengths = more repetitive, hooky, riff-like
- Long lengths = more evolving, less predictable
- Fast modulation = glitch, tearing, digital scrambling

## Direction CV
Flips pattern read direction with a trigger/gate. This is one of the most expressive features.

**Musically:**
- Creates palindromic / reversing motion
- Makes basslines “snap backward”
- Creates alternating rise/fall phrases in 3-bit vs 8-bit outputs

## Chance CV
This is huge. Fully clockwise tends to **loop/lock** the pattern. Fully counterclockwise favors **new data/XOR behavior**. Middle positions create unstable noisy interference.

**Musically:**
- CW = repeatable groove
- CCW = mutation/random intrusion
- Mid = unstable sweet spot, very alive

## Data input
Anything crossing 1V works. Since it goes through XOR logic, even simple sources become weird.

**Good data sources:**
- Noise output from the module
- One of the clock divisions
- Bus2
- Another sequencer gate line
- Audio-rate square wave
- Comparator output from a slow CV
- Envelope gate from a drum voice

## 1-bit / 3-bit / 8-bit outputs
- **1-bit**: gate related to the first bit
- **3-bit**: stepped CV with classic rungler flavor
- **8-bit**: longer, more detailed stepped contour

**General feel:**
- 3-bit = coarse, punchy, riff-like
- 8-bit = more complex, more “random sequencer”
- Both at audio rate = digital noise oscillator territory

---

# Core patch philosophy

For the sounds you want, think in 3 layers:

1. **Rhythm source:** use Bus1/Bus2 and divider outputs
2. **Tone source:** use 3-bit or 8-bit at audio rate, or use them to FM/filter-mod another oscillator
3. **Instability source:** modulate chance, length, direction, and data

The magic comes from making one part **repeat** while another part **mutates**.

For example:
- Keep **Chance mostly high** so a motif loops
- Modulate **Direction** every few beats
- Randomly alter **Length**
- Feed **Bus2** to a VCA or wavefolder CV
- Send **8-bit** to oscillator FM and **3-bit** to filter cutoff

That gives repetition plus surprise.

---

# Distorted percussive sounds

Rung Divisions is excellent for metallic, broken, digital percussion because it can generate:
- irregular triggers
- stepped digital timbre
- subharmonic pulse stacks
- chaotic pitch bursts

## 1. Digital kick / broken tom patch
### Patch
- Patch a VCO square or pulse into **Clock**
- Send **/2, /3, /5** to **Bus1**
- Take **Bus1** into a fast-decay envelope or LPG
- Take **8-bit** into oscillator FM input or directly to a filter/FMable voice pitch input
- Take **Bus2** from a different set, like **/4 and /7**, and use it to trigger accent envelopes
- Set **Chance** around 1–2 o’clock
- Set **Length** around 3–5
- Occasionally trigger **Direction**

### Result
You get uneven, lurching drum transients with tonal tails that feel half-synth, half-machine error.

### Make it nastier
- Overdrive the oscillator or filter after the voice
- Use the **3-bit** output instead of 8-bit for rougher pitch jumps
- Put a wavefolder on the voice and modulate fold amount with **Bus2**

---

## 2. Snare / clap from logic chaos
### Patch
- Use audio-rate clock into **Clock**
- Patch **Noise out** to **Data**
- Send **/2 and /7** to **Bus1**
- Send **/3, /5, /8** to **Bus2**
- Use **Bus1** to trigger a short VCA envelope opening the module’s **8-bit** output or a noise source
- Modulate **Chance CV** with a decaying envelope or random stepped voltage
- Send occasional gates to **Direction**

### Why it works
The XOR’d data and unstable chance region create noisy, shifting digital bursts. The polyrhythmic buses give non-static transient timing.

### For clap-like flams
- Send **Bus2** to a second envelope with slightly different decay
- Mix both envelopes into one VCA or into separate VCAs
- Use different divisions on Bus1 and Bus2 so the transients smear in a pseudo-handclap way

---

## 3. Glitched hi-hats / industrial ticks
### Patch
- Audio-rate pulse to **Clock**
- Short pulse-width clock works best
- Use **Noise** or a fast square LFO/VCO into **Data**
- Keep **Length** short, around 2–4
- Modulate **Chance** with a fast but shallow random source
- Use **1-bit** or **Bus2** as trigger streams for hat envelopes
- Use **3-bit** output as audio through HPF/BPF and distortion

### Sound
Harsh, aliased, metallic hats and insect-like ticks.

### Strong trick
Send **Direction** a sparse trigger every bar or half bar. This suddenly reorders the rhythmic microstructure and sounds like ratchets or reverse hats.

---

## 4. FM percussion with self-similar bursts
### Patch
- Use Rung Divisions as modulation brain, not the final audio source
- Clock from an audio oscillator
- Send **3-bit** to linear FM on a sine VCO
- Send **Bus1** to envelope trigger
- Send **Bus2** to VCA CV or LPG strike
- Feed **8-bit** back into the clock oscillator’s pitch or FM amount
- Set **Chance** high enough to repeat, but not fully locked
- Modulate **Length** slowly

### Result
Percussive tones with recurring families of transients—like machine drums that almost repeat but keep mutating.

---

# Crazy basslines for dubstep / drum and bass

This is where Rung Divisions really gets fun. The best approach is to use it as a **hybrid sequencer + modulation source + chaos feedback network**.

---

## 1. Reversing stepped reese bass
### Patch
- VCO square/pulse into **Clock** at sub-audio or low audio rate depending on whether you want sequence CV or direct audio
- Send **/2, /3, /4** to **Bus1**
- Patch **8-bit** to oscillator pitch FM input or quantizer -> VCO pitch
- Patch **3-bit** to filter cutoff
- Use **Bus2** to trigger an envelope for VCA or filter
- Send a rhythmic gate pattern into **Direction**
- Set **Chance** fairly high for loop retention
- Modulate **Length** with a slow triangle LFO or stepped random

### Why it sounds good
The reverse encoding of 3-bit and 8-bit gives contrary motion. When direction flips, one contour rises while the other falls, which is perfect for bass timbre animation.

### For reese energy
- Use two detuned oscillators
- 8-bit modulates one oscillator pitch or FM
- 3-bit modulates filter, wavefolder, or stereo spread
- Distort after filtering

---

## 2. Wobble bass with unstable internal groove
### Patch
- Use a tempo-synced clock into **Clock**
- Send **Clock, /2, /5, /7** to **Bus1**
- Send **/3, /4, /8** to **Bus2**
- Bus1 clocks the register
- Patch **8-bit** to a quantizer for bass pitch
- Patch **Bus2** to filter-envelope trigger or directly to LPG/VCA CV
- Patch **3-bit** to wavetable position, wavefolder amount, or filter FM
- Modulate **Chance CV** from an LFO synced slower than the main tempo
- Trigger **Direction** at phrase boundaries

### Sound
This creates basslines that feel sequenced but unstable, with the rhythmic modulation itself evolving.

### To make it more dubstep
- Put **Bus2** through a clock divider or envelope follower to create half-time wobble accents
- Use **Direction** flips on the 4th or 8th bar
- Push **Chance** toward the middle during fills for mutation, then back up to “lock” for the drop

---

## 3. Self-feeding chaos bass
The manual specifically recommends feeding the 3-bit or 8-bit output back to the clock source.

### Patch
- Audio-rate VCO square to **Clock**
- Send **/2 and /6** or **/2 and /7** to **Bus1**
- Patch **8-bit** back into the clock oscillator’s FM or 1V/oct attenuated input
- Patch **3-bit** to a filter or second oscillator FM
- Patch **Bus2** to accent a VCA or open distortion amount
- Set **Chance** near the unstable middle
- Keep **Length** between 4–7
- Occasionally hit **Reset** externally to force phrase restarts

### Result
Snarling, chaotic bass that latches into temporary motifs, then escapes. Very suitable for neuro/DnB-style phrases.

### Tip
- **3-bit feedback** tends to produce more burst-like behavior
- **8-bit feedback** tends to sound more random and attractor-like

Use 3-bit if you want rhythmic growls; use 8-bit if you want more unhinged crawling instability.

---

## 4. Subharmonic monster bass
### Patch
- Audio-rate pulse oscillator into **Clock**
- Use divider outputs directly as subharmonics
- Send **/2, /3, /5** to a mixer or to separate processing paths
- Use **Bus1** and **Bus2** as additional subharmonic layers
- Use **8-bit** to modulate filter cutoff
- Use **3-bit** to modulate PWM on the clock oscillator
- Distort and lowpass the result

### Why it works
The clock dividers preserve pulse width, so PWM on the source clock becomes harmonically related PWM on divided outputs. This can create extremely heavy, organ-like or tearing bass stacks.

### Make it more alive
Use **Chance CV** and **Direction CV** to animate the 3-bit/8-bit modulation while the pulse-divider layer provides a stable low-end body.

---

## 5. Talking bass / vowel growl
### Patch
- Patch **8-bit** to one filter’s cutoff
- Patch **3-bit** to another filter’s cutoff or resonance
- Run a saw/reese through dual filters or a multimode filter
- Use **Bus2** to trigger envelopes controlling VCA and filter depth
- Modulate **Length** with stepped random
- Send rhythmic gates to **Direction**
- Use **Data** from noise or a rhythm gate source

### Result
The reverse-encoded outputs create opposing filter motions, very effective for speech-like movement.

---

# Haunting atmospheric pads

Rung Divisions can absolutely do pads, especially if you use it as a **slow-evolving CV brain** rather than only a harsh digital source.

The trick is:
- keep clocks slower
- use high chance for looping with occasional mutation
- modulate direction and length slowly
- route 3-bit and 8-bit to different dimensions of a voice

---

## 1. Slow haunted sequence pad
### Patch
- Feed a slow clock into **Clock**
- Send one or two divisions to **Bus1**, maybe **/4** and **/7**
- Patch **8-bit** through a quantizer to oscillator pitch
- Patch **3-bit** to filter cutoff, wavefolder depth, or FM index
- Use **Bus2** to trigger very slow envelopes
- Set **Chance** mostly clockwise so phrases loop
- Use very slow random or manual modulation on **Length**
- Trigger **Direction** only occasionally

### Sound
A repeating but ghostly pitch contour that gradually rewrites itself. Very effective with long reverb and delay.

---

## 2. Clocked digital cloud
### Patch
- Use an audio-rate clock but filter heavily after
- Patch **Noise** to **Data**
- Set **Chance** around the middle for noisy interference
- Set **Length** long, 6–8
- Patch **8-bit** or **3-bit** as audio into a lowpass filter
- Use **Bus2** to modulate reverb freeze, delay feedback, or VCA tremolo
- Send sparse gates to **Direction**
- Optionally reset occasionally for scene changes

### Result
A digital-noise oscillator that can be sculpted into wind, choir-like haze, haunted radio texture, or broken tape ambience depending on filtering.

---

## 3. Palindromic pad movement
This module’s reverse encoding is ideal for slowly shifting contrapuntal motion.

### Patch
- Use a slow clock
- Send **Bus1** simple divisions like **/2 and /3**
- Patch **3-bit** to one oscillator’s pitch
- Patch **8-bit** to a second oscillator’s pitch or to a secondary quantizer
- Or patch one to pitch and the other to filter
- Set **Chance** high so material loops
- Send a slow gate every 8–16 bars to **Direction**
- Modulate **Length** with a slow triangle or smooth random

### Why it works
Direction changes make one contour rise while the other falls. This creates beautiful mirror-like motion with very little patching.

---

## 4. Frozen-memory pad
### Patch
- Build a pattern with manual **Data write switch** and/or Data input
- Set **Chance** fully clockwise to lock the loop
- Use a very slow Bus1 clock
- Patch **8-bit** to pitch
- Patch **3-bit** to timbre or filter
- Occasionally unlock chance briefly with CV, then re-lock
- Use **Direction** flips for reverse-memory effects

### Result
Like a haunted phrase sampler made of bits. Very musical and cinematic.

---

# The most effective modulation sources to patch into Rung Divisions

## For Chance CV
Best sources:
- Slow triangle or sine LFO
- Slewed random
- Envelope from your kick/snare
- Another sequencer lane
- One of the module’s own outputs, attenuated

**What it does musically:**
- low modulation depth = living repetition
- high depth = abrupt alternation between looped and chaotic states

For bass and percussion, this is often the **single best CV input** to animate.

---

## For Length CV
Best sources:
- Sample-and-hold
- Stepped random
- A slow sequencer row
- Pressure/joystick/manual offset
- 1-bit or Bus2 through attenuation/offset

**What it does musically:**
- changes phrase length
- causes missing or “lost” bits when loop point changes
- great for fill-like hiccups and polymetric shifts

For pads, use slow smooth or stepped modulation.
For percussion, use abrupt stepped CV.

---

## For Direction CV
Best sources:
- Sparse trigger stream
- End-of-cycle gate from an envelope
- Bus2
- Manual gate button
- Euclidean trigger source

**What it does musically:**
- phrase inversion
- reverse-feel bass turns
- asymmetrical repetitions
- pseudo-tape-rewind effect in the stepping pattern

This input is amazing when triggered **less often than the main rhythm**.

---

## For Data input
Best sources:
- Built-in **Noise**
- Bus2
- A clock division output
- External square wave VCO
- Comparator on a slow LFO
- Drum trigger pattern

**What it does musically:**
Because of XOR, even regular inputs become unstable. Data acts like the “seed of corruption.”

My favorite choices:
- **Noise** for atmospheres and metallic percussion
- **Bus2** for self-related rhythmic mutation
- **External VCO square** for audio-rate structured insanity

---

# Advanced patch ideas

## 1. Cross-coupled bass/drum system
- Bus1 clocks the register
- Bus2 triggers drum envelopes
- 8-bit controls bass pitch/FM
- 3-bit controls drum tone/filter
- Reset from a master bar clock
- Direction triggered only at fill points
- Chance opened up only during fills

This gives a full groove ecosystem where drums and bass are structurally related.

---

## 2. Feedback but with restraint
The manual suggests feeding 3-bit or 8-bit back to the clock source. Do it through:
- attenuator
- VCA
- slew
- filter
- offset

This makes the feedback much more playable.

### Great options:
- 8-bit -> attenuator -> VCO FM
- 3-bit -> VCA -> FM amount, opened by Bus2
- 8-bit -> slew -> clock VCO pitch for more gliding instability

---

## 3. Dynamic bus choreography
Don’t leave the bus switches static in performance. The switches decide which divisions feed Bus1 vs Bus2, and therefore:
- what clocks the register
- what accents the patch
- what rhythms are generated externally

Changing bus assignments while modulating length/chance is one of the fastest ways to move from groove to chaos.

---

## 4. Reset as phrase punctuation
The reset input resets all counts. Use it:
- every bar for tighter loops
- irregularly for asymmetry
- manually for live fills
- from Bus2 or another sequencer lane

For DnB and dubstep, reset is excellent for forcing “drop return” coherence after chaotic mutation.

---

# Best practical recipes

## Recipe: distorted modular kick line
- Clock: audio-rate pulse VCO
- Bus1: /2 + /5
- Bus2: /3 + /7
- 8-bit -> oscillator FM
- Bus1 -> short env -> VCA
- Bus2 -> accent env -> filter/distortion drive
- Chance: around noon to 2 o’clock
- Length: 3–5
- Direction: sparse triggers

---

## Recipe: neuro bass growler
- Clock: square VCO
- 8-bit -> FM on main oscillator
- 3-bit -> filter cutoff / wavefolder
- Bus1: /2 + /3 + /4
- Bus2: /5 + /7
- Data: Noise or Bus2
- Chance: modulated slowly around middle/high
- Length: stepped random
- Direction: every 1 or 2 bars
- Add distortion, phaser, comb, or notch filtering after

---

## Recipe: eerie looping pad
- Clock: slow pulse
- Bus1: /4 + /7
- Bus2: /3 or /8
- 8-bit -> quantizer -> oscillator pitch
- 3-bit -> filter cutoff
- Bus2 -> slow envelope -> VCA or LPG
- Chance: high
- Length: 6–8, slowly modulated
- Direction: occasional
- Add long shimmer reverb/delay

---

# Performance tips

## Sweet spots
- **Chance fully CW**: loop lock, stable motifs
- **Chance near middle**: best for unstable life
- **Short Length**: hooky and punchy
- **Long Length**: evolving and cinematic

## For percussion
Use:
- audio-rate clock
- short pulse width
- noise or gates into Data
- Bus outputs as trigger logic
- fast modulation to Length and Chance

## For bass
Use:
- 8-bit for pitch/FM
- 3-bit for timbre/filter
- sparse Direction changes
- feedback into the clock oscillator
- reset at phrase boundaries

## For pads
Use:
- slow clocks
- high Chance
- occasional unlocks
- slow Length modulation
- rare Direction flips
- quantization plus lots of effects

---

# A few especially strong combinations

## Combination 1: 8-bit to pitch, 3-bit to filter
Classic and effective. Great for bass and pads.

## Combination 2: 3-bit feedback to clock oscillator
More bursty and percussive. Great for DnB/neuro sound design.

## Combination 3: Bus2 to Direction
Turns the rhythm generator into a self-reversing pattern engine.

## Combination 4: Noise to Data, Chance under envelope CV
Excellent for percussion that starts noisy and settles into pattern.

## Combination 5: Reset at bar line, Chance mutation before reset
Perfect for controlled chaos in club-oriented patches.

---

# Final thoughts

The most unique thing about Rung Divisions is that it lets you blur the lines between:

- clock
- rhythm
- logic
- sequence
- oscillator
- chaos system

For the styles you mentioned, I’d especially recommend exploring these three workflows:

1. **Percussion:** audio-rate clock + noise/data XOR + Bus-triggered envelopes  
2. **Basslines:** 8-bit/3-bit controlling pitch+timbre with direction flips and feedback  
3. **Pads:** slow Bus1 clocking, high chance looping, and occasional direction/length modulation  

If you want, I can also turn this into:
- a **set of 10 specific patch recipes**
- a **“best modulation sources by jack” cheat sheet**
- or a **beginner-to-advanced guide** for patching this module in a full Eurorack system.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)