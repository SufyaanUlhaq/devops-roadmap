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

# [Terminal & Commands] 

## Key Concepts

- The Terminal grants access to a device's operating system
- Commands are given to the Terminal as user input to stdout a result
- Commands are Textual instructions given to the Terminal
- Commands can be used with options and arguments to give them more behaviour
- Commands have manual instructions and theyre case sensitive

## Commands

`ls` - lists all directories and files within a directory
     - also comes with options such as `-a` and `-la` where `-a` lists all
       files and directories within the current directory & `-la` lists
       all files and directories WITH permissions for each within the current directory
`pwd` - print working directory
`cd` - change directory
`mkdir` - make a new directory
`rmdir` - remove a directory (IF and ONLY IF the directory is EMPTY)
`touch` - to create a file
`rm` - to remove a file
`tab` - not literally the word 'tab'. Tab key autofills the file/directory
`cat` - can read files and create files but primarily use `touch` to create files
`whoami` - outputs the user of the operating system onto the terminal
`ctrl L` - clears terminal screen
`clear` - clears terminal screen
`>` - redirect operator outputs from content e.g. a string into a file
`>>` - append operator to add additional content to a file without removing
        the current contents.
`echo` - prints contents

## Examples

`ls` ./foo/zoo
`ls -la` ./foo/zoo
`pwd`
`cd` ~
`mkdir` parent
`rmdir` parent
`touch` hello-world.txt
`rm` hello-world.txt
`cat` hello-world.txt 
`whoami` - returns 'sufyaan'
`cd /` - access the root directory
`echo "Hello World" > world.txt` - inputs "Hello World" into a file
`echo "Hello World2" >> world.txt` - appends "Hello World2" into that same file

## What I learned

I learnt that commands are instructions given to the terminal to output a result
the developer is looking for. For example, when creating a directory within 
a current directory, the command to do this would be `mkdir parent/child`. 

I also learnt that the Terminal gives access to a device's software and applications
IF the correct permissions are set for a certain user/group. 
