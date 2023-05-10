# Table of Contents
```
Several Contents are based on HTB Academy
```

1. Linux Basics Command

## Linux Basics Command

### Manual of command
To see detail manual and its explanations, run:
man <name_of_command>, ex: man ls

for the quick option of manual, run:
<name_of_command> --help, ex: curl --help
OR for the short version
<name_of_command> -h
```

### System Information
```
command | description
---------------------
whoami | Displays current username

id | returns user identity

hostname | Sets or Prints the name of current host system

uname | Prints basic information about the operating system name and system hardware

pwd | Returns working directory name

ip | Ip is a utility to show or manipulate routing, network devices, interfaces and tunnels

ss | Another utility to investigate sockets

ps | Shows process status

who | Displays who is logged in

env | Prints environment or sets and executes command
```

### Navigation
```
To see current directory:
pwd

To see all file in directory:
current directory:
ls
ls -l (with detail description)
ls -al (include the hidden file)

other directory:
ls <directory_path>, ex: ls /etc

To go to other directory
cd <directory_path>, ex: cd /etc

Back to previous directory
cd -

clear written command
clear
OR 
ctrl + l (Not always working in every terminal)
```