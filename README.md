![Build Status](https://img.shields.io/github/actions/workflow/status/matrix-org/matrix-rust-sdk/ci.yml?style=flat-square)
[![codecov](https://img.shields.io/codecov/c/github/matrix-org/matrix-rust-sdk/main.svg?style=flat-square)](https://codecov.io/gh/matrix-org/matrix-rust-sdk)
[![License](https://img.shields.io/badge/License-Apache%202.0-yellowgreen.svg?style=flat-square)](https://opensource.org/licenses/Apache-2.0)
[![#matrix-rust-sdk](https://img.shields.io/badge/matrix-%23matrix--rust--sdk-blue?style=flat-square)](https://matrix.to/#/#matrix-rust-sdk:matrix.org)
[![Docs - Main](https://img.shields.io/badge/docs-main-blue.svg?style=flat-square)](https://matrix-org.github.io/matrix-rust-sdk/matrix_sdk/)
[![Docs - Stable](https://img.shields.io/crates/v/matrix-sdk?color=blue&label=docs&style=flat-square)](https://docs.rs/matrix-sdk)

# matrix-rust-sdk

**matrix-rust-sdk** is an implementation of a [Matrix][] client-server library in [Rust][].

[Matrix]: https://matrix.org/
[Rust]: https://www.rust-lang.org/

## Project structure

The rust-sdk consists of multiple crates that can be picked at your convenience:

- **matrix-sdk** - High level client library, with batteries included, you're most likely
  interested in this.
- **matrix-sdk-base** - No (network) IO client state machine that can be used to embed a
  Matrix client in your project or build a full fledged network enabled client
  lib on top of it.
- **matrix-sdk-crypto** - No (network) IO encryption state machine that can be
  used to add Matrix E2EE support to your client or client library.

## Status

The library is considered production ready and backs multiple client implementations such as Element X [[1]](https://github.com/element-hq/element-x-ios) [[2]](https://github.com/element-hq/element-x-android) and [Fractal](https://gitlab.gnome.org/World/fractal). Client developers should feel confident to build upon it.

Development of the SDK has been primarily sponsored by Element though accepts contributions from all.

## Bindings

Some crates of the **matrix-rust-sdk** can be embedded inside other
environments, like Swift, Kotlin, JavaScript, Node.js etc. Please,
explore the [`bindings/`](./bindings/) directory to learn more.

## License

[Apache-2.0](https://www.apache.org/licenses/LICENSE-2.0)
