***************************************
Programming Language chosen: C#

Title of the program: SyncFolders.cs

Run Program in prompt command line

All files in SyncFolder needs to in sameplace, to execute SyncFolder.exe 
***************************************

---------------------------------- Program ----------------------------------

This program will do the one-way sync between two folders: "source" and "replica".
The objective of program: 
. All the file and folders of the source have a copy in the replica
. The sync will have a time interval
. The time interval is chosen by the user
. If a file/folder is deleted in the source, will be deleted too in the replica
. If a file/folder is modified in the source, will be updated in the replica
. If a new file/folder is created, will be copied to the replica
. All changes and copies will occur within the time interval choosed by the user 
. All files/folders that are in the replica but not in the source, will be deleted
. A log file will record all updates, removals and copies



---------------------------------- what the program does ---------------------------------  

. Initially, the program will compare the two folders, and see if they are identical, if not, the replica folder will be updated
. After each time interval, the program will compare the folders again. If changes are detected, the replica folder will be updated
. To ensure that the replica is identical to the source, updates, copies, and deletions of files/folders will be made.
. Every changes made by the program, will be recorded in a log file
. The changes will be  displayed in the console of your command line
. The time interval check will be done until the program is stopped



---------------------------------- How to do ----------------------------------

. execute the programm from your command line, four arguments needs to be passed: path to the source folder, path to the replica folder, the time interval and path to the log file
exemples of command line input:

for Windows: cd "C:/path/to/executable"
SyncFolders.exe --source "C:/Users/<name>/<folder>/source_folder" --replica "C:/Users/<name>/<folder>/replica_folder" --interval 30 --logfile "C:/Users/<name>/<folder>/sync.log"

for Mac/Linux: ./SyncFolders --source "/home/<name>/source_folder" --replica "/home/<name>/replica_folder" --interval 30 --logfile "/home/<name>/logs/sync.log"

 
## Requirements

- **Operating System:** Windows, macOS, or Linux.
- **.NET Runtime:** Version 7.0 or newer.
- **File System Access:** Read and write permissions for the specified `source`, `replica`, and log file directories


** Notes **
In the .zip file, there a copy of Readme.txt, copy of sync.log, two folders, source and replica, and some files for test. I don't have the rights of the image in .zip file.
In the .rar are the program and necessary files
Created as part of a job application project
