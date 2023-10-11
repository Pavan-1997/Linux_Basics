# Linux-Shell Basic Commands             
 
### Below are the commands that are documented by me and will be updating. 
  
---  
     
- `touch `   
    
  (Create empty files or update file timestamps.  Primarily used in Automation)
  
 
- `ls`   
   
  (List files or List directory contents)

 
- `ls -ltr`
  
  (Lists the files with dates or lists files in long format sorted by time, with the latest files at the bottom)


 - `id`

    (Find out user and group names and numeric ID’s (UID or group ID) of the current user or any other user in the server)


- `cut`

   (Extract specific fields or columns from a file or standard input)


- `sed`

   (Perform basic text transformations on an input file. It stands for "stream editor" and is a powerful tool for editing text files or streams in a Linux environment)

  
-  `man ls`

   (Manual for Linux)

 
- `vim`
  
  (Command-line text editor in Linux used for editing files)

  ![image](https://github.com/Pavan-1997/Linux-Shell_Basic_Commands/assets/32020205/d0e08eb3-fe25-4508-b97d-07f03aa8d466)


  `vi`
  
  (Editing files, By default available in Linux)

 
- `#!/bin/bash`
  ```
  #! - Shebang 
  
  Where bash, dash, ksh and sh are called executables 
   
  bash is commonly used 
   
  Earlier there was a soft link between #!/bin/sh to #!/bin/bash 
   
  Now in ubuntu there is a soft link between #!/bin/sh to #!/bin/dash 
  ```


- `echo "Test"`
  
    (Print message or display text or variables in the terminal)


-  `sh script.sh` or `./script.sh`

    (To execute the script shell file)

  
- `cat`

  (Concatenate and display files on the terminal. It can also be used to modify existing ones)

![image](https://github.com/Pavan-1997/Linux-Shell_Basic_Commands/assets/32020205/9953ee6b-9780-4605-867d-cba586cdc8b2)


  
- `chmod`
  
  (ch- change, Change file permissions)
  
  ![image](https://github.com/Pavan-1997/Linux-Shell_Basics_Commands/assets/32020205/33fa84e9-1b21-4b31-b640-c41f566d7fc5)

```  
  -   User
  -   Group 
  -   Other   
 
   `chmod 777 <file-name>`
 
   4-Read | 2-Write | 1-Execute 
```


- `chown`

   (Change the file Owner or group)
  

- `history`

  (Shows a list of previously executed commands in the terminal)

  `history 10`

  (Last 10 executed commands)


 - `lsof`

    (Display a list of all the open files on a Linux system)

   
- `pwd`

  (Displays the current working directory (path))


- `cd`

  (Change the current working directory)

 
- `mkdir`

  (Create a new directory)

 
- `hostid`

   (Shows the host id of the system assigned by the OS)


- `sort`

  (Sort lines of text in a file or input stream alphabetically or numerically)
  
  ![image](https://github.com/Pavan-1997/Linux-Shell_Basic_Commands/assets/32020205/9bb5747f-a211-426c-821d-42da3e7ac81d)


- `tail`

   (Prints the last N number of data of the given input. By default, it prints 10 lines)


- `diff`

  (Find the difference between two files, diff file1.txt file2.txt)


- `nslookup`

  (Checking DNS hostname to Ip or Ip to Hostname)


- `tr`
  
  (Translation. This command is for translating or deleting characters)
  

- `nproc`
  
  (Displays the number of available processing units (CPU cores)) 

  
- `free` 

  (Shows the system's memory usage and available memory)

  
- `top` 

  (Provides real-time system monitoring, displaying information about processes and system usage)


- `htop`

  (Monitor the system’s resources and processes that are running in real time)
  
 
- `df`
  
  (Displays information about disk space usage on file systems) 

  `du`

  (Displays size of directory tree including all the content)


- `tnc`

  (This is “Test Network Connection” command. Mostly used command while troubleshooting. It displays diagnostic information for a connection)

  
- `apt-get`

  (Install, update, and remove packages, as well as to manage the package repository sources)

  ![image](https://github.com/Pavan-1997/Linux-Shell_Basic_Commands/assets/32020205/1af627dd-f213-442e-a23a-e9a492f8ee7b)


- `ps`
  (Check the unique id behind every process)

 ![image](https://github.com/Pavan-1997/Linux-Shell_Basic_Commands/assets/32020205/0f6b6e10-3cff-47a9-af81-872939deb691)

 
- `ps -ef` 

  (Lists all running processes in full format in Linux)  

  
- `ps -ef | grep "amazon"`  

  (Lists processes containing the string "amazon" using the "grep" command to filter the output)


- `awk` 

  (It is a versatile text-processing tool used in Linux for extracting and manipulating data in structured text files)


- `ps -ef | grep "amazon" | awk -F" " '{print $2}'`

  (Extracts the second column (process IDs) of processes containing "amazon" using the "awk" command after filtering with "grep.")

 
- `set -x` 

  (In debug mode) 


- `date`

  (Displays the current date and time)

  (Date sends the output to stdin, hence using `|` doesn't re-direct the output of first command to the second command)

  (See the below command for example)


- `date | echo "test"`

  (The command "date | echo "test"" will just output "test" without including the output of the "date" command)


- `curl -x GET api.foo.com`

  (Gives output of info provided by API of foo.com)
 

- `curl https://github.com/Pavan-1997/Linux-Shell_Basics_Commands/blob/main/dummylog01122022.log | grep ERROR` 

  (Transfers data to or from a server using various protocols, including HTTP, HTTPS, FTP or Retrieves information from the above URL, and gives only the ERROR logs)
 

- `wget https://github.com/Pavan-1997/Linux-Shell_Basics_Commands/blob/main/dummylog01122022.log`

  (Download files from the internet using various protocols, such as HTTP, HTTPS, and FTP or Using the above we can't view the info but downloads the file)  

   
- `sudo su -`  

  (Switch to the root user)

 
- `sudo find / -name pavan`

   (Searches the entire filesystem for files or directories named "pavan," with elevated privileges using "sudo" to access restricted areas)

![image](https://github.com/Pavan-1997/Linux-Shell_Basic_Commands/assets/32020205/e3ad2319-bc07-4174-a56b-75be8bb3bf59)


 ---
 ### Loops:
  
```
a=4 
b=10 
 
if [$a > $b] 
then  
    echo "a is greater than b" 
else 
    echo "b is greater than a" 
fi 
```


```
for i in {1.100}; do echo $1; done
```

---
### Trap & Kill:

- `trap "echo don’t use the Ctrl+c" SIGINT` 

  (Trapping signals, even when if they send a Ctrl + C signal they get the above echo message)
 
- `trap "rm -rf *" SIGINT` 

  (Delete everything from the database when hitting Ctrl + C)
 
- `kill -9 1111` 

  (Pass a kill signal to Linux to terminate 1111 process ID)


  
