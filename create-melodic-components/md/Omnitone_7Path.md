# Omnitone — 7Path

- [Manual PDF](../../manuals/7Path - Ethernet Patch Cable Bridge - Omnitone.pdf)

---

# [Manual PDF / Product Page](https://omnitone.ca/products/7path-connect-eurorack-cases-in-synth-jams-eurorack-module-to-connect-cases-no-long-patch-cables)

## Module identified
From the attached PDF, the module is:

- **Omnitone 7Path – Ethernet Patch Cable Bridge**

This PDF appears to be a product page rather than a full manual, but it includes enough information to understand the module’s function.

## What the module does
**7Path** is a **pair of passive Eurorack bridge modules** that lets you send **7 independent patch signals** between:

- two different Eurorack cases, or
- two distant points in a large system

using a single **ethernet cable**.

### Key details from the PDF
- **4HP**
- **3U**
- **20mm deep**
- **Passive**
- **No power required**
- **7 signal paths**
- **Jack mapping is direct:** jack **1→1**, **2→2**, etc.
- Supports **any type of Eurorack signal**
- Claimed support up to **10 ft with unshielded ethernet cable**, more with shielded cable
- Box includes:
  - **2x 7Path modules**
  - **4x mounting screws**
- **Ethernet cable not included**

## Important musical reality check
Because **7Path does not generate, process, quantize, sequence, or shape pitch on its own**, it is **not a melodic voice module** by itself.

Instead, it is a **signal transport utility**. Its role in melodic patching is to let your **melody-related signals** travel neatly across cases without a mess of long patch cables.

So the best answer to “how these modules can be used together to create melodic components” is:

- the two included **7Path modules** work together as a **7-channel bridge**
- they enable **melodic systems spread across multiple cases**
- they let you separate:
  - sequencers
  - quantizers
  - controllers
  - oscillators
  - envelopes
  - VCAs
  - effects

while still patching them as one instrument

---

## How the two 7Path modules work together melodically

Think of the pair as a **remote 7-channel patchbay**.  
Whatever melodic control or audio signal enters one side appears at the matching jack on the other side.

### Typical signal types you can send
For melodic work, the most useful signals are:

- **1V/oct pitch CV**
- **gate**
- **trigger**
- **clock**
- **modulation CV** (LFO, random, envelope, pressure, velocity-like CV)
- **audio** (oscillator output, submix, voice return)
- **transpose CV**

---

## Best melodic use cases

## 1. Remote sequencer to voice connection
If your sequencer lives in one case and your oscillators/voices live in another, 7Path is ideal.

### Example patch
**Case A:**
- Pitch sequencer out → 7Path jack 1
- Gate sequencer out → 7Path jack 2
- Mod lane / accent CV → 7Path jack 3
- Clock out → 7Path jack 4

**Case B:**
- 7Path jack 1 → oscillator **1V/oct**
- 7Path jack 2 → envelope gate in
- 7Path jack 3 → filter cutoff CV or wavefold amount
- 7Path jack 4 → clock input on a local modulation source or sequencer

### Result
You get a complete melodic voice controlled remotely:
- stable pitch stream
- note articulation via gate
- expressive timbral modulation
- synchronized movement

This is probably the most straightforward use.

---

## 2. Build a distributed melodic voice across two cases
A melodic voice often uses multiple modules:
- pitch source
- quantizer
- oscillator
- envelope
- VCA
- filter
- effects

7Path lets these pieces live in different cases without chaos.

### Example
**Case A**
- keyboard or random CV source
- quantizer
- clocked sequencer

**Case B**
- VCO
- filter
- LPG/VCA
- envelope
- delay/reverb

### Patch
- Quantizer out → 7Path 1 → VCO 1V/oct
- Gate source → 7Path 2 → envelope gate
- Secondary CV → 7Path 3 → filter FM / cutoff
- Accent CV → 7Path 4 → VCA CV
- Audio return from VCO or final voice → 7Path 5 back to Case A mixer

### Result
You can keep control modules in one case and sound-generation modules in another while treating them like one melodic instrument.

---

## 3. Send multiple pitch-related signals for harmonies
Since there are **7 channels**, you can transmit several melodic lines at once.

### Example harmonic allocation
- **1:** Voice 1 pitch CV
- **2:** Voice 1 gate
- **3:** Voice 2 pitch CV
- **4:** Voice 2 gate
- **5:** Shared clock
- **6:** Transposition CV
- **7:** Audio return or modulation

### Result
One 7Path pair can support:
- two independent mono melodic voices, or
- one voice plus lots of expressive control, or
- a lead plus bassline setup across cases

This is especially useful in live systems where one skiff holds sequencing and another holds voices.

---

## 4. Transport quantized pitch to avoid moving the whole pitch engine
A common modular melody workflow is:

1. Create raw CV from:
   - sequencer
   - random source
   - sample & hold
   - pressure controller
2. Quantize it
3. Send it to a VCO

If the quantizer is in a separate case from the oscillator, 7Path makes that simple.

### Example
**Case A**
- Random stepped CV → quantizer
- Quantizer out → 7Path 1
- Trigger pattern → 7Path 2

**Case B**
- 7Path 1 → oscillator 1V/oct
- 7Path 2 → envelope trigger/gate

### Result
You get musically constrained melodies in one case and synth voice generation in another.

This is one of the strongest musical uses because **pitch CV integrity and clean physical routing matter**.

---

## 5. Use one case as a control skiff and the other as a sound case
Many performers keep:
- sequencers
- touch controllers
- clocks
- utilities

in a shallow portable skiff, while keeping:
- oscillators
- filters
- VCAs
- effects

in a larger main case.

7Path is almost purpose-built for this.

### Good 7-channel assignment for melodic performance
- **1:** main pitch CV
- **2:** main gate
- **3:** modulation wheel / fader CV
- **4:** transpose CV
- **5:** clock/reset
- **6:** accent or velocity-style CV
- **7:** audio return from the voice

### Why this works musically
This gives you a playable remote mono synth architecture:
- note selection
- articulation
- expressive control
- synced timing
- returned audio to the performance mixer

---

## 6. Create call-and-response or multi-zone melodic systems
If your modular is physically spread out, 7Path lets one melodic subsystem “talk” to another.

### Example
- Sequencer in case 1 drives bass voice in case 2
- A second CV lane in case 1 transposes a lead in case 2
- Audio from case 2 returns via another path to a mixer in case 1

### Result
You can design:
- bass/lead separation
- control/sound separation
- voice clusters in separate cases

This is very useful for complex melodic arrangements.

---

## 7. Carry both control and audio for a complete melodic signal chain
Because the module can pass **any Eurorack signal**, you don’t have to use all channels for CV/gates.

You can use some for **audio returns**.

### Example full voice over 7 lines
- **1:** pitch CV
- **2:** gate
- **3:** envelope/mod CV
- **4:** accent CV
- **5:** oscillator audio
- **6:** post-filter audio
- **7:** final voice output or effect send/return

This makes 7Path function like a compact multicore snake for your modular.

For melody building, that means you can:
- send note control to a remote voice
- bring the resulting sound back to where your mixer or performance interface lives

---

## Concrete melodic patch ideas

## Patch idea 1: Remote mono lead
**Case A**
- Step sequencer pitch out → 7Path 1
- Step sequencer gate out → 7Path 2
- Accent row → 7Path 3

**Case B**
- 7Path 1 → VCO 1V/oct
- 7Path 2 → envelope gate in
- Envelope out → VCA CV
- VCO → filter → VCA
- 7Path 3 → filter cutoff CV
- Final audio → local mixer or 7Path 4 back to Case A

**Musical result:**  
A classic sequenced lead voice with dynamic accents.

---

## Patch idea 2: Bassline plus lead over one ethernet cable
**Channel layout**
- 1: bass pitch
- 2: bass gate
- 3: lead pitch
- 4: lead gate
- 5: shared clock
- 6: transpose CV
- 7: summed audio return

**Musical result:**  
Two coordinated melodic parts between cases with minimal cable clutter.

---

## Patch idea 3: Generative melody control bridge
**Case A**
- Random stepped CV → quantizer → 7Path 1
- Trigger sequencer → 7Path 2
- Slow LFO → 7Path 3
- Clock → 7Path 4

**Case B**
- 7Path 1 → oscillator pitch
- 7Path 2 → envelope trigger
- 7Path 3 → timbre/fold/filter modulation
- 7Path 4 → clock divider or synced delay modulation

**Musical result:**  
A generative melodic line with synchronized movement and evolving tone.

---

## Patch idea 4: Playable keyboard-to-voice bridge
**Case A**
- MIDI-to-CV or keyboard controller:
  - pitch CV → 7Path 1
  - gate → 7Path 2
  - mod wheel CV → 7Path 3
  - aftertouch/aux CV → 7Path 4

**Case B**
- 7Path 1 → 1V/oct
- 7Path 2 → envelope
- 7Path 3 → vibrato depth / FM amount
- 7Path 4 → filter or wavefolder

**Musical result:**  
A physically separated but expressive performance voice.

---

## Strengths for melodic use
### 1. Cleaner live setup
Instead of multiple long patch cables between cases, you use one ethernet cable.

### 2. Easier system organization
You can group modules by function:
- controllers together
- sound sources together
- effects together

### 3. Better ergonomics
You can keep performance-critical melodic tools close at hand while your larger voice architecture lives elsewhere.

### 4. Multi-signal efficiency
Seven simultaneous lines is enough for a surprisingly complete melodic ecosystem.

---

## Limitations
## 1. Not a sound source
7Path does **not** create melodies by itself.

You still need other modules such as:
- sequencers
- quantizers
- oscillators
- envelopes
- filters
- VCAs

## 2. No normalization or processing
It simply passes signals straight through. There’s:
- no buffering
- no attenuation
- no mixing
- no multing
- no pitch correction
- no active amplification

## 3. Cable-length considerations
The product page states:
- up to **10 ft** with **unshielded ethernet**
- more with **shielded cable**

For precise melodic work, especially **1V/oct pitch CV**, practical testing is wise. Passive transmission can be sensitive depending on:
- cable quality
- length
- destination module input behavior
- the source driving the signal

If pitch precision matters, test your exact setup.

## 4. No ethernet data/networking
This is important: it uses an **ethernet cable as physical wiring**, not computer networking.  
Do **not** treat it like a network device.

---

## Best ways to use 7Path in a melodic system
If I were building around this as a musician, I’d use it in one of these three ways:

### Option A: Sequencer case → voice case
Best for live use and large systems.

### Option B: Controller skiff → performance voice
Best for expressive melodic playing.

### Option C: Voice send/return bridge
Best when your melody generator and final mixer are in different cases.

---

## Bottom line
**Omnitone 7Path** is not a melody generator, but it is very useful for **making multi-case melodic patches practical**.

It shines when you want to send:
- **pitch CV**
- **gates**
- **clocks**
- **modulation**
- and even **audio returns**

between cases in a clean, organized way.

So in a melodic workflow, the two 7Path modules are best thought of as a **7-lane highway** connecting your melody brain in one case to your voice architecture in another.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)