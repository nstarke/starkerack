# Mutable Instruments — Clouds

- [Manual PDF](../../manuals/Mutable Instruments - Clouds.pdf)

---

[Manual PDF](attachment)

# Mutable Instruments Clouds — using it to create melodic material

Clouds is not a traditional oscillator or sampler; it’s a **real-time granular texture processor**. That means its melodic usefulness comes from how you feed it, freeze it, pitch it, and trigger grains. If you pair it with pitch CV, clocks, sequencers, envelopes, random sources, and sound sources, it can absolutely become a strong melodic voice.

## What Clouds contributes musically

From the manual, Clouds lets you control:

- **POSITION**: where in the buffer grains are taken from
- **SIZE**: grain length
- **PITCH**: transposition, with **V/Oct input**
- **DENSITY**: grain generation rate / overlap / random vs regular sowing
- **TEXTURE**: envelope shape and diffusion
- **FREEZE**: stop recording and play from captured audio
- **TRIGGER input**: explicitly start grains
- **BLEND section**: dry/wet, stereo spread, feedback, reverb

That combination makes Clouds useful for melodic duties in a few different ways.

---

## The key idea: Clouds can become a pitch-playable micro-sampler

The most important melodic trick in the manual is this:

- Set **DENSITY to 12 o’clock** so Clouds does **not** continuously generate grains.
- Send pulses to the **TRIGGER input**.
- Use the **V/OCT PITCH input** to transpose each grain melodically.

In this mode, Clouds behaves a lot like a tiny granular sample player. Instead of long evolving textures, you get **discrete notes** from whatever is in the buffer.

So the basic melodic patch is:

1. Send audio into Clouds.
2. Capture or **FREEZE** a useful sound.
3. Clock or sequence the **TRIGGER** input.
4. Send sequenced pitch CV to **V/OCT**.
5. Tune **POSITION** and **SIZE** until the grains speak like notes.

This is the most direct way to use Clouds for melodies.

---

## Best source modules to pair with Clouds for melody

Clouds works best with modules that provide one or more of the following:

- **Stable pitched audio source**  
  Example: VCO, wavetable oscillator, physical modeling voice, filtered saw/sine
- **Pitch sequencer / keyboard / MIDI-CV**
- **Trigger or gate sequencer**
- **Clock / divider / rhythm source**
- **Random or sample-and-hold modulation**
- **Envelope + VCA before Clouds or after Clouds**
- **Quantizer**, if using random CV melodically

### Particularly strong pairings

#### 1. Oscillator + sequencer + Clouds
Feed a simple oscillator line into Clouds, freeze a moment, then resequence the grains at new pitches.  
This gives you:

- chord-like melodies from single notes
- transposed fragments
- shimmering arpeggios
- “frozen vocal/string/saw” lead sounds

The manual specifically notes that **raw sawtooth and sine waves sound very good**, especially with random modulation.

#### 2. Noise/random + quantizer + Clouds
The manual suggests randomizing **grain position or pitch**. If you quantize that randomness, Clouds becomes a **semi-generative melodic voice**.

Use:
- random CV → quantizer → V/OCT
- random or slow CV → POSITION
- clock → TRIGGER

Result:
- shifting melodies built from one captured sound
- pseudo-arpeggios
- evolving tonal fragments

#### 3. Chord or sequence source into Clouds
The manual mentions a great trick:
- send a **very fast sequence of 3 or 4 notes** to the **V/O input**
- if grains are sown randomly, each grain can pick one of those notes
- the result is effectively **a chord**

In practice, this means Clouds can turn rapid pitch motion into harmonic clouds or melodic chord clusters.

---

## Melodic patch strategies

## 1. Frozen lead voice

### Patch
- Audio source (sine, triangle, vocal snippet, pluck, or filtered saw) → **Clouds IN L**
- Sequencer pitch CV → source oscillator pitch
- Then when you hear an interesting timbre, hit **FREEZE**
- Send a melodic sequence to **Clouds V/OCT**
- Send gates or clock to **TRIGGER**
- Set **DENSITY at noon**
- Adjust **SIZE** short to medium
- Set **BLEND dry/wet** fairly wet

### What happens
You’ve captured a tiny “instrument sample” inside Clouds. Now each trigger plays a grain from that frozen sound at a chosen pitch.

### Why it works
This is the closest Clouds gets to a playable sampler voice. Great for:
- leads
- bell-like notes
- vocal synth melodies
- glassy plucks

---

## 2. Granular arpeggiator

### Patch
- Sustained oscillator, drone, or chord source → Clouds
- Freeze a rich harmonic moment
- Clock divider / trigger sequencer → **TRIGGER**
- Arpeggiator or step sequencer → **V/OCT**
- Slow LFO or random CV → **POSITION**
- Moderate **SIZE**
- **DENSITY at noon**
- Slight reverb/spread via BLEND

### Result
Each trigger plays a different sliver of the frozen sound, while pitch CV imposes a melodic pattern. Because POSITION is moving, every note has a different color.

This gives:
- shimmering arps
- pseudo-sampled mallet lines
- animated digital melodies

---

## 3. Harmonic chord machine from one voice

The manual explicitly hints at this: rapid pitch changes into V/OCT can create a chord effect when random grains pick among those pitches.

### Patch
- Freeze a harmonically rich tone
- Set **DENSITY clockwise** for random grain generation
- Send a rapid stepped CV pattern with 3–4 quantized notes to **V/OCT**
- Keep **SIZE** short
- Add a little **stereo spread**
- Use moderate **reverb**

### Result
Clouds smears those notes into a harmonic cluster. It’s not a clean polyphonic chord synth, but it produces:
- lush pads
- harmonic swarms
- chord washes that can still imply melody

This is especially strong if your source sound is simple, like a saw or sine, because the granular behavior supplies complexity.

---

## 4. Melodies from rhythmic slices

### Patch
- Drum loop, plucky sequence, or rhythmic patch → Clouds
- Freeze a short segment
- Trigger grains rhythmically
- Send quantized pitch sequence to **V/OCT**
- Scan **POSITION** manually or with CV

### Result
You get a hybrid of melody and rhythmic sample slicing:
- tuned percussive riffs
- glitch melodies
- “granular MPC” style phrases

Short **SIZE** values make this more pointillistic. Longer values make it more legato.

---

## 5. Expressive touch-played melodic instrument

The manual suggests using:
- contact microphone or touch strip to trigger grains and modify position

### Patch
- Capture a sound in Clouds
- Pressure plate / touch controller / manual gate → **TRIGGER**
- Touch strip CV → **POSITION**
- Keyboard CV → **V/OCT**

### Result
This gives a very expressive performance instrument:
- finger-triggered granular notes
- scrubbed sample-position melody
- tactile microsound phrasing

This is a great live-performance use.

---

## Parameter roles in melody building

## POSITION
This is not only a timbral control; in a melodic patch it acts like **sample selection**.

Use it to:
- choose bright vs dark parts of the buffer
- move through an evolving input recording
- create note-to-note timbral variation

With a sequencer or stepped random CV on POSITION, each note can sound like a different instrument articulation.

---

## SIZE
SIZE strongly changes articulation.

- **Short SIZE**: plucks, clicks, mallets, percussive melody
- **Medium SIZE**: more intelligible notes, sampled tone feel
- **Long SIZE**: smeared, legato, pad-like melodic lines

If you want recognizably pitched notes, medium settings are often easiest. Too short can become noisy; too long can blur note definition.

---

## PITCH / V-OCT
This is the core melodic input.

From the manual:
- the PITCH CV input has **V/Oct response**
- center position is original pitch

So Clouds can track melodic sequencing like an oscillator or sampler transpose input.

Best uses:
- sequence pitch from a keyboard/sequencer
- quantize random voltages for generative melodies
- transpose frozen textures into scales

---

## DENSITY
For melody, this knob changes Clouds from “texture generator” to “note instrument.”

- **12 o’clock**: no automatic grains; use **TRIGGER**
- **Clockwise from noon**: random grain sowing, better for swarming melodic clouds
- **Counterclockwise from noon**: more regular grain generation

For clear melodies:
- keep it near **noon**
- drive notes from TRIGGER

For melodic atmospheres:
- move clockwise and let grains self-generate

---

## TEXTURE
TEXTURE controls envelope shape and later activates diffusion.

For melody:
- **sharper envelope settings** = clearer attacks, more rhythmic definition
- **smoother Hann-style settings** = more pad-like notes
- **past 2 o’clock** = diffuser for blurred, ambient melodic lines

If you want a lead, keep diffusion low.  
If you want a melodic haze or background harmony, push it higher.

---

## FREEZE
FREEZE is the heart of intentional melodic use.

Without freeze, Clouds is constantly recording new audio, so the source material keeps changing. That’s great for texture, but less stable for melody.

With **FREEZE on**:
- the buffer becomes fixed
- Clouds behaves more predictably
- transposition and triggering become more instrument-like

A very practical approach:
- perform source sound live
- listen for a beautiful moment
- hit **FREEZE**
- then play that moment melodically from the keyboard/sequencer

---

## BLEND parameters in melodic contexts

The BLEND knob can control:
- dry/wet
- stereo spread
- feedback
- reverb

For melody:

### Dry/wet
Essential. If fully dry, you’ll think nothing is happening.  
For melodic use, set it mostly wet or fully wet.

### Stereo spread
Excellent for widening arps and chord-like textures.

### Feedback
Can create repeating harmonic tails or resonant buildup. In moderation, useful for melodic sustain.

### Reverb
Helps frozen grains feel like a playable ambient instrument.

The manual also notes that with FREEZE active, feedback behavior changes and becomes more reverb-like due to internal routing. That can make frozen melodic patches feel especially spacious.

---

## Best source material for melodic results

According to the manual and in practice, these inputs work very well:

- **Sine waves**: pure, bell-like, clean transposition
- **Saw waves**: rich harmonics, strong granular color
- **Simple filtered tones**: stable, musical, easy to tune
- **Short plucks**: excellent for percussive melody
- **Voice or field recordings**: expressive but less stable
- **Chords**: good for harmonic pad and cluster melody

If you want pitch clarity, use harmonically simple and stable sources.  
If you want character, feed in complex timbres and modulate POSITION.

---

## Concrete “used together” workflows with common eurorack companions

## Clouds + sequencer + oscillator
Use the oscillator as source material and the sequencer twice:
- once to create the recorded phrase
- then again to transpose Clouds via V/OCT

This lets Clouds derive a second melodic line from the first.

### Example
- Oscillator sequence into Clouds
- Freeze on a note or phrase
- Different sequencer row into Clouds V/OCT
- Clocked triggers into TRIGGER

Now the frozen phrase becomes a new melodic instrument.

---

## Clouds + random source + quantizer
A classic generative setup.

### Example
- Random stepped CV → quantizer → V/OCT
- Another random or smooth CV → POSITION
- Clock → TRIGGER
- Frozen oscillator waveform in buffer

Result:
- scale-locked melodic fragments
- non-repeating but coherent lines
- ideal for ambient, IDM, soundtrack work

---

## Clouds + keyboard + envelope/VCA
Use Clouds as a playable voice under the keyboard.

### Example
- Hold or freeze a source sound
- Keyboard CV → V/OCT
- Gate → TRIGGER
- Clouds output → VCA
- Keyboard gate also → envelope → VCA CV

This gives note articulation after Clouds, making it behave more like a standard synth voice.

---

## Clouds + logic/clock modules
Because TRIGGER explicitly starts grains, rhythmic modules are very useful.

Use:
- trigger sequencers
- Euclidean rhythms
- clock multipliers/dividers
- burst generators

This turns Clouds into a rhythmic melodic generator, especially when paired with pitch sequencing.

---

## Clouds + sampler/looper/voice module
If another module gives stable audio phrases, Clouds can transform them into melodic matter:
- capture a loop
- freeze a small region
- replay it at different pitches

This is very effective for:
- vocal chop melody
- tuned texture riffs
- re-harmonizing loops

---

## Practical patch recipes

## Recipe 1: Glass bell melody
- Sine wave oscillator into Clouds
- Freeze a stable sine or FM tone
- DENSITY at noon
- Trigger from 16th-note clock
- Quantized sequence into V/OCT
- SIZE short-medium
- TEXTURE smooth but not diffused
- Wet signal only

Produces clean bell/pluck melodies.

---

## Recipe 2: Vocal ghost lead
- Spoken/sung phrase into Clouds
- Freeze on a vowel-rich moment
- Manual or sequenced triggers
- Keyboard/sequencer into V/OCT
- Moderate POSITION modulation
- Light reverb

Produces haunting melodic leads from voice.

---

## Recipe 3: Chord shimmer pad
- Rich saw wave or chord source into Clouds
- Freeze
- DENSITY random and fairly high
- Fast 3–4 note sequence into V/OCT
- Large stereo spread
- Reverb up
- Slow POSITION modulation

Produces floating harmonic/melodic pad structures.

---

## Recipe 4: Granular pluck sequencer
- Short pluck or filtered noise burst into Clouds
- Freeze
- Trigger from sequencer
- Quantized melody into V/OCT
- Small SIZE
- Sharp TEXTURE envelope
- Minimal diffusion

Produces pointillistic tuned percussion lines.

---

## Important limitation to understand

Clouds does **not** generate melody on its own in the same way a dedicated oscillator plus envelope would. It needs:
- meaningful input audio
- pitch CV or trigger structure
- careful dry/wet setup

Also, very dense settings can blur pitch. The manual notes that dense clouds often sound best with random position or pitch modulation; otherwise they can resemble a resonant comb filter.

So for **clear melody**, think:
- frozen source
- triggered grains
- sequenced V/OCT
- moderate size
- controlled density

For **melodic atmosphere**, think:
- random grain generation
- moving position
- more spread/reverb/diffusion

---

## Best overall use cases for melody

Clouds is especially good for:

- **sampled/frozen leads**
- **granular arpeggios**
- **generative quantized melodies**
- **harmonic swarms and chord clouds**
- **pitched glitch/percussive riffs**
- **expressive transformed vocal/instrument phrases**

It is less ideal if you want:
- very precise transient reproduction
- clean polyphony
- straightforward subtractive synth melodies

But if you want melody with motion, memory, and texture, it excels.

---

## Bottom line

To use Clouds for melodic components, the strongest approach is:

1. Feed it a musically rich source.
2. Freeze a compelling moment.
3. Set **DENSITY to noon**.
4. Trigger grains externally.
5. Sequence the **V/OCT** input.
6. Shape articulation with **SIZE**, **TEXTURE**, and post-VCA/envelopes.
7. Add controlled movement with **POSITION** modulation.

That turns Clouds from a texture processor into a playable melodic granular voice.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)