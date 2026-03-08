# Erica Synths — Black Delay

- [Manual PDF](../../manuals/Black_Delay_Manual.pdf)

---

[Manual PDF](#)

# Using the Erica Synths Black Stereo Delay for Melodic Music

From the attached manual, the module shown is:

- **Erica Synths Black Stereo Delay**

This is primarily an **effect/module for delay and looping**, not a pitch generator or oscillator by itself, but in a Eurorack system it can still play a strong role in creating **melodic components** by turning simple notes, sequences, and plucks into rhythmic and harmonic material.

## What this module contributes musically

The Black Stereo Delay provides:

- **Stereo delay**
- **Tape / Digital / Ping-Pong modes**
- **Tap tempo or clock-style timing**
- **CV over time, mix, and feedback**
- **Reverse delay**
- **Hold looping**
- **Add/overdub in Hold mode**
- **Stereo spread**

These features are especially useful for melody because they can create:

- repeating note patterns
- call-and-response echoes
- harmonically rich feedback tails
- reversed melodic phrases
- layered loop-based motifs
- wide stereo melodic movement

---

## Best melodic uses

## 1. Turn a simple sequence into a richer melody

If you patch a basic melodic voice into the delay:

- **Oscillator → VCF/VCA → Black Stereo Delay**
- Sequence a short 1–4 note pattern
- Set delay time to a rhythmic division of the tempo
- Keep feedback moderate

Result:

- the delay repeats fill in space between notes
- a simple motif becomes a more intricate melodic line
- ping-pong mode creates alternating left/right motion that makes the melody feel more alive

This works especially well with:

- short plucky envelopes
- sequenced basslines
- arpeggios
- bell-like or FM sounds

---

## 2. Create counterpoint with delay time

Because the delay time goes from **3 ms to 3000 ms**, you can use it as more than just an echo.

Set delay time so repeats land musically:

- **short times** for comb-like resonant doubling
- **medium times** for rhythmic note repetition
- **long times** for phrase-level echoes

For melodic writing, medium values are most useful. A melody can effectively play against its own repeats, producing:

- syncopation
- canon-like imitation
- pseudo-polyrhythms

Using **Tap** lets you synchronize repeats to your track tempo. That makes the module very useful for live melodic performance.

---

## 3. Use feedback as a melodic density control

The **Feedback** control determines how long repeats continue.

- **Low feedback**: one or two repeats, ideal for clarity
- **Medium feedback**: evolving melodic trails
- **High feedback**: cascading phrases, possible self-oscillation

For melodic applications, medium feedback is often the sweet spot. It can create the impression of a more complex sequence without adding another sequencer.

If you modulate **FBK CV**, you can make certain notes bloom into long tails while others stay dry. That creates phrase dynamics and variation.

---

## 4. Build looped melodic phrases with Hold

The **Hold** function records incoming audio into a memory buffer and loops it. The manual says you can record **up to 20 seconds**.

This is one of the strongest melodic features.

You can:

- play or sequence a melody into the module
- press **Hold** to capture it
- let it loop
- then play another voice over it

This turns the delay into a **phrase looper** for melodic fragments.

Musically, this is great for:

- ostinatos
- repeating lead hooks
- ambient motif looping
- layered melodic beds

Since the module continues to let you adjust **delay** and **feedback** on the held audio, you can keep reshaping the loop after capture.

---

## 5. Overdub harmonies or extra notes with Add

In **Hold** mode, **Add** lets you overdub more material into the loop buffer.

That means you can:

- record a single-note line
- overdub harmony notes
- add rhythmic accents
- build chord fragments from monophonic input

This is especially powerful if your system has only one main melodic voice. You can gradually stack parts into a richer melodic texture.

For example:

1. Record a short arpeggio
2. Enable **Add**
3. Send a higher counter-line
4. Add a few low notes for harmonic grounding

Now the delay becomes a compositional tool, not just an effect.

Because **IN LVL** affects overdub level in Hold mode, you can control how dominant each new melodic layer becomes.

---

## 6. Use Reverse to transform phrases

The **Reverse** function reverses the **delayed signal**.

This is useful for melody because it can create:

- swelling pre-note textures
- ghosted backward phrases
- contrast sections in a live set

Important note from the manual:

- Reverse affects the **delayed signal**
- it does **not reverse the audio in the hold buffer**

So for melodic use, Reverse is best thought of as a way to give your melody’s repeats a different articulation rather than reversing the original loop itself.

This can be beautiful on:

- lead lines
- sparse piano-like patches
- vocal-like synth phrases
- atmospheric melodies

---

## 7. Use stereo spread to widen melodic lines

The module lets you add extra delay to the **right channel**, creating **stereo spread up to 500 ms**.

This can make a melody feel much bigger.

How to set it:

- make sure **Hold is off**
- press and hold **Add**
- rotate **Time** to set stereo spread

Musically this gives:

- width for mono melodies
- a sense of two players answering each other
- gentle left/right phrase separation

For melodic content, subtle spread often works best. Too much can make the line feel detached rhythmically, but moderate spread can make a lead or arpeggio sound polished and immersive.

---

## 8. CV animation for evolving melodic effects

The module has CV inputs for:

- **TIME CV**
- **MIX CV**
- **FBK CV**

These are excellent for adding motion to melodies.

### TIME CV
Modulating delay time changes rhythmic spacing and, in some contexts, pitch-like smear behavior depending on mode.

Use it for:

- phrase expansion/contraction
- unstable tape-style melodic echoes
- transitions between rhythmic densities

### MIX CV
This lets you bring the delayed melody in and out dynamically.

Use it for:

- dry verses / wet choruses
- delayed fills at phrase ends
- ducking or swelling repeats

### FBK CV
This changes repeat length.

Use it for:

- occasional long echoes on important notes
- crescendo-like repeat blooms
- performance accenting

A slow LFO, random voltage, or gate-to-envelope source can make static melodies feel composed and alive.

---

## 9. Tape vs Digital mode for different melodic roles

The **Mode** switch selects:

- **Tape**
- **Digital (no pitch shifting)**

### Tape mode
Best for:

- expressive leads
- slightly unstable echoes
- vintage melodic trails
- more organic phrase repetition

### Digital mode
Best for:

- clean arpeggios
- precise sequences
- tempo-locked repeats
- transparent melodic layering

If your melodic line needs clarity, use **Digital**.  
If it needs character and movement, use **Tape**.

---

## 10. Ping-Pong mode for melodic dialogue

**Ping Pong** sends repeats across stereo channels, which is perfect for melodic interplay.

A single line can feel like:

- a question/answer phrase
- two instruments trading notes
- a melody moving through space

This is particularly effective with:

- short motifs
- syncopated plucks
- high-register sequences
- sparse ambient note patterns

The result is musical even before adding more voices.

---

## Practical patch ideas

## Patch 1: Arpeggio widener
- Patch a sequenced pluck voice into **IN L**
- Output **OUT L/R** to mixer
- Set **Digital** mode
- Tap the tempo
- Use moderate feedback
- Add slight stereo spread

Result: a mono arpeggio becomes a wide, rhythmic stereo melodic pattern.

---

## Patch 2: Looped lead phrase
- Play or sequence a short lead line into the module
- Press **Hold** to capture it
- Let it loop
- Use **Add** to overdub a higher harmony

Result: layered melodic phrase from one voice.

---

## Patch 3: Reverse ambient melody
- Send a sparse melody or slow sequence into the delay
- Set longer delay time
- Enable **Reverse**
- Use moderate wet mix and moderate feedback

Result: haunting reversed melodic echoes around the original line.

---

## Patch 4: Self-accompanying bassline
- Send a bass sequence into the delay
- Set time to dotted or syncopated rhythm
- Keep mix low-to-medium
- Feedback medium

Result: bass notes create a supporting upper rhythmic/melodic pattern through repeats.

---

## Patch 5: Live melodic resampling
- Sequence a melody
- Capture a phrase with **Hold**
- Mute original source or switch sequence
- Overdub with **Add**
- Modulate **Mix CV** and **FBK CV**

Result: evolving loop-based melodic texture suitable for live improvisation.

---

## What this module needs from other modules

To create melody, this delay works best when paired with:

- **oscillators or complete voices** for sound source
- **sequencers** for pitch and note order
- **envelopes/VCA** for articulation
- **filters/waveshapers** for tone shaping
- **LFOs/CV sources** for delay modulation
- **clock/trigger sequencers** for tap and trigger inputs

It does not generate pitch sequences by itself, but it strongly enhances and multiplies melodic material coming from those modules.

---

## Summary

The **Erica Synths Black Stereo Delay** is best used for melodic work as a:

- phrase repeater
- stereo motif enhancer
- loop recorder
- overdub tool
- reverse phrase processor
- rhythmic harmony builder

It is especially effective for turning:

- simple sequences into complex patterns
- monophonic lines into layered hooks
- short motifs into ambient melodic beds

If you send it strong melodic material and use **Hold**, **Add**, **Reverse**, **Ping Pong**, and CV modulation creatively, it can become a major part of the composition rather than just a finishing effect.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)