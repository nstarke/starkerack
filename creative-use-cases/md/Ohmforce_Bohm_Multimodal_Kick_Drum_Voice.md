# Ohmforce — Bohm Multimodal Kick Drum Voice

- [Manual PDF](../../manuals/Bohm_Eurorack_Manual_Compiled.pdf)

---

[Manual PDF / Source](https://bohm-eurorack-manual.readthedocs.io/en/latest/index.html)

# Creative patch ideas for the Bohm Eurorack system

Bohm looks like much more than a simple kick module: it’s a **stereo dual-voice kick platform** with model-based synthesis, performance modes, optional **Groove** layering, and **Performer** stereo/DJ-style processing. That means you can treat it as:

- a kick drum voice
- a bass percussion synth
- a layered low-end system
- a stereo effects destination
- a live techno performance centerpiece

Because the manual suggests the controls behave differently per model, a lot of the fun will come from **modulating familiar parameters across different models** and using external modules to create structure, groove, and movement.

---

## What stands out from the manual

A few things suggest the best creative uses:

- **Multiple kick models** with different architectures  
  This means model selection and parameter sweeps can give you multiple drum-machine personalities in one patch.

- **Stereo dual-voice concept**
  Useful for layered kicks, call-and-response percussion, stereo movement, and low-end + texture splits.

- **Groove expander**
  Especially suited for **rumbles, layered percussion, and secondary impacts**.

- **Performer expander**
  Adds **ducking, DJ-style effects, and stereo processing**, which is huge for live transitions and making a kick patch feel like a finished record.

- **Studio / Live Song / Jam modes**
  This strongly suggests pairing Bohm with **sequencers, CV memories, switches, and performance controllers**.

- **Pitch curve behavior inspired by 808/909**
  This means Bohm likely responds very musically to **pitch CV, envelopes, accent, and transient shaping**.

---

# Best module pairings

## 1. Trigger sequencers and drum sequencers
Bohm will shine with a sequencer that can do more than simple quarter notes.

### Good pairings
- **ALM Pamela’s Pro Workout**
- **Xaoc Moskwa II**
- **Intellijel Steppy**
- **Winter Modular Eloquencer**
- **Five12 Vector Sequencer**
- **Noise Engineering Numeric Repetitor**
- **Verbos Multi-Stage / Voltage Multistage** for more experimental sequencing

### Why
Use them to create:
- standard 4-on-the-floor
- broken kicks
- fills
- probability-based ghost hits
- pattern-specific accent variations
- alternating main kick / Groove voice patterns

### Patch idea
Send a main trigger pattern to Bohm and a sparser or shuffled pattern to Groove.  
Then use a sequencer lane or probability trigger to create occasional layered hits for transitions.

---

## 2. Accent and velocity modulation
Since Bohm has **VELOCITY**, it’ll benefit enormously from dynamic triggering or CV modulation.

### Use with
- CV sequencers
- offset/attenuator modules
- random stepped voltage generators
- function generators
- MIDI-to-CV interfaces with velocity output

### Specific recommendations
- **Mutable Instruments Marbles**
- **Bastl CV Trinity**
- **Make Noise Maths**
- **Frap Tools Falistri**
- **After Later / Mutable Peaks-style modulation sources**
- **Hermod+** if working with MIDI velocity

### Patch idea: “Humanized warehouse kick”
- Trigger Bohm with a rigid 4/4 clock.
- Modulate VELOCITY slightly with a stepped random source, attenuated carefully.
- Send another very subtle modulation to ATTACK or COLOR.
- Result: a kick that keeps the pulse steady but feels alive in a long techno set.

---

## 3. Envelope generators for macro kick sculpting
Even if Bohm has internal shaping, external envelopes are perfect for animating model-dependent parameters.

### Great targets
- PITCH
- CURVE
- LENGTH
- COLOR
- FX
- TRS DECAY / TRS TONE

### Modules
- **Make Noise Maths**
- **Intellijel Quadrax**
- **Xaoc Zadar**
- **Cosmotronic Delta-V**
- **ALM Pip Slope**
- **Doepfer A-171-2**

### Patch idea: “Pseudo-sidechained pitch rip”
Use a fast-decay envelope into PITCH or CURVE on selected hits only.  
This can exaggerate the classic downward pitch sweep and create huge modern hard-techno transient impacts.

---

## 4. VCAs and CV processors
A lot of people underrate this with drum modules, but CV processing is where Bohm becomes a serious instrument.

### Useful module types
- attenuverters
- offsets
- VCAs for CV
- polarizers
- sequential switches
- logic modules

### Recommendations
- **Happy Nerding 3xMIA**
- **Frap Tools 321**
- **Befaco A*B+C**
- **Intellijel Triplatt**
- **Mutable Blinds / clones**
- **Doepfer A-172 / A-185 style utility support**

### Why
Different models likely react very differently to the same CV range. Utilities let you:
- narrow modulation sweet spots
- invert envelopes
- combine random + envelope motion
- create different response depths for different songs

### Patch idea
Mix a slow triangle LFO with a tiny random stepped source, then attenuate heavily into COLOR.  
You’ll get subtle model drift rather than obvious wobble.

---

## 5. Random and generative modulation
Because Bohm has many timbral parameters, random voltage can transform it from “kick module” to “evolving percussion system.”

### Modules
- **Mutable Marbles**
- **Make Noise Wogglebug**
- **SSF Ultra-Random Analog**
- **XAOC Devices Batumi** in stepped mode through sample-and-hold
- **Turing Machine + expanders**

### Patch idea: “Intelligent industrial kickline”
- Main kick on every quarter note.
- Random modulation to ATTACK and COLOR at low depth.
- Probability-based extra trigger to Groove.
- Send Groove through a long decay or external feedback path.
- Result: a controlled but unstable industrial techno low-end bed.

---

## 6. Sequential switches and scene switching
Since Bohm has multiple running modes and likely rewards parameter changes, external switching is a strong pairing.

### Modules
- **Doepfer A-151 Sequential Switch**
- **Tenderfoot quad switch types**
- **Shakmat Bard Quartet**
- **Vice Virga**
- **Noise Engineering Vice Virga**
- **WMD SSM / similar switch modules**

### Patch idea: “Four kick personalities”
Prepare four CV sources or offsets for PITCH/COLOR/FX and switch between them every 8 or 16 bars.  
This lets Bohm move through:
1. dry club kick
2. distorted hard kick
3. boomy rumble layer
4. washed transition kick

This is especially effective in **Live Song Mode**.

---

## 7. Distortion, saturation, and wavefolding
Bohm likely already covers a lot of internal kick colors, but external saturation is still one of the best pairings.

### Great module choices
- **Noise Engineering Ruina Versio**
- **Noise Engineering Terci Ruina**
- **Strymon Magneto input drive**
- **Bastl Dark Matter**
- **Instruō tanh[3]**
- **SSF Triptych**
- **100 Grit**
- **Metasonix / tube modules** if you like dangerous low-end chaos

### Patch ideas

#### A. Hard techno destroyer
Run Bohm into a distortion with parallel dry blend.  
Keep the sub intact and smash only the mids/high transient.

#### B. Folded click layer
High-pass a copy of Bohm, then wavefold it.  
Mix that back with the dry signal for a custom top-click that tracks your kick pattern.

#### C. Rumble exciter
Send Groove into saturation before reverb/delay to make the rumble denser and more harmonic.

---

## 8. Filters and EQ modules
A kick module through a filter sounds obvious, but there are some less obvious uses.

### Good module types
- multimode filters
- fixed filter banks
- stereo filters
- resonant low-pass gates
- parametric EQ / sculpting modules

### Recommendations
- **QPAS**
- **Bastl Ikarie**
- **Sara VCF**
- **Worng Parallax**
- **Doepfer Wasp / SEM filters**
- **ADDAC fixed filter banks**
- **Joranalogue Filter 8**

### Patch ideas

#### A. Split-band processing
Mult Bohm:
- one copy stays clean for sub
- one copy goes through a band-pass filter and distortion
Mix to taste.

This keeps low-end solid while adding a controllable attack band.

#### B. Resonant kick bassline
Patch PITCH CV melodically and run Bohm through a low-pass filter that opens only on selected hits.  
This can turn Bohm into a bass-percussion hybrid.

#### C. Stereo Performer widening
If using Performer, process its stereo output through a stereo filter with slow modulation for breakdowns and transitions.

---

## 9. Delays and reverbs for techno rumble
The manual explicitly points toward **Groove** as a rumble/layering tool. External effects can push this much further.

### Best effect pairings
- synced delay
- reverb with filtering
- feedback processors
- stereo diffusion
- clocked delay into saturation

### Specific modules
- **Make Noise Mimeophon**
- **Strymon Magneto**
- **Happy Nerding FX Aid XL**
- **Xaoc Timiszoara**
- **Intellijel Sealegs**
- **Erica Synths Black Hole DSP 2**
- **Desmodus Versio**
- **Nautilus**

### Patch ideas

#### A. Classic rumble loop
- Send Groove output to reverb.
- High-pass the reverb return.
- Compress or saturate it.
- Duck it against the main kick using Performer or an external envelope/VCA setup.

This gives you the classic rolling techno basement rumble.

#### B. Pinged sub tail
Use a very short delay with feedback and low-pass filtering on Groove only.  
This can create a tuned resonant tail behind the main kick.

#### C. Stereo transition wash
During fills or breakdowns, push Bohm or Groove into long stereo reverb, then snap back to dry for the drop.

---

## 10. Compressors, envelope followers, and sidechain tools
Since Performer already includes ducking, external dynamics modules can still open up more advanced routing.

### Useful modules
- **WMD MSCL**
- **Cosmotronic Messor**
- **Frap Tools CGM dynamics setups**
- **Mutable Ears / envelope follower types**
- **Detect-Rx**
- **Endorphin.es Cockpit / Ghost**
- **Shakmat Archer’s Rig / sidechain-capable mixers**

### Patch ideas

#### A. Self-ducking rumble bus
Use Bohm’s trigger or an envelope follower from Bohm audio to duck a reverb return or bass voice.

#### B. Kick drives the whole patch
Let Bohm control the sidechain on:
- drones
- pads
- acid lines
- sampled textures

This makes the kick the central rhythmic authority in the patch.

#### C. Dynamic transient emphasis
Compress a distorted parallel version of Bohm while keeping the dry transient uncompressed.

---

## 11. Mixers and parallel processing
Bohm is the kind of module that rewards **parallel chains**.

### Useful module types
- submixers
- stereo mixers
- sends/returns
- performance mixers
- crossfaders

### Recommendations
- **Happy Nerding PanMix**
- **Befaco Hexmix**
- **WMD Performance Mixer**
- **Cosmotronic Cosmix**
- **Toppobrillo Minimix**
- **Joranalogue Mix 3**
- **XOH / OUT-style stereo outputs**

### Patch structure
Try 3 parallel lanes:
1. **dry Bohm** for punch
2. **distorted lane** for aggression
3. **reverb/delay lane** for space

Blend live. This is especially powerful if Performer is present.

---

## 12. LFOs for long-form motion
Slow modulation can make a repetitive kick evolve over 5–10 minutes.

### Great pairings
- **Xaoc Batumi**
- **DivKid øchd**
- **Intellijel Quadrax cycling**
- **Joranalogue Orbit 3**
- **Pamela’s Pro Workout**

### Best parameter destinations
- COLOR
- FX
- ATTACK
- CURVE
- stereo processing parameters via Performer

### Patch idea: “Set-and-forget evolution”
Use very slow unsynced LFOs at tiny depth into 2–3 parameters.  
The kick subtly changes tone over the course of a track, keeping long loops interesting.

---

## 13. Quantizers and melodic pitch CV
The manual says PITCH roughly covers **C1 to C2**, which opens up more than just drum tuning.

### Modules
- **Intellijel Scales**
- **Ornament & Crime**
- **ADDAC quantizers**
- **Bard Quartet**
- **Mimetic Digitalis + quantizer**

### Patch idea: “Kick-bassline hybrid”
Sequence Bohm’s PITCH melodically over a 1-octave range while keeping trigger density sparse.  
You can create:
- tuned electro toms
- bass kicks
- industrial percussive basslines
- 808-style melodic booms

Pair with an acid line one octave up for huge groove lock.

---

## 14. Sample and hold / stepped modulation
This is ideal if you want repeatable-but-changing kick settings every bar or phrase.

### Good tools
- sample & hold
- clock divider
- stepped random
- addressable CV source

### Patch idea
Clock a sample-and-hold every 8 steps and route it to COLOR or FX.  
The kick timbre changes once per phrase, which feels musical rather than chaotic.

---

## 15. Logic and clock utilities
Kick layers become much more interesting when trigger relationships are derived logically.

### Module suggestions
- **Doepfer logic modules**
- **Joranalogue Compare 2**
- **ALM Pamela’s Pro Workout**
- **Mutable Kinks / logic utilities**
- **Klavis Logica XT**

### Patch ideas

#### A. Accent from coincidence
Generate a second trigger only when two rhythmic streams coincide, then use that to fire Groove or modulate VELOCITY.

#### B. Fill generator
Use a clock divider reset and logic combination to create end-of-bar fills that alter Bohm parameters for a single beat.

#### C. Triggered FX burst
Use logic-derived gates to open an external FX send only on special hits.

---

# Performance-focused setups

## Setup 1: Minimal techno core
**Modules**
- Bohm
- Pamela’s Pro Workout
- 3xMIA
- distortion
- stereo reverb
- mixer

**Patch**
- Pam triggers Bohm in 4/4
- Another Pam channel modulates VELOCITY subtly
- Slow random via Pam into COLOR/FX
- Distortion on a parallel send
- Reverb on Groove or selected fills

**Result**
A compact but club-ready techno kick ecosystem.

---

## Setup 2: Live performance drum centerpiece
**Modules**
- Bohm + Groove + Performer
- trigger sequencer
- CV recorder or scene controller
- stereo mixer
- external delay/reverb

**Patch**
- Main pattern to Bohm
- Syncopated layers to Groove
- Performer handles ducking and stereo transitions
- Use scene-based CV changes every 16 bars
- Push FX and stereo width in breakdowns

**Result**
A highly performable low-end section that can carry an entire live set.

---

## Setup 3: Experimental industrial percussion lab
**Modules**
- Bohm
- random source
- sequential switch
- wavefolder/distortion
- band-pass filter
- delay
- envelope follower

**Patch**
- Irregular trigger patterns to Bohm
- Random CV to ATTACK, CURVE, COLOR
- Switch between different modulation depths
- Distorted filtered parallel lane
- Delay feedback only on selected hits

**Result**
Bohm becomes a brutal percussion synth rather than just a kick.

---

# Less obvious uses

## Use Bohm as a bass voice
Because of the pitch range and envelope-like character of kick synths, Bohm may work well as:
- sub bass stabs
- plucky mono bass
- tuned low toms
- 808-style booming notes

Pair with:
- quantizer
- glide/portamento CV source
- VCA for external amplitude articulation if needed
- low-pass filter and saturation

---

## Use Groove as a dedicated send effect source
Instead of thinking of Groove as “second kick,” treat it as:
- the reverb-fed rumble voice
- the distorted mid-bass layer
- the ghost-hit percussion lane
- the breakdown swell lane

That frees the main Bohm voice to stay clean and mix-stable.

---

## Use Performer as a pseudo-master bus for your rhythm section
If Performer has ducking and stereo effects, feed related percussion or bass into a shared bus around it if your system allows that kind of routing.  
This can make Bohm the anchor of a more cohesive live mix.

---

# Practical modulation targets to try first

If you’re just starting with Bohm, I’d prioritize these pairings:

### Most musically useful CV targets
1. **VELOCITY** — immediate groove improvement  
2. **PITCH** — tuned kicks, fills, bass-kick hybrids  
3. **COLOR** — tonal movement without losing timing  
4. **ATTACK** — helps define placement in the mix  
5. **CURVE** — major impact on classic drum-machine feel  
6. **FX / TRS DECAY** — excellent for transitions and rumble work  

### Best modulation sources
1. stepped random
2. short envelope
3. slow LFO
4. sequenced CV lane
5. logic-derived trigger converted to CV
6. manual performance controller

---

# My top recommended companion modules

If I were building around Bohm, I’d especially consider:

## Compact utility-oriented system
- **Pamela’s Pro Workout**
- **Happy Nerding 3xMIA**
- **Make Noise Maths**
- **FX Aid XL**
- **Ruina Versio**
- **small stereo mixer/output**

## Performance techno system
- **Vector Sequencer** or **Eloquencer**
- **Bohm + Groove + Performer**
- **Messor** or **MSCL**
- **Mimeophon** or **Sealegs**
- **performance mixer**
- **filter or saturator for parallel bus**

## Experimental sound design system
- **Marbles**
- **Falistri or Maths**
- **Vice Virga**
- **Filter 8**
- **Triptych / Ruina**
- **Desmodus Versio / Timiszoara**

---

# Final creative advice

The biggest creative opportunity with Bohm is to avoid treating it as “just the kick.” Instead, think of it as a **low-frequency performance voice system**.

The winning strategies are:

- keep one layer **clean and reliable**
- make another layer **dirty, spatial, or unstable**
- modulate **small amounts** for long-form movement
- use **parallel processing** rather than destroying the main signal
- exploit **sequenced CV and scene changes** to make one kick engine behave like an entire rhythm section

If you want, I can also turn this into:
1. a **genre-specific patch guide** for techno / electro / industrial / ambient, or  
2. a **shopping list of the best companion modules by budget**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)