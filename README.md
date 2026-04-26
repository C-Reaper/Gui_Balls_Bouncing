# Project README

## Overview
The project "Balls Bouncing" is a simple 2D application that simulates bouncing balls within a window. The application uses a custom windowing system and handles user input for panning and zooming.

## Features
- Simulated bouncing balls within a window.
- User interaction to pan and zoom the view using keyboard shortcuts.
- Real-time rendering of the scene.

## Project Structure
```
Balls_Bouncing/
├── build/              # .exe files produced by Main.c
├── src/
│   ├── Main.c          # Entry point
│   └── *.h             # Standalone header-based C-files, without *.c files that implement it
├── Makefile.linux      # Linux Build configuration
├── Makefile.windows    # Windows Build configuration
├── Makefile.wine       # Wine Build configuration for cross-compiling to Windows on Linux
└── README.md           # This file
```

### Prerequisites
- C/C++ Compiler and Debugger (GCC)
- Make utility
- Standard development tools
- X11 library (for Linux)

## Build & Run
### Build Process
To build the project for Linux:
```bash
cd Balls_Bouncing
make -f Makefile.linux all
```

For Windows (using MinGW):
```bash
cd Balls_Bouncing
make -f Makefile.windows all
```

For Wine cross-compilation to Windows on Linux:
```bash
cd Balls_Bouncing
make -f Makefile.wine all
```

### Execution
To run the application after building, use:
```bash
make -f Makefile.(os) exe
```
Replace `(os)` with `linux`, `windows`, or `wine` depending on your target platform.