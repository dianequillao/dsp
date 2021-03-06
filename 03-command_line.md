# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

> > 
* show current working directory path
    pwd
* creating a directory
    mkdir
* deleting a directory
    rm -r mydir
    rm -rf mydir to delete without a prompt
* creating a file using `touch` command
    touch
* deleting a file
    rm
* renaming a file
* listing hidden files
* copying a file from one directory to another
    mv "old location" "new location"
* organize a computer's files and folders into a tree structure 
    filesystem
* change directory
    cd
* move up one directory
    cd ..

---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  

> > `ls`  #lists the files and folders of the directory you are in
`ls -a`  #lists hidden and unhidden files
`ls -l`  #lists all contents of a directory in long format/as a table
`ls -lh`  #lists long format with readable file size
`ls -lah`  #lists hidden and unhidden files in long listing and readable format 
`ls -t`  #order files and directories by the time they were last modified.
`ls -Glp` #lists contents in a long listing (not group names), in a long listing format, and adds / to end of directories

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > `ls -x` #Displays files as rows across the screen.
`ls -1` #Displays each entry on a line.
`ls -q` #Displays all nonprinting characters as ?
`ls -d` #Displays only directories
`ls -m` #Displays the names as a comma-separated list

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > reads data from standard input (stdin) and executes the command (supplied to it as argument) one or more times based on the input read.



 

