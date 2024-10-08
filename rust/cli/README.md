# Magika CLI

This binary crate implements a command-line interface (CLI) to the library crate
[magika](https://crates.io/crates/magika) which provides file type detection with deep-learning.

## Disclaimer

This project is not an official Google project. It is not supported by Google and Google
specifically disclaims all warranties as to its quality, merchantability, or fitness for a
particular purpose.

The `magika` library and this `magika-cli` binary are still unstable (as indicated by the major
version of zero) and new versions might introduce breaking changes (all changes will follow [cargo
semver compatibility](https://doc.rust-lang.org/cargo/reference/semver.html)). In particular,
version 0.1.0-rc.0 ships a new model in comparison to the Python binary and we would love feedback
on [GitHub](https://github.com/google/magika/issues).

## Installation

To install the latest version from crates.io:

```shell
cargo install --locked magika-cli
```

It is also possible to install from the git repository, in which case the version (accessible with
`magika --version`) will be suffixed by `-dev` (e.g. `0.1.0-dev`) to indicate that the binary is the
development version of the version prefix (e.g. `0.1.0` for the previous example).

To install the latest version from the git repository:

```shell
cargo install --locked --git=https://github.com/google/magika.git magika-cli
```

To install from a local clone of the git repository (possibly with custom changes):

```shell
git clone https://github.com/google/magika.git
cd magika
cargo install --locked --path=rust/cli
```
