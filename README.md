# [Ruffle](https://ruffle.rs)

Ruffle is an Adobe Flash Player emulator written in the Rust programming language.

## Building

Just `make` and Ruffle will be built and installed.

## Regenerating Sources

In order to regenerate `cargo-sources.json` run the following command
replacing `<commit>` with the commit hash from upstream.

```shell
make regenerate-sources RUFFLE_COMMIT=<commit>
```
