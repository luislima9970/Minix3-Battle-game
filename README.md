# Minix3 Battle Game

A battle game in C for MINIX 3, built on top of custom device drivers. Made for the **LCOM** (Computer Labs) course unit at FEUP, University of Porto.

## About

All interaction with the hardware goes through drivers written from scratch for the course, with no external graphics or input libraries. The game reads input and draws to the screen using I/O ports and interrupts.

## Drivers

- **Timer**: frame timing and game loop
- **Keyboard**: keyboard input
- **Mouse**: mouse input
- **RTC**: real-time clock
- **Graphics**: video card, drawing sprites and the game screen

## Gameplay

TODO: 2 to 3 sentences on what the game is and how you win.

**Controls**
- TODO: keys / mouse actions

## Screenshots

TODO: add 1 or 2 screenshots in a `docs/` folder and link them here, e.g. `![Game screen](docs/screenshot.png)`.

## Build and run

TODO: the exact commands you use, e.g. `make` and how to start it in MINIX.

## Authors

- Luís Lima
- TODO: teammates, if they agree to be listed

Developed for LCOM, 2025/26.
