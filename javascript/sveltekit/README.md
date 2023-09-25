# SvelteKit

## Requirements

- SvelteKit >= v1.

## Setup

In your moon workspace, create a `.moon/tasks/tag-sveltekit.yml` file, and paste the following
contents:

```yaml
# .moon/tasks/tag-sveltekit.yml
extends: 'https://raw.githubusercontent.com/moonrepo/moon-configs/master/javascript/sveltekit/tasks.yml'
```

In your SvelteKit projects that you'd like to inherit these tasks, add the following tags:

```yaml
# moon.yml
tags: ['sveltekit']
```
