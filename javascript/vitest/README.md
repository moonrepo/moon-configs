# Vitest

## Requirements

- Vitest >= v0.

## Setup

In your moon workspace, create a `.moon/tasks/tag-vitest.yml` file, and paste the following
contents:

```yaml
# .moon/tasks/tag-vitest.yml
extends: 'https://raw.githubusercontent.com/moonrepo/moon-configs/master/javascript/vitest/tasks.yml'
```

In your Vitest projects that you'd like to inherit these tasks, add the following tags:

```yaml
# moon.yml
tags: ['vitest']
```
