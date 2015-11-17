---
title: action requires restart
---

This command will place the action in a *Pending Restart* state until the
computer is restarted.

If the optional `name` is specified, then the [pending
restart](/relevance/reference/string.html#pending-restart-string-boolean)
inspector will report that `name` requires a restart.

## Syntax

    action requires restart [name]

## Examples

Require a restart before the action is reported as completed.

```actionscript
run patch.exe
action requires restart "my-awesome-patch"
```

After running this, the action will be in a *Pending Restart* state and the
following relevance will return `True`:

```relevance
pending restart "my-awesome-patch"
```
