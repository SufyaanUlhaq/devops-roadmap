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
# Sudo

## Key Concepts
- Sudo is 'Super User Do' which allows a permitted user to makes changes on files
with root user access.
- Creating a new user in the system

## Commands
`sudo`
`sudo su`
`sudo useradd`
`sudo passwd`
`su -`
`sudo usermod -aG sudo`
`sudo deluser`
`sudo groupadd`
`sudo gpasswd -d`
`sudo groupdel`
`groups`

## Examples
`sudo vim hello.md`
`sudo su` - enters into the root with full access as a root user without the need of entering a password
`sudo su rm -rf /` - removes the entire Linux, wiping the OS.
`sudo user add newuser` - creates a new user `newuser`
`sudo passwd newuser` - prompts user to create a password for `newuser`
`su - newuser` - prompts user to enter the password to access the `newuser` user. The word `su` means 'substitute user'
`sudo usermod -aG sudo newuser` - type this in the main user's terminal to grant sudo permissions to the `newuser` user
`sudo deluser newuser sudo` - revoke the sudo permissions from `newuser` in the main user's terminal
`sudo groupadd animals` - creates a new group within `/etc/group`
`sudo usermod -aG animals newuser` - adds `newuser` to the `/etc/group/animals` group
`sudo gpasswd -d newuser animals` - removes `newuser` from the `animals` group
`sudo groupdel animals` - removes the `animals` group from `/etc/group`
`groups` - checks which groups the user is in
`sudo groupadd admin3 && groupadd admin4` - creates 2 groups simultaneously in `/etc/group`
`sudo usermod -aG admin3 newuser` - adds `newuser` to `admin3` group
`sudo usermod -aG admin4 newuser` - adds `newuser` to `admin4` group
`sudo gpasswd -d newuser admin3` - removes `newuser` from `admin3` group

## What I Learned
- To be able to edit configuration files in the root folder `/`, using `sudo su` is effective as it gives permitted users control access of a root user.
- Users can be created using the `sudo useradd newuser` `sudo userpasswd newuser` commands and be granted permissions such as `sudo usermod -aG sudo newuser`. To access this newuser account, type `su - newuser`. And to revoke its sudo permissions, type `sudo deluser newuser sudo`.
- Ability to create user groups in `/etc/group` and add users to them as well as removing them from groups and removing groups using `sudo gpasswd -d newuser group` & `sudo groupdel group`.
