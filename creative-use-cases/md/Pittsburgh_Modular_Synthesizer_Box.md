# Pittsburgh Modular — Synthesizer Box

- [Manual PDF](../../manuals/Synthesizer Box - Pittsburgh Modular Synthesizers.pdf)

---

[Manual PDF](https://pittsburghmodular.com/s/Synthesizer-Box-Manual.pdf)

# Pittsburgh Modular Synthesizer Box — creative patch ideas with other modules

The **Synthesizer Box** is basically a compact semi-modular voice made from:
- a **complex analog oscillator** with sub, blade wave shaping, FM, PWM/waveshape modulation
- a **wave mixer**
- a **3-mode LPG / filter / VCA**
- a **wide-range LFO**
- an **ADSR**
- a **final VCA**
- built-in **glide**

What makes it especially fun in a larger Eurorack system is that the normalled internal routings can be overridden almost everywhere. So it can be:
1. a complete standalone synth voice,  
2. a collection of utility submodules, or  
3. a modulation/audio hub for other voices.

---

## Quick summary of the normalled architecture

Useful to keep in mind before patching externally:

- **LFO TRI** is internally routed to:
  - oscillator **FM**
  - oscillator **MOD CV**
- **Envelope OUT** is internally routed to:
  - **LPG CV**
  - **VCA CV**
- Oscillator/mixer is internally routed toward the **LPG**
- **LPG OUT** is internally routed to **VCA IN**
- **1V/O IN** is hardwired through **Glide** into the oscillator

That means the module already gives you a playable “default voice,” and every patch cable you insert can selectively break that normalization.

---

# Best roles for the Synthesizer Box in a system

## 1. Compact main voice
Use it as your primary mono voice and expand its modulation and timbral range with external modules.

Best companions:
- **sequencer** or keyboard CV source
- **clocked modulation**
- **sample & hold / random**
- **extra envelopes**
- **effects** like delay, reverb, wavefolder, distortion

## 2. West-coast flavored voice core
The **blade waveform**, **sub**, **LPG ping mode**, and internal modulation make it particularly nice for plucky, organic, woody, and animated tones.

Best companions:
- **function generator / slope**
- **random voltage**
- **low pass gate or resonator**
- **wavefolder**
- **strike / trigger sequencer**

## 3. Breakout utility cluster
You can split it apart:
- use the **LFO** elsewhere
- use the **ADSR** on another voice
- use the **VCA** as a utility amp
- use the **LPG** as an external processor
- use oscillator outputs independently

This is especially valuable in small systems.

---

# Creative patch ideas

## 1. Dual-motion oscillator animation
The oscillator has two juicy destinations:
- **FM CV IN**
- **MOD CV IN**

Instead of relying on the internal LFO for both, send **two different modulation sources**:
- a **slow random** or stepped CV into **MOD CV IN**
- a **sine/triangle LFO** or envelope into **FM CV IN**

### Result
The pitch movement and waveform movement become decorrelated, which makes the oscillator feel much more alive.

### Great companion modules
- **Make Noise Wogglebug**
- **Mutable Instruments Marbles**
- **Xaoc Batumi**
- any **function generator** like Maths, Rampage, Delta-V

---

## 2. Audio-rate modulation from another oscillator
Because the LFO can go wide range and the oscillator has FM input with **linear/exponential switch**, the Synthesizer Box likes cross-modulation.

### Patch
- External oscillator sine/triangle -> **FM CV IN**
- Try **linear FM** first
- Tune the external oscillator to harmonic intervals or detuned offsets

### Result
Metallic, vocal, bell-ish, tearing, and complex analog FM tones.

### Best module partners
- a clean sine-core VCO:
  - **Intellijel Dixie II+**
  - **Doepfer A-110-6**
  - **Instruō Ts-L**
- or another character oscillator for dirty FM

Tip: also send a related envelope to **MOD CV IN** for evolving spectra.

---

## 3. Use the blade input as a timbre injection point
The **BLADE IN** is one of the most interesting inputs on the module. Since the blade waveform is a special complex saw-derived shape, feeding voltage there should let you animate it in ways that differ from ordinary PWM.

### Try feeding BLADE IN with
- a slow triangle LFO
- an envelope
- audio-rate oscillator
- filtered noise
- stepped random voltage

### Result
Shifting asymmetry, spectral movement, sharp vocal/tearing textures, and unstable “alive” harmonics.

### Best partners
- another VCO
- random source
- envelope follower
- chaotic modulation source

A neat patch:
- **noise -> slew limiter -> BLADE IN**
This gives semi-fluid, organic timbral drift.

---

## 4. Ping the LPG with trigger patterns
The module’s **LPG** has a **PING** mode that converts modulation into a short trigger-like strike. This is one of the most musical parts of the Synthesizer Box.

### Patch
- Set LPG mode to **LPG**
- Set mod/ping switch to **PING**
- Send triggers, gates, or rhythmic pulses into **LPG CV IN**
- Feed oscillator, external audio, or noise into **LPG IN**

### Result
Bongo-like, plucked string, woody percussion, struck-filter sounds.

### Companion modules
- trigger sequencers:
  - **Tiptop Circadian Rhythms**
  - **Steppy**
  - **Pamela’s New Workout**
- probability trigger generators
- burst generators
- noise/percussion sources

This patch is fantastic with:
- **noise into LPG IN** for hand drum / shaker / click percussion
- **external wavetable or FM oscillator into LPG IN** for plucked digital-organic hybrids

---

## 5. Use the LPG as an external processor
Because **LPG IN** overrides the internal audio routing, the Synthesizer Box can become a character processor for other modules.

### Feed into LPG IN
- drum loops from a sample player
- a digital oscillator
- chords from a polyphonic voice mixed to mono
- noise or field recordings
- another synth voice

Then use:
- internal envelope normalled to LPG CV
- or external modulation into **LPG CV IN**

### Result
A more organic, dynamic, less static version of the source. In LPG mode especially, louder moments get brighter while quieter parts stay more natural.

### Best source types
- harsh digital oscillators
- wavetable voices
- samples
- external drum voices

This is a very strong way to “analog-ize” sterile sound sources.

---

## 6. Use envelope and LPG separately for two jobs
One overlooked trick is to break the module into independent sections.

### Example patch
- Use **ENV OUT** to modulate an external filter or oscillator
- Feed an external modulation source into **LPG CV IN**
- Use Synthesizer Box oscillator through LPG/VCA as usual

### Result
You effectively gain an extra system envelope while still using the voice.

Even better:
- Use **ENV OUT** on an external reverb/delay CV input while the internal LPG is pinged by triggers.

This gives coherent articulation across the whole patch.

---

## 7. Parallel waveform processing
The oscillator offers multiple outs:
- **TRI OUT**
- **S/B OUT**
- **SQR OUT**
- **MIX OUT**

These are gold in a modular setup.

### Patch idea
- **TRI OUT** -> wavefolder
- **SQR OUT** -> clock divider / subharmonic processing / logic / comparator
- **S/B OUT** -> filter
- mix externally

### Result
A single oscillator becomes a layered composite voice with separate spectral lanes.

### Great supporting modules
- mixers
- VCAs
- wavefolders
- filters
- resonators
- crossfaders

Specific modules:
- **Xaoc Tallin** or **Intellijel Quad VCA** for dynamic mixing
- **Bastl Ikarie** or **QPAS** for stereo filtering
- **Joranalogue Fold 6** or **Intellijel Bifold** for triangle folding

---

## 8. Build a pseudo-duophonic patch
The Synthesizer Box is monophonic, but you can make it behave like two related voices.

### Patch
- Use **MIX OUT** as voice A through the internal LPG/VCA
- Send **TRI OUT** or **SQR OUT** to an external filter + VCA as voice B
- Use same pitch CV to both paths
- Modulate one path differently

### Result
Layered intervals, pseudo-paraphonic behavior, stereo spreads, body + edge combinations.

For example:
- internal path = plucky LPG voice
- external path = long filtered drone or delayed pad layer

---

## 9. Turn the LFO into an audio oscillator
The LFO is described as **wide range**, including audio-rate modulation territory.

### Patch
- LFO **TRI OUT** or **SQR OUT** -> external mixer / filter / VCA
- Sequence the rate manually or CV it indirectly through a VCA-and-offset setup elsewhere

### Result
A bonus lo-fi oscillator or modulation-rate audio source.

### Fun uses
- audio-rate modulation for another oscillator
- sub-audio square for rhythmic gates
- triangle as a second crude audio source to layer with the main VCO

Especially good if you want:
- beating
- rough FM
- pseudo-sync-like interactions

---

## 10. Clock the whole voice with stepped random
Since the oscillator and LPG both respond well to modulation, combining a **sample & hold** or **quantized random** source with trigger-derived articulation gets very musical.

### Patch
- random quantized CV -> **1V/O IN**
- trigger sequence -> **ENV IN**
- slower random -> **MOD CV IN**
- another slow random or envelope -> **LPG CV IN**

### Result
Self-playing melodic lines with animated timbre and organic articulation.

### Excellent partner modules
- **Mutable Marbles**
- **Turing Machine**
- **Pam’s** with random/quantizer support
- any quantizer + noise/sample-hold combo

---

## 11. External wavefolder after the triangle output
The **triangle output** is perfect folder material.

### Patch
- **TRI OUT** -> wavefolder -> external VCA/filter
- keep internal voice running from **MIX OUT** or LPG/VCA chain

### Result
You get two versions of the same oscillator:
- one smoother and folded
- one raw/internal

This is a fantastic stereo or layered patch.

### Recommended modules
- **Make Noise Fold**
- **Intellijel Bifold**
- **Joranalogue Fold 6**
- **Serge-style wavefolder clones**

---

## 12. Use square out for logic-derived rhythms
The **SQR OUT** is useful not only as audio but as a modulation/gate source when tuned/LFO’d creatively.

### Patch
- send **SQR OUT** into:
  - logic modules
  - clock dividers
  - comparators
  - switch modules

Combine with the internal LFO square or external clock.

### Result
Rhythmic structures derived from pitch relationships. Great for techno, generative, and polyrhythmic patches.

### Companion modules
- **Doepfer logic**
- **Joranalogue Compare 2**
- **switches** like Doepfer A-151
- clock dividers / Boolean modules

---

## 13. LPG percussion voice from noise or samples
The LPG section can make excellent percussion even without using the oscillator.

### Patch
- noise / sample / click source -> **LPG IN**
- triggers -> **LPG CV IN** in **PING** mode
- optional: **LPG OUT** -> internal VCA or external distortion

### Result
Bongos, toms, claves, hi-hats, muted plucks, wooden knocks.

### Best source modules
- noise source
- sample player
- very short envelopes/clicks
- digital percussion modules

A great trick:
- send **pitched noise** or resonant filter noise into the LPG for hand-drum style sounds.

---

## 14. Animate the final VCA separately from the LPG
Because there is both an **LPG** and a separate **VCA**, you can get more nuanced articulation than on many compact voices.

### Patch
- external envelope -> **VCA CV IN**
- different external envelope or trigger source -> **LPG CV IN**
- use LPG for tone/body transient
- use VCA for macro amplitude contour

### Result
Very expressive plucks, bowed-like shapes, reverse-feeling swells, punch + tail behavior.

### Ideal modulation sources
- snappy envelope for LPG
- slower ADSR for VCA
- or vice versa

This is one of the most powerful upgrades you can give the module.

---

## 15. Run the oscillator into external spectral processors, then back
You can take one oscillator output externally, process it, and then return it to the module’s downstream sections.

### Example
- **S/B OUT** -> phaser / wavefolder / resonator / frequency shifter
- processed signal -> **LPG IN** or **VCA IN**

### Result
You keep the Synthesizer Box’s articulation path while radically changing the timbre source.

### Especially good processors
- resonators
- comb filters
- phasers
- analog distortion
- frequency shifters
- spectral processors

Examples:
- **Mutable Rings** as resonator
- **Doepfer A-126-2** frequency shifter
- **Erica Phaser**
- **triphonic/stereo filter**

---

## 16. Use glide with quantized sequencing for liquid acid lines
The built-in glide is hardwired between **1V/O IN** and oscillator, which makes it naturally playable.

### Patch
- quantized sequencer -> **1V/O IN**
- gate sequencer -> **ENV IN**
- set moderate resonance in lowpass mode or use LPG mode
- route accent-like envelope to **MOD CV IN** or **FM CV IN**

### Result
Acid-adjacent monosynth lines, but with more analog organic variation than a classic ladder synth.

### Great sequencer types
- step sequencer with slides
- generative quantizer
- probability sequencer

### Bonus
Use the **sub oscillator** for huge bassline weight.

---

## 17. Turn it into a drone laboratory
The module is also great without conventional note gates.

### Patch
- open the VCA partially
- set LPG to filter or LPG mode
- use slow modulation into:
  - **FM CV IN**
  - **MOD CV IN**
  - **LPG CV IN**
- optionally process outputs through delay/reverb

### Result
Dense analog drone beds with evolving harmonics.

### Great support modules
- slow CV sources
- chaotic modulators
- matrix mixer
- stereo effects

Specific ideas:
- **Batumi** for 4 related LFOs
- **Maths** for drifting envelopes
- **matrix mixer** for cross-patched modulation blends
- long stereo delay + shimmer reverb

---

## 18. Create self-playing feedback ecosystems
Because there are several outputs and several modulation inputs, the Synthesizer Box invites controlled feedback.

### Safe-ish feedback experiments
- **S/B OUT** -> external attenuator/VCA -> **BLADE IN**
- **LFO TRI OUT** externally attenuated/mixed with random -> **FM CV IN**
- **ENV OUT** -> external attenuator -> **MOD CV IN**
- **LPG OUT** -> distortion/filter -> external VCA -> back to **VCA IN** or **LPG IN**

### Result
Wild, semi-chaotic analog behaviors, especially with careful attenuation.

### Important
Use attenuators, attenuverters, or VCAs in feedback loops.

### Best helper modules
- **Happy Nerding 3xMIA**
- **Frap 321**
- **Intellijel Triplatt**
- **Quad VCA**

---

## 19. Pair it with a matrix mixer
If I were adding one “secret weapon” utility to maximize this module, it would be a **matrix mixer**.

### Why
You have multiple modulation targets:
- FM
- MOD CV
- LPG CV
- VCA CV externally if overridden
- BLADE IN externally

And multiple modulation sources:
- internal LFO
- envelope
- external random
- external envelopes
- external audio-rate oscillators

A matrix mixer lets you distribute and combine them in subtle amounts.

### Result
A small voice turns into a highly animated ecosystem.

### Great options
- **Doepfer A-138m**
- **AISynthesis matrix mixer**
- any compact CV matrix

---

## 20. Stereo expansion patch
The Synthesizer Box itself is mono, but it expands beautifully to stereo.

### Patch
- internal main voice -> left-side effect chain
- separate waveform output -> right-side effect chain
- modulate each side differently

Example:
- **MIX OUT** -> LPG/VCA -> chorus -> left
- **TRI OUT** -> wavefolder -> filter -> delay -> right

### Result
Huge stereo images from a single oscillator core.

### Good stereo helpers
- stereo delay
- stereo filter
- dual VCA
- panner / crossfader

---

# Best module types to pair with Synthesizer Box

If you want the most mileage, these are the highest-value additions:

## Essential companions
- **attenuator / attenuverter**
- **utility mixer**
- **extra VCA**
- **sequencer**
- **clock source**

## Modulation expansion
- **random voltage source**
- **function generator**
- **multi-LFO**
- **sample & hold**
- **envelope follower**

## Timbre expansion
- **wavefolder**
- **resonator**
- **stereo filter**
- **distortion / saturation**
- **frequency shifter**

## Performance expansion
- **joystick controller**
- **pressure controller**
- **touch controller**
- **manual gate / trigger source**

---

# Specific module pairings I’d recommend

## Make Noise Maths
Perfect with Synthesizer Box because it gives:
- extra envelopes
- slews
- modulation mixing
- cycling LFOs
- trigger manipulation

Use it for:
- shaped pings into LPG
- slewed random into BLADE IN
- envelope variations to FM or MOD CV

## Xaoc Batumi
A great modulation expander:
- quadrature motion
- synced LFOs
- multiple related shapes

Excellent for evolving FM, waveform morphing, and LPG animation.

## Mutable Instruments Marbles
Fantastic if you want the module to become a generative voice:
- pitch
- triggers
- random modulation
- musical unpredictability

## Intellijel Quad VCA
Super useful because the Synthesizer Box gets much deeper when modulation is attenuated and mixed carefully.

## Joranalogue Fold 6 / Intellijel Bifold
The triangle output begs for folding.

## Pamela’s New Workout
Great as a timing and modulation brain:
- clocks
- triggers
- synced LFOs
- random
- envelopes in a pinch

## Make Noise Mimeophon / XAOC Timiszoara / stereo delays and reverbs
The Synthesizer Box sounds great through time-based effects, especially plucks and drones.

---

# Patch recipes

## Recipe 1: Organic plucked bass
- Sequencer pitch -> **1V/O IN**
- Sequencer gate -> **ENV IN**
- Oscillator **MIX OUT** internal to LPG/VCA
- LPG mode = **LPG**
- Mod/Ping = **MOD**
- Envelope internal to LPG/VCA
- slow random -> **MOD CV IN**
- sub oscillator on

Add:
- mild saturation after **VCA OUT**

Result: woody, rubbery, animated bass.

---

## Recipe 2: Metallic dual-FM lead
- External sine oscillator -> **FM CV IN**
- Set FM switch to **linear**
- envelope or LFO -> **MOD CV IN**
- use **S/B OUT** into LPG
- reverb/delay after VCA

Result: bright, singing, metallic lead tones.

---

## Recipe 3: LPG drum lab
- noise source -> **LPG IN**
- trigger sequencer -> **LPG CV IN**
- LPG set to **PING**
- LPG mode = **LPG**
- **LPG OUT** -> VCA IN
- external envelope -> **VCA CV IN**

Result: shaped percussion with more control over tail length.

---

## Recipe 4: Split oscillator stereo
- **TRI OUT** -> wavefolder -> left channel
- **S/B OUT** -> filter -> right channel
- same pitch sequence to Synth Box
- independent modulation for each chain

Result: wide stereo voice with shared tuning but different spectral motion.

---

## Recipe 5: Self-playing ambient machine
- Random quantizer -> **1V/O IN**
- sparse gates -> **ENV IN**
- slow LFO -> **FM CV IN**
- random slew -> **MOD CV IN**
- another slow CV -> **LPG CV IN**
- VCA OUT -> delay -> reverb

Result: generative ambient lines with constantly shifting timbre.

---

# Things to watch out for

- The module gets much better with **attenuation**. A lot of the most musical patches will depend on reducing modulation depth.
- The **LPG ping** can be especially sensitive to trigger level and shape; try different trigger/gate sources.
- The **wide-range LFO** may enter audio-rate territory, which is great, but can quickly become intense in FM patches.
- Since several routings are internally normalled, if something behaves differently after patching, check whether you’ve overridden an internal source.

---

# Overall creative verdict

The Synthesizer Box is strongest when treated not just as a “small synth voice,” but as a **patch-programmable analog ecosystem**. Its best tricks come from:
- separating the normalled sections,
- using external modulation to replace the built-in routings,
- exploiting the **blade waveform** and **LPG pinging**,
- layering the multiple oscillator outputs in parallel,
- and adding utilities like **VCAs, attenuverters, mixers, and random sources**.

If you want, I can also provide:
1. **10 genre-specific patches** for the Synthesizer Box,  
2. a **small-system pairing guide** (e.g. best 3 modules to add), or  
3. a **signal-flow diagram** of its internal routings and how to override them.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)