# BlogOS

A minimal Rust kernel. This repo is based on the [Writing an OS in Rust](https://os.phil-opp.com) series by [Philipp Oppermann](https://github.com/phil-opp).

## Overview

BlogOS is a simple operating system kernel that runs on bare-metal. It demonstrates key concepts like:
- Creatin a freestanding Rust binary
- Bootstrapping a mininmal kernel for x86_64
- Basic VGA text output
- Except and interrupt handling
- Memory management concepts
- Cooperative task management

## Prerequisites

To build and run BlogOS, you'll need a Rust nightly toolchain, QEMU, cargo-xbuild and a bootimage tool.

The following commands should set everything up:
```bash
rustup default nightly
cargo install bootimage
cargo install cargo-xbuild
```

## Building

Clone the repo:
```bash
git clone https://github.com/HDauven/BlogOS.git
```

Build and run the project:
```bash
cargo run
```

This should open a QEMU window, running the kernel.

## License

This project is licensed under the Apache License, Version 2.0. See the [LICENSE](./LICENSE) file for details.
