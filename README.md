# Linux-Cmds

absolute path: mention the whole path starting from the root
relative path: mention the path from the current dir you are in

tree -a <dir>
- hierarchy

1. pwd
Find the path of the working directory

2. cd
change directory depending on the path specified
Options:
cd .. : moves to one directory down
cd ~ : bring to home directory

3. ls
list the files and dir from current working directory
Options:
ls -R : list all files in dir and subdir
la -a : show files and the hidden ones
ls -lh : shows files in readable format like MB, GB and TB
ls -l : show long list like permission, user, grp, owner, last modification

4. cat
5. cp or cp -R <SOURCE> <DEST>

6. mv
to rename or move the file

7. mkdir
creates directory

8. rmdir
removes directory

9. rm 
Deletes files within directory
Options:
 -r : deletes files and dir recursively

10. touch
Creates an empty file

11. find
Searches for files n dir. Supports searching by file, folder, name, creation date, modification date, owner and permissions.
By using the ‘-exec’ other UNIX commands can be executed on files or folders found. 
Options:
find [options] [path] [expression]
find -name <filename> : finds files in current dir
find ./ -type d -name <dir_name> : looks for dir  
find ./<dir_name> -name <file_name> -exec rm -i {} \;

12. grep
Finds by word in all the texts in specified file adn prints all lines that contains specific pattern.
Options:
grep [options] pattern [files]
-i : case sensitive
-f : files

13. df
gives the system disk space usage
Options:
df -h : gives current dir disk space in readable fmt
df -a : display all the file system
df -m : displays info in MBs
df -k : displays info in KBs

14. du 
Checks how much space a file or a dir takes up
Options:
du -s : display total size of a specified folder
du -m

15. head -n
displays starting lines of a text

16. tail -n 
displays last lines of a text

17. tar
create Archive and extract the Archive files
Options:
-c : Creates Archive 
-x : Extract the archive 
-f : creates archive with given filename 
-t : displays or lists files in archived file 
-v : Displays Verbose Information 
-z : zip, creates tar file using gzip 
tar cvf file.tar *.c : creates a tar file called file.tar
tar xvf file.tar : extracts files from Archives
tar xvzf file.tar.gz : extracts files from tar archived file.tar.gz files
 
18. chmod

19. chown

20. kill

21. ping

22. wget

23. history

24.echo

25. zip, unzip

26. hostname

27. nano, vi

28. su

29. ps

30. 
