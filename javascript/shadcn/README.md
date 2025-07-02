# shadcn

## Requirements

- shadcn/ui installed in your project.

## Setup

In your moon workspace, create a `.moon/tasks/tag-shadcn.yml` file, and paste the following contents:

```yaml
# .moon/tasks/tag-shadcn.yml
extends: 'https://raw.githubusercontent.com/moonrepo/moon-configs/master/javascript/shadcn/tasks.yml'
```

In your projects that use shadcn/ui and should inherit these tasks, add the following tags:

```yaml
# moon.yml
tags: ['shadcn']
```
