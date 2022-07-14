# Notes for Jul_14_2022

This is a note or a diary for the things I research in a day, this note intended for me not to forget the knowlegde I has gain (or things I has read).

## What is integrity level in Windows 10 | Process Integrity level 

Link: <https://redcanary.com/blog/process-integrity-levels/>
Link: <https://redcanary.com/blog/process-command-line/>
Link: <http://terminus.rewolf.pl/terminus/>

## Integrity Level


## PEB and Process Commandline | Where adversary get it 

To futher my understanding about Windows logs we will take a look at PEB

Process command-line information is stored within the ProcessParameters field of the process environment block (PEB), a user-mode data structure present in all processes. There are no APIs for directly retrieving process command line from another process. 

