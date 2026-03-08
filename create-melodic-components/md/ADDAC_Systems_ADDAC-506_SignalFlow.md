# ADDAC Systems — ADDAC-506 SignalFlow

- [Manual PDF](../../manuals/ADDAC506_SignalFlow.pdf)

---

[Manual PDF](attachment)

# ADDAC506 VC Stochastic Function Generator & Expansion
How to use it for **melodic** patching

The ADDAC506 is primarily a **4-channel stochastic envelope / function generator**, not a dedicated oscillator or sequencer. But in Eurorack, that still makes it very useful for melody because it can generate:

- evolving control voltages
- stepped or re-randomized timing relationships
- phrase contours
- trigger structures
- layered modulation for pitch, timbre, and articulation

The attached pages describe the **main module plus expansion**, with these important functions:

- **4 independent envelope channels**
- **Randomized rise and fall times** between user-set min/max ranges
- **CV control** over all rise/fall min/max settings
- **Loop / One-shot**
- **Slew / Trigger** behavior
- **Amplitude** control: approximately **-10V to +10V**
- **Offset** control: approximately **-10V to +10V**
- **Envelope curve** from **linear to logarithmic/exponential**
- **Gate out** during rise
- **EOR** (end of rise) and **EOF** (end of fall) outputs
- **Average Mix Out**
- **Summing Mix Out**
- Expansion:
  - **Random trigger inputs** to force new randomization mid-cycle
  - **Random CV outputs** reflecting the random value used for rise or fall time

## What this means musically

This module does **not directly output quantized pitch sequences**. Instead, it creates **animated control voltages** that can become melodic when sent to:

- a **VCO 1V/oct input** through an attenuator/quantizer
- a **quantizer**
- a **sample & hold**
- a **sequential switch**
- a **wavefolder/filter/resonator** to create pitch-like timbral melodies
- logic or clocking utilities for phrase generation

In practice, the ADDAC506 is best thought of as a **melody-shaping source**, not a conventional note sequencer.

---

# Core melodic use cases

## 1. Use one channel as a pitch contour source
Patch:

- **ADDAC506 channel output** → **quantizer input**
- **quantizer output** → **VCO 1V/oct**
- Trigger the channel with gates or put it in **loop**
- Adjust:
  - **Rise Min/Max**
  - **Fall Min/Max**
  - **Amplitude**
  - **Offset**
  - **Curve**

### Result
The envelope becomes a continuously changing melodic contour. Once quantized, the slopes turn into note motion.

### Tips
- Use **small amplitude** for narrow melodic ranges.
- Use **offset** to place the melody into a useful register.
- If **Rise Min > Rise Max** or similarly for Fall, the manual says it behaves as a **fixed** time control. That’s useful when you want one side stable and the other stochastic.
- **Log/exp curves** can bias the melody toward lingering around some notes and moving faster through others.

---

## 2. Create 4 interrelated melodic lanes
Since there are **4 independent channels**, you can build:

- 4 voices
- 4 modulation lanes for one voice
- 3 voices plus one master phrase modulator

Patch idea:

- **Output 1** → quantizer → VCO A pitch
- **Output 2** → quantizer → VCO B pitch
- **Output 3** → filter cutoff or wavefolder depth
- **Output 4** → VCA CV or FM amount

### Why it works
Even if each channel is independent, they share the same panel logic and can be set to similar or contrasting timing regions. That gives a family resemblance between voices, which often feels more musical than fully unrelated random sources.

---

## 3. Use EOR and EOF to make melodic cascades
The manual states:

- **EOR** outputs when rise ends
- **EOF** outputs when fall ends
- **Gate out** is high during rise

This makes the 506 very strong for **event chaining**.

Patch:

- **Channel 1 EOR** → trigger **Channel 2**
- **Channel 2 EOF** → trigger **Channel 3**
- **Channel 3 EOR** → trigger a **sample & hold**
- S&H output → quantizer → VCO pitch

### Result
You get a phrase where melodic note changes happen at structurally meaningful points in the envelopes rather than on a strict clock.

This is excellent for:
- generative melodies
- rubato phrases
- pseudo-counterpoint
- self-evolving note timing

---

## 4. Use the expansion Random CV outputs as melodic sources
The expansion provides:

- **Random trigger inputs** for re-randomizing rise/fall values
- **Random CV outputs** that expose the CV value used for rise/fall randomization
- jumper selection between **rise random** or **fall random**

This is one of the most immediately melodic features.

Patch:

- **Random CV out** → quantizer → VCO 1V/oct
- **Random Trigger In** receives clocks, gates, or irregular triggers

### Result
Every randomization event can generate a new pitch-related voltage. Because that voltage is tied to the envelope timing calculation, your **note choices and note shape/timing become correlated**.

That correlation is musically powerful: notes and articulation evolve together.

### Great use
- Rise random CV controls **pitch**
- Same channel envelope output controls **VCA**
- The note and its articulation are linked

This often sounds more intentional than using unrelated random sources.

---

## 5. Build melody from the Average Mix output
The manual describes:

- **Average Mix Out** = average CV from all 4 channels
- **Summing Mix Out** = sum of all 4 outputs

Patch:

- **Average Mix Out** → quantizer → oscillator pitch

### Why use average instead of sum?
Average tends to be:
- smoother
- more centered
- less likely to jump wildly

This is useful for:
- singable melodic lines
- slowly evolving lead lines
- modal drifting phrases

If each channel has different rise/fall ranges, the average output becomes a composite phrase made from several interacting gestural layers.

---

## 6. Use the Summing Mix output for wider melodic leaps
Patch:

- **Summing Mix Out** → attenuator → quantizer → VCO pitch

### Result
The sum output is generally more energetic and volatile than the average. This is better for:
- angular melodies
- experimental atonal lines
- dramatic interval jumps
- chaotic arpeggio-like movement

Because the module can output large voltages, attenuation before the quantizer is often very important.

---

## 7. Slew mode as melodic glide processor
The manual says:

- **Slew** works for CVs, gates, and triggers
- It behaves somewhat like a **CV envelope follower**
- **Trigger** mode generates one cycle per trigger

In melodic systems, **Slew mode** can reshape incoming pitch or modulation CV.

Patch:

- external sequencer CV → **channel signal input**
- channel set to **Slew**
- channel output → quantizer or directly to VCO pitch

### Uses
- smooth glides between sequenced notes
- randomized portamento behavior if rise/fall min/max are spread
- expressive pitch lag
- converting stepped random into curved melodic movement

A particularly nice patch:
- sequencer CV → Slew channel
- output → quantizer
- quantizer → VCO

This gives a melody that keeps the broad gesture of the original sequence but gains stochastic timing and contour.

---

## 8. Trigger mode for articulated note shapes
In **Trigger** mode, each incoming trigger fires one envelope cycle.

Patch:

- clock or rhythm source → channel input
- channel output → quantizer → VCO pitch
- same trigger or gate out → envelope/VCA for audio articulation

### Result
Each note can have a pitch trajectory over the duration of the triggered envelope. Depending on speed, this may sound like:
- ornamentation
- pitch bends
- micro-phrases
- plucked/struck melodic gestures

This works especially well with:
- LPGs
- FM voices
- resonators
- pinged filters

---

# Best ways to combine the main module and expansion for melody

## A. Correlated pitch + articulation patch
Patch:

- **Expansion Random Trigger In 1** ← rhythmic trigger pattern
- **Random CV Out 1** → quantizer → oscillator pitch
- **Envelope Out 1** → VCA CV
- **Gate Out 1** → envelope trigger or logic clock

### Why it’s good
Pitch changes happen when the rise/fall randomization changes, while the envelope controls note articulation. This creates phrases where timing, note choice, and dynamics feel related.

---

## B. One channel per melodic function
A very effective 4-channel allocation:

- **Channel 1**: main pitch contour
- **Channel 2**: transposition amount
- **Channel 3**: timbre movement
- **Channel 4**: phrase-level amplitude or density

Patch example:

- Ch1 out → quantizer A input
- Ch2 out → attenuator → add to Ch1 before quantizer, or transpose quantizer reference
- Ch3 out → filter cutoff / fold / FM index
- Ch4 out → VCA CV or clock probability modulation

This creates melodies that breathe and transform rather than just changing notes.

---

## C. Self-generating canon / round
Patch:

- Ch1 **EOF** → trigger Ch2
- Ch2 **EOF** → trigger Ch3
- Ch3 **EOF** → trigger Ch4
- Ch4 **EOF** → trigger Ch1

Then:
- all 4 outputs → 4 quantizer channels → 4 oscillators  
or
- all 4 outputs mixed/selected into one pitch path

### Result
A rotating network of envelopes, each with randomized rise/fall times, creates staggered melodic entries and evolving relationships. Very good for ambient, minimalism, and generative counterpoint.

---

## D. Random CV outputs as hidden sequencer
The expansion’s Random CV outputs can function like a strange sequencer lane.

Patch:

- **Random CV Out 1–4** → precision adder mixer or sequential switch
- output → quantizer → VCO pitch
- trigger the random inputs with related but not identical clocks

### Result
You effectively get four stochastic pitch sources whose update timing is independently controllable. This can produce:
- non-repeating melodies
- polymetric note changes
- phrase memory-like behavior if clocks are slow

---

# Practical melodic patch recipes

## Patch 1: Generative lead voice
You need:
- ADDAC506 + expansion
- quantizer
- VCO
- VCA
- envelope or LPG
- trigger source

Patch:
- Random trigger source → **Expansion Random In 1**
- **Random CV Out 1** → quantizer → VCO 1V/oct
- **Output 1** → VCA CV or filter CV
- **Gate Out 1** → trigger envelope/LPG
- Audio voice → VCA → output

Set:
- medium speed
- trigger mode
- moderate rise/fall ranges
- small pitch range via quantizer/attenuation

Result:
A coherent generative melody where note selection and envelope behavior are connected.

---

## Patch 2: Melodic drone with internal movement
Patch:
- **Average Mix Out** → attenuator → quantizer → oscillator pitch
- **Output 1** → filter cutoff
- **Output 2** → wavefolder amount
- **Output 3** → FM index
- **Output 4** → stereo movement or reverb send CV

Set channels to loop with different random ranges.

Result:
A slowly shifting drone with a pitch center that continuously evolves.

---

## Patch 3: Pseudo-arpeggiator
Patch:
- master clock → trigger Ch1
- Ch1 EOR → trigger Ch2
- Ch2 EOR → trigger Ch3
- Ch3 EOR → trigger Ch4
- Ch1–4 outputs → sequential switch CV inputs or mixer
- switched/mixed result → quantizer → VCO

Result:
A chain of linked contour events that acts like an arpeggiator, but with variable note lengths and spacing.

---

## Patch 4: Humanized melody processor
Patch:
- external sequencer pitch CV → channel input in **Slew** mode
- channel output → quantizer → VCO pitch
- expansion random trigger input receives sparse accents

Result:
Your normal melody becomes organic and slightly unpredictable, with changing glide/response behavior.

---

# Important musical behaviors from the manual

## Randomization happens at cycle start
The manual specifically says the rise/fall randomization occurs **at the start of a cycle**. If you move controls during the cycle, changes are not applied until the next trigger/loop.

### Musical implication
This makes phrase behavior stable within each note/event, which is good for melody. You don’t get erratic mid-note parameter changes unless you use the **expansion random trigger input**.

---

## Expansion random trigger can change timing mid-cycle
The expansion allows re-triggering the randomization **at any point in time**.

### Musical implication
This is ideal for:
- accents
- fills
- phrase mutations
- occasional surprise notes or bends

Use a separate rhythm source to inject this only on selected beats.

---

## Lock / Unlock supports focused channel editing
The manual says lock holds each channel’s rise/fall settings and prevents changes, making it easier to treat channels independently.

### Musical implication
You can tune one channel as a stable melodic voice while letting others remain volatile.

---

## Amplitude and offset are crucial
Because the envelope amplitude can span approximately **-10V to +10V**, and offset also shifts overall voltage, the raw output range is too large for direct melodic use in many patches.

### Recommendation
For pitch work, use:
- attenuator
- offset utility
- quantizer
- precision adder

This module becomes much more musically controllable when scaled carefully.

---

# Strengths for melodic composition

## What it excels at
- generative melody
- correlated pitch and articulation
- phrase evolution
- non-grid timing
- expressive CV contours
- ensemble-like multi-voice motion
- slow shifting tonal structures

## What it is not ideal for by itself
- exact step sequencing
- repeatable tonal basslines
- strict 16-step melodies
- direct scale-locked pitch output without a quantizer

---

# Best companion modules

To get the most melodic value from the ADDAC506, pair it with:

- **Quantizer**  
  Essential if you want tonal melodies.

- **Precision adder / CV mixer**  
  For transposition and combining multiple channels.

- **Sequential switch**  
  Great for turning the four channels into ordered melodic events.

- **Sample & Hold / Track & Hold**  
  Useful for extracting stable note values from moving envelopes.

- **Clock divider / logic**  
  To create interdependent phrase timing from EOR/EOF/Gate signals.

- **Oscillator with good FM/timbre response**  
  The module is excellent not just for pitch but also for melodic timbral animation.

- **Attenuators / offsets**  
  Very important due to the voltage range.

---

# Bottom line

The ADDAC506 and its expansion are best used for melody as a **stochastic phrase generator** rather than a classic sequencer. The most powerful melodic strategies are:

1. **Quantize the envelope outputs**
2. **Use the expansion Random CV outputs for pitch**
3. **Use EOR/EOF/Gate outputs to chain events**
4. **Use Average and Summing outputs for higher-level phrase contours**
5. **Correlate pitch, articulation, and timbre using the same channel**

If you patch it with a quantizer and a few utility modules, it can produce melodies that feel:
- organic
- self-evolving
- structurally coherent
- less repetitive than ordinary step sequencing

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)