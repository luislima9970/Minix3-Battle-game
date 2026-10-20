# Minix3 Battle Game

A game written in C for MINIX 3, built entirely on hand-written device drivers. Developed for the **LCOM** (Computer Labs) course unit at FEUP, University of Porto.

## Overview

The project talks to the hardware directly through I/O ports and interrupt handlers, with no external graphics or input libraries. The game runs on top of the drivers, which cover the main peripherals[...]

## Drivers

| Device | Role |
|--------|------|
| Timer (i8254) | Frame timing and game loop |
| Keyboard (KBC) | Input via interrupts |
| Mouse (PS/2) | Input via interrupts |
| RTC | Real-time clock |
| Graphics (VBE) | Video mode setup and sprite rendering |

## Technical details

- Language: C
- Platform: MINIX 3
- Interrupt-driven I/O: each device uses an interrupt subscription, with handlers dispatched from a central loop
- Direct hardware access through port I/O and memory-mapped video memory

## Build and run

Build the lab support libraries first, then compile and run the game from the project directory:

```bash
cd lab2 && make
cd ../lab3 && make
cd ../lab4 && make
cd ../lab5 && make
cd ../proj && make
./proj
```

This project depends on the shared libraries built in `lab2`, `lab3`, `lab4`, and `lab5` before the final `proj` binary can be compiled.

## Authors

- Luís Lima
