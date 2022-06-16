# Notes for Jun_14_2022

This is a note or a diary for the things I research in a day, this note intended for me not to forget the knowlegde I has gain (or things I has read).

## APT28/SOFACY called SKINNYBOY Reading

- <https://cybergeeks.tech/skinnyboy-apt28/>

The malware extracts configuration information about the machine that it infects using the systeminfo command, and then it retrieves the list of processes by spawning a tasklist process.

### What is AppData\Roaming?

AppData is a hidden folder in windows and each user will has its own AppData folder with its own content

Roaming is a folder belong to the AppData, its hold information about the

## SOAR Event Playbook Training

Filter out your Event before your Analyst see it

If config right -> 70% False Positive will be cut off

### How can you dismiss Event in Event Playbook and Passdown

-> Passdown data to these field

- Trigger Output Data
- $.Dismiss
- True

## Blog I read

- <https://blog.notso.pro/2022-06-12-avoiding-cyber-nihilism/>
