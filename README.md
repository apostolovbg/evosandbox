# EvoSandbox

EvoSandbox is an experimental world simulation written in [Rust](https://www.rust-lang.org/) using the [Bevy](https://bevyengine.org/) game engine. The goal is to model a self-contained ecosystem where programmable organisms interact in real time. Each creature is powered by a DNA-like data structure that defines its behaviour, appearance and interaction with the environment. GPU-based rendering provides smooth visuals across platforms while letting the simulation run at high speeds.

## Project Goals

- **Evolving world** driven by DNA-based logic for each cell or entity.
- **Real-time simulation** of resources, movement and simple physics.
- **Cross-platform support** targeting Windows, macOS and Linux using Bevy's abstraction layers.
- **GPU accelerated rendering** to handle potentially thousands of agents efficiently.
- Extensible architecture for experimenting with emergent behaviour and new mechanics.

## Planned Features

1. **DNA-driven cells** with mutation and reproduction rules.
2. **Physics integration** for movement and collision detection.
3. **GPU rendering** using Bevy's wgpu backend.
4. **Resource management** such as food, energy and environmental factors.
5. **Cross-platform executables** for desktop OSes (Windows, macOS, Linux).
6. **Plugin system** to add new creature types and behaviours.

## Building and Running

This project requires a recent stable version of Rust. Install dependencies for Bevy such as ALSA on Linux for audio support.

```bash
# Compile in debug mode
cargo build

# Or run the game directly
cargo run
```

Building on Windows and macOS may require additional system packages for windowing and audio as described in the [Bevy setup guide](https://bevyengine.org/learn/book/getting-started/). On Linux, development files for `alsa` and other graphics libraries must be available.

## License

EvoSandbox is distributed under the terms of the [GNU General Public License v3.0](LICENSE). You are free to use, study and modify the code, but derivative works must remain GPL compatible.

## Contributing

Contributions are welcome! Please open an issue to discuss ideas before submitting pull requests. By contributing you agree that your code will be licensed under GPLv3. Follow Rust formatting conventions (`cargo fmt`) and ensure builds succeed before creating a PR.
