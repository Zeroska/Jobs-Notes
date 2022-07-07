# Notes for Jul_06_2022

This is a note or a diary for the things I research in a day, this note intended for me not to forget the knowlegde I has gain (or things I has read).

## Linux Logging 

Link: <https://www.siemplify.co/blog/your-security-operations-cheat-sheet-for-windows-and-linux-logs-and-how-to-tie-them-to-the-mitre-attck-framework/>
Link: <https://cyberblueteam.medium.com/blue-team-tips-linux-os-finding-evil-running-process-3f12b17c3b8e>

Syslog format and Linux format

A Syslog message has the following format: A header, followed by structured-data (SD) followed by a message

**HEADER** contains "priority", "version", "timestamp", "hostname", "application", "process id", and "message id"
-> Most of the time this will be parsed by the engine of siem or anything you use

**SD** Structure data, it is just data in format

So the most important thing is to learn which log folder is important 

### Why Linux doesn't log command line 

When I search for this question on the internet the result I got back is not what I expected and need so I dig a little bit deeper to 
know more about the log -

The Research is PENDING
