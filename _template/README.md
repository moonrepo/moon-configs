# <tool>

## Requirements

- ???

## Setup

In your moon workspace, create a `.moon/tasks/tag-<tag>.yml` file, and paste the following contents:

```yaml
# .moon/tasks/tag-<tag>.yml
extends: 'https://raw.githubusercontent.com/moonrepo/moon-configs/master/<tool>/tasks.yml'
```

In your <tool> projects that you'd like to inherit these tasks, add the following tags:

```yaml
# moon.yml
tags: ['<tag>']
```
