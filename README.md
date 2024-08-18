# rust-os
Basic OS written in Rust, using https://os.phil-opp.com as a guide.

---
### Requirements
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
  - [x] VGA TextMmode
  - [x] Testing
* Interrupts
  - [x] CPU Exceptions
  - [ ] Double Faults
  - [ ] Hardware Interrupts
* Memory Management
  - [ ] Intro to Paging
  - [ ] Paging Implementation
  - [ ] Heap Allocation
  - [ ] Allocator Designs
* Multitasking
  - [ ] Async/Await
