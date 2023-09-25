# moon configs

This is a collection of community driven and maintained moon task configurations for popular
programming languages, frameworks, libraries, and more.

## Usage

This repository provides task configuration presets, which can be inherited in your moon projects
through our
[configuration sharing and extending feature](https://moonrepo.dev/docs/guides/sharing-config).

Browse the repository for the configuration you would like to use, and refer to the setup
instructions in the associated `README`.

### Modifying inherited tasks

The config presets work great as a standard solution, but they aren't designed to accomodate all use
cases. For those outliers, you can modify the inherited tasks, or simply ignore them.

```yaml
# moon.yml
tags: ['configs', 'to', 'inherit']

# Merge with additional args
tasks:
  build:
    args: '--pass --additional --args'

# Ignore the task entirely
workspace:
  inheritedTasks:
    exclude: ['task-name']
```

> Learn more about [task merging](https://moonrepo.dev/docs/concepts/task#merge-strategies) and
> [task inclusion/exclusion](https://moonrepo.dev/docs/config/project#inheritedtasks).

### Extending file groups

All config presets provide `sources` and `tests` file groups, that all tasks in the preset inherit,
allowing you to further customize the inputs.

```yaml
# moon.yml
tags: ['configs', 'to', 'inherit']

fileGroups:
  sources:
    - 'other/files/**/*'
```

> Learn more about [file groups](https://moonrepo.dev/docs/concepts/file-group).
