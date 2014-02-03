TerminalCommands
================

Just some useful commands you can do in the terminal

##### Table of Contents  
* [chmod](#chmod)  
* [touch](#touch)



## chmod
Changes the attributes of a file.  [chmod on Wikipedia](http://en.wikipedia.org/wiki/Chmod) 

#####Most useful arguments

    -R        Recursively sets the attributes in all subdirectories as well
#####Example usage
```Shell
chmod 777 examplefile.file
    Lets all users and groups read and write to the file 'examplefile.file'
```
__________
## touch
Creates a new file with the name you specify in the arguments. If run on an existing file it will reset the file`s created date. [touch on Wikipedia](http://en.wikipedia.org/wiki/Touch_(Unix))

#####Example usage
```Shell
touch newfile.html
     creates an empty new file called 'newfile.html'

```
__________
