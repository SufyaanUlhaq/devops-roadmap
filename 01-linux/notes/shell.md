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
# Intro to the SHELL

## Key Concepts
- The Shell is a User Interface which provides access to the OS's services:
    Layers between user and the core of the OS to translate commands into actions
    e.g. Hierarchy: User -> Shell -> Kernel -> Hardware
- Commands ran in the shell are programs developed by developers which are then compiled in binary format for the computer to read. The terminal finds its contents in the Path Environment variable.

## Commands
`ls -la` - Terminal finds the program that has the command name and looks into its contents to run it

## Examples
`ls -la` - listing all contents within the current directory
`usr/local/bin` - bin means binary, the Path Environment variable tells the shell
                where to look to retrieve the contents of the program in order
                to run the command
`zsh, fish, ksh, csh, bash`
`cat /etc/shells` - to read all shells available on the device's OS

## What I learned
Commands are not only keywords, rather they are programs in the shell which are
programmed by developers and compiled into binary for the computer to execute 
to output or run the contents of the program for the user. The Path Environment variable
holds these programs in binaries - it tells the shell where to search for the command.
