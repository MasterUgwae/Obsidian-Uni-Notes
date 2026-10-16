
# Getting familiar with Linux

- /etc/passwd contains which shell each user is using
	- username:*:UID:GID:UserInfo:HOME:SHELL
- /etc/shadow contains the hash for each user's passwd
	- file permissions are 000

- There are other shells:
	- Bash
	- sh
	- csh
	- zsh
	- bsh
	- Use ```cat /etc/shells``` to view all shells 
- They don't provide interactive interfaces for certain accounts such as ftp.

## Environmental variables
```bash
export LH=Ligang
echo $LH
```
- env shows all environmental variables

## Shell config files
- bash has 2 config files
	- .bash_profile
		- run on login
	- .bashrc
		- run on shell startup

## Directory Structure
- root
	- home
		- home directories for users
	- etc
		- System wide config files
	- var
		- Contains variable data
	- usr
		- User data and application installed by users
	- bin
	- dev
	- tmp
	- lib
	- sbin
		-  System admin commands

## File permisisons
- (d/l)rwxrwxrwx
	- d: directory or link
	- rwx: read/write/execute permissions for user
	- rwx: read/write/execute permissions for group
	- rwx: read/write/execute permissions for others

## Root Privilage
Can be gained by 1 of 3:
- Login as root
- su command
- sudo command

# Encryption
- 