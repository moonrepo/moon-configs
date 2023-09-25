# Vite

## Requirements

- Vite >= v3.

## Setup

In your moon workspace, create a `.moon/tasks/tag-vite.yml` file, and paste the following contents:

```yaml
# .moon/tasks/tag-vite.yml
extends: 'https://raw.githubusercontent.com/moonrepo/moon-configs/master/javascript/vite/tasks.yml'
```

In your Vite projects that you'd like to inherit these tasks, add the following tags:

```yaml
# moon.yml
tags: ['vite']
```
