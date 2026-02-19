# 2hp — Tune

- [Manual PDF](../../manuals/Tune_Manual_2023.pdf)

---

[2hp Tune Manual (PDF)](https://twohp.com/manuals/tune_manual.pdf)

---

## Using the 2hp Tune for Densely Rhythmic, Hyper-Complex Percussion Sequences

**2hp Tune** is a voltage quantizer—it does not generate sound itself but precisely shapes voltages coming from sequencers, LFOs, random sources, or any modulation into musically constrained melodic values based on selected scales. Here’s how you can leverage it for intricate, polyrhythmic, percussive eurorack patches:

---

### Techniques for Percussive & Complex Patterns

#### 1. **Quantize Modulations for Percussive Voices**
- Use **complex CV sources** (such as random stepped voltages, Turing Machine, Euclidean sequencers, or rhythmic LFOs clocked at different rates) as **inputs** to the 2hp Tune’s `Input`.
- The quantized **output** can be sent to the pitch CV input of a percussive voice (e.g., synth voice, percussion module, or self-oscillating filter).
- By quantizing trigger- or clock-driven CVs, you generate **pitched rhythmic pulses, tuned noise, or metallic percussion** that follow exotic time relationships.

#### 2. **Bias Knob/Control Voltage Tricks**
- Modulate the **Bias knob** or use its CV input with another rhythmic source—for example, a clock-divider, logic gate, or manually trigger-by-hand—so the availability of pitches within the chosen scale is **rhythmically “scanned.”**
- With CV control, you can dynamically morph drum pitches or accents in **polyrhythmic layers** without changing the core rhythm.

#### 3. **Microtonal Percussive Melodies**
- Set the **Scale** to Octatonic, Whole Tone, or Diminished for “offgrid” melodic quantization. Feed in a fast clocked CV, like a burst generator or clock-multiplied LFO, for **unusual stepped patterns** that can be routed to percussion oscillators or even noise-based voices.
- Using complex clock divisors/multipliers on different CV sources patched to input and bias yields constantly evolving, overlapping patterns.

#### 4. **Create Drum Voices Out of Pitch**
- Send the quantized output to both the **V/Oct input** of a short-decay envelope-controlled sine/triangle oscillator and the **decay length** of that envelope.
- By quantizing rapidly, each new note triggers a new percussion “hit” that’s in tune, creating **rhythmic tuned percussion with unpredictable (poly)rhythms**.

#### 5. **Trigger Manipulation**
- Use the output of Tune as a source for switched routing or sample selection (e.g., with sequential switch modules or drum sample players).
- Different scales correspond to different sample triggers or effect parameters—each scale change or quantized output represents a **trigger in a polyrhythmically evolving grid**.

#### 6. **Scale Modulation for Polyharmony**
- Patch modulation into the scale select (accomplished by manual or sequential trigger if you have hands-on time) to shift between different scale layouts for the same input CV.
- Rapidly cycling or switching between scales on rhythmic boundaries creates “metric modulation” for percussion—accents and hits shift in both pitch and tonality.

---

### Patch Example

1. **Rhythm Source #1**: Stepped random voltage from a noise module clocked by a 5/4 Euclidean rhythm.
2. **Rhythm Source #2**: LFO synced to a different division (e.g., 7 triggers per 3 measures).
3. **Patch**: 
    - Stepped random to Tune’s `Input`
    - LFO to Tune’s `Bias CV Input`
    - Set scale to Diminished or Whole Tone
    - Output quantized CV to the 1V/Oct of a percussion oscillator (e.g., drum synth)
    - Gate/trigger output from the same rhythm sources triggers drum envelopes.
4. **Result**: Drum voice shifts pitch, harmonics, or resonance in sync with overlapping, irregular polyrhythms.

---

### Making it Unique, Punchy, Percussive

- **Fast Modulation**: The Tune tracks up to 5V input-range, so velocity or accent sources can further “animate” triggers or envelopes with quantized output.
- **Non-standard Scales**: Use Octatonic or Egyptian Minor for exotic percussion flavors—tuned but unusual intervals.
- **Stacking**: Use several Tune modules, or mult output to numerous voices for complex polyrhythmic interlocking melodies.
- **Feedback Patching**: Try routing drum envelope outputs into the `Bias CV input` for “self-modulating” percussion grooves.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)