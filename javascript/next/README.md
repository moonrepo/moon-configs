# Next.js

## Requirements

- Next.js >= v13.

## Setup

In your moon workspace, create a `.moon/tasks/tag-next.yml` file, and paste the following contents:

```yaml
# .moon/tasks/tag-next.yml
extends: 'https://raw.githubusercontent.com/moonrepo/moon-configs/master/javascript/next/tasks.yml'
```

In your Next.js projects that you'd like to inherit these tasks, add the following tags:

```yaml
# moon.yml
tags: ['next']
```
