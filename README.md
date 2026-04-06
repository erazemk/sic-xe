# Simplified Instructional Computer

This repository contains various educational resources for the Simplified Instructional Computer (SIC) and its eXtended Edition (SIC/XE).
The aim of the project is to help students learn about the SIC architecture and consequently systems programming in general.

## Project structure

- [Website](https://sic.erazemk.com): The main resource is the website [sic.erazemk.com](https://sic.erazemk.com).
It contains extensive documentation about the architecture, including its history, design, addressing modes, registers, assembly sintax etc. The website is deployed from the [docs](docs/) directory in the project.
- [Toolchain](toolchain/): An example implementation of an all-in-one compiler, assembler, linker, and simulator for SIC and SIC/XE, written in Go. This project is written as part of my master's thesis at the Faculty of Computer and Information Science, University of Ljubljana.
- [Examples](examples/): A collection of example Go, assembly and object code programs for SIC and SIC/XE. These can be run directly in the example toolchain at whichever step you want (compiler for the Go code, assembler for the assembly, and simulator for the object code). They also contain detailed comments of what each example does.

The project is still a work in progress, and there are a few potential projects that might potentially join the above ones:
- VSCode extension: A Visual Studio Code extension for syntax highlighting, code completion, etc.
- FPGA implementation: An implementation of SIC/XE on a RealDigital Blackboard FPGA board, with support for interacting with the Blackboard's peripherals (LEDs, HDMI output, etc.) from SIC assembly code.

## License

The code and documentation in this repository is licensed under the [GNU AGPLv3 license](LICENSE).
