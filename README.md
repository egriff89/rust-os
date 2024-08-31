# rust-os
Basic OS written in Rust, using https://os.phil-opp.com as a guide.

---
### Requirements
- [QEMU](https://www.qemu.org/download/)
- Rust nightly build
- `thumbv7em-none-eabihf` target 
- `bootimage` crate for building the kernel
- `llvm-tools` and `rust-src` components to recompile `core`

```shell
rustup toolchain install nightly
rustup target add thumbv7em-none-eabihf
rustup component add llvm-tools rust-src
cargo install bootimage
```

---
### Progress
* Bare Bones
  - [x] Freestanding Rust Binary
  - [x] Minimal Rust Kernel
  - [x] VGA Text Mode
  - [x] Testing
* Interrupts
  - [x] CPU Exceptions
  - [x] Double Faults
  - [x] Hardware Interrupts
* Memory Management
  - [x] Intro to Paging
  - [x] Paging Implementation
  - [x] Heap Allocation
  - [x] Allocator Designs
* Multitasking
  - [ ] Async/Await
