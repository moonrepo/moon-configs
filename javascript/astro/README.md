# Astro

## Requirements

- Astro >= v2.

## Setup

In your moon workspace, create a `.moon/tasks/tag-astro.yml` file, and paste the following contents:

```yaml
# .moon/tasks/tag-astro.yml
extends: 'https://raw.githubusercontent.com/moonrepo/moon-configs/master/javascript/astro/tasks.yml'
```

In your Astro projects that you'd like to inherit these tasks, add the following tags:

```yaml
# moon.yml
tags: ['astro']
```
