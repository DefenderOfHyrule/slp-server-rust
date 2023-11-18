# slp-server-rust

[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/spacemeowx2/slp-server-rust)

[switch-lan-play](https://github.com/DefenderOfHyrule/switch-lan-play-aarch64) Server written in Rust.

## Usage

Goto release page: https://github.com/spacemeowx2/slp-server-rust/releases, grab the latest release, and run it.

## Build from source

1. Install [`rustup`](https://rustup.rs/) first, and make sure using the latest stable rust version.

2. `cd` to cloned repository

3. Run `cargo update`:

```
cargo update
```

4. Replace `use serde::export::PhantomData` with `use core::marker::PhantomData`:

In
``` 
~/.cargo/registry/src/index.crates.io-6f17d22bba15001f/async-graphql-1.18.2/src/subscription/simple_broker.rs
```
And
```
~/.cargo/registry/src/index.crates.io-6f17d22bba15001f/async-graphql-1.18.2/src/guard.rs
```

5. Compiling slp-server-rust:

```
cargo run --release
```

6. Done, the binary will be located in /target/release.
