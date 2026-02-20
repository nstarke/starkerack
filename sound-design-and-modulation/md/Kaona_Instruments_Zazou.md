# Kaona Instruments — Zazou

- [Manual PDF](../../manuals/Zazou_manual_ENG_V1-0.pdf)

---

[Download the Zazou Eurorack Module Manual PDF](https://www.kaona.fr/uploads/files/zazou_manual_en_v1_0.pdf)  
*(Official English PDF from Kaona's website)*

---

# Modulating Zazou for Unique and Advanced Sound Design

The Kaona Zazou is a generative music module with a powerfully flexible MIDI and CV output interface, deeply algorithmic note creation, polyphony/multitimbrality, and plenty of parameters suited for creative modulation. While **Zazou does not generate audio directly**, you can utilize its rich note and CV outputs to drive external synths, drum modules, or samplers in wild and unpredictable ways.

Below, we’ll look at techniques to leverage Zazou’s features for:

- **Distorted Percussive Sounds**
- **Gnarly Dubstep/Drum & Bass Basslines**
- **Haunting Atmospheric Pads**

*(Assuming you are using Zazou to drive drum synth modules, aggressive monosynths, or polyphonic pads via MIDI/CV)*

---

## Distorted Percussive Sounds

### 1. **Algorithm**: Use **Random, Serial, or Arpeggio**
- **Random**: Set short and highly variable note durations (DURATION RND high, short overall DURATION), and restrict the octave range to 1–2 to keep things punchy.
- **Serial**: Use the chromatic scale for 12-tone “atonal” percussion, like glitchy IDM or harsh, broken beats.
- **Arpeggio**: Try ‘Double’ and ‘Strum’ types with root/scale chords for rapid note repeats and erratic rhythms.

### 2. **Ornamentation**: Utilize **TRILL**, **TRIPLET**, or **REPEAT** ornaments.
- These can create rapid-fire, granulated note triggers suitable for metallic, rattling, or broken-sounding percussion when sent to percussive modules.

### 3. **Gate Modulation**
- Route crazy stepped random gates (or Skippy or other rhythm modules) to Zazou’s gate ins for irregular, jittery percussive patterns.
- Use GATE duration so the amounts map directly to trigger length (great for drum synths like BIA, Plonk, SSF Entity, etc).

### 4. **Velocity Modulation**
- Set **VELOCITY RND** high—this will make every hit different in accent and drive further distortion downstream if you’re modulating VCA drive or a drum module’s input level.

### 5. **CV Trick: Layering Tracks**
- Assign multiple tracks (each with a different algorithm and insert points, maybe one in random, one in arpeggio) to the same drum synth via MIDI or CV, creating layered, stuttering, and polyrhythmic trigger beds.

---

## Crazy Basslines (Dubstep / D&B)

### 1. **Algorithm**: Use **Walkingbass, Mandelbrot, Julia, or Sierpinski**
- **Walkingbass**: Choose “Boogie”, “Blues”, or “RnRoll” types for classic walking patterns. Set **VELOCITY ODD/EVEN** for groove.
- **Mandelbrot/Julia**: Set parameters (STARTING POINT, DIVAGATION, TARGET, DRIFT) for evolving, unpredictable bass patterns with quick pattern mutation (“Steps” low for repetitive riffs, high for wild atonality).
- **Sierpinski**: Low recursion and subdivisions with an aggressive root can create jagged, angular riffs.

### 2. **Pitch Movement**
- Set a narrow **OCTAVE RANGE** for subby, consistent bass, or a wide range for ‘talking’ sequences reminiscent of neuro bass.

### 3. **Gate Control**
- Use an *external rhythmic source* for the gate input (like Skippy) for syncopation/complex rhythm, and set DURATION to “GATE” for punchy bass chunks.

### 4. **Ornamentation**
- Add **APPO. +** and **APPO. -** (appoggiaturas) to mimic glide/slides.
- Try **TRILL** for rapid stepwise movement to simulate old tracker/glitch effects.

### 5. **Sequence Mod Tricks**
- Use the **II-V-I**, **TIERCE UP/DOWN**, or **ANATOLE** sequence to push the bassline through rapid chordal changes—create a foundation for moving, harmonically restless bass.

### 6. **Velocity**
- High random velocity (or alternating even/odd) to push your downstream synth/filter into overdrive or modulate distortion.

---

## Haunting Atmospheric Pads

### 1. **Algorithm**: Use **Fibonacci, Sierpinski, Mandelbrot, Julia**
- **Fibonacci**: Great for organic, slowly-evolving, always-morphing pad sequences.
- **Sierpinski**: High recursion and subdivisions for cyclical, endlessly self-similar patterns—perfect for drones.
- **Julia/Mandelbrot**: Complex, unpredictable, fractal-like progression for evolving pads—set high “steps” for slow motion.

### 2. **Scale & Chord Configuration**
- Use **chromatic** or **exotic** modes (Blues, Dorian, Lydian, Locrian, Bebop, etc) for mysterious, non-traditional tonalities.
- Assign different tracks to different scales and chords (e.g., one in pentatonic, one in blues, one in harmonic minor) and stack their MIDI/CV to a pad synth for thick chord voicings and microtonal drones.

### 3. **Sequence Progression**
- Use **SCALE UP/DOWN** or **CIRCLE OF 5ths/4ths** for gradual, endlessly turning harmonic motion (great for pads that never resolve).
- Set each track to staggered sequences for complex, shifting harmonies.

### 4. **Note Durations**
- Set long note durations (x2, x4), whole notes, or even longer, so notes overlap and blend for smears of harmony.
- Mix in occasional **BREVE** ornaments for extra-long, drone-like events.

### 5. **Velocity**
- Gentle velocity modulation (small VELOCITY RND) for expressive, "alive" pads when sent to velocity-sensitive synths.

### 6. **Live Modulation**
- Use Zazou’s Live mode to mute/unmute tracks in real-time, swap out sequences/algorithms with long encoder clicks, and create on-the-fly evolving atmospheres.

---

## Patch Example Ideas

- **Distorted Percussive Patch:**
  - Zazou Track 1 (Random, short DURATION RND max, ORNAMENT: TRILL) → BIA/Plonk via CV/Gate. Track 2 (Serial) → metallic percussion synth. Gate from high-entropy trigger source/Skippy.
  - Distort and process both signals externally for crunchy, unpredictable IDM percussion.

- **Dubstep Bass Patch:**
  - Track 3 (Mandelbrot, mid RANGE, low STEPS, VELOCITY RND high), sequence to rapidly changing chords (TIERCE DOWN), output to aggressive analog/digital bass module. Gate input from shuffled groove clock.
  - Filter/overdrive after for even more movement and punch.

- **Atmospheric Pad Patch:**
  - All 4 tracks, each a different fractal algorithm, different scale/chord, slow durations, sequence through CIRCLE OF 5ths. All outputs summed via MIDI to a multi-timbral digital synth for deep ambient washes.

---

## Additional Tips

- **MIDI Out:** Stack, layer, or split tracks to various synths for multimbral chaos.
- **Gate Outs:** Use as not only note triggers but CVs for rhythmic modulation of other parameters in your rack (filters, fx, etc).
- **CV Outs:** Use for velocity, aftertouch, or wild external modulation.
- **Live:** Jam by muting/unmuting tracks, or swapping sequences/algorithms in real time for morphing soundscapes.

---

Explore, experiment, and abuse the limits—the real fun will be in finding new unexpected behaviors from combining Zazou’s note/CV madness with your wildest synths and FX.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)