# Wenzellabs — NSA Selector

- [Manual PDF](../../manuals/wenzellabs_the_NSA_selector_ the NSA selector eurorack module.pdf)

---

```markdown
# The NSA Selector Eurorack Module Cheat Sheet

**Manual PDF:** *No direct PDF provided, content referenced from [NSA Selector GitHub Manual/Readme](https://github.com/wenzellabs/the_NSA_selector)*

---
## Quick Overview

- The NSA Selector is a unique Eurorack module that acts as a Fast Ethernet (100 Mbps) switch with two front-panel RJ45 Ethernet jacks and a single audio output.
- It does **not** function as a standard audio interface; it does not decode conventional protocols or audio formats. **All Ethernet traffic** passing between the two ports is tapped and converted into audio.
- The audio output reflects the raw binary data (bits) present on the network, not the decoded analog signal.

---

## Connections & Controls Reference

| Jack / Control       | Type            | Function                                                                                   | Voltage Range / Notes                                   |
|----------------------|-----------------|--------------------------------------------------------------------------------------------|--------------------------------------------------------|
| **LAN A (RJ45)**     | Input/Output    | Ethernet network connection; port 1 (switched with LAN B)                                  | Standard Ethernet; not voltage controlled              |
| **LAN B (RJ45)**     | Input/Output    | Ethernet network connection; port 2 (switched with LAN A)                                  | Standard Ethernet; not voltage controlled              |
| **AUDIO OUT**        | Output (TS/Mono)| Analog audio output derived from all bits on the network                                    | Line level, 4-bit, 25MS/s (MII), filtered through LPF  |

- **No panel controls**: No knobs, buttons, sliders, or toggles are present.
- **No CV inputs or outputs**.

---

## Basic Usage Instructions

1. **Patch Network**: Connect two Ethernet devices (computers, hubs, etc.) to LAN A and LAN B ports.
2. **Patch Audio**: Connect AUDIO OUT to desired Eurorack audio input, mixer, or recording interface.
3. **Send/Receive Data**: Any network traffic passing between LAN A and LAN B is mirrored & converted to audio in real time.
    - Use ping, file transfers, or any unencrypted/unencrypted data to manipulate the resulting audio.
4. **Creative Patching Tips**:
    - Use tools/scripts (included in the GitHub repo) to sequence or generate traffic (e.g., ping different IPs for rhythmic clicks).
    - Streaming uncompressed BMP image files" through the network creates audio patterns corresponding to image pixel data.
    - You can encode a .wav to raw 4-bit/25MHz (`.nsa` format, delta-sigma modulator needed) for maximum control.
5. **Network Echo/Delay Trick**:
    - Use tcpdump or similar commands (see manual) on a computer connected to the network to generate echo-like effects by forwarding/dumping packets.

---

## Reference Summary

- **Ethernet Ports (LAN A, LAN B)**: Bi-directional, 100 Mbps Fast Ethernet.
- **Audio Output**: Analog, mono, 4-bit digital interpreted through a DAC and low-pass filter. Output is *not voltage controlled* — purely data driven.
- **No direct voltage or CV integration.**


---

### Example tcpdump Commands (for Network Echo):

```sh
tcpdump -ni eth0
tcpdump -nvi eth0
tcpdump -nvi eth0 icmp
tcpdump -nvxi eth0
tcpdump -nxi eth0 not port ssh
```
Use these on a connected computer to maximize/modify traffic for creative results.

---

**For more documentation/tools**:  
- [NSA Selector GitHub Repository](https://github.com/wenzellabs/the_NSA_selector)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
```