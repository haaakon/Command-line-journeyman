#Command line journeyman
Useful stuff you can do with the command line.

##### Table of Contents  
* [chmod](#chmod)  
* [curl](#curl)
* [touch](#touch)
* [Useful keyboard shortcuts](#Keyboard shortcuts)

# At a glance

```
bg       - start a background job
fg       - take background job to foreground    
ls       - list files in directory                     ex: ls -l
chmod    - change attributes of a file                 ex: chmod test.swift 777
cat      - show content of a file                      ex: cat hello.txt
tail     - show last part of a file                    ex: tail test.log
kill     - send a process a signal                     ex: kill INT 8133
sudo     - run a command as root                       ex: sudo gem install
grep     - search for a string in a file               ex: grep -i "saturn" planets.txt
ifconfig - view or config network interface            ex: ifconfig -a
  
```

## chmod
Changes the attributes of a file.  [chmod on Wikipedia](http://en.wikipedia.org/wiki/Chmod) 

##### Most useful arguments
    -R         Recursively sets the attributes in all subdirectories as well
##### Example usage
```
chmod 777 examplefile.file
    Lets all users and groups read and write to the file 'examplefile.file'
```

## grep
Search for a string in a file (case insensitive)

```
$ grep -A 5 -i "blue dot" carl_sagan.txt
    printing the matched line with 5 lines followin it
$ grep -r "jupiter" *
    Search for a string "jupiter" in all files recursively
```

## find
Find files with filename (case insensitive)

```
$ find -iname "launchplan.swift"
```

## redirect >
send the output from a command to a file
```
$ ls -l > files.txt
   set content of files.txt to be what is prited from ls
```

## pipe |
Send output from one process as input to another process

```
$ ps aux | grep Terminal.app
    shows you only the processes thats named Terminal.app
```


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

## ps 
Display information about the processes that are running.



## Keyboard shortcuts
```
CTRL-a     Sets cursor to start of line
CTRL-k     Clears everything after cursor
CTRL-u     Clears everything before and after cursor
CTRL-l     'Resets' the terminal clearing all output
CTRL-r     Search through history of everything you have written in command line
```
