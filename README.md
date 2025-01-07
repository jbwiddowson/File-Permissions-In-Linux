# Linux File and Directory Management
## Overview
This project demonstrates the use of Linux commands to manage files and directories. It includes checking file details, describing and modifying permissions, and working with hidden files and directories. These skills are fundamental for system administration and ensuring secure file systems.

## Table of Contents
1.[Check File and Directory Details](Check-File-and-Directory-Details)
2.[Describe the Permissions String](Describe-the-Permissions-String)
3.[Change File Permissions](#Change-File-Permissions)
4.[Change File Permissions on a Hidden File](#Change-File-Permissions-on-a-Hidden-File)
5.[Change Directory Permissions](#Change-Directory-Permissions)
6.[Summary](#Summary)

## Check File and Directory Details
To view detailed information about files and directories:

bash
Copy code
ls -l
Displays: File type, permissions, owner, group, size, and modification date.
Example:
bash
-rw-r--r-- 1 user group Cyber_team Jan 4 11:00 example.txt
To get detailed metadata about a file:
bash
stat example.txt

## Describe the Permissions String
Linux permissions consist of 10 characters:

File type:
- Regular file
d Directory
l Symbolic link

Permissions for owner, group, and others:
Read (r), write (w), and execute (x)

Example:
bash
-rw-r--r-- 1 user group 1234 Jan 1 12:00 example.txt

## Change File Permissions
Use chmod to modify file permissions:

bash
chmod u+x script.sh  # Adds execute permissions for the owner
chmod g-w document.txt  # Removes write permissions for the group

## Change File Permissions on a Hidden File
To modify permissions for hidden files (files starting with .):

bash
chmod u-r .hiddenfile
This command sets the file to be readable and writable only by the owner.

## Change Directory Permissions
Directory permissions control who can access or modify its contents:

bash
chmod 700 mydir  # Full access for the owner
chmod 755 public  # Read and execute for others

## Summary
This project highlights essential Linux commands for managing file and directory permissions. Mastery of these commands enables secure and efficient system administration

