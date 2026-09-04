---
layout: default
---

# Analog Synthesizer Project

An experimental analog synthesizer designed and built from discrete analog circuitry and controlled using an RP2350-based embedded system.

---

## Demo Video

<div style="position:relative; padding-bottom:56.25%; height:0; overflow:hidden; max-width:900px; margin:30px auto;">
  <iframe
    src="https://www.youtube.com/embed/kVt6d5Q3_-w"
    title="Analog Synthesizer Project Demo"
    style="position:absolute; top:0; left:0; width:100%; height:100%;"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    allowfullscreen>
  </iframe>
</div>

---

## Project Overview

This project involved the design and construction of an analog synthesizer along with a custom embedded control system.

The controller uses an **RP2350 microcontroller** to interface digital controls with the analog synthesizer circuitry.

### Key Technologies

- RP2350 microcontroller
- Raspberry Pi Pico SDK
- C/C++
- MCP4725 DACs
- I²C communication
- ADC feedback
- Button matrix
- Analog filters and amplifiers
- Control-voltage generation

---

## System Architecture

The embedded controller translates user input into analog control voltages used by the synthesizer.

```text
Button Matrix
      │
      ▼
    RP2350
      │
      │ I²C
      ▼
   MCP4725
      │
      ▼
Control Voltage
      │
      ▼
Analog Synthesizer
      │
      ▼
    Audio
