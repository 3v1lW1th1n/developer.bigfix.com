---
title: delete
---

This command deletes a file. Any script with the `delete` command will terminate
if the file exists but cannot be deleted. This can happen due to write
protection or an attempt to delete from a CD-ROM, for instance. If the file does
not exist at all, however, the action script will continue to execute.

## Syntax

    delete <filename>

## Examples

Delete the `module.dll` file.

```actionscript
delete "c:\program files\bigsoftware\module.dll"
```

Delete the `win.com` file.

```actionscript
delete "{name of drive of windows folder}\win.com"
```

## Notes

It’s good practice to enclose file paths in quotes to preserve spaces. Without
quotes, the file system will not be able to access files with spaces in the path
or file name.
