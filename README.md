https://github.com/esp-rs/esp-idf-template#prerequisites

# Quickstart
- [Install Rust](https://www.rust-lang.org/tools/install).

- rustup toolchain install nightly --component rust-src

- cargo install ldproxy
- cargo install espup
- cargo install espflash
- cargo install cargo-espflash # Optional

- Install the compilation target for your MCU. Eg run `rustup target add riscv32imc-esp-espidf`.
- Install flash and debug tools: `cargo install flip-link`, `cargo install probe-rs --features cli`.
- Connect your device. Run `cargo run --release` to compile and flash.

If, on Windows, you run into a path length error, open `regedit`, and set 
`Computer\HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\FileSystem\LongPathsEnabled` to `1`, then restart the PC.
