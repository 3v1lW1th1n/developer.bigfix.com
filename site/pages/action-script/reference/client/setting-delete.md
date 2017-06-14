---
title: setting delete
---

This command deletes a named setting variable on the client computer. It
includes a timestamp which will be compared to the timestamp on the original
setting. If the delete date is later than the setting date, the setting will be
deleted. Otherwise, the delete command will be ignored.

The command is available on all platforms starting from the first versions of IBM BigFix.

## Syntax

    setting delete "<name>" on "<date>" for client
    setting delete "<name>" on "<date>" for current site
    setting delete "<name>" on "<date>" for site "<site_url>" 

## Examples

Deletes the `name` variable on the client machine.

```actionscript
setting delete "name" on "{now}" for client
```
