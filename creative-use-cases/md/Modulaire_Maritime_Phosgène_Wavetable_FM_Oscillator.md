# Modulaire Maritime — Phosgène Wavetable FM Oscillator

- [Manual PDF](../../manuals/Phosgène _ Modulaire Maritime.pdf)

---

[Manual PDF / source page](https://www.modulaire-maritime.com/phosgène)

# Modulaire Maritime Phosgène — patch ideas and creative uses

Phosgène looks like a **2hp digital wavetable/FM oscillator** with a pretty unusual character:

- **60 wavetables** in **2 banks of 30**
- **Two parallel sound paths / outputs**:
  - **Waveshaping / folded wavetable output**
  - **FM output**
- **Shared controls** influence both paths differently
- **External CV** can push wave/folding/FM behavior further
- **100 Hz FM base** for a darker, tighter, less splashy FM spectrum
- **Tracks 1V/oct across 8 octaves**
- **Octave up/down switch**
- **Octave displace function** for shifting wavetable range lower while leaving FM range intact
- **11-bit-ish lower-resolution digital tone**, with aliasing/noise as part of the flavor
- **Saves last settings** after power cycle

This tells me Phosgène is not just a “small oscillator,” but really a **compact digital character source** that can cover:
- basses
- metallic tones
- dirty leads
- industrial percussion
- dual-layered timbres from its separate outputs
- CV-reactive digital textures

Below are the most interesting ways I’d use it in a Eurorack system.

---

## 1. Treat it as a **dual personality oscillator**
Because it offers separate wavetable/folded and FM outputs, the first creative move is to **never think of it as one voice**.

### Patch idea
- Send the **wavetable output** to a **low-pass filter**
- Send the **FM output** to a **wavefolder, LPG, or band-pass filter**
- Pan them left/right in a stereo mixer
- Modulate wave selection and FM depth with two related but different modulation sources

### Why it works
You get one coherent pitch source but two very different timbral interpretations:
- one side can be the “body”
- the other side can be the “grit,” “air,” or “machine noise”

### Great companions
- **Stereo mixer / panner**: Happy Nerding PanMix, Worng SoundStage, Befaco STMix
- **Dual filter**: Bastl Ikarie, Make Noise QPAS, Frap Fumana if you want spectral madness
- **LPG / dynamics**: Make Noise Optomix, Takaab LPG, Doepfer A-101-2

---

## 2. Build a **bass voice that stays dark and solid**
The manual specifically mentions the FM implementation is based around **100 Hz**, making it ideal for **tight FM basses** and **deep modulation**. That suggests Phosgène can do bass without the brittle upper-mid splash many digital FM voices get.

### Patch idea
- Sequence 1V/oct into Phosgène
- Use the **FM output** as your main oscillator
- Send it into a **clean VCA**
- Add a **snappy envelope** to amplitude
- Use a **slow envelope or offset CV** to animate wave/folding controls subtly
- Layer the **wavetable output** one octave lower or with octave displacement engaged

### Why it works
The FM side gives punch and harmonic focus, while the lower-displaced wavetable side can add weight.

### Great companions
- **Envelope**: Intellijel Dual ADSR, Zadar, Quadrax
- **VCA**: Veils, Tallin, Quad VCA
- **Bass-friendly filter**: AJH MiniMod VCF, Doepfer SEM, Joranalogue Filter 8
- **Saturation**: Instruō tanh[3], Ritual Guillotine, Endorphin.es Golden Master for final polish

---

## 3. Use the **octave displace** feature as a sound-design tool, not just pitch management
This is one of the coolest features described. It seems meant to keep the wavetable engine in a lower, more usable range while preserving full FM range.

### Creative use
Instead of thinking “this just prevents harshness,” use it to create **split-register timbres**:
- wavetable output stays low, thick, and dirty
- FM output remains high, articulate, and bright
- both are tracking the same melody

### Patch idea
- Mult your pitch CV to Phosgène and another oscillator
- Use Phosgène’s **wavetable output** with octave displace on as a sub/undertone
- Use another analog VCO or the **FM output** for the top layer
- Mix to taste

### Great companions
- **Analog VCO pairing**: Dixie II+, STO, Ts-L, A-110-1
- **Subharmonic enhancers**: Joranalogue Fold 6, analog saturation, resonant filter ping layer

This creates a “one module does low digital filth, another does stable top-end” hybrid voice.

---

## 4. Exploit the **11-bit / aliasing / noisy wavetable character**
The manual explicitly celebrates the “digital trash.” That means you should lean into it rather than trying to sterilize it.

### Patch idea: “broken sampler” lead
- Use the wavetable output
- Add moderate wave/fold CV from a stepped random source
- Send into a **high-pass filter**
- Add **short digital delay** or **clocked delay**
- Reverb after that

### Result
You get a lead that feels like:
- degraded ROMpler
- busted game-console synth
- early sampler wavetable edge

### Great companions
- **Stepped random / S&H**: Mutable Kinks, Wogglebug, Doepfer A-148, SSF Ultra-Random Analog
- **Clocked delay**: Mimeophon, Chronoblob 2, Erica Pico DSP
- **Bit/phase/digital FX**: Data Bender, FX Aid, Timiszoara, MFX

---

## 5. Turn it into an **industrial percussion source**
Phosgène’s harsh digital partials, noise-containing tables, and FM path make it ideal for non-traditional drum synthesis.

### Patch idea: kick/metal hybrid
- Sequence very short pitches or trigger envelopes into pitch modulation
- Use the **FM output** for the body
- Use the **wavetable output** through a VCA for the attack/noise layer
- Envelope the noise layer with an extremely short decay
- Add distortion and compression

### Patch idea: hi-hats / clanks
- Tune Phosgène high
- Modulate wave selection with random voltages
- Gate with a short decay envelope
- Run through band-pass filtering or LPG
- Optional: ring mod with another oscillator or noise source

### Great companions
- **Percussion envelopes**: Quadrax, Pingable Envelope Generator, Delta-V
- **Distortion**: Noise Engineering Ruina series, Bastl Dark Matter, Ritual Miasma
- **Compressor**: WMD MSCL, Cosmotronic Messor, Endorphin.es Cockpit 2 sidechain tricks

---

## 6. Pair it with a **resonator or physical modeling module**
The slightly crude digital tone can become very alive when used as an exciter rather than the final voice.

### Patch idea
- Send one of Phosgène’s outputs into:
  - a resonator
  - Karplus-Strong input path
  - modal filter bank
- Use bursts or short envelopes instead of sustained notes
- Modulate wave selection every few triggers

### Great companions
- **Resonator / physical modeling**: Mutable Rings, 2hp Pluck, Tubbutec/4ms resonant options, Schlappi Three Body used resonantly
- **Karplus tools**: delay line with short feedback, Mimeophon zones, Chronoblob, Sarajewo
- **Exciter helpers**: LPGs, burst generators, trigger sequencers

### Why it works
Phosgène’s edgy harmonics and aliasing give resonators a more complex excitation signal than a simple sine or noise burst.

---

## 7. Use it as a **modulator**, not only an audio oscillator
Because it tracks well and has controllable digital shape changes, Phosgène can be a fantastic **audio-rate modulation source** for other modules.

### Patch idea
- Use the **FM output** to frequency-modulate another oscillator
- Use the **wavetable output** to phase-modulate a digital oscillator or filter cutoff FM
- Sequence both oscillators harmonically

### Excellent targets
- Through-zero FM oscillators
- Filters with good FM response
- Delay time CV
- Wavefolders
- PLL modules

### Great companions
- **Oscillators for cross-mod**: Generate 3, Furthrrrr Generator, Cs-L, Brenso, Neoni
- **Filters that like audio-rate FM**: Filter 8, Belgrad, Ikarie, Three Sisters
- **PLL / logic weirdness**: Doepfer A-196, Joranalogue Compare 2, logic modules

### Result
Phosgène can inject “digital chewiness” into otherwise smooth analog modules.

---

## 8. Crossfade the two outputs for **morphing articulation**
Since there are two sonic interpretations available, voltage-controlled crossfading is an obvious and very musical move.

### Patch idea
- Send both outputs into a **VC crossfader**
- Use:
  - an envelope for plucked transitions
  - an LFO for evolving drones
  - velocity or aftertouch from your controller for expressive morphing

### Great companions
- **VC crossfader**: Doepfer A-134-2, Happy Nerding Xfade, Joranalogue Morph 4
- **Performance control**: Tetrapad/Tête, Pressure Points, Planar 2, 0-CTRL

### Why it works
You can perform between:
- stable-ish wavetable tone
- rougher FM articulation
- or vice versa depending on the patch

It gives the voice a macro “gesture” control.

---

## 9. Make it the center of a **small 2hp/compact skiff voice**
Since it’s only 2hp, it begs to be part of a very tiny but high-impact voice chain.

### Minimal voice recipe
- **Phosgène**
- **Envelope/LFO**
- **VCA**
- **Filter or LPG**
- **Multi-FX**
- **Compact sequencer**

### Suggested compact ecosystem
- 2hp EG / VCA / MMF / Verb / Delay
- ALM Pip Slope / Pip Filter / MFX
- Happy Nerding 3xVCA + FX Aid
- Xaoc Sewastopol or Tallin for extra gain and drive

### Result
A tiny skiff with one tiny oscillator can still make:
- dark techno basslines
- acid-adjacent sequences
- industrial bleeps
- cinematic drones

---

## 10. Use slow CV on **wave selection** for quasi-granular movement
Even without true wavetable interpolation details in the text, stepped or slewed modulation through wave indices can create a pseudo-scan effect.

### Patch idea
- Feed a **very slow random voltage** into wave select
- Use a **slew limiter** if needed
- Keep pitch static or drone-based
- Process through reverb and stereo delay

### Great companions
- **Random / chaos**: Triple Sloths, Marbles, Wogglebug, Orbit 3
- **Slew**: Doepfer A-170, Joranalogue Contour 1, Maths
- **Spatial FX**: Mimeophon, Nautilus, Desmodus Versio, Beads

### Result
A living digital drone that moves between “machine hum,” “radio ghosts,” and “corroded glass harmonics.”

---

## 11. Patch it into a **wavefolder anyway**
Even though it already contains waveshaping/folding behavior, external folding on digital waveforms often produces a very different result than internal shaping.

### Patch idea
- Use the wavetable output into an analog wavefolder
- Modulate folder symmetry/fold amount with envelopes and audio-rate LFOs
- Compare with the FM output processed separately

### Great companions
- **Wavefolders**: Intellijel Bifold, Joranalogue Fold 6, Serge-style folder, Bastl Timber
- **Mod source**: another oscillator, cycling envelope, random burst

### Why it works
Digital source + analog nonlinear processing = excellent contrast.  
Phosgène supplies stepped/aliased complexity; the external folder adds continuous analog instability.

---

## 12. Build a **drone voice with parallel signal processing**
This module seems especially strong when split into multiple processing lanes.

### Patch idea
- Wavetable output → low-pass gate → spring reverb
- FM output → resonant band-pass filter → distortion → delay
- Mix both at different levels
- Modulate wave and FM depth with unrelated slow CVs

### Great companions
- **Spring / character reverb**: Doepfer A-199, Knas Ekdahl Moisturizer (if external), FX Aid spring emulations
- **Band-pass filter**: Three Sisters, Ikarie, QPAS
- **Slow modulators**: Batumi, Ochd, Just Friends, Maestro

### Result
Huge dark drones with an “engine room / submarine / abandoned factory” character.

---

## 13. Pair it with **sequenced CV offsets and precision utilities**
Because the manual emphasizes octave range management and careful timbral positioning, precision utilities will be especially rewarding.

### Patch idea
- Use a **precision adder** for octave jumps
- Use a **CV offset/attenuator** to place the wave/FM sweet spot exactly
- Trigger switches to jump between banks or octave settings in performance

### Great companions
- **Precision / utility**: Ornament & Crime, Doepfer A-185-2, Frap 321, Happy Nerding 3xMIA
- **Sequential switching**: Doepfer A-151, Vice Virga, Switch 4

### Why it matters
Digital oscillators with lots of sweet spots benefit massively from:
- attenuating modulation
- offsetting it into “musical” zones
- recalling repeatable intervals

---

## 14. Clocked sample-and-hold on timbre controls for **machine speech / robotic melody**
Digital wavetable modules often sound amazing when timbre changes are rhythmically quantized.

### Patch idea
- Send a synced clock to sample-and-hold
- Feed S&H with noise, random, or another slow oscillator
- Patch that into wave selection or modulation depth
- Sequence pitch normally

### Great companions
- **S&H**: A-148, Kinks, Select 2, Sapèl
- **Clock source**: Pam’s Pro Workout, Tempi, Workout-style modules
- **Quantizer for melodic certainty**: Scales, O_C, Bard Quartet

### Result
Every note can have a different “phoneme,” producing robotic lines that feel speech-like.

---

## 15. Process it through **formant or spectral modules**
Phosgène’s bright, irregular harmonics are ideal fodder for spectral animation.

### Patch idea
- Wavetable output into a **formant filter** or **fixed filter bank**
- FM output direct or through VCA
- Animate filter bands with envelopes or LFOs
- Tune oscillator low and let filtering define the apparent motion

### Great companions
- **Filter banks / spectral**: Bark Filter, Fumana, fixed filter banks, Serge Resonant EQ
- **Formant processing**: Rossum Morpheus, Xaoc Koszalin for weird enhancement, spectral EQ modules

### Result
Industrial choir, radio voices, dystopian pads.

---

## 16. Use it as a **dirty clockable texture source** for granular or looper modules
Instead of “playing” it conventionally, record snippets and repitch/process them elsewhere.

### Patch idea
- Run Phosgène through changing CV states
- Sample short phrases into:
  - granular processor
  - looping delay
  - sampler
- Then repitch, reverse, freeze, and resequence

### Great companions
- **Granular / buffer**: Arbhar, Beads, Morphagene, Nebulae
- **Sampler**: Assimil8or, Bitbox, Radio Music-style playback tools
- **Looper**: Lubadh, Magneto, Morphagene

### Why it works
Its tone is already rich and unstable, so even tiny captured fragments remain interesting after transformation.

---

## 17. Pair it with **comparators, logic, and envelope followers** for control extraction
A digital oscillator with sharp transitions can be useful as a source of control logic too.

### Patch idea
- Send an audio output into a **comparator**
- Derive gates based on waveform crossings
- Use those gates to trigger envelopes elsewhere
- Or use an **envelope follower** on one output to animate processing on the other

### Great companions
- **Comparator / logic**: Joranalogue Compare 2, Doepfer logic modules, Klavis Two Bits
- **Envelope follower**: Sewastopol, Detect-Rx, Mutable Ears, A-119

### Result
Self-derived rhythms and feedback ecosystems where Phosgène partly controls its own processing.

---

## 18. Patch ideas by genre

## Dark techno
- FM output as bass voice
- Wavetable output layered quietly for grit
- Saturation + low-pass filter
- Modulate wave select every 8 or 16 bars with stepped random
- Add sidechain compression from kick

## Industrial / EBM
- High-register wavetable output into distortion
- FM output for metallic transient layer
- Triggered sample-and-hold on timbre
- Band-pass filtering and mono delay

## Ambient / sci-fi
- Slow random on wave select
- Octave-displaced wavetable for lower drone bed
- FM output through resonator and long reverb
- Manual crossfading between paths

## Electro / IDM
- Use Phosgène for percussion and bass alternately
- Audio-rate modulate filter cutoff
- Sample slices into a sampler
- Sequence octave jumps with precision adder

---

## A few especially strong pairing recommendations

## If you want it to sound bigger
- **Filter:** Bastl Ikarie or Joranalogue Filter 8
- **VCA/mixer:** Veils or Happy Nerding 3xVCA
- **FX:** FX Aid XL or Mimeophon

## If you want industrial destruction
- **Distortion:** Noise Engineering Ruina Versio / Terci Ruina
- **Dynamics:** Messor or MSCL
- **Random:** Ultra-Random Analog or Wogglebug

## If you want experimental timbre motion
- **Modulation:** Batumi, Ochd, Triple Sloths
- **Crossfader:** Morph 4 or Planar 2
- **Resonator:** Rings or a resonant filter bank

## If you want a tiny but serious voice
- **Envelope:** Pip Slope / Zadar
- **VCA:** Tallin / 2hp VCA
- **Filter:** 2hp MMF / Ikarie
- **FX:** MFX / FX Aid

---

## Best practical advice for patching Phosgène

1. **Use both outputs whenever possible**  
   That’s where a lot of its uniqueness probably lives.

2. **Attenuate CV heavily**  
   Small digital modules often have narrow sweet spots.

3. **Use octave displacement musically**  
   It’s not just a corrective feature; it’s a voicing feature.

4. **Let aliasing be part of the patch**  
   Don’t over-filter too early.

5. **Try it as a modulation source**  
   Especially into filters and analog oscillators.

6. **Pair it with analog processors**  
   Filters, VCAs, wavefolders, LPGs, and saturation can make the digital core feel much larger and more dimensional.

---

## Quick starter patch recipes

### 1. Brutal bass
- Pitch seq → Phosgène
- FM out → VCA → LPF
- Env → VCA
- Slow LFO → wave/mod input
- Wavetable out mixed quietly underneath

### 2. Machine drone
- Static pitch or very slow sequence
- Wavetable out → LPG → reverb
- FM out → distortion → delay
- Two unsynced slow LFOs on wave/fold controls

### 3. Metallic percussion
- Trigger envelope to VCA
- FM out → band-pass filter
- Fast decay envelope to pitch for transient
- Random stepped CV to wave select

### 4. Glitch lead
- Wavetable out → HPF → delay → reverb
- Clocked sample-and-hold to wave select
- Short envelope to VCA
- Manual crossfade with FM out for accents

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)