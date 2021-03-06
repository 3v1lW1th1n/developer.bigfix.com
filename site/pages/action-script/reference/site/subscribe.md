---
title: subscribe
---

This command subscribes the client to the site identified in the masthead file.

Version | Platforms
--- | ---
8.0.584.0 | AIX, HP-UX, Mac, Red Hat, SUSE, Solaris, Windows
8.1.535.0 | Debian, Ubunt

## Syntax

    subscribe <masthead-file-name>

## Examples

Subscribe the client computer to the site with the masthead `cool-site.fxm`.

```actionscript
subscribe "__Download\cool-site.fxm"
```

## Notes

The command should not be used directly. Instead, use the BigFix Console to
manage site subscriptions.

This command returns an error unless it is executed in the master action site.
