#### Linux-Cmds

*absolute path*: mention the whole path starting from the root<br>
*relative path*: mention the path from the current dir you are in

__tree -a <dir>__ 
>gives the hierarchy structure of the dir

**1. pwd** 
>Find the path of the working directory

**2. cd**
>change directory depending on the path specified<br>
**Options:** <br>
cd .. : moves to one directory down <br >
cd ~ : bring to home directory 

**3. ls**
>list the files and dir from current working directory <br>
**Options:** <br>
ls -R : list all files in dir and subdir<br>
la -a : show files and the hidden ones<br>
ls -lh : shows files in readable format like MB, GB and TB<br>
ls -l : show long list like permission, user, grp, owner, last modification<br>

**4. cat**

**5. cp or cp -R <SOURCE> <DEST>**

**6. mv**
>to rename or move the file

**7. mkdir**
>creates directory

**8. rmdir**
>removes directory

**9. rm** 
>Deletes files within directory<br>
**Options**:<br>
 -r : deletes files and dir recursively

**10. touch**
>Creates an empty file

**11. find**
>Searches for files n dir. Supports searching by file, folder, name, creation date, modification date, owner and permissions.<br>
By using the ‘-exec’ other UNIX commands can be executed on files or folders found. <br>
>**Options:**<br>
find [options] [path] [expression]<br>
find -name <filename> : finds files in current dir<br>
find ./ -type d -name <dir_name> : looks for dir  <br>
find ./<dir_name> -name <file_name> -exec rm -i {} \

**12. grep**
>Finds by word in all the texts in specified file adn prints all lines that contains specific pattern.<br>

>**Regix:**<br>
^ : Matches characters at the beginning of the line<br>
$ : Matches characters at the end of the line<br>
"." : Matches any characters<br>
[a-z] : Matches characters between a and z<br>

>**Options:**<br>
grep [options] pattern [files]<br>
-i : case sensitive<br>
-f : files

**13. df**
>gives the system disk space usage<br>

>Options:<br>
df -h : gives current dir disk space in readable fmt<br>
df -a : display all the file system<br>
df -m : displays info in MBs<br>
df -k : displays info in KBs<br>

**14. du** 
>Checks how much space a file or a dir takes up<br>

>**Options:**<br>
du -s : display total size of a specified folder<br>
du -m<br>

**15. head -n**
>displays starting lines of a text

**16. tail -n** 
>displays last lines of a text

**17. tar**
>create Archive and extract the Archive files

>**Options:**
-c : Creates Archive <br>
-x : Extract the archive <br>
-f : creates archive with given filename<br> 
-t : displays or lists files in archived file<br> 
-v : Displays Verbose Information <br>
-z : zip, creates tar file using gzip <br>
tar cvf file.tar *.c : creates a tar file called file.tar<br>
tar xvf file.tar : extracts files from Archives<br>
tar xvzf file.tar.gz : extracts files from tar archived file.tar.gz files
 
**18. chmod**
>Modifies the read, write and execute permissions for file or directory<br>
4 stands for "read",<br>
2 stands for "write",<br>
1 stands for "execute", and<br>
0 stands for "no permission."

>**Examples:**<br>
chmod 754 <file_name>, same as, chmod u=rwx,g=rx,o=r <file_name><br>
7 is the combination of permissions 4+2+1 (read, write, and execute)<br>
5 is 4+0+1 (read, no write, and execute)<br>
4 is 4+0+0 (read, no write, and no execute).

**19. chown**
>Modifies the ownership of files and directory (only a root or a sudo can perform it)<br>
sudo chown -R <user>:<group> <files>

**20. kill**
>Terminates the unresponsive program manually. Signals the applications and instruct them to close their processes.<br>
To kill a program you need a PID. you can get it using: ``` ps ux ```

>**Options:**
kill [signal_option] pid<br>
kill <pid_no><br>

>Most commone signals are : <br>
 *SIGTERM:* request a program to stop runnign and give some time to save all of its progress. The system uses it by default if not specified<br>
 *SIGKILL:* forces the programs to stop withour saving the progress

**21. ping**
>To check if network servers are reachable
**Examples:**
ping -c 5 google.com

**22. wget**
>To download files using http, https and ftp from the internet. Works in background

>**Options:**<br>
wget [options] [url]<br>
-o <logfile>: Log all messages to <logfile><br>
-O <file_name>: Ouput the files under the name specified<br>

**23. history**
>list up all the previous;y executed cmds

**24. echo**
>print texts

**25. zip unzip**
>Compresses the file into ZIP files, automatically choose the compression ratio<br>

>**Options:**<br>
>zip <zip file name>.zip <file to zip>

**26. hostname**
>To know the system hostname<br>
  -A : displays fqdn<br>
  -a : displays hostname alias<br>
  -i : displays machine ip address

**27. nano vi**
>Text Editor

**28. su**
>Allows to run program as a different user. Changes the administrative account to current log-in user. Beneficial while accessing through ssh

>Options:<br>
su -s : let you specify different shell environment to run<br>
su -l : runs a login script to switch to a diff user

**29. ps**
Gives the snapshot of the running processes<br>
ps aux <br> 
>**Options:**<br>
ps -u : list the processes associated with specific user<br>
ps -A or -e : shows all running processes<br>
ps -T : displays all processes associated with current shell session

**30. ssh-keygen** 
 >Generates a public/private authentication key pair

**31. openssl**
 >Tool that is commonly used to generate private keys, create CSRs, install your SSL/TLS certificate, and identify certificate information.

**32. curl**
>Enables data transfer over various network protocols.<br>
-o : Store output in a file.<br>
-O : Specify that the local file should have the name of the remote file that was downloaded.
