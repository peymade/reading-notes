# Module 2 Reading

## Choosing a Text Editor

Selecting a text editor is an important step for developers. It is a personal choice that depends on an individual’s workflow, and what is important to them in their coding process. 

There are multiple types of text editors. 

* Plain Text Editors (Notepad++, Atom, VS Code)
* Word Processors (Google Docs, Word)

Make sure that you are creating code in a “plain text editor.” This means, not something like Word Processor, that lets one bold or italicize words. Plain text has no formatting options. It can, however, have code competion and syntax highlighting. 

## Terminal

### The Command Line
A command line is a responsive text interface. It will give a user prompts, and the user will be able to respond with commands.

### Shortcuts
-	Command + K = clear the terminal
-	Use the up arrow to repeat commands from previous lines
-	Use the tab key to have the terminal auto-complete the line

### Basic Commands
* ```pwd``` = print working directory
* ```cd ___``` = change directory
* ```cd ..``` = move up to parent directory
* ```cd\ (enter, enter)``` = moves to root directory
* ```ls``` = display the names of the files in current directory
* ```ls -a``` = displays hidden files and directories as well as shown ones
* ```mkdir ___``` = make directory
* ```/``` = root directory, within which all other directories exist, branching down like a tree
* `cp` = making a copy of a file and moving it somewhere `cp ~/Current Location/File ~/New location`

### Paths

Two types- **absolute & relative**

**Absolute** -> The location of a file or directory in relation to the root 
	*Example*: /home/documents/game
An absolute path with yield the same results regardless of current location

**Relative** -> The location of a file in relation to where one currently is
	*Example*: being in/home/documents and running `ls game`

### Further Notes and Examples

```~``` This can be written in place of the text that makes up the “home” directory    
*Example*: /users/Peyton/Documents = ~/Documents

```.``` By using “ls .” one can see the contents of the current directory. Make sure to add a space before the dot. 

```..``` Two dots will reference the parent directory.  
*Example*: The command `cd ..` will move one back up to the previous directory, and the command `ls ../../` will list the contents of the directory that is up, 2 hierarchical steps. 

* ```ls ~/Documents```
* ```ls ./Documents```
* ```ls /home/users/peyton/Documents```

These all three will yield the same results. The first and third are absolute paths, and the middle one is relative, since the dot represents the pwd.

```ls ../../```

This command would list the items in a directory two above the current one. It is a relative path. 

```ls /``` 

This command lists the items in the root directory, meaning it is an absolute path. 

### Files

* The text at the end of a file denotes what kind it is.
*Example*: exe / txt / jpg 
* The command `file [path]` can be used to see what type of file something is.  
* Linux will not recognize files names with spaces. Use ‘’ quotes or a \ backslash before the space



