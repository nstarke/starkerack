# Tiptop Audio — BD808

- [Manual PDF](../../manuals/Tiptop_Audio_BD808_ns.pdf)

---

[Manual PDF](https://www.tiptopaudio.com/808-2)

# Tiptop Audio BD808 — using it for melodic components

Even though the **BD808** is a bass drum module, the manual makes it clear that it is very usable as a **pitched, resonant analog sound source** inside a Eurorack patch. In a modular context, that means it can contribute much more than just kick drums: it can become a **bass voice, tuned percussion layer, transient oscillator, modulation source, or audio-rate excitation source** for melodic patches.

## What the manual tells us musically

From the manual, the important behaviors are:

- **The core sound is a resonating low-frequency sine-based circuit**
  - This means the BD808 naturally produces a pitched low-frequency body.
  - With the right decay and processing, that body can read as a **note**, not only a kick.

- **DECAY can be extended very far**
  - Long decay makes the resonant pitch more audible.
  - At the extreme, some units may **self-oscillate**, which effectively turns the module into a continuous tone source.

- **TONE is a low-pass filter control**
  - Higher TONE passes more attack harmonics and gives the recognizable “basketball” / techno 808 click.
  - Lower TONE softens the attack and emphasizes the rounded body, which is often better for melodic bass use.

- **ACCENT changes more than loudness**
  - The manual notes that accent “hits” the resonating circuit harder, changing both **level and attack character**.
  - This makes accent useful as a **performance articulation control** for melodic lines.

- **LEVEL can get very hot**
  - The output can overdrive downstream modules, interfaces, filters, VCAs, pedals, and effects.
  - That makes the BD808 especially good as a source for **harmonic enhancement**, which is useful when turning a drum voice into something more melodic and present in a mix.

- **The sound becomes inconsistent when decay overlaps the next trigger**
  - This is not a defect; it is part of the analog resonant behavior.
  - Musically, this can be used intentionally to create **legato bass movement, pitch-smearing, or evolving tonal phrases**.

- **Tiptop explicitly encourages patching drum modules through other modules**
  - The manual suggests ring modulation, filters, VCAs, bit crushers, DSP, CV destinations, and cross-modulation with other drum voices.
  - That strongly supports using the BD808 as a building block in larger melodic systems.

---

## How the BD808 can create melodic material

## 1. 808 bassline voice

This is the most direct melodic use.

### Patch
- Send a trigger sequence into **GATE IN**
- Take **BD OUT** into:
  - a VCA/envelope chain, or
  - directly into a mixer/filter
- Set:
  - **DECAY** fairly long
  - **TONE** lower to medium
  - **LEVEL** to taste
  - **ACCENT** moderate

### Result
The resonant sine body becomes a **sub-bass note event**. If the sequence is rhythmic and sparse enough, the ear hears each hit as a bass tone. This works especially well for:

- electro basslines
- Miami bass style patterns
- techno low-end riffs
- minimal dub pulses

### Musical trick
Use two trigger streams:
- one to **GATE IN**
- one to **ACCENT IN**

Now you can articulate some “notes” more strongly than others. Even though the BD808 is not pitch-tracking from CV, the difference in attack and loudness creates the perception of phrasing, almost like a melodic accent pattern.

---

## 2. Tuned percussion / pseudo-melody through filtering

The module itself does not offer pitch CV input, but you can still extract melodic behavior by using external modules.

### Patch
- **BD OUT → resonant filter**
- Sequence the filter cutoff with a CV sequencer
- Optionally modulate resonance with another rhythmic CV
- Trigger the BD808 from a pattern source

### Why this works
The BD808 provides:
- a strong low-frequency fundamental
- a transient click
- harmonics controlled by TONE and output saturation

A resonant filter can emphasize different spectral regions per step, making a repeated BD808 line feel like it is moving through different notes or vowel-like tones.

### Best settings
- **TONE** medium-high if you want the filter to have harmonics to grab
- **DECAY** medium-long
- **LEVEL** high if you want filter drive

This is one of the strongest ways to derive melodic content from a non-pitched drum module.

---

## 3. Self-oscillation as a drone or pitch source

The manual notes that with maximum decay, some BD808 units may begin **self-oscillating**.

### Patch
- Turn **DECAY** to maximum
- Back it off slightly if needed to stabilize the tone
- Use **BD OUT** as a drone source
- Run it through:
  - a VCA for note gating
  - a filter for timbral movement
  - wavefolder/distortion for upper harmonics

### Result
If your unit self-oscillates, the BD808 can act as a **raw analog sine-ish oscillator**. It will not be a precision 1V/oct voice, but it can still be used for:

- drones
- bass pedals
- tuned ambient layers by ear
- FM/modulation source for other oscillators or filters

### Musical use together with other modules
Pair the BD808 drone with a melodic oscillator:
- Use BD808 as the sub layer
- Use a conventional VCO for the clearly tuned upper melody
- Gate and accent the BD808 rhythmically underneath

This gives a very classic modular hybrid: **pitched melody above, resonant analog body below**.

---

## 4. Use the BD808 as an exciter for resonators

Because the BD808 has a strong transient plus a resonant body, it is excellent for exciting external resonant processors.

### Patch
- **BD OUT → resonator / physical modeling module / tuned delay / comb filter**
- Sequence trigger input to BD808
- Tune the resonator chromatically

### Result
The BD808 becomes the **strike mechanism**, while the resonator supplies the actual pitch. This can create:

- tuned tom-like melodies
- marimba or plucked-bass illusions
- metallic melodic sequences
- dubby tuned percussive lines

### Why this is effective
A plain click can excite a resonator, but the BD808 is richer than a click:
- it has body
- it has controllable attack
- it can be overdriven
- it responds dynamically to accent

That gives the resonator a more expressive input signal.

---

## 5. Accent as articulation in melodic rhythm

The manual explains that accent is internally normalized from the gate input unless a cable is inserted into **ACCENT IN**. Once patched separately, accented and unaccented hits diverge in gain and attack.

### Melodic application
Think of accent as similar to:
- note velocity
- phrasing
- emphasis
- dynamic contour

### Patch idea
- Clock divider or trigger sequencer to **GATE IN**
- A separate sparse accent pattern to **ACCENT IN**

Use this for:
- call-and-response bass phrases
- syncopated low-end motifs
- pseudo-melodic movement where dynamics imply line shape

In groove-based music, this can be more important than literal pitch movement.

---

## 6. Overdrive for harmonically richer melodic bass

The manual emphasizes that **LEVEL** can go up to around **20 Vp-p**, which is extremely hot and enough to clip many downstream devices.

### Patch
- Set **LEVEL** high
- Set **ACCENT** high
- Set **DECAY** medium
- Run **BD OUT** into:
  - wavefolder
  - saturating filter
  - VCA with gain
  - distortion
  - analog delay
  - bit crusher

### Result
The BD808 develops more harmonic complexity, making it easier to hear as a **bass voice with note identity** in a musical arrangement.

Pure sub-heavy 808 sounds can disappear melodically because they are too sine-like. Overdriving them creates upper harmonics, which makes rhythmic bass phrases read more clearly on smaller speakers and in dense mixes.

---

## 7. Audio-rate modulation source for melodic systems

The manual explicitly says drum outputs can be sent into CV inputs, FM inputs, sync inputs, and other unusual destinations.

That means the BD808 can be used not only as audio, but as a **contoured modulation source**.

### Patch ideas

### A. Filter FM
- **BD OUT → filter FM/CV input**
- Another oscillator provides the pitched melody

The BD808 imposes a per-hit pitch/timbre contour onto the melodic voice.

### B. Oscillator FM
- **BD OUT → linear or exponential FM input of a VCO**
- Sequence the VCO melodically

Now each kick hit adds a transient pitch bend or grit to the melodic oscillator.

### C. Waveshaper modulation
- **BD OUT → fold/symmetry CV**
- Another oscillator or chord source through the shaper

The BD808 rhythmically animates harmonic color, creating melodic movement without changing pitch.

This is one of the most “modular” ways to use the BD808 melodically: not by making the drum itself play notes, but by letting it animate notes elsewhere.

---

## 8. Ring modulation with other voices

The manual specifically suggests running two drum sounds into a **ring modulator** or **VCA** for amplitude modulation.

Even if you only have the BD808, the same principle works with any melodic oscillator.

### Patch
- **BD808 → ring mod input A**
- **VCO or other pitched voice → ring mod input B**

### Result
You get sidebands and bell-like or growling tones shaped by the BD808’s transient and body. This can generate:

- metallic bass tones
- tuned industrial percussion
- unstable melodic textures
- hybrid kick/bass voices

If the pitched oscillator is sequenced, the resulting output can function as a genuine melodic layer with strong rhythmic identity.

---

## 9. Layered kick + bass note from one source

One very practical approach is to split the BD808 into parallel paths.

### Patch
- Mult **BD OUT** to two chains

#### Path 1: Kick body
- direct to mixer
- shorter decay setting on the module itself
- moderate level

#### Path 2: Melodic enhancement
- through filter/distortion/resonator/delay
- EQ or high-pass as needed
- maybe VCA-gated separately

### Result
You can make one BD808 behave like:
- a normal kick in the low end
- plus a tonal or melodic layer in the mids

This is especially effective in techno, electro, and experimental styles where the kick itself participates in the harmonic language of the track.

---

## 10. Controlled instability as melodic variation

The manual notes that if the **DECAY** exceeds the interval between hits, the sound can become inconsistent because the resonant circuit has not fully settled.

Normally this is treated as a warning, but musically it is a feature.

### Use it for:
- sliding-feel bass ostinatos
- evolving repeated phrases
- acid-adjacent low-end instability
- humanized analog variation

### Patch
- Program repeating 8th or 16th note triggers
- Raise **DECAY** until hits begin interacting
- Adjust **ACCENT** pattern for contour
- Run through a filter or saturation stage

This produces bass movement that is not conventionally quantized in pitch, but still feels melodic because the resonant state of one note influences the next.

---

# Best musical roles for the BD808 in a melodic patch

## 1. Sub-bass punctuation
Use it as the low fundamental under a separate pitched synth line.

## 2. Pitched percussion
Use long decay and resonators/filters to turn it into tuned strikes.

## 3. Articulated bass rhythm
Use separate accent sequencing to create phrase shape.

## 4. Drone oscillator
If your unit self-oscillates, exploit it as a primitive analog tone source.

## 5. Modulation source
Patch the audio into FM/CV/filter inputs to animate melodic voices.

## 6. Harmonic exciter
Drive downstream processors so the drum contributes note-like harmonics.

---

# Practical patch recipes

## Patch 1: 808 bass melody illusion
- Trigger sequencer → **GATE IN**
- Accent sequencer → **ACCENT IN**
- **BD OUT → low-pass filter → VCA → mixer**
- Set:
  - DECAY: 1–3 o’clock
  - TONE: 9–11 o’clock
  - LEVEL: 11–1 o’clock
  - ACCENT: to taste

The filter cutoff sequence supplies “note movement,” while BD808 supplies body and articulation.

---

## Patch 2: Resonator bassline
- Trigger pattern → **GATE IN**
- **BD OUT → resonator tuned to scale → mixer**
- Optional accent pattern → **ACCENT IN**

This gives tuned percussive notes using the BD808 as the strike source.

---

## Patch 3: Kick-controlled melody animation
- Main melodic VCO sequence → voice chain
- **BD OUT → VCO FM input** or **filter CV input**
- Trigger BD808 rhythmically

The melody remains pitched by the VCO, but the BD808 injects rhythmic movement and transient aggression.

---

## Patch 4: Self-oscillating sub drone
- Set DECAY near max
- Find self-oscillation point if your unit supports it
- **BD OUT → VCA**
- Use external envelope or gate to shape notes
- Add saturation/filtering

Useful for dark drones, bass pedals, and semi-tuned low-end beds.

---

## Patch 5: Split-path kick/bass hybrid
- Mult **BD OUT**
- Path A → dry kick mix
- Path B → distortion + filter + delay/resonator
- Mix both together

You get a functional kick plus a tonal/melodic aura around it.

---

# Important limitations

The BD808 is **not a conventional melodic oscillator**. Based on the manual:

- there is **no pitch CV input**
- melodic use relies on:
  - resonance
  - filtering
  - excitation of other modules
  - overtones from distortion
  - articulation from accent
  - self-oscillation if available
  - interaction with external resonators or processors

So if your goal is precise scales and keyboard tracking, the BD808 is not the primary voice. But if your goal is **musically useful low-end melody, tuned percussion, phrase articulation, and modular cross-patching**, it is very strong.

---

# Bottom line

The manual presents the **BD808** as more than a drum sound: it is a **resonant analog sound generator** that becomes especially powerful in a modular system. For melodic components, its best uses are:

- **808-style bassline pulses**
- **tuned percussion through resonators and filters**
- **drone or sine-like source near self-oscillation**
- **dynamic articulation via separate accent sequencing**
- **audio-rate modulation for melodic voices**
- **harmonic bass generation through saturation and processing**

In short: the BD808 won’t replace a 1V/oct oscillator, but it can absolutely become part of the **melodic architecture** of a Eurorack patch—especially for bass, tuned percussion, and rhythmic tonal movement.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)