# Rust

Choose the config appropriate for your Rust repository structure.

- `tasks-workspace.yml`
  - Using Cargo workspaces and the `moon.yml` is at the workspace root, relative to the `Cargo.lock`
    file.
- `tasks-project.yml`
  - Using Cargo workspaces and the `moon.yml` is within each crate, relative to a nested
    `Cargo.toml`.
  - Not using Cargo workspaces (is a single Cargo crate) and `moon.yml` is relative to the
    `Cargo.lock` file.

## Requirements

- Uses [`nextest`](https://nexte.st/) for tests.
- For workspaces, crates are organized in a `crates/` directory.
- Config files (`.cargo`, `rust-toolchain.toml`, etc) are located at the repository root.

## Setup

In your moon workspace, create a `.moon/tasks/tag-rust.yml` file, and paste the following contents
(with the file chosen above):

```yaml
# .moon/tasks/tag-rust.yml
extends: 'https://raw.githubusercontent.com/moonrepo/moon-configs/master/rust/<config>'
```

In your Rust projects that you'd like to inherit these tasks, add the following tags:

```yaml
# moon.yml
tags: ['rust']
```
