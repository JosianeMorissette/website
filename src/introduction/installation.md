# Installation
## Cornucopia
You can use Cornucopia as a [CLI](/usage/cli.html) or a library [API](/usage/api.html), depending on your needs. Make sure to check out these sections later for more info.

#### CLI
To install the latest released version of the CLI, use `cargo install`:
```
cargo install cornucopia
```
#### API
Import `cornucopia` in your project's `Cargo.toml`:
```toml
cornucopia = "..." # choose the desired version
```

## Container manager
When running in managed mode, Cornucopia spawns a postgres container that acts as an ephemeral database. Therefore, you need a working `docker` or `podman` command available on your system.

#### Docker
To use Cornucopia with `docker` on Linux, non-sudo users need to be in the docker group. For a step-by-step guide, please read the official Docker [installation](https://docs.docker.com/get-docker/) and [post-installation](https://docs.docker.com/engine/install/linux-postinstall/) docs.

```admonish note
You don't need a container manager if you manage the database yourself.
```
