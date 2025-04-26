## [60 Linux Commands you NEED to know (in 10 Minutes)](https://www.youtube.com/watch?v=gd7BXuUQ91w)

> Import this file into [Mochi](https://mochi.cards/) or give it to your favorite AI tool and have it proxy a quiz and check your answers. When importing make sure you select Markdown as the format, "Multiple cards per .md file", and a ```triple backslash``` as the string delimiter. You can use the link to the raw file in GitHub instead of downloading and importing if you prefer.

### SSH and System Access
- SSH (Secure Shell) - Connect to remote Linux machines
- Login with username and IP address
- Accept fingerprints and provide password for access

### File Navigation and Management
- ls - List files in current directory
  - -l option provides detailed list view
  - -a option shows hidden files
- pwd - Print working directory
- cd - Change directory
  - cd / - Go to root directory
  - cd .. - Go back one directory
  - cd - Return to home directory
- touch - Create files quickly
  - Can create multiple files at once
  - Can set file creation date with -d
- mkdir - Create new directories
- cp - Copy files to another location
- mv - Move files to a new location
- rm - Remove files
  - -r option removes directories recursively
- rmdir - Remove empty directories
- ln - Create links to files
  - -s option creates soft links

### File Editing and Viewing
- echo - Display text or write to files
- nano - Simple text editor
  - Control+X, Y, Enter to save and exit
- vim - Advanced text editor
  - i to insert text
  - Escape, :wq to write and quit
- cat - Display file contents
- less - View files one page at a time
- head - View beginning of file
- tail - View end of file
- shred - Securely delete files

### User Management
- whoami - Display current username
- useradd - Create new user
- adduser - Create new user with more options
- su - Switch to another user
- exit - Exit current session
- passwd - Change user passwords
- sudo - Execute commands with elevated privileges

### Package Management
- apt - Package manager for Debian-based systems
  - apt update - Update repository information
  - apt install - Install new packages
- yum - Package manager for Red Hat systems

### Help and Information
- man - Display manual pages for commands
- whatis - Brief description of command
- which - Show location of command
- whereis - Show all locations of command

### Networking
- ifconfig - Display network interface information
- ip address - Modern command for IP information
- ping - Test connectivity to hosts
- traceroute - Show path to destination
- netstat - Display network connections
  - -tulpn shows listening ports
- ss - Modern replacement for netstat
- iptables - Configure firewall rules
- ufw - Simplified firewall management
  - ufw allow/deny - Control port access
  - ufw enable/disable - Turn firewall on/off

### File Comparison and Manipulation
- cmp - Compare two files
- diff - Show differences between files
- sort - Sort file contents
- find - Search for files
- grep - Filter text based on patterns
- awk - Advanced text processing

### System Information
- uname - Display system information
- neofetch - Show system info in a visually appealing way
- free - Display memory usage
- df - Show disk space usage
  - -H option for human-readable format
- ps - Display running processes
  - aux options show all processes
- top/htop - Interactive process viewer

### Process Management
- kill - Terminate processes by PID
- pkill - Kill processes by name
- systemctl - Manage system services
  - start/stop/restart/status options

### Miscellaneous
- clear - Clear terminal screen
- history - Show command history
- cal - Display calendar
- shutdown - Power off system
- reboot - Restart system

### Terms
- SSH - Secure Shell protocol for encrypted remote system access
- Terminal - Text-based interface to interact with the system
- Shell - Command interpreter that processes user commands
- Directory - Folder in the Linux file system
- Root - Top-level directory in the Linux file system
- sudo - "Superuser do" - execute commands with administrative privileges
- Package - Software bundle that can be installed on Linux
- Repository - Collection of software packages
- Daemon - Background service in Linux
- Process - Running instance of a program
- PID - Process ID, unique identifier for running processes
- Pipe - Symbol (|) used to send output of one command as input to another
- Grep - Global Regular Expression Print - tool for pattern matching
- Firewall - Security system controlling network traffic
- Recursive - Operation that applies to all subdirectories and their contents

///

## What command allows you to connect to a remote Linux machine?

---

A) connect

B) login

C) ssh

D) remote

---

ssh

///

## Which command will show you your current location in the file system?

---

A) ls

B) pwd

C) cd

D) where

---

pwd

///

## How do you create a new empty file in Linux?

---

A) new

B) touch

C) create

D) make

---

touch

///

## Which command is used to edit text files with a simple interface?

---

A) vim

B) nano

C) cat

D) edit

---

nano

///

## What command shows the contents of a file in the terminal?

---

A) cat

B) view

C) show

D) read

---

cat

///

## How do you remove a file in Linux?

---

A) delete

B) remove

C) rm

D) erase

---

rm

///

## What command is used to create a new directory?

---

A) newdir

B) createdir

C) mkdir

D) makedir

---

mkdir

///

## Which command lets you know what user you are logged in as?

---

A) me

B) username

C) user

D) whoami

---

whoami

///

## What command is used to execute commands with elevated privileges?

---

A) admin

B) root

C) sudo

D) super

---

sudo

///

## How do you switch to another user in Linux?

---

A) change

B) switch

C) su

D) become

---

su

///

## Which command is used to update package repositories on Debian-based systems?

---

A) apt update

B) yum update

C) update repos

D) package refresh

---

apt update

///

## What command shows manual pages for other commands?

---

A) help

B) info

C) man

D) guide

---

man

///

## How do you check if a remote server is accessible?

---

A) connect

B) check

C) ping

D) access

---

ping

///

## Which command displays network interface information?

---

A) network

B) ifconfig

C) netinfo

D) interfaces

---

ifconfig

///

## What command is used to find files in the Linux file system?

---

A) search

B) locate

C) find

D) lookup

---

find

///

## Which command is used to filter text or search for patterns?

---

A) filter

B) search

C) grep

D) pattern

---

grep

///

## What command is used to check disk space usage?

---

A) disk

B) space

C) df

D) storage

---

df

///

## Which command shows running processes?

---

A) ps

B) proc

C) run

D) process

---

ps

///

## How do you terminate a process by its Process ID (PID)?

---

A) end

B) terminate

C) kill

D) stop

---

kill

///

## What command is used to manage system services in modern Linux distributions?

---

A) service

B) systemctl

C) control

D) daemon

---

systemctl

///

## What do you call a background service in Linux?

---

A) Background

B) Service

C) Daemon

D) Process

---

Daemon

///

## What is a PID in Linux?

---

A) Personal Identifier

B) Program ID

C) Process ID

D) Priority Identifier

---

Process ID

///

## What symbol is used to send output from one command as input to another?

---

A) >

B) |

C) &

D) #

---

|

///

## What is the top-level directory called in the Linux file system?

---

A) Top

B) Main

C) Home

D) Root

---

Root

///

## What is "sudo" short for?

---

A) Super User Do

B) System User Domain Operations

C) Single User Domain Override

D) Super User Domain Operator

---

Super User Do

///

## What is a software bundle that can be installed on Linux called?

---

A) Bundle

B) App

C) Package

D) Program

---

Package
