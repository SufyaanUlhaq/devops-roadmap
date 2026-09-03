# Notes

Add your notes here as you progress through this module.

## Template

When creating a new note, you can use this structure:

```markdown
# Topic Name

## Key Concepts

- Point 1
- Point 2

## Commands

`command` - what it does

## Examples

(code examples)

## What I Learned

(your own summary)
```

## Your Notes

- [ ] Add your first note
# File Permissions

## Key Concepts
- File permissions on a Linux system give control access to users, groups and other entities
- File permissions are crucial when configuring root files
- the Binary/Octal/String representation of file permissions are based on:
    - Directory|File|Link/User/Group/Others
    - the Str representation for a directory that's public to anyone would be `rwxrwxrwx`
    - `rwx` = read-write-execute
    - the Octal representation would be `777`.
    - r = 4, w = 2, x = 1. (4 + 2 + 1 = 7)
- Creating a shell script to change the file permissions of the file using `#!/bin/bash`    at the beginning of the script and adding the `chmod` command statement inside file

## Commands
`chmod`

## Examples
`chmod u+x,g+r,o-w hello.txt` - grants file permissions to hello.txt where the user will now have execute permissions, the group will have read permissions, and others will no longer have write permissions.
`chmod 751 hello.txt` - grants file permissions to hello.txt where User will have all rwx permissions, Group will have rx permissions, and others will have x permissions.
`chmod +x hello.txt` - grants execute permissions to User/Group/Others for `hello.txt`
`./set_permissions.sh` - runs a shell script to set permissions for a file. Ensure the file permissions for this are set to execute for the User.

## What I Learned
- A Linux system requires file permissions on directories and files to ensure Users, Groups and Others can access them appropriately. For example, giving full Read-Write-Execute access to a User.
- The String/Binary/Octal representation of file permissions are crucial to understand and memorise as it is easier to give user permissions with the command `chmod 751 hi.txt` rather than `chmod u+rwx,g+rx,o+x hi.txt`
- Shell Scripting is very important as it can be used to run in the terminal to grant file permissions to specific files when ran. It's important to understand to give execute permissions to the shell script so it can be ran via: `./shell_script.sh`
