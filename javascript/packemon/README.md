# Packemon

## Requirements

- Packemon >= v3.

## Setup

In your moon workspace, create a `.moon/tasks/tag-packemon.yml` file, and paste the following
contents:

```yaml
# .moon/tasks/tag-packemon.yml
extends: 'https://raw.githubusercontent.com/moonrepo/moon-configs/master/javascript/packemon/tasks.yml'
```

In your Packemon projects that you'd like to inherit these tasks, add the following tags:

```yaml
# moon.yml
tags: ['packemon']
```

### Setting the output directory

Depending on your Packemon configuration, you'll need to change the task outputs per project like
so:

```yaml
# moon.yml
tags: ['packemon']

tasks:
  build:
    outputs:
      - 'cjs'
  build-release:
    outputs:
      - 'esm'
```
