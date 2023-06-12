# Rust tasks

Choose the config appropriate for your Rust repository structure.

- `tasks-workspace.yml`
  - Using Cargo workspaces and the `moon.yml` is at the workspace root, relative to the `Cargo.lock`
    file.
- `tasks-project.yml`
  - ???

## Setup

In your moon workspace, create a `.moon/tasks/tag-rust.yml` file, and paste the following contents
(with the file chosen above):

```yaml
# .moon/tasks/tag-rust.yml
extends: 'https://raw.githubusercontent.com/moonrepo/moon-configs/master/rust/<config>.yml'
```

In your Rust projects that you'd like to inherit these tasks, add the following tags:

```yaml
# moon.yml
tags: ['react']
```
