# Rust - Language Compiler

Rust is designed to provide a balance between low-level control and high-level abstractions, making it a good choice for systems programming tasks such as building numerical simulations, game engines and operating systems.
The Rust toolchain includes a compiler, a package manager, and documentation generator.
The package manager (`cargo`) can also be used like Homebrew to install and manage Rust packages (named "crates") and binaries that have been published to https://crates.io.

## Installation

Rust can be installed via Homebrew, but it is recommended to install it via the official installer, which can be found at https://www.rust-lang.org/tools/install.

On macOS you'll be instructed to run a command similar to the following:

```shell
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

This will download and run a script that will install Rust and `cargo` for you.
In general, be wary of running scripts from the internet like this.

## Usage

To create a new Rust project, run the following command:

```shell
cargo new my_project
```

You can then build the project using the following command:

```shell
cargo build
```

You can then run the project using the following command:

```shell
cargo run
```

If you want to add a new dependency to the project, you can do so using the following command:

```shell
cargo add some_dependency
```

If you want to add a new development dependency to the project, you can do so using the following command:

```shell
cargo add --dev some_dev_dependency
```

To publish the project to `crates.io`, run the following command:

```shell
cargo publish
```

## Return

[Return to the top-level README](./../../README.md)
