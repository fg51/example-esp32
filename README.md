# example-esp32 (C3)
esp32

# 1. setup

## ldproxy
ldproxy crate is required when building applications using the Rust standard libary, std.

```sh
cargo install ldproxy
```

## target RISC-V chips

```sh
$ rustup toolchain install nightly --component rust-src
$ rustup target add riscv32imc-unknown-none-elf
```

## espup
espup is a tool for installing and maintaining the required ecosystem to develop applications in Rust for Espressif SoC's.


```sh
$ cargo install espup
$ espup install
```


## tools

```sh
$ cargo install cargo-espflash cargo-espmonitor
```

## template

```sh
$ cargo install cargo-generate
```

### std

```sh
$ cargo generate --git https://github.com/esp-rs/esp-idf-template
```

### no_std

```sh
$ cargo generate --git https://github.com/esp-rs/esp-template
```

when esp-alloc is true, cause the build error.
