# Terminal Basics
- [ ] Can describe shell environment variables
```bash

```
- [ ] Can get a shell environment variable's value, in the terminal
```bash

```
- [ ] Can set a shell environment variable's value, in the terminal
```bash

```
- [x] Can describe what the shell $PATH environment variable is used for
```bash
 PATH specifies a set of directories where executable programs are located
```
- [x] Can and modify your shell's $PATH, in the terminal
```bash
$ export PATH="/folder_name:$PATH" # Prepend folder to $PATH
$ export PATH="$PATH:/folder_name" # Append folder to $PATH
$ sudo atom /etc/paths # Edit PATH in atom (for permanance)
```
- [ ] Can use the echo terminal command
```bash
 $ echo "Hello World!" # Hello World
```
- [ ] Can use the cd terminal command
```bash
$ cd ~/Documents
```
- [ ] Can use the ls terminal command
```bash
$ ls -l # lists all files in a directory and their permissions
```
- [ ] Can use the cat terminal command
```bash
$ cat test.txt
```
- [ ] Can use the pwd terminal command
```bash
$ pwd #/Users/vagabonding.io/Documents
```
- [ ] Can use the touch terminal command
```bash
$ touch new_file.txt # creates a new file
```
- [ ] Can use the mkdir terminal command
```bash
$ mkdir new_folder_name # creates a new folder
```
- [ ] Can use the rmdir terminal command
```bash
$ rmdir folderName
```
- [ ] Can use the rm terminal command
```bash
$ rm -r folderName
```
- [ ] Can use the mv terminal command
```bash
$ mv filename1 filename2 # renames filename1 to filename2
$ mv filename1 ~/Documents/filename1 # moves file to Documents folder
$ mv foldername/* . # extracts the files in the folder into the current directory
```
- [ ] Can use the cp terminal command
```bash
$ cp filename.txt ~/Documents/ # Copies file and preserves filename
$ cp filename.txt ~/Documents/renamedfile.txt # Copies file and renames file
```
- [ ] Can describe what a filesystem is
```bash

```
- [ ] Can describe what a filesystem path is
```bash

```
- [ ] Can describe the difference between absolute vs. relative filesystem paths
```bash

```
- [ ] Can open a file or directory in their editor from the terminal
```bash
$ code foldername
$ code filename
$ atom foldername
$ atom filename
```
- [ ] Can open a directory in the Finder.app from the terminal
```bash
$ open foldername
```
- [ ] Can open a file in its default app from the terminal
```bash
$ open filename
```
- [ ] Can use ctrl-c in the terminal
```bash
Sends a SIGINT 
```
- [ ] Can use ctrl-a in the terminal
```bash
Moves cursor to the beginning of a line
```
- [ ] Can use ctrl-e in the terminal
```bash
 Moves cursor to the end of a line
```
- [ ] Can configure a Bash shell by modifying the ~/.bashrc and ~/.bash_profile files
```bash

```
- [ ] Can define a BASH alias
```bash
$ alias ddg="lynx https://duckduckgo.com/lite/" 
$ alias ddg="/Applications/Google\ Chrome.app/Contents/MacOS/Google\ Chrome https://duckduckgo.com/lite/"
```
- [ ] Can customize your BASH $PS1
```bash

```
- [ ] Can use BASH brace expansion
```bash
$ echo {a..z}
a b c d e f g h i j k l m n o p q r s t u v w x y z
$ echo {1..10}
1 2 3 4 5 6 7 8 9 10
```
- [ ] Can set $EDITOR to their preferred editors terminal command
```bash
$ export EDITOR=atom
$ echo $EDITOR
atom
```

# Terminal Advanced
- [ ] Can start and stop services with brew services, in the terminal
```bash
$ brew services start
$ brew services stop
```
- [ ] Can add a custom bin directory to their Shell config, in the terminal
```bash
$ sudo nano /etc/paths 
$ sudo atom /etc/paths
$ sudo code /etc/paths
```
- [ ] Can use | (pipe) in the terminal
```bash
cd ~/Documents && ls -a | grep fileNameToSearchFor
```
- [ ] Can use > (redirect) in the terminal
```bash

```
- [ ] Can use ctrl-z in the terminal
```bash

```
- [ ] Can use ctrl-r in the terminal
```bash

```
- [ ] Can use the tail terminal command
```bash
tail -n 10 WarAndPeace.txt # Display the last 10 lines of WarAndPeace
```
- [ ] Can use the grep terminal command
```bash
$ grep "search_string" filename # search for string in a given file
$ grep "search_string" *.txt # search for a string in all text files
$ grep -i "search_string" filename # search for a case-insensitive string
$ grep "above.*empty" *.txt # search for a line starting with above & ending with empty
$ grep -iw "is" filename # case-insensitive search for the whole word is
$ grep -A 3 -i "example" # case-insensitive search prints 3 lines AFTER the match
$ grep -B 3 -i "example" # case-insensitive search prints 3 lines BEFORE the match
$ grep -C 2 -i "example" # case-insensitive search prints 2 lines BEFORE AND AFTER
$ grep -r #recursive search of all files, directories, and subdirectories
$ grep -v "example" # invert search
$ grep -icw "I" filename # finds individual case-insensitive 
```
```txt
$ grep -C 1 -iw "cool" War\ and\ Peace.txt 
This short man nodded to Dolgorúkov as to an intimate friend and stared
at Prince Andrew with cool intensity, walking straight toward him and
evidently expecting him to bow or to step out of his way. Prince Andrew
--
--
which had been moved forward and was in action, deafening them with the
noise of firing, they came to a small wood. There it was cool and quiet,
with a scent of autumn. Pierre and the adjutant dismounted and walked up
```
- [ ] Can use the wc terminal command
```bash
$ wc * 
# displays words, lines, and characters for all files
    4853   28983  178983 RomeoAndJuliet.txt
       0       0       0 Test.js
   66055  566313 3359550 WarAndPeace.txt
       5      48     232 demo_file
       5      48     232 demo_file1
      17     119     593 demo_text
       4       4       8 test-file.txt
   70939  595515 3539598 total
```
```bash
$ wc -l * # Displays line count for all files
```
- [ ] Can use the du terminal command
```bash
$ du -h # creates a human readable printout of the disk usage of every file
```
```bash
$ df -h
Filesystem      Size   Used  Avail Capacity iused      ifree %iused  Mounted on
/dev/disk1     233Gi   56Gi  176Gi    25%  848618 4294118661    0%   /
devfs          186Ki  186Ki    0Bi   100%     643          0  100%   /dev
map -hosts       0Bi    0Bi    0Bi   100%       0          0  100%   /net
map auto_home    0Bi    0Bi    0Bi   100%       0          0  100%   /home
```
- [ ] Can use the man terminal command
```bash
$ man du # displays the man pages for a particular command
```
- [ ] Can use the file terminal command
```bash
$ file * # determines the filetype of all files in the directory
```
- [ ] Can use the ps terminal command
```bash
$ ps -M
USER             PID   TT   %CPU STAT PRI     STIME     UTIME COMMAND
vagabonding.io  2057 s000    0.0 S    31T   0:00.01   0:00.01 -bash
vagabonding.io  1940 s001    0.0 S    31T   0:00.00   0:00.01 -bash
vagabonding.io  1969 s002    0.0 S    31T   0:00.03   0:00.06 -bash
vagabonding.io  2351 s003    0.0 S    31T   0:00.01   0:00.02 -bash

$ ps -p 1969 # displays information relating to a specific PID
PID TTY           TIME CMD
1969 ttys002    0:00.11 -bash
```
- [ ] Can use the kill terminal command
```bash
$ kill 142 157 # Terminate the processes with PIDs 142 and 157

$ kill -s HUP 507 # Send the hangup signal (SIGHUP) to the process with PID 507

##      Some of the more commonly used signals:
     1       HUP (hang up) 
     2       INT (interrupt)
     3       QUIT (quit)
     6       ABRT (abort)
     9       KILL (non-catchable, non-ignorable kill)
     14      ALRM (alarm clock)
     15      TERM (software termination signal)
```
- [ ] Can use the chmod terminal command
```bash
$ sudo chmod -x Test.sh # sets the executable permission on the file
$ sudo chmod 755 Test.sh # executable by all, only writable by owner
```
- [ ] Can use the pbcopy terminal command
```bash
cat RomeoAndJuliet.txt | pbcopy
```
- [ ] Can use the pbpaste terminal command
```bash
pbpaste # pastes the entire text of Romeo and Juliet
```
- [ ] Can write an executable bash script
```bash
#!/bin/bash
# Test.sh
echo 'This is just a test'
exit 0
```
```bash
$ sudo chmod -x Test.sh # sets the executable permission on the file
$ sudo chmod 755 Test.sh # executable by all, only writable by owner
```
- [ ] Can and modify your shell's $PATH, in the terminal
```bash
$ export PATH="/newFolder:$PATH" # adds new folder to the beginning of the path
$ export PATH="$PATH:/newFolder" # adds new folder to the end of the path
```
- [ ] Can redirect STDOUT to a file, in the terminal
```bash
$ grep -iw "Brandon" > new_file.txt
$ ls -l | tee filename.txt
```
- [ ] Can describe UNIX command flags
```bash

```
- [ ] Can describe UNIX file permissions
```
	0000 abcd a - group, b - owner, c - group members d - others
	0124 0 - no access, 1 - execute, 2 - write, 4 - read
	 So odd numbers are executable even numbers are not
```
- [ ] Can get a file's permissions, in the terminal
```bash
$ ls -la
```
- [ ] Can set a file's permissions, in the terminal
```bash
$ sudo chmod -x filename
```
