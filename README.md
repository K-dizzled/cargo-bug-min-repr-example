Taken the [simplest cargo project](https://github.com/K-dizzled/cargo-bug-min-repr-example) with at least one dependency, if you:

1. Build it using `cargo build --target aarch64-apple-ios-sim`
2. Make `cargo check`
3. Build it again using `cargo build --target aarch64-apple-ios-sim`

Cargo will recompile all the dependencies even tho nothing has changed.

Versions:

* cargo 1.66.0