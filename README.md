# moon configs

This is a collection of community driven and maintained moon task configurations for popular
programming languages, frameworks, libraries, and more.

## Usage

### Modifying inherited tasks

The config presets work great as a standard solution, but they aren't designed to accomdate all use
cases. For those outliers, you can modify the inherited tasks, or simply ignore them.

```yaml
# moon.yml
tags: ['configs', 'to', 'inherit']

tasks:
  build:
    args: '--pass --additional --args'

workspace:
  inheritedTasks:
    exclude: ['task-name']
```

> Learn more about [task merging](https://moonrepo.dev/docs/concepts/task#merge-strategies) and
> [task inclusion/exclusion](https://moonrepo.dev/docs/config/project#inheritedtasks).

### Extending file groups

All config presets provide an `other` file group, that all tasks in the preset inherit, allowing you
to further customize the inputs.

```yaml
# moon.yml
tags: ['configs', 'to', 'inherit']

fileGroups:
  other:
    - 'other/files/**/*'
```

> Learn more about [file groups](https://moonrepo.dev/docs/concepts/file-group).
