# [Ruffle](https://ruffle.rs)

Ruffle is an Adobe Flash Player emulator written in the Rust programming language.

## Building

Just `make` and Ruffle will be built and installed.

## Updating Ruffle

In order to update Ruffle to another version, replace `commit` and `tag` in the descriptor.
You can optionally comment out the tag.

Remember to regenerate sources afterwards! (See below.)

There's no need to commit the update, as it's done automatically.
However, if you plan on doing so, remember to update `patches/release.patch`.

## Regenerating Sources

In order to regenerate `cargo-sources.json` run the following command
replacing `<commit>` with the commit hash from upstream.

_Note: this does not update Ruffle! Only its dependencies!_

```shell
make regenerate-sources RUFFLE_COMMIT=<commit>
```
