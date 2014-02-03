TerminalCommands
================

Just some useful stuff you can do in the terminal

##### Table of Contents  
* [Useful keyboard shortcuts](#Keyboard shortcuts)
* [chmod](#chmod)  
* [curl](#curl)
* [touch](#touch)


## Keyboard shortcuts
```
CTRL-a     Sets cursor to start of line
CTRL-k     Clears everything after cursor
CTRL-u     Clears everything before and after cursor
CTRL-l     'Resets' the terminal clearing all output
```
# Terminal Commands

## chmod
Changes the attributes of a file.  [chmod on Wikipedia](http://en.wikipedia.org/wiki/Chmod) 

#####Most useful arguments

    -R         Recursively sets the attributes in all subdirectories as well
#####Example usage
```Shell
chmod 777 examplefile.file
    Lets all users and groups read and write to the file 'examplefile.file'
```
__________
## curl
Downloads file at given URL and writes it to the command line.  [curl on Wikipedia](http://en.wikipedia.org/wiki/CURL)

#####Most useful arguments
     -O        Downloads the content on the URL to a file with the same name as the remote file
     -d <data> Sends the data in a HTTP post to the given URL

#####Example usage
```Shell
curl https://raw.github.com/haaakon/TerminalCommands/master/README.md
     Writes out all the content of this file you are reading now to the command line.
curl -O https://raw.github.com/haaakon/TerminalCommands/master/README.md
     Writes this this Readme file to a file named README.md on your current command line location 

```

## touch
Creates a new file with the name you specify in the arguments. If run on an existing file it will reset the file`s created date. [touch on Wikipedia](http://en.wikipedia.org/wiki/Touch_(Unix))

#####Example usage
```Shell
touch newfile.html
     creates an empty new file called 'newfile.html'

```
__________

