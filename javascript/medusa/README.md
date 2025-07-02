# Medusa

## Requirements

- Medusa.js installed in your project.

## Setup

In your moon workspace, create a `.moon/tasks/tag-medusa.yml` file, and paste the following contents:

```yaml
# .moon/tasks/tag-medusa.yml
extends: 'https://raw.githubusercontent.com/moonrepo/moon-configs/master/javascript/medusa/tasks.yml'
```

In your Medusa projects that you'd like to inherit these tasks, add the following tags:

```yaml
# moon.yml
tags: ['medusa']
```
