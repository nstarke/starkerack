# Quanalog Instruments — Boubou

- [Manual PDF](../../manuals/Boubou – Quanalog Instruments.pdf)

---

[Quanalog Boubou Manual (Website)](https://quanalog.com/boubou/)

# Quanalog Boubou Eurorack Drum Synthesizer Cheat Sheet

**Module Size:** 28HP  
**Voices:** 5 (Kick, Lo Tom, Hi Tom, Snare, Hats)  
**Build:** All-metal pots, switches, and jacks, black and gold panel

---

## Quick Start
- **Patch simple short triggers into TRIG inputs for normal drum hits.**
- **Apply CV or audio rate signals to TRIG and CV jacks for experimental sounds and dynamic variation.**
- **Use outputs independently or layer/feedback between voices using additional patching.**

---

## Channel Reference

### KICK DRUM
- **Outputs:**  
  - *Kick Out*
- **Inputs:**  
  - *Trig In* – accepts triggers/gates/audio (standard: 5V trigger; accepts cv/audio: -5V to +5V)
  - *Tune CV* – pitch (typical 0–5V; V/oct scaling not guaranteed)
  - *Decay CV* – decay (approx. 0–5V)
- **Knobs/Controls:**  
  - *Freq, Resonance* – tuning the fundamental
  - *Click Freq, Click Mix* – shape and mix attack click
  - *Volume* – output level
  - *Overdrive* – analog drive for harder sounds
  - *Compression* (toggle/knob?) – soft, punchy, overdriven
- **Special:**  
  - *Audio-rate at TRIG = wavefolder/bitcrushing FX*
  - *Can self-resonate as sine oscillator (with Overdrive high)*
  - *Classic 808/909-style sounds*

---

### DUAL TOM (LO/HI)
- **Outputs:**  
  - *Lo Tom Out, Hi Tom Out*
- **Inputs:**  
  - *Trig In (per voice)* – triggers (standard: 5V), audio/CV possible (-5V to +5V)
  - *Resonance CV* (per voice) – tune/drum pitch (0–5V)
- **Knobs/Controls:**
  - *Freq, Resonance* (per voice) – set tom pitch/body
  - *Retrig* (shared) – controls volume of retriggered note (creates rolls/flams/“hand play” feel)
  - *Volume* – per tom
- **Special:**  
  - *Without trigger: become dual notch filters with CV freq*
  - *Feed other engines for filtering/harmonic FX*

---

### SNARE 
- **Outputs:**  
  - *Snare Out*
- **Inputs:**  
  - *Trig In* – triggers (standard: 5V), audio/CV (-5V to +5V)
  - *Decay CV* – snare tail (0–5V)
  - *Resonance CV* – snare pitch (0–5V)
- **Knobs/Controls:**  
  - *Freq, Resonance* – snare body/“spring” sharpness
  - *Decay* – envelope length
  - *Volume* – output
- **Special:**  
  - *If Hi Tom Trig not patched, Hi Tom acts as resonance/body for snare (patching separates them)*
  - *Wide sound range — snare, clap, noise hats*

---

### HATS
- **Outputs:**  
  - *Hats Out*
- **Inputs:**  
  - *Trig In* – open/close hat (5V triggers), CV/audio (-5V to +5V)
  - *Decay CV* – envelope length (0–5V)
  - *External In* – mix another VCO/sound for custom hats
- **Knobs/Controls:**  
  - *Freq, Resonance* – hat sizzle/character
  - *Decay* – open/close time
  - *Noise Mix, Ext In Mix* – blend noise/osc input
- **Special:**  
  - *Acts as decay VCA for Ext In if noise turned off*
  - *Can ring external VCO, create noise VCO FX*

---

### GLOBAL / SHARED NOTES
- **Each section’s CV inputs:**  
  - *Pitch/Tune/Resonance* CV: 0–5V
  - *Decay CV*: 0–5V
  - *Trigger Inputs*: Accept short pulses, gates, audio, step CV (-5V to +5V gives velocity sens)
- **All voices can process audio as signal processors (filters, wave-shaping) if you patch audio to Trig/CV/Ext In.**
- **Natural accenting possible with gate/trigger length or step CV into Trig.**

---

## Summary Table

| Voice         | Trig In | CV Pitch/Res | CV Decay | Audio In | Output |
|---------------|---------|--------------|----------|----------|--------|
| Kick          | Yes     | Yes          | Yes      | Trig     | Out    |
| Lo Tom        | Yes     | Yes          | -        | Trig     | Out    |
| Hi Tom        | Yes     | Yes          | -        | Trig     | Out    |
| Snare         | Yes     | Yes          | Yes      | Trig     | Out    |
| Hats          | Yes     | -            | Yes      | Ext In   | Out    |

_All CV and audio inputs typ. -5V to +5V safe, 0–5V recommended for musical range, 5V triggers standard._

---

## Tips & Tricks
- **Low/Hi Tom unpatched behave as filters for other voices.**
- **Try patching section outputs to other section Trig inputs for experimental modulation!**
- **Adjust Retrig for flam/rolls (varied gate length triggers).**
- **Patch velocity or envelope CVs for dynamic hits.**
- **External In on Hats for custom cymbal/metallic timbres.**

---

## Further Reading

- [Manual/Website – Full details & sound examples](https://quanalog.com/boubou/)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)