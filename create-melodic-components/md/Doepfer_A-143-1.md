# Doepfer — A-143-1

- [Manual PDF](../../manuals/A1431_man.pdf)

---

# [Doepfer A-143-1 Quad AD/LFO Manual (PDF)](https://doepfer.de/a100_man/A1431_man.pdf)

## Doepfer A-143-1 Quad AD/LFO: using it for melodic patching

The A-143-1 is not a pitch sequencer in the usual sense, but it **can become a very musical modulation hub** for creating melodic motion when paired with oscillators, quantizers, VCAs, filters, switches, or sequential routing modules. Its strength is that it gives you **four attack/decay function generators**, each with:

- Trigger input
- Envelope output
- End-of-Attack (EOA) output
- Comparator output with adjustable threshold
- Polarizer amount into a shared mix output
- AD or looping LFO mode

The important musical idea is this:

> The A-143-1 generates **complex timed voltages and logic events**, which can be shaped into stepped or repeating melodic structures.

---

## What the module does well for melody

From the manual, the A-143-1 can operate as:

- **4 independent AD envelopes**
- **4 free-running AD-style LFOs**
- **A chained multi-stage envelope**
- **A complex cyclic modulation source**

Because the trigger inputs are **normalled** from one comparator to the next, the four sections can self-chain into a larger evolving shape. That means you can build:

- repeating phrase contours
- rising/falling pitch gestures
- pseudo-sequences
- call-and-response modulation patterns
- ratcheting or stage-advanced melodic events via EOA/Cp outputs

---

## Key features that matter musically

### 1. Envelope outputs as melodic control voltages
Each channel outputs about:

- **0 to +8V in AD mode**
- **about +0.5V to +8V in LFO mode**

This is useful for melodic work because envelope voltages can be sent to:

- **1V/oct pitch input** of an oscillator, usually through attenuation/offset and ideally a quantizer
- filter cutoff to emphasize notes
- wavefolder / timbre CV for note-dependent tone changes
- VCA CV for articulation

Raw envelope voltages are continuous, so if you want conventional notes, run them through a **quantizer** first.

---

### 2. Mix output as a composite melodic contour
The **Mix Out** sums all four envelopes according to each channel’s **Mix Polarizer**:

- clockwise = positive contribution
- counterclockwise = negative contribution
- center = no contribution

This is where the module becomes especially melodic.

By setting the four envelopes to different times and polarities, you can create a **compound CV shape** that rises and falls in repeatable phrase-like ways. Sent into a quantizer, this becomes a melodic line.

Think of Mix Out as a way to “compose” one control voltage out of four moving parts.

---

### 3. Comparator outputs create stage timing
Each section has a **Comparator output (Cp)** tied to a manually adjustable threshold. The comparator changes state according to the envelope crossing that threshold, and these outputs are internally chained to trigger the next stage.

Musically, this means:

- one envelope can determine **when the next melodic event happens**
- threshold changes alter **phrase timing**
- changing attack/decay changes **rhythmic spacing**
- you can get non-uniform, human, asymmetrical timing patterns

This is a huge advantage over a rigid clock divider if you want melody that breathes.

---

### 4. EOA outputs can trigger note events
The **End of Attack (EOA)** output goes high when the attack phase ends.

That can be used to:

- trigger another envelope/VCA for accent
- clock a switch or sequential switch
- trigger sample & hold
- strike a low pass gate
- advance an external sequencer or shift register

So one contour can both define pitch movement **and** trigger the next note articulation.

---

## Best melodic use cases

---

## 1. Create a melodic CV line with Mix Out + quantizer

### Patch idea
- Set all four sections to **AD**
- Leave normalled chain behavior active, or trigger section 1 externally
- Set different Attack/Decay times on each section
- Use different polarizer settings for each channel
- Patch **Mix Out → Quantizer → VCO 1V/oct**

### What happens
The combined output becomes a repeating analog phrase contour. The quantizer turns that contour into notes.

### Why it works
Each envelope contributes a timed rise/fall to the total CV. Because the stages trigger one another, you get a multi-segment melodic phrase rather than a simple triangle LFO.

### Tips
- Use **short attacks** for more stepped-sounding motion
- Use **different decay times** for phrase asymmetry
- Try:
  - Ch1 + full positive
  - Ch2 slight negative
  - Ch3 medium positive
  - Ch4 full negative  
  This often creates contour shifts that quantize into memorable note loops

---

## 2. Use the 4 individual envelope outs as four melodic lanes

Instead of using Mix Out, use each **Env Out** separately.

### Patch idea
- Env 1 → quantizer A → VCO pitch
- Env 2 → filter cutoff
- Env 3 → wavefolder CV
- Env 4 → VCA CV or second oscillator FM index

Or:

- Env 1/2/3/4 into a **sequential switch**
- Switch output → quantizer → oscillator pitch

### What happens
Each stage becomes its own melodic shape. If you route them one at a time through a switch, you effectively get a **4-source melodic selector**.

### Musical result
This can sound like:
- 4-note motif sources
- varying phrase fragments
- evolving lead lines
- pseudo-sequenced arpeggios

---

## 3. Make an 8-stage melodic phrase from the module’s natural chaining

The manual notes that with all trigger inputs open and the units chained, the module behaves like a **complex 8-stage LFO** because each section has a rise and fall segment.

That means musically you can think of it as:

- stage 1 rise
- stage 1 fall
- stage 2 rise
- stage 2 fall
- stage 3 rise
- stage 3 fall
- stage 4 rise
- stage 4 fall

### Patch idea
- Use default internal chaining
- Set all four units to AD or use cyclic behavior
- Patch Mix Out → quantizer → oscillator

### Result
You get a recurring 8-segment phrase contour, which often feels more “composed” than a simple LFO.

### Good for
- basslines
- repeating ostinatos
- Berlin-school style looping pitch movement
- generative melodies

---

## 4. Use comparator outputs as note clocks

The comparator outputs change according to threshold crossings. Since they’re related to each envelope’s decay phase and threshold setting, they produce logic events at musically meaningful times.

### Patch idea
- Mix Out → quantizer → VCO pitch
- Cp 1 → envelope trigger for VCA
- Cp 2 → trigger percussion or accent envelope
- Cp 3 → advance switch
- Cp 4 → trigger sample & hold

### What happens
Now pitch is moving continuously, but note articulation is driven by internal stage timing. This creates **melody plus rhythm from one module**.

### Musical benefit
You can separate:
- **pitch contour** from Mix Out
- **note onset timing** from Cp or EOA outputs

That’s a very powerful way to get melodic complexity.

---

## 5. Use EOA outputs to sample the melodic contour

A very strong melodic patch is to let the A-143-1 make a continuous changing CV, then **sample it** at chosen moments.

### Patch idea
- Mix Out → Sample & Hold input
- EOA 1 or Cp 1 → Sample & Hold trigger
- S&H out → quantizer → VCO 1V/oct

### What happens
Instead of hearing a glide, you hear discrete note changes taken from the evolving analog contour.

### Why this is good
This turns the module into a **phrase generator** with repeatable but adjustable note extraction points.

### Variation
Use different EOA outputs to trigger the sample & hold so different stages “pick” the note.

---

## 6. Use AD mode for phrase envelopes, LFO mode for autonomous melodies

The mode switch per section matters a lot.

### In AD mode
Each section behaves like a triggered envelope. Best for:
- externally clocked phrases
- repeatable note lengths
- synchronizing melody to drums/gates

### In LFO mode
Each section free-runs. The manual notes you should insert a **dummy cable** in the trigger input if you don’t want the preceding comparator to retrigger it.

Best for:
- drifting melodic motion
- semi-independent cyclical pitch sources
- phasing melodies

### Melodic strategy
- Put 2 channels in AD mode for phrase structure
- Put 2 channels in LFO mode for drifting pitch/timbre modulation
- Combine via Mix Out or externally in a CV mixer

This gives melody with both **form** and **instability**.

---

## 7. Make counter-melodies with positive and negative polarities

Because each channel has a polarizer into the mix, some envelopes can push pitch up while others pull it down.

### Patch idea
- Ch1 polarizer: high positive
- Ch2 polarizer: low negative
- Ch3 polarizer: medium positive
- Ch4 polarizer: medium negative
- Mix Out → quantizer → VCO pitch

### Result
This creates contour interference:
- some stages lift the phrase
- some stages drag it downward

Quantized, this can sound like:
- tension/release
- answers to previous notes
- recurring melodic “hooks”

This is one of the most musical features of the module.

---

## 8. Trigger multiple voices sequentially for melodic rounds

The manual specifically mentions controlling multiple similar modules in sequence. For melodic work, that means you can use the four envelope outs to animate **four voices or four VCAs**.

### Patch idea
- One oscillator drone or chord source
- Four VCAs or four filters
- Env 1 → voice 1 amplitude/filter
- Env 2 → voice 2 amplitude/filter
- Env 3 → voice 3 amplitude/filter
- Env 4 → voice 4 amplitude/filter

If each voice has a different pitch, the chained envelopes create a **rotating melodic pattern** across voices.

### Good for
- round-robin melodies
- quadraphonic phrases
- stereo ping-pong note animation
- chord tones appearing one after another

---

## 9. Use retrigger behavior musically

The manual notes unusual retrigger behavior:

- During **attack**, the envelope cannot be retriggered/reset
- During **decay**, a trigger changes direction from decay back to attack

This is very musical.

### Why
If you feed triggers during decay, the contour bends upward again instead of restarting hard. That produces:
- elastic phrasing
- pitch “bounces”
- curved melodic ornaments
- less mechanical repetition

### Patch idea
- Send a clock or burst generator into one trigger input
- Use that envelope output for pitch CV through a quantizer

The resulting phrase will feel less grid-locked than a standard sequencer.

---

## 10. Use threshold as a phrase spacing control

The **Threshold** knob is easy to underestimate. It affects when the comparator changes state, which affects when the next stage is triggered in the internal chain.

### Musically, threshold changes:
- note spacing
- amount of overlap/urgency between stages
- phrase swing
- density of melodic movement

### Patch practice
Set similar Attack/Decay values on all four channels, then change only thresholds.

You’ll hear the phrase timing shift significantly without changing the basic envelope lengths.

This is great for:
- evolving ostinatos
- irregular “sequencer” timing
- humanized repeating phrases

---

## Example melodic patches

## Patch 1: Simple looping melody
**Goal:** repeating 4–8 note melodic line

- Leave trigger inputs unpatched for internal chaining
- Set all channels to **AD**
- Set varied attack/decay times
- Polarizers to mixed positive/negative values
- Mix Out → quantizer → VCO 1V/oct
- One EOA output → trigger envelope for VCA

**Result:** self-running melodic loop with articulated note events.

---

## Patch 2: Triggered phrase generator
**Goal:** one externally clocked phrase per gate

- External gate/trigger → Trig In 1
- Chained internally from there through stages 2–4
- Mix Out → quantizer → oscillator pitch
- Separate ADSR/VCA handles loudness

**Result:** every input trigger launches a full melodic phrase.

This is especially useful for leads and bass phrases.

---

## Patch 3: Semi-random note selection
**Goal:** generative but structured melody

- Mix Out → sample & hold input
- Cp 2 → sample & hold trigger
- S&H out → quantizer → VCO pitch
- Cp 4 → trigger accent envelope

**Result:** notes are extracted from the changing contour at repeating but uneven times.

---

## Patch 4: Two-voice melodic conversation
**Goal:** lead and answer line

- Env 1 + Env 2 mixed/quantized → VCO A pitch
- Env 3 + Env 4 mixed/quantized → VCO B pitch
- EOA outputs used to trigger separate VCAs

**Result:** one module generates two related melodic lines with shared timing DNA.

---

## Patch 5: Arpeggio-like phrase with switch
**Goal:** stepped melody from four contour sources

- Env 1/2/3/4 → sequential switch inputs
- Clock or EOA drives switch advance
- Switch output → quantizer → VCO pitch

**Result:** the melody jumps among four differently shaped control sources.

---

## Best companions for melodic use

The A-143-1 becomes much more directly melodic when paired with:

- **Quantizer** – essential for tonal note output
- **Sample & Hold** – turns evolving contours into steps
- **Sequential switch** – selects among envelope sources
- **Clock / trigger source** – synchronizes phrase starts
- **VCA / LPG** – articulates notes
- **Precision adder / offset / attenuator** – places pitch in a useful range
- **Oscillator with good 1V/oct tracking**
- **Logic / clock divider** – for structured stage triggering

Without a quantizer, it is still great for glides, portamento-style lines, and atonal or experimental pitch movement.

---

## Practical melodic advice

### Use attenuation on pitch
The envelope range is large for 1V/oct use. If patched directly to pitch, it may span many octaves. Usually you’ll want:

- attenuator
- offset
- quantizer with input scaling if available

### Quantize after mixing
For musical scales, the most effective order is often:

**A-143-1 Mix Out → attenuate/offset → quantizer → oscillator**

### Use EOA for articulation
The contour itself can define pitch, but use EOA or comparator outputs to generate note gates.

### Keep some channels subtle
If every channel contributes strongly to Mix Out, the melody may become too jumpy. Often the best results come from:
- one dominant contour
- two medium influences
- one small destabilizer

---

## Summary

The Doepfer **A-143-1** is best understood melodically as a **complex control-voltage phrase generator**, not a conventional sequencer.

It can create melodic material by:

- generating continuous pitch contours from the four envelope sections
- summing them into one composite phrase at **Mix Out**
- using **polarizers** to shape melodic direction
- using **threshold/comparator timing** to create irregular stage progression
- using **EOA and comparator outputs** to trigger note articulation, switching, or sample & hold
- running as either a triggered phrase generator or a self-cycling melodic engine

If you add a **quantizer** and optionally a **sample & hold or sequential switch**, the A-143-1 becomes extremely effective for:

- looping melodies
- bassline contours
- generative note patterns
- multi-stage phrases
- evolving counter-melodies
- multi-voice sequential animation

In short:  
**the A-143-1 doesn’t write notes directly — it writes the motion that notes can be extracted from.**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)