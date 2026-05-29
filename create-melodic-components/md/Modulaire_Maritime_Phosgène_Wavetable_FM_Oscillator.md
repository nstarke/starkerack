# Modulaire Maritime — Phosgène Wavetable FM Oscillator

- [Manual PDF](../../manuals/Phosgène _ Modulaire Maritime.pdf)

---

# [Manual PDF / Source](https://www.modulaire-maritime.com/phosg%C3%A8ne)

From the provided manual pages, the module documented here is:

- **Modulaire Maritime Phosgène**
  - **2hp digital wavetable / FM oscillator**
  - **60 wavetables** arranged in **2 banks of 30**
  - **Two parallel sound paths / outputs**:
    - **Wavetable / waveshaping output**
    - **FM output**
  - **Wave folding / shaping** under manual control and external CV
  - **V/Oct tracking over 8 octaves**
  - **Octave up/down switching**
  - **Octave displace function** for shifting the wavetable range lower
  - **Settings memory** on reboot for bank, wave, octave
  - **11-bit digital character**, with intentional low-resolution/aliasing flavor at extremes

Because only one module manual is attached, I’ll focus on how **Phosgène** can be used with the rest of a typical Eurorack system to create **melodic components**: leads, basses, arpeggios, harmonized lines, and evolving tonal motifs.

---

## What Phosgène contributes melodically

Phosgène is fundamentally a **pitchable sound source**, so it is naturally suited to melodic work. Its most important musical strengths are:

- **Stable pitch tracking** via V/Oct
- **Large timbral range** from wavetable selection and folding
- **A darker, more controlled FM voice** due to its low FM base frequency approach
- **Two distinct tones at once** from separate wavetable and FM outputs

That means it can act as:

- a **main voice oscillator** for melodies
- a **bass oscillator**
- a **layered dual-timbre melodic source**
- a **countermelody generator** when its two outputs are treated separately
- a **dynamic digital voice** that changes timbre while keeping pitch constant

---

## Core melodic patch roles

## 1. Simple mono lead voice

This is the most direct use.

**Patch concept**
- Sequencer or keyboard **Pitch CV** → **Phosgène V/Oct**
- Gate/trigger → envelope generator
- Phosgène **wavetable output** → VCA or low-pass gate → mixer
- Envelope → VCA CV
- Optional modulation source → **wave select / folding CV**

**Why it works**
- The module tracks pitch over a wide range, so it can play melodies conventionally.
- The wavetable side gives you a bright, synthetic lead voice.
- Subtle CV over wave selection/folding adds expression without changing the notes.

**Best melodic use**
- Acid-adjacent digital leads
- Video-game flavored themes
- Industrial synth lines
- Sharp melodic ostinatos

---

## 2. Bassline voice

The manual specifically points toward **tight FM basses** and deep modulation. The **octave displace** function is especially useful here.

**Patch concept**
- Pitch CV → V/Oct
- Use the **octave down** setting and/or **octave displace**
- Take either:
  - **FM output** for darker bass
  - **wavetable output** for more aggressive bass
- Route to VCA/filter
- Use a short envelope for plucky bass or sustained envelope for drone bass
- Add slight wave/fold modulation from an envelope or slow LFO

**Why it works**
- The lower-register support helps preserve useful bass territory.
- FM is described as more “sober” spectrally than many harsher digital FM designs, which is good for focused low end.
- The wavetable side can add grind and edge.

**Best melodic use**
- Sequenced bass motifs
- Dark electro bass
- Industrial EBM patterns
- Melodic sub-bass with upper digital bite

---

## 3. Dual-layer melody from both outputs

A particularly interesting feature is that the **waveshaping and FM are available in parallel through separate outputs**. This is where the module becomes more than “just one oscillator.”

**Patch concept**
- Pitch CV → V/Oct
- **Wavetable output** → one VCA/filter chain
- **FM output** → second VCA/filter chain
- Same gate can open both VCAs, or separate envelopes can shape each differently
- Mix both voices together

**Why it works musically**
- Both outputs share pitch material, so they remain melodically coherent.
- But they differ in harmonic structure, so you get a layered tone from one oscillator.
- One output can carry the **body** of the note while the other supplies **attack**, **grit**, or **air**.

**Melodic applications**
- Lead + shadow layer
- Bass + upper articulation
- Clean-ish note core from one output, aggressive texture from the other
- Stereo melodic voice if panned left/right

**Example**
- Wavetable output: filtered, slightly resonant, central in mix
- FM output: brighter, shorter envelope, panned off-center
- Result: notes feel more alive and dimensional

---

## 4. Pseudo-counterpoint from one oscillator

Because the outputs are separate, you can process them differently enough to suggest two related melodic parts.

**Patch concept**
- Same pitch input drives Phosgène
- Wavetable output → quantizer-triggered sample-and-hold filter or delay line
- FM output → separate envelope/VCA path with rhythmic gate variation
- Send the two paths to different effects

**Musical result**
You won’t get two independent pitches from the module alone, but you can create the feeling of:
- melody + answer
- foreground line + ghost echo
- note + rhythmic harmonic accent

This is especially effective if one output is:
- short and plucky
- heavily delayed
- octave-shifted externally
- processed with wavefolder/filter/distortion

---

## 5. Evolving melodic timbre without changing pitch

A strong melodic patch often depends not only on the note sequence, but also on how timbre evolves per note.

Phosgène is good at this because:
- wave selection can be changed
- folding/shaping can be modulated
- FM depth responds well to CV

**Patch concept**
- Sequencer row 1 → V/Oct
- Sequencer row 2 or slow CV → wave selection / fold / FM modulation amount
- Envelope or random stepped CV → timbre parameter
- Keep pitch sequence fixed while timbre changes continuously

**Why this matters**
This creates melodies that feel:
- animated
- phrased
- non-repetitive
- “composed” rather than merely looped

**Great for**
- Berlin-school style motifs
- generative melodic patches
- soundtrack pulses
- machine-like themes with evolving color

---

## Practical melodic strategies

## A. Use wavetable output for note identity, FM output for accent

A very effective compositional approach:

- Let the **wavetable output** define the fundamental melodic note
- Bring in the **FM output** only on accented steps

**Patch**
- Main gate opens wavetable VCA every note
- Accent gate or secondary trigger opens FM VCA on selected notes

**Result**
- Melody stays clear
- Certain notes become more intense, edgy, or emotionally weighted

This is excellent for:
- 8-step basslines
- syncopated motifs
- techno and electro phrasing

---

## B. Use octave switching to separate register roles

Because the module includes octave controls and octave displacement, you can reposition the same sequence into different musical roles.

Examples:
- Mid-register wavetable lead
- Low-register FM bass
- High-register brittle arpeggio
- Lowered wavetable drone under a sequenced line

For melodic arrangement, this means Phosgène can be repurposed quickly in a patch from:
- melody
- to bass
- to ornament
- to drone support

---

## C. Exploit aliasing and 11-bit character as a melodic feature

The manual is explicit that at some ranges, especially high or heavily folded settings, you may get:
- more pronounced aliasing
- digital trash
- noisy wave behavior

For melodic work, don’t think of that only as a flaw. It can become:

- note attack texture
- expressive roughness on high melody notes
- a way to distinguish chorus/bridge sections
- a “broken digital” upper voice contrasting with a cleaner bass

A useful method:
- Keep verses or initial loop iterations on cleaner wave settings
- Increase wave/folding or select noisier waves in a later section
- This turns timbre into arrangement

---

## Melodic patch recipes

## 1. Dark digital bassline

**Use**
- V/Oct from sequencer
- FM output as main audio
- Low-pass filter after oscillator
- Short decay envelope to VCA
- Slight envelope to FM modulation depth or wave control

**Character**
- Focused low end
- Deep, brooding melodic bass
- Tight without becoming too metallic

**Style fit**
- Electro
- darkwave
- industrial techno
- soundtrack tension beds

---

## 2. Bright wavetable arpeggio

**Use**
- Arpeggiator/sequencer → V/Oct
- Wavetable output → LPG or VCA
- Clocked random or stepped CV → wave select
- Fast attack/short decay envelope

**Character**
- Crisp, animated notes
- Each step gets slight spectral variation
- Great for melodic sparkle

**Style fit**
- IDM
- synth pop
- chiptune-adjacent textures
- modular ambient with rhythmic articulation

---

## 3. Hybrid lead with parallel outputs

**Use**
- Pitch CV → V/Oct
- Wavetable output → filter → VCA
- FM output → separate VCA, maybe no filter
- One envelope for body, second shorter/snappier envelope for FM path
- Mix to taste

**Character**
- Strong melodic intelligibility
- Controlled aggression
- Feels more “produced” than a single raw oscillator

**Style fit**
- lead hooks
- solo lines
- cinematic industrial melodies
- live performance voice

---

## 4. Morphing sequence

**Use**
- 8- or 16-step sequencer for pitch
- Another CV lane or slow LFO for wave selection
- Manual bank changes between song sections
- Optional octave displace engaged for lower, weightier passage

**Character**
- Same melody can move through several emotional colors
- Useful for long-form repetition without boredom

**Style fit**
- techno
- ambient sequences
- post-industrial modular jams
- generative melodic systems

---

## 5. Call-and-response processing patch

**Use**
- Wavetable output → dry/main melodic voice
- FM output → delay/reverb/distortion chain
- Rhythmically gate or duck one against the other

**Character**
- The melody seems to answer itself
- Very effective in sparse arrangements

**Style fit**
- experimental pop
- minimal wave
- soundtrack composition
- live improvisation

---

## What other modules pair best with it for melody

Since this is an oscillator, it benefits most from the usual “voice chain” modules:

### Essential companions
- **Pitch sequencer or keyboard controller**
- **Envelope generator**
- **VCA**
- **Mixer**
- **Filter or low-pass gate**

### Especially useful companions
- **Quantizer**  
  For turning random CV into tonal melodies.

- **Sequential switch / clocked switch**  
  To alternate between wavetable and FM paths or different processing chains.

- **Precision adder / octave switcher**  
  To transpose melodic phrases while preserving tuning.

- **Utility attenuator / offset**  
  Very useful for dialing in sweet spots on timbre CV.

- **Clocked random / sample-and-hold**  
  Great for stepped wave changes that stay rhythmically tied to melody.

- **Stereo effects**  
  Delay, chorus, or reverb can turn the dual outputs into expansive melodic textures.

---

## Best compositional uses in a rack

If I were building melodic material around Phosgène in a Eurorack patch, I would treat it in one of these three ways:

### 1. As the main melody oscillator
Use the wavetable output as the core tone and animate timbre with CV.

### 2. As a bass and hook generator
Use the FM output for bass and reserve more aggressive wavetable settings for hook phrases.

### 3. As a layered voice source
Use both outputs simultaneously and process them differently for a richer melodic line from minimal rack space.

Because it’s only **2hp**, this is especially attractive in compact performance systems where one module needs to do a lot of work.

---

## Overall musical assessment

For melodic use, Phosgène seems best suited to:

- **digital basslines**
- **aggressive or characterful leads**
- **evolving sequenced melodies**
- **layered mono voices**
- **industrial / electro / dark melodic textures**

Its strengths are not “vintage warmth” or traditional subtractive purity. Instead, it offers:

- compactness
- strong digital personality
- useful pitch tracking
- timbral variation under CV
- dual parallel outputs that can make a single melodic line feel more complex

That makes it a very strong **melodic sound source** if your music benefits from:
- edge
- texture
- spectral movement
- darker FM color
- intentionally digital tone

If you want, I can also turn this into:
1. a **patch cookbook** with step-by-step cable routing, or  
2. a **musical role matrix** showing how Phosgène fits into bass / lead / arp / drone / counterpoint duties.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)