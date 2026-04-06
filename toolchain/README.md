# SIC/XE Toolchain

This directory contains an all-in-one SIC(/XE) toolchain, including a compiler from Go to SIC assembly, an assembler, linker, and simulator for both SIC and SIC/XE.

The toolchain is written fully in Go stdlib-only go, making it extremely portable.
All important functionality is exposed in separate packages, making it easy to reuse in other Go projects.

## Feature list

### Compiler

- [ ] Lexer
- [ ] Parser
- [ ] Semantic analysis
- [ ] IR generation
- [ ] IR optimizations
- [ ] Liveness analysis
- [ ] Register allocation
- [ ] Code generation

### Assembler

- [ ] Parser for assembly code
- [ ] Symbol resolver
- [ ] Object code generator
- [ ] Directives (`START`, `END`, `ORG`, `EQU`)
- [ ] Base directives (`BASE`, `NOBASE`)

### Linker

- [ ] Link multiple object files into one
- [ ] Multiple control sections
- [ ] Adjustable linker settings
- [ ] Inspecting and reordering control sections/symbols

### Simulator

The default user interface for the simulator is a CLI (prints the registers and memory after finishing).

- [ ] Registers
- [ ] Memory
- [ ] I/O devices
- [ ] Addressing modes
- [ ] Integer, floating point, and bitwise arithmetic
- [ ] Jumps
- [ ] Load and store
- [ ] Control instructions
- [ ] Object code parser
- [ ] All instruction sets
- [ ] Detect halt instruction
- [ ] Interrupts

Potential extras (outside of SIC/XE spec):
- [ ] Multi-processor support
- [ ] Adjustable-speed timer for executing instructions in sequence
- [ ] Automatic running modes (start, stop, step)
- [ ] Keyboard input (stdin)
- [ ] Breakpoints
- [ ] TUI mode (needed for step-by-step execution, seeing memory and registers change, etc.)
- [ ] GUI mode (needed for showing display output)
- [ ] Step-back in debugger (revert last instruction)
