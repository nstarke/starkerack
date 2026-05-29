# Buchla and Tiptop Audio — 248t

- [Manual PDF](../../manuals/Buchla_&_Tiptop_Audio_248t.pdf)

---

[Manual PDF](https://tiptopaudio.com/manuals/248t/Tiptop_Audio_248t_MARF_User_Manual.pdf)

# Tiptop Audio / Buchla 248t MARF Cheat Sheet

## What it is
The **248t MARF** is a **16-stage dual function generator / sequencer / arbitrary CV programmer**.  
It has **two independent Function Generators (FG1 and FG2)** that read the same bank of 16 programmed stages in different ways.

Each stage can store:
- **Voltage value**
- **Time value**
- **Pulse 1 on/off**
- **Pulse 2 on/off**
- **Voltage behavior**: quantized, sloped, range, source
- **Timing behavior**: time range, external/internal source
- **Stage behavior**: stop, sustain, enable, first, last

---

# Quick Start

## Basic 16-stage CV sequence
1. Set a Function Generator to **internal** stage advance.
2. Set its **Mode** to run using **Start**.
3. Program stage voltages with the **top row sliders**.
4. Program stage times with the **bottom row sliders**.
5. Patch:
   - **Voltage Out** or **ART Out** → oscillator pitch
   - **Pulse Out 1** → envelope gate
6. Add pulses to desired stages with **Output Pulses 1/2**.
7. Use **Stage Number** to select a stage for editing.

## Simple looping sequence
- Mark one stage as **First**
- Mark another as **Last**
- The FG will loop between them

## Quantized melodic sequence
1. For desired stages, enable **Quantize**
2. Choose **Key**
3. Choose **Scale**:
   - **10 = Major**
   - **11 = Minor**
   - **12 = Chromatic**

## Glide / portamento
- Enable **Sloped** on desired stages  
- Slew amount follows the stage’s **interval time**

## Variable stage timing
- Use bottom sliders for stage times
- Set global **Time Multiplier** to scale all stage times
- Or use **Time Source = External** and feed CV into A/B/C/D

---

# Core Concept

The module has 3 main areas:

## 1. Function Generators (left side, two identical sections)
Each FG reads the programmed stage data and outputs:
- pitch/CV
- time CV
- programmed pulses
- reference ramp
- all-stage pulse stream

## 2. Programming Section (center)
This is where you edit what each stage does.

## 3. Sliders + stage LEDs (right side)
- **Top 16 sliders** = stage voltage / external source selection
- **Bottom 16 sliders** = stage interval time
- **16 LEDs between rows** = stage indicators

---

# Programming Workflow

## Select a stage
Use **Stage Number** switch:
- left/right steps through stages
- hold to scroll quickly
- wraps around from 16→1 and 1→16

## Edit selected stage
Use the programming controls to set:
- pulses
- voltage mode
- operating mode
- time range
- internal/external sources

## Apply to all stages
While holding **Stage Number** so stage LEDs scroll, press a programming function to apply it to all 16 stages.

---

# Stage Programming Reference

## Output Pulses
Each stage can independently output:
- **Pulse 1**
- **Pulse 2**

Switch behavior:
- press **up** = add pulse
- press **down** = remove pulse

## Voltage programming
Per-stage options:

### Quantize / Continuous
- **Quantize on** = 1V/oct quantized output
- **Continuous** = unquantized CV

### Sloped / Stepped
- **Sloped** = glide between stages
- **Stepped** = hard step

### Range
- **Full** = **0 to 10 V**
- **Half** = **0 to 5 V**
- **Limited + octave offsets** = 2 V span with offsets

### Source
- **Internal** = use stage voltage slider
- **External** = use one of external CV inputs A/B/C/D selected by slider position

## Operating mode
Per-stage options:

### Stop
FG halts on this stage until a **Start pulse** is received.  
The stage still observes its interval time.

### Sustain
If a high gate is present at **Start**, the FG holds on the stage as long as gate stays high.

### Enable
FG waits on the stage until **Start input > 5 V**.

### First / Last
Defines loop start and loop end.

## Time programming
Per-stage options:

### Time Range
Four selectable timing ranges from:
- **0.002 s minimum**
- up to **2 minutes maximum**

Manual notes default panel range as:
- about **2 to 30 seconds** on the sliders unless otherwise modified

### Time Source
- **Internal** = use time slider + range setting
- **External** = use external CV input A/B/C/D

If set to **External** and no CV is patched, interval defaults to **fastest value** of selected range.

---

# Function Generator Operation

Each FG has its own transport and addressing controls.

## Mode controls
### Advance
Manual step to next stage.

### Start / Stop
Starts or stops internal clock, manually or by pulse input.

### Status LEDs
- **Green** = running
- **Yellow** = hold/waiting
- **Red** = stopped

Red stop can happen because of:
- stop command
- programmed stop stage
- stage address set to continuous

## Stage Address controls
### Reset
Returns FG to:
- first programmed **First** stage, or
- **Stage 1** if no First is set

### Display
Shows current stage position without interrupting operation.

### Cont / Strobe
- **Continuous** = sweep through stages with address control, internal clock stopped
- **Strobe** = load stage corresponding to current stage address

### Internal / External
Selects whether stage position is controlled by:
- internal address control
- external CV at Stage Address input

---

# Presets / Scales / ART

## Presets
### Load
Press **Load**, then stage button **1–12**

### Save
Press **Save**, then button **1–12**

Saved:
- all stage settings
- slider values

Important:
- after loading a preset, physical sliders are “caught” only when moved past stored values

## Key / Scale
### Key
Press **Key**, then select **1–12** for:
- C, C#, D, D#, E, F, F#, G, G#, A, A#, B

### Scale
Press **Scale**, then:
- **10** = Major
- **11** = Minor
- **12** = Chromatic

## ART + Auto Tune
- **ART Out** sends digital pitch data for compatible oscillators like the **259t**
- Press **Autotune** once = send tuning message
- Hold **Autotune** = send initial tune message

Tiptop recommends using **Half range (0–5 V)** or **Limited range** with 259t for practical pitch range.

---

# Clear / Reset Behavior

## Clear switch
Pressing **up** clears all 16 stages and resets programming:
- Pulse 1 and 2 cleared
- Voltage mode = **Continuous / Full Range / Internal**
- Operating mode cleared
- Time range = **2 to 3 seconds**
- Slider values set to current physical positions

---

# External Input Calibration
If 0 V external input does not produce 0 V behavior:
1. Unplug A–D inputs
2. Set both FGs to **STOP**
3. Press **External** switch **4 times**
4. LED flashes about 2 seconds

---

# Inputs / Outputs Reference

> Voltage ranges below are included where stated in the manual.  
> Some jack thresholds/scales are described functionally because the manual does not specify an exact full range.

## Inputs

### External Inputs A, B, C, D
- **Type:** CV inputs
- **Use:** per-stage selectable source for voltage or time
- **Range:** **not explicitly specified in manual**
- Notes:
  - for voltage source selection, slider picks A/B/C/D
  - for time control, if no CV present and source is external, time goes to fastest setting

### FG1 Start input
- **Type:** gate/pulse/CV input
- **Use:** start, sustain hold, enable logic
- **Threshold:** **Enable requires > 5 V**
- Other exact acceptable range: **not specified**

### FG2 Start input
- **Type:** gate/pulse/CV input
- **Use:** same as above
- **Threshold:** **Enable requires > 5 V**
- Other exact acceptable range: **not specified**

### FG1 Stop input
- **Type:** gate/pulse input
- **Use:** stop transport
- **Range:** not specified

### FG2 Stop input
- **Type:** gate/pulse input
- **Use:** stop transport
- **Range:** not specified

### FG1 Advance input
- **Type:** pulse input
- **Use:** manual/remote stage advance
- **Range:** not specified

### FG2 Advance input
- **Type:** pulse input
- **Use:** manual/remote stage advance
- **Range:** not specified

### FG1 Stage Address input
- **Type:** CV input
- **Use:** externally control stage addressing when set to external
- **Range:** not specified

### FG2 Stage Address input
- **Type:** CV input
- **Use:** externally control stage addressing when set to external
- **Range:** not specified

### FG1 Time Multiplier CV input
- **Type:** CV input with attenuverter
- **Use:** scales stage durations globally for FG1
- **Range:** not specified

### FG2 Time Multiplier CV input
- **Type:** CV input with attenuverter
- **Use:** scales stage durations globally for FG2
- **Range:** not specified

---

## Outputs

### FG1 ART Output
- **Type:** digital pitch/control output
- **Use:** ART oscillator control
- **Range:** digital ART signal, not standard analog voltage range

### FG2 ART Output
- **Type:** digital pitch/control output
- **Use:** ART oscillator control
- **Range:** digital ART signal

### FG1 Voltage Output
- **Type:** CV output
- **Use:** stage voltage output with modifiers applied
- **Range:**
  - **Full:** **0 to 10 V**
  - **Half:** **0 to 5 V**
  - **Limited:** **2 V span** with octave offsets
  - **Quantized mode:** 1 V/oct pitch behavior

### FG2 Voltage Output
- **Type:** CV output
- **Use:** same as FG1
- **Range:**
  - **0 to 10 V** full
  - **0 to 5 V** half
  - **2 V span** limited modes

### FG1 Time Output
- **Type:** CV output
- **Use:** outputs voltage proportional to interval time slider
- **Range:** not specified

### FG2 Time Output
- **Type:** CV output
- **Use:** outputs voltage proportional to interval time slider
- **Range:** not specified

### FG1 Pulse Output 1
- **Type:** gate/pulse output
- **Use:** stages programmed with Pulse 1
- **Range:** not specified

### FG1 Pulse Output 2
- **Type:** gate/pulse output
- **Use:** stages programmed with Pulse 2
- **Range:** not specified

### FG2 Pulse Output 1
- **Type:** gate/pulse output
- **Use:** stages programmed with Pulse 1
- **Range:** not specified

### FG2 Pulse Output 2
- **Type:** gate/pulse output
- **Use:** stages programmed with Pulse 2
- **Range:** not specified

### FG1 Reference Output
- **Type:** CV/ramp output
- **Use:** downward ramp over stage duration
- **Range:** not specified

### FG2 Reference Output
- **Type:** CV/ramp output
- **Use:** downward ramp over stage duration
- **Range:** not specified

### FG1 All Pulses Output
- **Type:** pulse output
- **Use:** emits pulse on every stage address change
- **Range:** not specified

### FG2 All Pulses Output
- **Type:** pulse output
- **Use:** emits pulse on every stage address change
- **Range:** not specified

---

# Controls Reference

## Sliders
### 16 Output Voltage sliders
- Set per-stage voltage
- In external voltage-source mode, select **A/B/C/D** source instead
- Output range depends on stage range mode:
  - **0–10 V full**
  - **0–5 V half**
  - **2 V span limited**

### 16 Interval Time sliders
- Set per-stage interval time
- Also generate corresponding **Time Output** CV
- Default panel behavior roughly **2 to 30 seconds**, modified by time range and multiplier

---

## Programming Section switches/buttons

### Output Pulses 1, 2
- 3-position momentary
- up = add pulse
- down = remove pulse

### Clear
- momentary
- up = clear/reset programming

### Stage Number
- 3-position momentary
- scroll/select stages for editing

### Quantize / Continuous
- 3-position momentary
- up = quantize
- down = continuous

### Sloped / Stepped
- 3-position momentary
- up = sloped
- down = stepped

### Range selector
- momentary options:
  - full
  - half
  - limited ranges with offsets

### Voltage Source: Internal / External
- 3-position momentary
- selects internal slider or external A/B/C/D source

### Stop
- 3-position momentary
- up = add stop stage
- down = remove

### Sustain
- 3-position momentary
- up = add sustain
- down = remove

### Enable
- 3-position momentary
- up = add enable
- down = remove

### Cycle First / Last
- 3-position momentary
- define loop start/end points

### Time Range switches
- 4 momentary switches
- select timing range from **0.002 s** to **2 min**

### Time Source: Internal / External
- 3-position momentary
- selects internal timing or external A/B/C/D timing CV

---

## Preset / scale buttons

### Load
Recall preset

### Save
Store preset

### Buttons 1–12
- preset slots
- key selection
- scale selection:
  - 10 major
  - 11 minor
  - 12 chromatic

### Key
Select root note

### Scale
Select scale type

### Hold / Initial Tune / Autotune
- press = autotune message
- hold = initial tune message

---

## Function Generator controls per side

### Advance button/input
Manual stage step

### Start button/input
Start/hold/enable interaction

### Stop button/input
Stop transport

### Reset
Return to first programmed stage or stage 1

### Display
Show current FG stage

### Cont / Strobe switch
- continuous address sweep
- stage strobe load

### Internal / External switch
Select internal or external stage address source

### Stage Address knob
Sets stage address in internal addressing mode / continuous sweep context

### Time Multiplier knob
Global time scaling:
- **0.5x to 4x**

### Time Multiplier CV attenuverter
Amount/polarity of time multiplier CV

### ART gate source switch
Selects ART gate source:
- **Pulse 1**
- **Pulse 2**
- **All**

---

# Useful Patch Ideas

## 1. Dual related melodies
- FG1 Voltage Out → Oscillator 1 pitch
- FG2 Voltage Out → Oscillator 2 pitch
- Same programmed stages, different loop boundaries via First/Last

## 2. Sequencer + envelope source
- Voltage Out → oscillator pitch
- Reference Out → LPG CV
- Pulse 1 → gate/trigger for articulation

## 3. Addressed wavetable-ish CV scanner
- Set Stage Address to **External**
- Feed slow CV into stage address input
- Use Voltage Out as a scanned arbitrary function

## 4. Rhythmic modulation source
- Use **Time Out** as a second CV lane
- Set time source to **External** if you want time sliders as pure CV without affecting stage timing

---

# Practical Tips

- **Half range** is easiest for tonal pitch work.
- **Sloped** stages create pitch glide tied to stage time.
- Use **First/Last** creatively to make different loop windows for FG1 and FG2.
- **All Pulses Out** is useful as a derived clock.
- **Reference Out** is excellent for LPG plucks and decays.
- In **External voltage source** mode, the top slider selects **which external input** is active for that stage.
- After loading presets, sliders use a **pickup/catch** behavior.

---

## Specs
- **Width:** 72 HP
- **Depth:** 45 mm
- **Power:** +12 V **340 mA**, -12 V **30 mA**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)