# Strapi

## Requirements

- Strapi >= v5.

## Setup

In your moon workspace, create a `.moon/tasks/tag-strapi.yml` file, and paste the following contents:

```yaml
# .moon/tasks/tag-strapi.yml
extends: 'https://raw.githubusercontent.com/moonrepo/moon-configs/master/javascript/strapi/tasks.yml'
```

In your Strapi projects that you'd like to inherit these tasks, add the following tags:

```yaml
# moon.yml
tags: ['strapi']
```
