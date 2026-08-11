# Erogenous Tones — Radar

- [Manual PDF](../../manuals/radar-instructions.pdf)

---

[Manual PDF](http://erogenous-tones.com)

# Erogenous Tones RADAR — Creative Patch Ideas and Pairings

RADAR is much more than “8 envelopes.” From the manual, the key creative strengths are:

- **8 independent AD/AR/repeating lanes**
- **Normalized trigger chaining**
- **Digital vs analog-modeled behavior**
- **Per-pair shape/model control**
- **Composite max outputs on lanes 4 and 8**
- **Phase-related QUAD and OCT modes**
- **Resettable repeating envelopes up into audio/LFO ranges**

That means RADAR can act as:

- an **envelope bank**
- an **octal function generator**
- a **complex modulation animator**
- a **phase-locked LFO source**
- a **pseudo-oscillator / audio modulator**
- a **rhythmic burst / motion sequencer**

Below are practical and musical ways to exploit that with other modules.

---

## 1. Use RADAR as an 8-lane modulation conductor

### Great pairings
- **Quad VCA / matrix mixer / CV mixer**
- **Filter bank or multiple filters**
- **Multi-voice oscillator setup**
- **Sequential switch**

### Patch concept
Use each lane as a dedicated modulation source for different parameters in a patch:
- Lane 1: filter cutoff
- Lane 2: wavefolder amount
- Lane 3: VCA amplitude
- Lane 4: FM index
- Lane 5: delay feedback
- Lane 6: reverb size
- Lane 7: panning CV
- Lane 8: pitch micro-modulation or second filter

Because RADAR can run **AD**, **AR**, or **Repeating** per lane, you can mix one-shot modulation and cyclic motion in the same patch.

### Why it’s powerful
You can create a patch where all motion feels related, especially if the triggers are normalized or derived from one rhythm source.

### Recommended modules
- **Intellijel Quad VCA**
- **Happy Nerding 3xVCA**
- **ALM Tangle Quartet**
- **Doepfer A-138m matrix mixer**
- Any **attenuverter bank**

---

## 2. Build complex percussion from one trigger stream

The manual notes that each channel trigger is **normalized to the next channel below it**, which is excellent for distributing one master pulse across multiple lanes.

### Great pairings
- Drum voices
- Noise source
- LPGs
- VCAs
- Resonant filters
- Sample players

### Patch concept
Send one trigger pattern into the top lane and let it cascade. Set each lane to different attack/release times and shapes:
- Very short lanes for clicks and hats
- Mid-length lanes for snares/toms
- Longer lanes for swells/noise bursts

Then use the lanes to animate:
- VCAs for amplitude envelopes
- Filter pings
- Noise bursts
- FM depth on drum oscillators

### Try this
Use **analog modeled AR mode** for more natural and variable drum articulation. Very short gates won’t always hit full amplitude, which gives dynamic, “played” feel.

### Recommended pairings
- **Noise Engineering Basimilus Iteritas Alter**
- **Mutable Peaks / drum modules**
- **SSF Entity series**
- **Low pass gates** like Optomix-style modules
- **Noise source + filter + VCA** for patch-programmed drums

---

## 3. Use analog vs digital mode as a musical character switch

One of RADAR’s coolest features is the distinction between:

- **Digital mode**: hard reset to zero, more abrupt, clock-like, precise
- **Analog modeled mode**: charging/discharging style, smoother, continuation from current level

### Creative use
Patch the same destination with two similar envelopes:
- one lane in digital mode
- one lane in analog mode

Use them on:
- two VCAs for layered voices
- two filter FM inputs
- two sides of a stereo patch

### Result
The digital lane sounds more rigid and percussive; the analog lane feels more elastic and organic.

### Best with
- Oscillators that respond well to subtle FM
- Filters with characterful resonance
- LPGs
- Stereo processors

---

## 4. Exploit AR behavior with variable gate lengths

In analog modeled AR mode, short gates produce incomplete attacks and release from whatever level they reached. This is incredibly expressive.

### Great pairings
- Gate length modulators
- Trigger/gate sequencers with ratcheting
- Bernoulli gate / probability modules
- Keyboard or touch controller

### Patch concept
Feed RADAR from a gate sequencer that varies gate length per step. Then use the envelope for:
- VCA amplitude
- Filter opening
- Wavefolder intensity

### Why it works
The same attack/release settings produce very different shapes depending on gate length, almost like velocity and articulation combined.

### Recommended modules
- **Pamela’s New/Pro Workout** for variable pulse width/gates
- **Intellijel Steppy**
- **Make Noise Tempi**
- **Acid Rain Maestro**
- Any sequencer with adjustable gate length

---

## 5. Composite “max” outputs as envelope combiners

The manual mentions that **lane 4** can output the max of lanes **3+4**, and **lane 8** can output the max of lanes **6+7+8**.

This is a very special function. It behaves like a dynamic “highest envelope wins” combiner rather than a sum.

### Musical uses

#### A. Peak-preserving macro envelope
Make multiple lanes with different timings and trigger patterns, then take the max output to a filter or VCA.  
This creates one evolving contour that always follows the strongest motion without clipping like summed envelopes can.

#### B. Accent extraction
Use several envelopes with different trigger rhythms. The max output naturally emphasizes whichever envelope is currently most active. Great for:
- accent CV
- FM bursts
- reverb send animation

#### C. Dynamic sidechain contour
Patch several percussive trigger-derived lanes, then take the max output as a sidechain CV to duck a drone or pad.

### Pairings
- Compressor-like patching through a VCA
- Filters
- FX send VCAs
- Morphing modules

---

## 6. Patch RADAR as a complex LFO network

In **Repeating mode**, RADAR becomes an LFO bank. The manual also notes that triggers can **reset** the waveform.

### Great pairings
- Clock dividers/multipliers
- Sequential switches
- Stereo effects
- Morphing oscillators
- CV recorders

### Patch concept
Set different lanes to Repeating mode with different shapes and times. Use reset triggers from your clock to keep them musically aligned.

Modulate:
- oscillator PWM
- filter cutoff
- effect parameters
- panning
- wavefolder symmetry
- granular density/position

### Advanced trick
Use **analog mode repeating** for more fluid, “voltage memory” style behavior, and **digital mode** for hard-synced repeating motions.

### Great with
- **Mimeophon / delay modules**
- **Morphagene / granular**
- **stereo VCAs / panners**
- **Rossum filters**
- **XAOC Timiszoara / effects**

---

## 7. Audio-rate modulation and pseudo-oscillator duties

The manual states RADAR can reach into the hundreds of Hz and around **1.18 kHz** in analog mode depending on shape. That means it can be used as an audio-rate modulation source or even a crude oscillator.

### Great pairings
- Filters
- FM-capable oscillators
- Ring mod / four quadrant VCA
- Wavefolder
- Comparator

### Patch ideas

#### A. Audio-rate filter FM
Patch a repeating lane into a filter’s FM input.  
Try several shapes:
- LOG
- LIN
- EXP

The shape changes will dramatically alter timbre.

#### B. AM voice
Take a VCO into a VCA, and use RADAR in repeating mode at audio rate as the VCA CV.  
This creates tremolo up into clangorous AM.

#### C. Crude voice through wavefolder
Patch a repeating lane as an audio source into a wavefolder or resonant filter. Then use another lane as its modulation source.

#### D. Comparator-derived pulse voice
Feed RADAR’s audio-rate output into a comparator or logic module to derive pulse/square-like audio from its shape.

### Recommended modules
- **Joranalogue Compare 2**
- **Bastl Tromsø comparator path**
- **wavefolder** like Fold 6, Bifold, or Serge-style folder
- **linear FM-capable oscillator**
- **VCF with FM input**

---

## 8. QUAD mode for rotating modulation fields

In **QUAD mode**, four lanes are **90 degrees apart**. This is perfect for cyclical, spatial, and morphing modulation.

### Excellent pairings
- Quad panner
- Four VCAs
- Four filters
- Four-voice chord patch
- Vector mixer

### Patch ideas

#### A. Rotating quadraphonic / stereo animation
Send the four outputs to four VCAs controlling four sound sources, or to a quad panner.  
This creates circular movement.

#### B. Phase-offset filter bank
Patch each quad lane to a different filter cutoff.  
With four similar voices, this creates a constantly shifting spectral animation.

#### C. Chord voice animation
Use the four lanes to independently animate:
- amplitude of each chord note
- FM depth
- wavefold amount
- timbre

Because they’re phase-related, the chord “breathes” as one organism.

### Additional QUAD CV features
The manual mentions **SPEED**, **GRAVITY**, and **SDELTA** on the extra lanes. These are especially good targets for slow modulation from:
- random sources
- offset LFOs
- joystick
- macro controller

### Recommended modules
- **Intellijel Planar 2**
- **Xaoc Praga / Hrad style mixers**
- **Happy Nerding PanMix**
- **Frap Tools QSC / VCAs**
- Any **quad VCA/panner**

---

## 9. OCT mode for 8-phase ecosystems

In **OCT mode**, all 8 lanes are **45 degrees apart**. This is where RADAR becomes a true modulation engine.

### Great pairings
- 8-step sequential switches
- 8-voice drum/sample systems
- Filter banks
- Additive synthesis setups
- Trigger-to-CV utilities

### Patch ideas

#### A. Additive animation
Use the 8 lanes to control 8 VCAs for 8 harmonics or 8 oscillators.  
This produces complex moving spectra with phase coherence.

#### B. Scanner patch
Use OCT outputs to sweep through:
- 8 channels on a sequential switch
- 8 VCAs holding different CVs or audio sources

This creates a scanning or circulating effect.

#### C. Multi-tap rhythmic modulation
Patch all 8 lanes to different destinations in one voice:
- pitch
- timbre
- FM
- wavefold
- filter
- resonance
- amplitude
- effects send

You get one “super-LFO” broken into phase slices.

### Best partners
- **Doepfer A-151 / A-152**
- **Joranalogue Step 8**
- **Verbos Scan & Pan**
- **Frap Tools CGM / grouped VCAs**
- **Befaco muxlicer-style switching**

---

## 10. Use shape CV for animated asymmetry

The manual notes that shape can sweep between **LOG, LIN, and EXP**, and CV offsets the knob setting.

This is huge: shape modulation on an envelope often sounds more interesting than simple time modulation.

### Try modulating shape with:
- Slow random
- S&H
- Another RADAR lane
- A joystick
- Velocity / aftertouch
- A sequencer row

### Great destinations
If RADAR is controlling:
- a VCA: shape CV changes groove/accent feel
- a filter: shape CV changes attack “gesture”
- repeating mode: shape CV changes waveform character

### Patch idea
Put one lane in repeating mode and patch another slow lane into its shape CV. Then use the output to modulate a filter or wavetable oscillator.  
This gives continuously morphing LFO geometry.

---

## 11. Cross-patch RADAR into itself

RADAR becomes much deeper when some lanes modulate the CV inputs or gate logic of other lanes.

### Self-patch ideas

#### A. Envelope modulates another lane’s shape
Lane 1 triggers lane 2; lane 1 output also modulates lane 2 shape CV.

#### B. Repeating lane modulates envelope shape
Use a slow repeating lane to animate another lane’s attack/decay curve over time.

#### C. Composite lane controls a group
Use lane 8 max output to control a global VCA or filter while lanes 5–7 modulate details.

### Result
Meta-envelopes: envelopes whose own contour behavior evolves in time.

---

## 12. Pair with random sources for organic life

RADAR loves random because it can turn unstable control information into shaped gestures.

### Good random sources
- Stepped random
- Smooth random
- Probability gates
- Burst generators
- Chaos modules

### Patch concepts

#### A. Random trigger ecology
Use a Bernoulli/probability trigger source into normalized trigger chain. Different lanes respond with different timings.

#### B. Random shape animation
Send stepped random through an attenuator into shape CV.

#### C. Randomized QUAD/OCT warp
In phase modes, random CV into SPEED, GRAVITY, or SDELTA gives evolving but still internally related movement.

### Recommended modules
- **Mutable Marbles**
- **SSF Ultra-Random**
- **Wogglebug**
- **Pam’s random outputs**
- **Turing machine type modules**

---

## 13. Use RADAR with sequential switches for evolving phrases

Because RADAR can provide many related envelopes/LFOs, a switch can turn them into a structured performance tool.

### Patch ideas

#### A. Switched envelope selection
Route several RADAR outputs into a sequential switch, then send the switched output to a VCA or filter.  
Each note or bar gets a different envelope contour.

#### B. Rotating modulation destination
Take one RADAR lane and use a switch to send it to different parameters over time.

#### C. Trigger-addressed phrases
Use different lanes as “stages” of a modulation phrase, selected by clocked switching.

### Great pairings
- **Doepfer A-151**
- **Boss Bow Two**
- **Vice Virga**
- Any manual/addressable switch

---

## 14. Build pseudo-sidechain and ducking systems

RADAR’s fast envelopes and max combiners make it good for sidechain-style control.

### Patch concept
- Feed kick/snare triggers into separate lanes
- Give kick a longer release, snare a shorter one
- Take a composite/max output
- Invert or attenuate it
- Send to a VCA controlling a pad/drone/bass

### Why RADAR excels here
You can build nuanced ducking curves from multiple rhythmic sources without needing a compressor.

### Great pairings
- Offset/inverter
- VCA
- Utility mixer
- Drone voice or stereo bus

---

## 15. Use it as a performance macro module

RADAR can define the “gesture grammar” of a patch. A good strategy is to dedicate it to controlling most time-based movement while another module handles notes/rhythm.

### Pair with
- A sequencer
- A touch controller
- Macro controllers
- Preset manager

### Performance setup
- Lanes 1–4: note articulation across voices
- Lanes 5–8: effects and timbral movement
- QUAD/OCT mode for global motion scenes
- Manual trigger/reset input for fills and transitions

### Great modules
- **Pressure Points / 0-CTRL / touch controllers**
- **Tetrapad / Planar 2**
- **Preset manager** like Morph 4 + scenes, or external MIDI-CV macro control

---

## 16. Particularly strong module combinations

Here are some especially good companion categories and why:

### 1. VCAs
RADAR really comes alive when every lane can animate something.
- Essential for amplitude, modulation depth, and routing

### 2. Attenuverters / offsets
The manual specifically warns that shape CV is offset-based and benefits from attenuation.
- Very important for controlled results

### 3. Trigger sequencers / clock tools
Variable gate length and resets make RADAR much more expressive.

### 4. Random/probability modules
Turns static envelopes into living structures.

### 5. Switches and matrix mixers
Help exploit the fact that RADAR gives you many simultaneous related voltages.

### 6. Stereo and spatial processors
QUAD/OCT phase relationships are fantastic for movement in space.

### 7. Wavefolders and FM-capable voices
Repeating mode into audio range is a hidden superpower.

---

## 17. A few full patch recipes

## Patch Recipe 1: “Breathing Drone Organism”
**Modules**
- 2–4 oscillators
- Mixer
- Filter
- Reverb/delay
- VCAs
- RADAR

**Patch**
- OCT mode
- Use 8 phase-offset outputs
- 4 lanes modulate oscillator amplitudes
- 2 lanes modulate filter cutoff/resonance
- 1 lane modulates delay feedback
- 1 lane modulates reverb send
- Slowly modulate SPEED or SHAPE

**Result**
A cohesive drone patch with internal circulation and slow evolution.

---

## Patch Recipe 2: “Self-playing Percussion Lab”
**Modules**
- Noise source
- 1–2 drum voices
- LPG
- Filter
- Random trigger source
- VCAs
- RADAR

**Patch**
- Envelope mode
- Random triggers into lane 1, normalized downward
- Different lanes set to AD/AR/repeating
- Use short envelopes for clicks, medium for noise snares, long for tom-like sweeps
- Take lane 8 max output to modulate global accent/filter sweep

**Result**
One trigger ecosystem producing many percussion articulations.

---

## Patch Recipe 3: “Rotating Stereo Machine”
**Modules**
- Stereo mixer or panner
- 2–4 voices
- Delay/reverb
- RADAR

**Patch**
- QUAD mode
- Patch four outputs to four VCAs or panning CVs
- Feed related audio into those channels
- Modulate GRAVITY slowly
- Reset periodically from clock

**Result**
A rotating, pulsing stereo/quad field that stays rhythmically coherent.

---

## Patch Recipe 4: “Envelope-as-Oscillator”
**Modules**
- Wavefolder
- VCF
- VCA
- Another modulation source
- RADAR

**Patch**
- Repeating mode at highest speeds
- Send lane output into wavefolder or filter audio input
- Modulate shape CV with another RADAR lane
- Use another lane as amplitude contour via VCA

**Result**
A strange synthetic voice somewhere between LFO, oscillator, and function generator.

---

## 18. Best mindset for using RADAR

The most creative way to think about RADAR is:

- not as “8 separate envelopes”
- but as **a voltage choreography system**

It excels when you make multiple parameters move together, but not identically. The **phase modes**, **analog vs digital behavior**, **shape control**, and **max outputs** are what push it beyond a typical envelope generator.

If you want, I can also give you:

1. a **“best companion modules for RADAR by budget” list**,  
2. a **set of 20 fast patch ideas**, or  
3. a **genre-specific RADAR guide** for ambient, techno, drone, or generative patching.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)