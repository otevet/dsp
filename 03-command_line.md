# Learn command line

Please follow and complete the free online [Command Line Crash Course
tutorial](https://web.archive.org/web/20160708171659/http://cli.learncodethehardway.org/book/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. Each "chapter" focuses on a command. Type the commands you see in the _Do This_ section, and read the _You Learned This_ section. Move on to the next chapter. You should be able to go through these in a couple of hours.

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

> > pwd: show current working directory path: 
mkdir: creating a directory  
rmdir: removing a directory 
touch: make a new empty file   
rm: removing a file  
mv: renaming a file  
ls -ld .?*    listing hidden files  
cp: copy  afile from one directory to another  
man: manual  
clear: clears the current window  


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

> > 

ls		lists files
ls -a		lists all files, including hidden ones
ls -l  		lists files in a long format, containing additional useful information 
ls -lh 		list long format with readable file size
ls -lah  	list long format with readable file size, includes hidden files
ls -t		list by time and date
ls -Glp 	G inhibits the display of group information, l displays the contents in long format, and p displays directories with '/'


---


### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > ls -d	displays only directories
ls -R 		displays subdirectories as well
ls -1 		displays each entry on a line
ls -c 	 	displays files by file timestamp
ls -u 		displays files by the file access time

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > xargs reads in items from standard input (stdin) and executes a command (default is /bin/echo) with any given initial arguments. For example, the xargs can be used with the grep and find commands:

find . -name "*.txt" | xargs grep "data"

The above command finds all text files from the current directory, and within each file, looks for occurences of "data". xargs unpacks arguments and feeds them into commands, one by one.

