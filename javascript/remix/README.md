# Remix

## Requirements

- Remix >= v1.16.

## Setup

In your moon workspace, create a `.moon/tasks/tag-remix.yml` file, and paste the following contents:

```yaml
# .moon/tasks/tag-remix.yml
extends: 'https://raw.githubusercontent.com/moonrepo/moon-configs/master/javascript/remix/tasks.yml'
```

In your Remix projects that you'd like to inherit these tasks, add the following tags:

```yaml
# moon.yml
tags: ['remix']
```
